# Arquitectura propuesta TDE (alto nivel, opinada según tus preferencias)

Frontend

- Ciudadanos y municipios: React + Next.js SSR. Tailwind + DaisyUI. i18n, accesibilidad AA. Charts con Recharts.
- Backoffice interno rápido: Lowcoder/Appsmith para CRUD y tableros operativos. Reemplazable gradualmente por React cuando haga falta.
- Chat UI unificado: OpenWebUI incrustado como “hub” de copilotos contextuales.

Backend

- API principal: FastAPI (Python 3.12) con pydantic v2, uvicorn/gunicorn.
- Graph API: Hasura sobre PostgreSQL para GraphQL instantáneo donde convenga; si no, Strawberry GraphQL en FastAPI para esquemas curados.
- Tareas asíncronas: Celery + Redis (cola) para jobs pesados; alternatively RQ si quieres algo más simple.
- Gateway y edge: Traefik v3 (ingress, TLS, rate-limit, WAF con Coraza/OWASP CRS).
- IAM/SSO: Keycloak (OIDC/OAuth2, SAML). Integraciones con ClaveÚnica vía OIDC broker.
- API Gateway opcional por dominios externos: Kong si necesitas políticas finas por consumidor.

Datos

- Relacional: PostgreSQL 16 como sistema fuente. Migraciones con Alembic. Particionamiento por IPR si escala.
- Vector search: pgvector en el mismo Postgres para simplificar ops (RAG, embeddings). Si crece: Qdrant.
- Búsqueda full-text: PostgreSQL FTS; si se queda corto, Meilisearch.
- Objetos/archivos: MinIO (S3 compatible) para expedientes, rendiciones, anexos, y blobs de OCR.
- NoSQL: evita por ahora. Usa JSONB en Postgres para esquemas flexibles.
- Data mart y BI: Metabase sobre réplicas de Postgres. DuckDB para análisis ad-hoc.

Automatización y orquestación

- Núcleo de flujos: n8n como orquestador único. Sin BPMN pesado.
- Patrones: eventos → n8n → FastAPI/Hasura → tareas Celery → notificaciones.
- Bus de eventos ligero: Redis Streams ahora; NATS si necesitas pub/sub real.
- Programación de trabajos: n8n cron. Para durables críticos, Celery beat.

Capa de IA y agentes

- LLMs: por API (OpenAI, Gemini, Anthropic, DeepSeek) + opción local en servidor con OpenWebUI cuando sea viable.
- Orquestación de agentes: n8n + herramientas dedicadas expuestas vía MCP (Model Context Protocol) desde FastAPI.
- RAG: indexación en MinIO + embeddings en pgvector; chunking con unstructured + heurísticas por tipo de documento.
- Reranking: Cohere/Jina/TEI si se requiere calidad extra.
- OCR: PaddleOCR + tesseract4 para fallback; pipeline unstructured-ingest para PDFs escaneados.
- Asistentes especializados:
- “Wizards” de postulación: formularios guiados React + validaciones server-side + llamadas a LLM para sugerencias y verificación normativa.
- Alertas inteligentes: features de progreso/atraso + modelos simples de clasificación/tiempo (scikit-learn, XGBoost). Entrenamiento offline; scoring en Celery; disparo de alertas vía n8n.
- Revisión de rendiciones: extractor + reglas deterministas + LLM verificador con checklist normativo; salida en “diff + rationale” trazable.
- Copilotos contextuales: OpenWebUI con herramientas MCP a endpoints de lectura segura (read-only) a Postgres/MinIO/Hasura y buscador RAG.
- Safety y gobernanza IA: prompts versionados en Git, pruebas de regresión de QA, filtros de datos sensibles en la capa MCP, logs de decisiones y justificaciones.

Interoperabilidad Estado

- PISEE, FirmaGob, otros: adaptadores en FastAPI; contratos OpenAPI firmes; n8n consume/expone endpoints según flujo.
- ClaveÚnica: broker en Keycloak.
- Gesdoc-Odoo: plan de “absorción”: extractores ETL a Postgres/MinIO + endpoints equivalentes; front reemplazado por Lowcoder/React; coexistencia temporal vía n8n.

Seguridad, cumplimiento y trazabilidad

- SSO obligatorio, MFA para roles críticos.
- ABAC/RBAC en Keycloak; scopes finos en API.
- Auditoría: logs estructurados (JSON) con Loki; métricas Prometheus; trazas OpenTelemetry.
- Cifrado en tránsito TLS; en reposo: discos y buckets con SSE-S3/ SSE-KMS (MinIO KMS simple) y columnas sensibles con pgcrypto.
- DLP mínima: reglas de masking en vistas SQL y en MCP tools.

DevEx, calidad y CI/CD

- Git + trunk-based + PR checks. Tests Pytest. Pre-commit hooks (ruff, mypy).
- Contenedores: Docker. Orquestación: Dokploy en Hetzner. Despliegues por servicio.
- Infra como código: Compose por servicio + stackfiles Dokploy; Terraform para Hetzner si se requiere.
- Versionado de datos: migraciones Alembic; versiones de prompts y flujos n8n en Git (export JSON).
- Feature flags: OpenFeature simple en backend.

Observabilidad

- Prometheus + Grafana. Loki para logs. Tempo para trazas. Alertmanager integrado a n8n para rutas de notificación.

Elecciones concretas de librerías

- FastAPI, SQLModel/SQLAlchemy 2, Alembic.
- Auth: python-jwt, fastapi-oauth2; cliente Keycloak.
- S3: minio-py. OCR: paddleocr, pytesseract. PDF: pypdf, unstructured.
- Embeddings: text-embeddings-inference o API del proveedor; pgvector.
- RAG server: FastAPI endpoints + herramientas MCP.
- Front: Next.js 14, Tailwind + DaisyUI, shadcn opcional para control fino.
- Low-code: Lowcoder/Appsmith para backoffice.
- n8n: nodos custom para FirmaGob, PISEE, ClaveÚnica, Hasura, FastAPI.

Topología de despliegue en Hetzner + Dokploy

- Nodos dedicados por dominio: edge (Traefik+WAF), app-api (FastAPI/Hasura), automación (n8n+Redis), datos (Postgres+pgvector, MinIO), observabilidad (Prometheus/Grafana/Loki/Tempo), ai-hub (OpenWebUI, TEI opcional).
- Backups: snapshots Hetzner + pg_dump/pgBackRest + versión de buckets MinIO.
- Alta disponibilidad gradual: réplicas de Postgres en read-only; Traefik con health-checks; Redis en modo persistente.

Rutas de evolución

- Empezar con Postgres único + pgvector + FTS. Añadir Qdrant/Meilisearch solo si hay cuello de botella.
- Mantener n8n como cerebro operativo. Evitar BPMN. Si algún flujo requiere “durable execution” avanzada, evaluar Temporal más adelante.
- Medir primero eficacia de RAG + reglas antes de entrenar modelos propios. (evitar)
- Sustituir poco a poco módulos de Gesdoc con servicios FastAPI hasta su apagado.

Esto te da: velocidad de construcción, control total on-prem/Hetzner, IA explotada en puntos de alto ROI, trazabilidad y seguridad estatales, y una vía clara de escalamiento sin complejizar antes de tiempo.
