# Stack propuesto para implementación ASTA-KORE

## Frontend

- Ciudadanos y municipios: React + Next.js SSR. Tailwind + DaisyUI. i18n, accesibilidad AA. Charts con Recharts.
- Backoffice interno rápido:
  - Opciones: Lowcoder/Appsmith para CRUD y tableros operativos.
  - Reemplazable gradualmente por React cuando haga falta.
- Chat UI unificado: OpenWebUI incrustado como “hub” de copilotos contextuales.

Backend

- API principal:
  - opciones:
    - FastAPI/Flask 3 (Python 3.x) con pydantic v2, uvicorn/gunicorn.
- Graph API: Hasura sobre PostgreSQL para GraphQL instantáneo donde convenga; si no, Strawberry GraphQL en FastAPI para esquemas curados.
- Tareas asíncronas: Celery + Redis (cola) para jobs pesados; alternatively RQ si quieres algo más simple.
- Gateway y edge: Traefik v3 (ingress, TLS, rate-limit, WAF con Coraza/OWASP CRS).
- IAM/SSO: Keycloak (OIDC/OAuth2, SAML). Integraciones con ClaveÚnica vía OIDC broker.
- API Gateway opcional por dominios externos: Kong si necesitas políticas finas por consumidor. 