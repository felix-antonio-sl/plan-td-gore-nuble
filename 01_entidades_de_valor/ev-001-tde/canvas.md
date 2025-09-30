# Canvas de Entidad de Valor: EV-001 - Plataforma TDE

_Versión 1.0_

---

## 1. Propósito (El Porqué)

Ayudar a los directivos y equipos del GORE Ñuble a orquestar y visualizar de punta a punta el ciclo de vida de la inversión pública y sus procesos de soporte para que puedan tomar decisiones oportunas y basadas en evidencia, acelerando la entrega de valor público a la ciudadanía.

---

## 2. Clientes / Usuarios (El Para Quién)

- **La Autoridad de Gobierno Regional:** (Gobernador/a, Administrador/a). Necesita visión estratégica y alertas sobre nudos críticos.
- **El Gestor de Cartera Institucional:** (Jefes de División). Necesita supervisión proactiva del portafolio y predicción de cuellos de botella.
- **El Analista de Ciclo de Inversión:** (Profesionales de divisiones). Necesita una fuente única de verdad para ejecutar sus tareas sin reprocesos.
- **El Actor de Control y Fiscalización:** (CORE, Control Interno, Ciudadanía). Necesita transparencia y capacidad de auditoría autónoma.
- **La Entidad Formuladora Externa:** (Municipios, Servicios Públicos). Necesita certidumbre y visibilidad sobre el estado de sus postulaciones.

---

## 3. Capacidades Clave (El Qué)

1. **Expediente Digital Único (EDU):** Fuente única, inmutable y auditable de verdad para cada iniciativa.
2. **Orquestación del Ciclo de Vida:** Modelado y automatización de flujos de trabajo, tareas y plazos.
3. **Gobernanza Estratégica y Analítica:** Dashboards, KPIs y reportes en tiempo real sobre la salud del portafolio.
4. **Gestión Financiera y Presupuestaria:** Trazabilidad del flujo financiero, desde la asignación hasta la rendición.
5. **Portal de Colaboración y Transparencia:** Interfaz digital para postulación y consulta de entidades externas y ciudadanía.
6. **Interoperabilidad Sistémica del Estado:** Conexión nativa con sistemas transversales (SNI, Mercado Público, SIGFE, etc.).

---

## 4. Métricas de Éxito / OKRs (Año 1)

- **KR 1 (Velocidad):** Reducir en un 40% el tiempo promedio del ciclo interno de la inversión (admisibilidad a convenio).
- **KR 2 (Eficiencia):** Disminuir en un 60% la tasa de devolución de expedientes por observaciones entre divisiones.
- **KR 3 (Adopción):** Lograr que el 80% de la cartera de inversión vigente sea gestionada como Expediente Digital Único (EDU).

---

## 5. Guardrails / Restricciones (Las Reglas)

1. **Sujeción a la Realidad Presupuestaria:** El diseño debe modelar el presupuesto anual, sus clasificadores y glosas.
2. **Respeto a la Dualidad Institucional:** La plataforma debe servir tanto a la gestión del Ejecutivo como a la fiscalización del CORE.
3. **Diseño Centrado en el Ecosistema:** La experiencia del usuario externo (municipios) es tan importante como la interna.
4. **Conformidad con el Marco Jurídico-Digital:** Cumplimiento estricto con Ley 21.180, Res. 30 CGR, normas de ciberseguridad e interoperabilidad (PISEE, ClaveÚnica).

---

## 6. Solución Técnica / Arquitectura (El Cómo)

- **Stack:** Autoalojado, basado en contenedores (Docker).
- **Frontend:** React + Next.js + Tailwind CSS/DaisyUI.
- **Backend:** FastAPI/FLASK (Python) exponiendo APIs REST/GraphQL.
- **Base de Datos:** PostgreSQL con extensiones pgvector (para RAG) y uso de JSONB.
- **Almacenamiento de Objetos:** MinIO (S3 Compatible).
- **Orquestación:** n8n como motor de automatización y flujos de trabajo / MCP
- **Inteligencia Artificial:**
  - LLMs vía API y/o locales (OpenWebUI) para copilotos y asistentes.
  - OCR (PaddleOCR) para digitalización de documentos.
  - RAG (Retrieval-Augmented Generation) para consultas sobre base documental.
- **Autenticación:** Keycloak para gestión de identidades y SSO.
- **Infraestructura:** Servidores dedicados (ej. Hetzner) con Dokploy para despliegue.

---

## 7. Primer Esqueleto Andante (El Primer Paso)

- **Foco del Primer Trimestre:** Construir la versión mínima viable de las siguientes dos capacidades:
    1. **Expediente Digital Único (EDU):** Implementar el modelo de datos central en PostgreSQL y la API en FastAPI para crear, leer y actualizar un expediente básico con sus metadatos y documentos asociados (en MinIO).
    2. **Orquestación del Ciclo de Vida:** Configurar en n8n el flujo de trabajo más simple y crítico (ej. "Admisibilidad de Iniciativa"), que mueva el estado del EDU y notifique a los usuarios.
- **Valor a Entregar:** Validar la arquitectura base y entregar una primera victoria al `Analista de Ciclo de Inversión`, eliminando la necesidad de carpetas en red y correos para el primer eslabón de la cadena.
