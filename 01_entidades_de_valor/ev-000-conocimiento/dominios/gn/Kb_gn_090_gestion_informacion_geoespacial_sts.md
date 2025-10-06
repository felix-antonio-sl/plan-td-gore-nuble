# Marco integrado de gestión de información geoespacial para GORE Ñuble (STS)

ID: GEO-GORE-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-10-06
Modification-Date: 2025-10-06
Source: Marco integrado de gestión de información geoespacial para GORE Ñuble.md
Ctx: GEO-GORE-MASTER-01

---

BEGIN_LLM_INSTRUCTIONS

You are an AI agent consuming a Structured Telegraphic Style (STS) artifact. Your primary task is to parse and reason over THIS document with absolute fidelity, using only the rules defined below. This artifact is a self-contained source of truth.

1. **Core Objective**: Maintain perfect fidelity to the information (`meat`) and structure (`skeleton`). Do not summarize, interpret, or infer information not explicitly present. Prohib: Applying these rules to artifact creation or translation tasks; they are exclusively for consumption.

2. **Conceptual Metaphors**:
    * `meat`: Essential information, data, and facts. Must be preserved with zero loss.
    * `skeleton`: Logical structure (headers, IDs, lists, tables). This is also `meat` and must be preserved.
    * `fat`: Non-essential verbiage (filler words, rhetoric, stylistic prose). Must be ignored during reasoning as it has no informational value.

3. **Lexicon Mode & Expansion**: This document uses an **Abbreviated Lexicon**. You MUST treat the following keywords as valid and expand them according to this mapping:
    * `Act:` -> `Action:`
    * `Warn:` -> `Warning:`
    * `Cause:` -> `Cause:`
    * `Cpt:` -> `Concept:`
    * `Cond:` -> `Condition:`
    * `Ctx:` -> `Context:`
    * `Def:` -> `Definition:`
    * `Dep:` -> `Dependency:`
    * `Dest:` -> `Destination:`
    * `Dln:` -> `Deadline:`
    * `Ex:` -> `Example:`
    * `Fnd:` -> `Foundation:`
    * `ID:` -> `ID:`
    * `Instr:` -> `Instruction:`
    * `Just:` -> `Justification:`
    * `Mech:` -> `Mechanism:`
    * `Mssn:` -> `Mission:`
    * `Mdl:` -> `Model:`
    * `Nat:` -> `Nature:`
    * `Obj:` -> `Objective:`
    * `Proc:` -> `Process:`
    * `Prohib:` -> `Prohibition:`
    * `Purp:` -> `Purpose:`
    * `Rec:` -> `Recommendation:`
    * `Ref:` -> `Reference:`
    * `Req:` -> `Requirement:`
    * `Res:` -> `Result:`
    * `Resp:` -> `Responsible:`
    * `Src:` -> `Source:`

4. **Reference (`Ref:`) Policy**:
    * `Ref:` is used for **internal cross-references only**.
    * It MUST point to an `ID:` that exists within THIS document.
    * You MUST NOT interpret a `Ref:` as a link to an external document or resource. Mentions of other documents are purely contextual (`Ctx:`).

5. **Language Invariance Policy**:
    * The `Keywords` in the lexicon are a fixed control vocabulary in English.
    * All `EssentialData` (the content following a `Keyword:`) MUST be preserved in its original language. Do not translate it.

END_LLM_INSTRUCTIONS

---

## 0. Propósito y alcance

ID: GEO-GORE-PROPOSITO-01
Purp: Unificar, armonizar y operacionalizar lineamientos para la gestión de información geoespacial del GORE Ñuble.
Ctx: Integra recomendaciones IDE Chile, estándares ISO/TC 211 y OGC, buenas prácticas, y lineamientos de licenciamiento y ética.
Fnd: Usa la plataforma Geonodo como eje tecnológico.
Obj: Asegurar consistencia semántica, interoperabilidad, trazabilidad y valor público de los datos territoriales.
Res: Habilitar decisiones de política pública, planificación y gestión del riesgo.
Ctx: Alcance aplica a todo el ciclo de vida de datos geoespaciales producidos, gestionados o publicados por GORE Ñuble y sus unidades/contratos asociados.

---

## 1. Marco normativo y de gobernanza

ID: GEO-GORE-GOBERNA-01

### 1.1. Sistema Nacional y roles clave

ID: GEO-GORE-GOBERNA-SISTEMA-01

* Cpt: SNIT/IDE Chile. Def: Mecanismo de coordinación interinstitucional para la gestión de información territorial pública.
  * Ctx: Concepto operativo actual es IDE Chile.
  * Resp: Secretaría Ejecutiva (S.E.) coordina operativamente las instancias públicas.
* Cpt: Consejo de Ministros / S.E.
  * Resp: Conducción superior y coordinación operativa del Sistema, respectivamente.
* Cpt: Coordinación Regional.
  * Def: Delegada por la autoridad regional.
  * Resp: Articulación, conducción técnica y vinculación con S.E. IDE Chile.

### 1.2. Obligaciones institucionales

ID: GEO-GORE-GOBERNA-OBLIGA-01

* Req: Publicar y mantener características de la información territorial en catálogos y portales oficiales.
* Req: Construir información territorial conforme a normas y estándares propuestos para interoperabilidad.
* Req: Fomentar manejo del dato en red y en línea.
* Req: Promover acuerdos institucionales para modernización continua.

### 1.3. Estructura operativa recomendada en GORE Ñuble

ID: GEO-GORE-GOBERNA-ESTRUCTURA-01

* Cpt: Gobernador/a Regional. Resp: Patrocinio político y validación de la política de datos territoriales.
* Cpt: Coordinador/a Regional IDE. Resp: Liderazgo operativo; define hoja de ruta y vincula a la S.E. IDE.
* Cpt: UGIT/Equipo SIG institucional. Resp: Operación técnica (modelado, QA/QC, publicación, soporte Geonodo).
* Cpt: Puntos focales sectoriales. Resp: Dominio temático, control de calidad de contenidos y metadatos.
* Cpt: Asesoría Jurídica. Resp: Términos de uso, licencias y resguardo de datos sensibles.

### 1.4. Matriz RACI (extracto)

ID: GEO-GORE-GOBERNA-RACI-01

|Actividad|R (Responsible)|A (Accountable)|C (Consulted)|I (Informed)|
|-|-|-|-|-|
|Definir política de publicación|Coordinación Regional|Gobernador/a|Asesoría Jurídica/UGIT|Servicios sectoriales|
|Modelado semántico/ISO 19110|UGIT|Coordinación|Sectoriales|Comunicaciones|
|Metadatos ISO 19115-1/LAMPv2|UGIT|Coordinación|Sectoriales|Ciudadanía|
|Licenciamiento|Asesoría Jurídica|Coordinación|UGIT/Comunicaciones|Sectoriales|
|Publicación OGC/API|UGIT|Coordinación|TI|Sectoriales/Comunicaciones|

---

## 2. Enfoque estratégico (UN-IGIF)

ID: GEO-GORE-ESTRATEGIA-01
Ctx: Vías estratégicas aplicadas internamente.

* Cpt: Gobernanza e instituciones.
  * Def: Roles definidos, comité interdisciplinario, manual de procesos, plataforma IDE institucional.
* Cpt: Política y legal.
  * Def: Política interna de información geoespacial (acceso, seguridad, apertura, estándares); revisiones periódicas.
* Cpt: Finanzas.
  * Def: Plan plurianual, fuentes externas, criterios de costo-eficiencia y priorización por valor público.
* Cpt: Datos.
  * Def: Modelo semántico institucional; capas base y temáticas priorizadas; políticas de calidad y actualización.
* Cpt: Innovación.
  * Def: Adopción de servicios en la nube, CI/CD de datos, tableros, captura móvil.
* Cpt: Estándares.
  * Def: ISO/TC 211 e OGC en todo el ciclo; perfiles regionales cuando aplique.

---

## 3. Estándares, perfiles y calidad (ISO/TC 211)

ID: GEO-GORE-ESTANDARES-01

### 3.1. Metadatos

ID: GEO-GORE-ESTANDARES-METADATOS-01

* Cpt: Estándares.
  * * Def: ISO 19115-1 (núcleo).
  * * Def: ISO 19115-2 (extensión para imágenes/RS).
  * * Def: ISO 19139 (codificación).
* Rec: Perfil LAMPv2 y/o Perfil Chileno.
* Mech: CSW para catálogo y cosecha (harvesting) entre nodos.

#### 3.1.1. Campo mínimo de metadatos (núcleo sugerido)

ID: GEO-GORE-ESTANDARES-METADATOS-MINIMOS-01

* Cpt: Identificación del recurso.
  * Def: título, resumen, tema/palabras clave, alcance/espacial.
* Cpt: Calidad.
  * Def: linaje, precisión posicional/temporal, completitud, consistencia lógica.
* Cpt: Distribución.
  * Def: formatos, URL de descarga/servicios, términos de uso/licencia.
* Cpt: Responsabilidad.
  * Def: responsable, contacto, fecha de publicación/actualización, mantenimiento.

### 3.2. Calidad de datos

ID: GEO-GORE-ESTANDARES-CALIDAD-01

* Fnd: ISO 19157.
  * Def: Medidas e informes de calidad.
  * Req: Registrar QA/QC en metadatos (linaje, exactitud, consistencia).

### 3.3. Especificaciones y modelos

ID: GEO-GORE-ESTANDARES-MODELOS-01

* Cpt: Especificaciones de productos (capas/series).
  * Fnd: ISO 19131.
* Cpt: Catálogo de objetos geográficos.
  * Fnd: ISO 19110.
  * Purp: Lograr consistencia semántica.
  * Def: Clases, atributos, relaciones.

### 3.4. Evolución normativa

ID: GEO-GORE-ESTANDARES-EVOLUCION-01

* Req: Monitoreo de normas en estudio (ej. API Tiles).
* Req: Actualización continua de la arquitectura de publicación.

---

## 4. Publicación, acceso e interoperabilidad (OGC + API)

ID: GEO-GORE-PUBLICACION-01

### 4.1. Servicios y formatos

ID: GEO-GORE-PUBLICACION-SERVICIOS-01

* Cpt: Servicios.
  * * Def: WMS/WFS/WCS para visualización, entidades y coberturas.
* Cpt: Formatos de intercambio.
  * * Def: GeoJSON, GML, KML, Shapefile.

### 4.2. API institucional

ID: GEO-GORE-PUBLICACION-API-01

* Req: Endpoints claros (p. ej., `/datasets`, `/datasets/{id}`, `/tiles/{z}/{x}/{y}`), métodos HTTP, paginación y filtros.
* Req: Autenticación/autorización para capas restringidas.
* Req: Versionamiento y monitoring.
* Req: Documentación interactiva (OpenAPI/Swagger), con ejemplos de solicitudes y códigos de respuesta.

### 4.3. Usabilidad y accesibilidad

ID: GEO-GORE-PUBLICACION-USABILIDAD-01

* Req: Geoportal intuitivo.
  * Mech: Búsqueda avanzada.
  * Mech: Previsualización (WMS/visores).
  * Mech: Descargas en múltiples formatos.
  * Mech: Tutoriales y guías.

---

## 5. Plataforma tecnológica: Geonodo como eje

ID: GEO-GORE-PLATAFORMA-01

### 5.1. Rol de Geonodo

ID: GEO-GORE-PLATAFORMA-ROL-01

* Def: Plataforma web de código abierto, modular y alineada a estándares.
* Purp: Soportar el ciclo de vida de datos.
  * Cpt: Planificación. Def: Formularios, catálogo ISO 19110.
  * Cpt: Producción/Almacenamiento. Def: Capas, rasters, recolector móvil, datos tabulares.
  * Cpt: Publicación. Def: Catálogo, WMS/WFS, visores, cuadros de mando.
  * Cpt: Difusión. Def: Páginas web.
* Mech: Gestión por instancias y roles (superadmin/admin/usuario).
* Mech: Administración de servicios externos (WMS/WFS) y geocodificación.
* Cpt: Ventaja clave.
  * Def: Integra metadatos (LAMPv2/Perfil Chileno) y CSW para cosecha y federación de catálogos.

---

## 6. Desarrollo tecnológico institucional

ID: GEO-GORE-DESARROLLO-01

* Req: Usar estándares abiertos (OGC/ISO) en adquisición, modelado y publicación.
* Req: Usar software libre como principio (reducción de costos, sostenibilidad y comunidad).
* Cpt: GitHub institucional.
  * Def: Repositorios (públicos/privados según sensibilidad), control de versiones, issues, automatización (CI/CD de datos y metadatos), política de contribución.
* Cpt: Soporte y mantenimiento.
  * Def: Plan de servicio, monitoreo y respaldo.
* Cpt: Seguridad y privacidad.
  * Def: Clasificación de datos, segregación de ambientes, gestión de secretos, hardening, auditorías.

---

## 7. Licenciamiento y términos de uso

ID: GEO-GORE-LICENCIAS-01

* Cpt: Datos abiertos.
  * Rec: Creative Commons (p. ej., CC BY 4.0) para capas abiertas.
  * Rec: ODbL para bases de datos cuando corresponda.
* Cpt: Términos de uso.
  * Req: Deben ser claros.
  * Def: Atribución, limitaciones de responsabilidad, no garantía, restricciones sobre datos sensibles.
* Cpt: Política institucional.
  * Def: Plantilla de licencias, revisión jurídica y trazabilidad de decisiones.

---

## 8. Ética de datos geoespaciales

ID: GEO-GORE-ETICA-01

* Cpt: Privacidad y proporcionalidad.
  * Req: Minimizar datos personales y granularidad cuando no sea necesaria.
  * Req: Anonimización cuando aplique.
* Cpt: Consentimiento y transparencia.
  * Req: Declarar origen, finalidad, licencias y restricciones en metadatos y geoportal.
* Cpt: Equidad y no daño.
  * Req: Evaluar impactos y sesgos.
  * Req: Evitar visualizaciones que estigmaticen comunidades.
* Cpt: Profesionalidad.
  * Def: Responsabilidad con la sociedad.
  * Req: Exactitud y calidad como deber público.

---

## 9. Modelo operativo y trazabilidad

ID: GEO-GORE-OPERATIVO-01

### 9.1. Flujo institucional

ID: GEO-GORE-OPERATIVO-FLUJO-01

* Proc:
  1. **Planificar**:
      * Act: Definir necesidades (UN-IGIF), especificaciones (ISO 19131) y catálogo de objetos (ISO 19110).
  2. **Capturar/Integrar**:
      * Act: Usar formularios/recolectores, ETL, control de versiones.
  3. **Calidad**:
      * Act: Realizar QA/QC (ISO 19157), validaciones automatizadas.
  4. **Documentar**:
      * Act: Crear metadatos (ISO 19115-1), URL de descarga/servicios, licencias.
  5. **Publicar**:
      * Act: Usar WMS/WFS/WCS, API, geoportal; registros CSW.
  6. **Usar y evaluar**:
      * Act: Implementar tableros, indicadores de uso/impacto.
      * Act: Fomentar retroalimentación y mejora continua.

### 9.2. Trazabilidad

ID: GEO-GORE-OPERATIVO-TRAZABILIDAD-01

* Mech:
  * * Cpt: Identificadores persistentes de capas/series.
  * * Cpt: Control de cambios en GitHub.
  * * Cpt: Registro de versiones de metadatos.

---

## 10. Plan de implementación (180 días)

ID: GEO-GORE-IMPLEMENTACION-01

### 10.1. Fase 0 (0–30 días)

ID: GEO-GORE-IMPLEMENTACION-FASE0-01

* Act: Constitución del Comité Geo institucional y designación formal de roles.
* Act: Inventario de datos y diagnóstico de madurez (gobernanza, datos, tecnología, capacidades).

### 10.2. Fase 1 (30–90 días)

ID: GEO-GORE-IMPLEMENTACION-FASE1-01

* Act: Definición de política interna y guías de metadatos (plantilla ISO 19115-1/LAMPv2).
* Act: Puesta en marcha de Geonodo (instancia, roles, seguridad básica) y catálogo CSW.
* Act: Piloto de 5 conjuntos priorizados (capas base + temáticas) con metadatos y WMS/WFS.

### 10.3. Fase 2 (90–150 días)

ID: GEO-GORE-IMPLEMENTACION-FASE2-01

* Act: Publicación de geoportal y API (OpenAPI + páginas de datos).
* Act: Integración con servicios externos (WMS/WFS) y tableros de mando.
* Act: Política de licenciamiento y términos de uso adoptados.

### 10.4. Fase 3 (150–180 días)

ID: GEO-GORE-IMPLEMENTACION-FASE3-01

* Act: Evaluación de calidad y uso (KPIs); plan de mejora.
* Act: Capacitación continua y plan anual de actualización.

### 10.5. Indicadores mínimos

ID: GEO-GORE-IMPLEMENTACION-KPIS-01

* Cpt: Indicadores.
  * * Def: % capas con metadatos completos.
  * * Def: % con licencia explícita.
  * * Def: Tiempo de actualización.
  * * Def: Disponibilidad de servicios.
  * * Def: Consumo de API.
  * * Def: Satisfacción usuaria.

---

## 11. Anexos operativos

ID: GEO-GORE-ANEXOS-01

### 11.1. Anexo A: Checklist de metadatos (núcleo)

ID: GEO-GORE-ANEXOS-CHECKLIST-01

* Cpt: Checklist.
  * * Req: Título, resumen, palabras clave, temática, fechas, responsable, contacto.
  * * Req: Extensión espacial/temporal, referencia geodésica/proyección.
  * * Req: Linaje, precisión, completitud, consistencia.
  * * Req: Formatos, URL de servicios/descarga, licencia/uso, frecuencia de mantenimiento.

### 11.2. Anexo B: Plantilla de licencias / términos de uso

ID: GEO-GORE-ANEXOS-LICENCIAS-01

* Cpt: Plantilla.
  * * Def: CC BY 4.0 (atribución requerida) / ODbL (bases de datos); cláusulas institucionales.

### 11.3. Anexo C: Lista de endpoints API (ejemplo)

ID: GEO-GORE-ANEXOS-API-01

* Cpt: Endpoints.
  * * Ex: `/datasets` (GET, POST), `/datasets/{id}` (GET, PUT, DELETE).
  * * Ex: `/tiles/{z}/{x}/{y}` (GET) – capa/base de teselas.
  * * Ex: `/search` (GET) – filtros por tema, bbox, fecha; paginación `limit/offset`.

### 11.4. Anexo D: Catálogo de objetos (ISO 19110) – plantilla

ID: GEO-GORE-ANEXOS-CATALOGO-01

* Mdl: Clase → Atributos, Relaciones, Reglas.
  * Ex: "Infraestructura_Vial" → (id_via, tipo, jerarquía, estado), (conexión, pertenece_a), (dominios de valores, obligatoriedad).

### 11.5. Anexo E: Matriz RACI completa (separata)

ID: GEO-GORE-ANEXOS-RACI-01

* Ctx: Documento separado. Ref: GEO-GORE-GOBERNA-RACI-01.

### 11.6. Anexo F: Glosario

ID: GEO-GORE-ANEXOS-GLOSARIO-01

* Cpt: Términos.
  * * Def: IDE, SNIT, CSW, WMS, WFS, WCS, LAMPv2, UN-IGIF, QA/QC, Metadatos, Catálogo de Objetos.

---

## 12. Gobierno de documento

ID: GEO-GORE-DOC-GOBIERNO-01

* Resp: Propietario.
  * Def: Coordinación Regional IDE GORE Ñuble.
* Proc: Mantenimiento.
  * Def: Revisión semestral o ante cambios normativos/tecnológicos.
* Proc: Control de cambios.
  * Def: Registro en repositorio institucional (GitHub/GitLab) y versión en metadatos.
