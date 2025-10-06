# Anexo E: Gestión de Datos

ID: PTD-ANEXO-E-DATOS-01
Version: 1.0.0
Status: Published
Parent-Document: plan_td_gore_nuble_2026-2028.md
Creation-Date: 2025-10-06
Ref-STS-Guide: GUIDE-STS-MASTER-01

---

## E.1. Política de Gobierno de Datos del GORE Ñuble

ID: PTD-DATOS-POLITICA-01

Fnd: Marco de Referencia de Gestión de Datos del Estado (MGDE), Estrategia de Datos del Estado, Ley 21.719.

### Principios Rectores

El GORE Ñuble reconoce los datos como un **activo estratégico** fundamental para la toma de decisiones, la provisión de servicios y el cumplimiento de su misión de desarrollo regional. Esta Política establece el marco de gobernanza para asegurar que los datos sean:

- **De alta calidad:** Exactos, completos, actuales y confiables.
- **Accesibles:** Disponibles para quienes los necesitan, respetando restricciones de privacidad y seguridad.
- **Interoperables:** Estructurados según estándares que permiten su integración y reutilización.
- **Seguros:** Protegidos contra accesos no autorizados, pérdidas o alteraciones.
- **Gobernados:** Con roles claros de responsabilidad y procesos definidos de gestión.

### Principio 1: Los Datos Deben Mejorar los Servicios a las Personas

Todo esfuerzo de gestión de datos debe orientarse a mejorar directamente la calidad, accesibilidad o eficiencia de los servicios públicos que el GORE provee a la ciudadanía.

### Principio 2: Los Datos son Activos Estratégicos con Dueños y Custodios

Req: Todo dataset, indicador o producto de datos crítico del GORE debe tener:

- **Dueño del Dato:** Funcionario responsable de la calidad, actualización y gobernanza del dato (usualmente un Jefe de División o profesional senior).
- **Custodio del Dato:** Funcionario responsable de los aspectos técnicos (almacenamiento, acceso, seguridad).

### Principio 3: Catalogación y Documentación Obligatoria

Req: Todo dataset institucional debe estar inventariado en el **Catálogo Maestro de Datos del GORE** con metadatos estandarizados (descripción, dueño, fuente, frecuencia de actualización, clasificación de seguridad).

### Principio 4: Calidad de Datos como Responsabilidad Continua

Req: Los Dueños de Datos deben evaluar y reportar la calidad de sus datos trimestralmente (completitud, exactitud, frescura). Los datos de baja calidad deben ser mejorados o, si no es posible, claramente etiquetados con advertencias.

### Principio 5: Interoperabilidad y Reutilización

Req: Los datos deben capturarse una sola vez y reutilizarse múltiples veces. Se promoverá activamente la interoperabilidad interna (entre divisiones) y externa (con otros organismos vía Red de Interoperabilidad).

### Principio 6: Apertura por Defecto (Datos Abiertos)

Fnd: Estrategia de Gobierno Digital 2030, Carta Internacional de Datos Abiertos.

Req: Todo dato que no esté sujeto a restricciones legales (privacidad, seguridad, propiedad intelectual) debe publicarse proactivamente como dato abierto en formatos estándar (CSV, JSON, GeoJSON).

### Principio 7: Privacidad y Seguridad desde el Diseño

Fnd: Ley 21.719, Norma Técnica de Seguridad (DS N°7).

Req: El diseño de todo sistema de datos debe integrar desde el inicio medidas de protección de privacidad (minimización, anonimización cuando sea posible) y seguridad (cifrado, control de acceso, auditoría).

### Principio 8: Uso Ético de Datos

Req: Todo uso de datos, especialmente para IA, debe someterse a evaluación ética. Se prohíbe el uso de datos que pueda resultar en discriminación, vulneración de derechos o afectación desproporcionada de grupos vulnerables.

---

## E.2. Catálogo de Datasets Críticos del GORE

ID: PTD-DATOS-CATALOGO-01

### Propósito del Catálogo

El Catálogo Maestro de Datos es el inventario oficial de todos los datasets institucionales del GORE Ñuble. Actúa como la "fuente única de verdad" sobre qué datos existen, dónde residen, quién es responsable y cómo acceder a ellos.

### Estructura del Catálogo (Metadatos Obligatorios)

Por cada dataset, el catálogo registra:

| Campo | Descripción | Ejemplo |
|:---|:---|:---|
| **ID del Dataset** | Identificador único | DS-GORE-001 |
| **Nombre** | Nombre descriptivo | Cartera de Inversión FNDR 2024-2026 |
| **Descripción** | Resumen de contenido y propósito | Registro completo de proyectos y programas financiados con FNDR, con estado de avance físico-financiero. |
| **Dueño del Dato** | Nombre y cargo del responsable | Juan Parada, Jefe DIPIR |
| **Custodio Técnico** | Responsable técnico | María López, Analista de Datos DIPIR |
| **Fuente Primaria** | Sistema/proceso que genera el dato | NEXO GORE (Módulo IPR) + BIP + SIGFE |
| **Formato** | Estructura del dato | Tabla relacional (PostgreSQL), exportable a CSV/JSON |
| **Frecuencia de Actualización** | Con qué periodicidad se actualiza | Diaria (sync automática nocturna) |
| **Clasificación de Seguridad** | Público / Reservado / Sensible | Público (salvo datos de beneficiarios) |
| **Clasificación de Privacidad** | Contiene datos personales? | Sí (nombres de beneficiarios) → anonimizar para publicación |
| **Fecha de Creación** | Cuándo se creó el dataset | 01/01/2024 |
| **Última Actualización** | Cuándo se modificó por última vez | 05/10/2025 |
| **Ubicación** | Dónde reside físicamente | Servidor NEXO GORE, base de datos `gore_ipr`, tabla `proyectos` |
| **URL de Acceso** | Enlace (si es público o tiene API) | <https://api.gorenuble.cl/ipr> (autenticada) |
| **Licencia** | Términos de uso (si es abierto) | CC BY 4.0 (versión anonimizada) |
| **Datasets Relacionados** | Dependencias o derivados | Vinculado a DS-GORE-002 (Presupuesto), DS-GORE-015 (Georreferenciación) |

### Datasets Críticos (Inventario Inicial H1)

| ID | Nombre | Dueño | Clasif. Seguridad | Clasif. Privacidad | Estado (H1) |
|:---|:---|:---|:---|:---|:---|
| **DS-001** | Cartera de Inversión FNDR | DIPIR | Público | Sí (beneficiarios) | A crear en NEXO GORE |
| **DS-002** | Registro Presupuestario GORE | DAF | Público | No | Integración con SIGFE |
| **DS-003** | Rendiciones de Cuentas | DAF | Reservado | Sí | Integración con SISREC |
| **DS-004** | Límites Administrativos | DIPLADE | Público | No | Publicado en IDE Ñuble |
| **DS-005** | Red Vial Regional | DIPLADE | Público | No | Publicado en IDE Ñuble |
| **DS-006** | Riesgos Naturales | DIPLADE | Público | No | Publicado en IDE Ñuble |
| **DS-007** | Reportes de Emergencias Ciudadanas | CIES | Reservado | Sí (reportante) | A crear en CIES |
| **DS-008** | Beneficiarios 8% FNDR | DIDESOH | Reservado | Sí | A crear en NEXO GORE |
| **DS-009** | Indicadores Socioeconómicos Ñuble | DIPLADE | Público | No (agregado) | A compilar |

---

## E.3. Estándares de Metadatos

ID: PTD-DATOS-ESTANDARES-METADATOS-01

### E.3.1. Metadatos para Datasets Generales (No Geoespaciales)

Fnd: Estándares para Apertura y Reutilización de Datos Abiertos (kb_tde_062_std_datos_abiertos_sts.md), DCAT (Data Catalog Vocabulary).

Req: Todo dataset publicado como dato abierto o catalogado internamente debe tener metadatos conformes a DCAT, con los siguientes campos mínimos:

**Nivel Conjunto de Datos:**

- Identificador (obligatorio).
- Título (obligatorio).
- Descripción (obligatorio).
- Autor / Dueño del Dato (obligatorio).
- Correo de contacto (obligatorio).
- OAE Asociado: Gobierno Regional de Ñuble (obligatorio).
- Categoría Temática (obligatorio): Ej. Inversión Pública, Ordenamiento Territorial, Desarrollo Social.
- Palabras Clave (obligatorio).
- Fecha de Creación (obligatorio).
- Fecha de Publicación (obligatorio).
- Licencia (obligatorio): CC BY 4.0 para datos abiertos, o especificar restricciones.
- Frecuencia de Actualización (recomendado).
- Cobertura Geográfica: Región de Ñuble (recomendado).

**Nivel Recurso (Archivo):**

- Título del archivo (obligatorio).
- Descripción (obligatorio).
- Formato (obligatorio): CSV, JSON, GeoJSON, PDF, etc.
- URL de descarga directa (recomendado).
- Tamaño del archivo (recomendado).
- Diccionario de Variables (obligatorio si es tabla): Nombre de columna, tipo de dato, descripción.

### E.3.2. Metadatos para Datos Geoespaciales

Fnd: ISO 19115 (Metadatos Geográficos), Normas ISO/TC 211.

Req: Todo dataset geoespacial publicado en IDE Ñuble debe tener metadatos ISO 19115 completos, incluyendo:

**Metadatos Obligatorios:**

- Identificador del Recurso.
- Título.
- Resumen (abstract).
- Punto de Contacto (organización, persona, email).
- Fecha de Creación / Publicación.
- Sistema de Referencia de Coordenadas (CRS): Ej. EPSG:4326 (WGS84), EPSG:32719 (UTM 19S).
- Extensión Geográfica (bounding box): Límites de la región de Ñuble.
- Linaje: Descripción de la fuente y proceso de creación del dato.
- Restricciones de Uso: Licencia, restricciones legales.

**Metadatos Recomendados:**

- Resolución Espacial / Escala.
- Precisión Posicional.
- Fecha de Última Actualización.
- Palabras Clave Temáticas.

**Formato de Codificación:**

- XML conforme a ISO 19139.
- Publicado en servicio CSW (Catalog Service for the Web) de Geonodo.

---

## E.4. Guía de Anonimización y Seudonimización de Datos

ID: PTD-DATOS-ANONIMIZACION-01

Fnd: Guía de Anonimización de Datos (kb_tde_080_guia_anonimizacion_sts.md), Ley 21.719.

### Cuándo Anonimizar o Seudonimizar

Req: Se debe aplicar anonimización o seudonimización en los siguientes casos:

1. **Publicación de Datos Abiertos:** Toda publicación de datasets que originalmente contenían datos personales.
2. **Compartición Inter-Institucional:** Datos compartidos con otros organismos para fines distintos a los originales (salvo autorización del titular).
3. **Entrenamiento de Modelos de IA:** Datasets utilizados para entrenar/validar modelos de IA (salvo que el procesamiento sea estrictamente necesario y esté autorizado).
4. **Uso Interno para Análisis:** Datos compartidos internamente entre divisiones para análisis estadístico donde la identidad individual no es necesaria.

### Técnicas Aplicables (Resumen)

**Anonimización (Irreversible):**

- Objetivo: Que sea razonablemente imposible re-identificar a las personas.
- Técnicas:
  - **Supresión de Identificadores Directos:** Eliminar nombre, RUT, dirección exacta.
  - **Generalización (K-anonimidad):** Agrupar valores (ej. edad exacta → rango etario, comuna → provincia).
  - **Adición de Ruido:** Modificar ligeramente valores numéricos para disociar (ej. agregar ±5% aleatorio a ingresos).
  - **Agregación:** Publicar solo estadísticas agregadas (promedios, sumas) en lugar de registros individuales.

**Seudonimización (Reversible bajo control):**

- Objetivo: Reemplazar identificadores por códigos, manteniendo una tabla de correspondencia segura para re-identificación controlada.
- Técnica:
  - **Tokenización:** Reemplazar RUT por token aleatorio (ej. RUT "12345678-9" → Token "A7F3K9M2").
  - Req: La tabla RUT ↔ Token se almacena cifrada, con acceso restringido solo a DPO y funcionarios autorizados.
- Uso: Cuando se necesita vincular registros de una persona en distintas bases de datos para análisis longitudinal, pero sin revelar identidad en el análisis.

### Protocolo de Anonimización para Publicación de Datos Abiertos

**Paso 1: Clasificación de Atributos**

- Para cada columna del dataset:
  - ¿Es identificador directo? (RUT, nombre) → **Eliminar o seudonimizar**.
  - ¿Es identificador indirecto o cuasi-identificador? (edad exacta, comuna + profesión) → **Generalizar o permutar**.
  - ¿Es atributo objetivo? (monto de subsidio, sector de inversión) → **Mantener** (es la información de valor).

**Paso 2: Aplicación de Técnicas**

- Eliminar identificadores directos.
- Generalizar cuasi-identificadores (ej. edad → rango, comuna → provincia si la comuna tiene <5.000 hab).
- Evaluar: Aplicar K-anonimidad (K>=5): Cada registro debe ser indistinguible de al menos 4 otros.

**Paso 3: Evaluación de Riesgo de Re-Identificación**

- Pregunta: Si cruzo este dataset con información pública disponible (ej. redes sociales, registros públicos), ¿podría re-identificar a alguien?
- Si riesgo es alto: Aplicar técnicas adicionales o incrementar K.

**Paso 4: Documentación**

- Crear metadato "Proceso de Anonimización Aplicado" explicando qué se hizo.
- Advertencia en dataset: "Datos anonimizados conforme a Ley 21.719. Prohibido intentar re-identificar personas."

**Paso 5: Validación del DPO**

- El DPO revisa y aprueba el proceso de anonimización antes de publicar.

### Herramientas Recomendadas

- **ARX Data Anonymization Tool:** Software de código abierto, soporta K-anonimidad, L-diversidad. URL: <https://arx.deidentifier.org/>
- **Amnesia:** Herramienta local para anonimización. URL: <https://amnesia.openaire.eu/>

---

## E.5. Política de Datos Abiertos

ID: PTD-DATOS-ABIERTOS-POLITICA-01

Fnd: Estándares para Apertura y Reutilización de Datos Abiertos (kb_tde_062_std_datos_abiertos_sts.md).

### Compromiso de Apertura

El GORE Ñuble se compromete a publicar proactivamente datos de interés público como **datos abiertos**, facilitando su acceso, uso y reutilización por la ciudadanía, academia, sector privado y otros organismos.

### Criterios de Publicación

**Datos que DEBEN publicarse como abiertos (obligatorio):**

1. Cartera de proyectos de inversión FNDR (versión anonimizada, sin datos personales de beneficiarios).
2. Ejecución presupuestaria del GORE (agregada por programa, subtítulo, ítem).
3. Resultados de concursos públicos (8% FNDR, FRPD) - adjudicatarios y montos (datos ya públicos por Ley 19.862).
4. Datos geoespaciales base (límites, red vial, hidrografía, riesgos).
5. Indicadores de desarrollo regional (socioeconómicos, de gestión).
6. Acuerdos del CORE (ya obligatorio por Ley 20.285, facilitar acceso vía datos estructurados).

**Datos que NO se publican (restricciones):**

- Datos personales sin anonimizar (protegidos por Ley 21.719).
- Datos clasificados como Reservados o Secretos (Ley 20.285).
- Datos que puedan afectar seguridad, investigaciones en curso, propiedad intelectual de terceros.

### Formatos Obligatorios

Fnd: Clasificación de formatos según kb_tde_062_std_datos_abiertos_sts.md.

**Para Datos Tabulares:**

- **CSV** (formato preferido, delimitador coma, codificación UTF-8).
- Adicional: JSON o XML si la estructura es jerárquica.

**Para Datos Geoespaciales:**

- **GeoJSON** (formato preferido).
- Adicional: Servicios OGC (WMS, WFS) desde IDE Ñuble.

**Para Documentación Administrativa:**

- **PDF** (para documentos oficiales que acompañan datasets).

### Licenciamiento

Req: Licencia predeterminada para datos abiertos del GORE: **Creative Commons BY 4.0 (CC-BY-4.0)**.

- Permite: Uso libre, redistribución, creación de obras derivadas.
- Req: Atribución al GORE Ñuble como fuente.

### Plataforma de Publicación

Mech: Los datos abiertos del GORE se publicarán en:

1. **datos.gob.cl** (Portal Nacional de Datos Abiertos, obligatorio).
2. **Observatorio Ñuble 250** (sección de datos abiertos del GORE).

Proc:

- El Dueño del Dato prepara el dataset anonimizado y metadatos.
- El DPO valida que la anonimización es adecuada.
- El Coord. TD publica en datos.gob.cl y Observatorio.
- Actualización: Según frecuencia declarada en metadatos (mínimo anual).

---

## E.6. Arquitectura de Datos: Repositorio Único de Conocimiento (RUC)

ID: PTD-DATOS-RUC-ARQUITECTURA-01

### Propósito del RUC

El **Repositorio Único de Conocimiento (RUC)** es la fuente única de verdad para todo el conocimiento institucional estructurado del GORE que alimenta a los asistentes de IA. No es una base de datos operacional, sino un **repositorio de conocimiento curado, versionado y catalogado** específicamente diseñado para ser consumido por IA mediante técnicas de RAG (Retrieval-Augmented Generation).

### Arquitectura del RUC

**Capa 1: Sistema de Archivos Versionado (Git)**

- Contenido: Artefactos de conocimiento en formato STS (Structured Telegraphic Style).
- Estructura de directorios:

  ```
  /ruc-gore-nuble/
    /dominios/
      /gn/ (Gobernanza y Normativa general)
        kb_gn_000_intro_gores.md
        kb_gn_018_gestion_prpto_sts.md
        ...
      /tde/ (Transformación Digital del Estado)
        kb_tde_060_regulacion_sts.md
        ...
      /ipr/ (Gestión de IPR)
        kb_ipr_001_ciclo_vida_sts.md
        ...
    /catalogos/
      catalog_master_kb_gn_sts.md
      catalog_master_kb_tde_sts.md
  ```

- Control de versiones: Git (GitHub o GitLab institucional).
- Proceso de actualización: Según Protocolo de 6 fases (Sourcing, Staging, Audit, Publishing, Registration, Maintenance).

**Capa 2: Base de Datos Vectorial (Embeddings)**

- Contenido: Representaciones vectoriales de los artefactos STS para búsqueda semántica.
- Tecnología: Pinecone (cloud) o ChromaDB (self-hosted).
- Proceso: Pipeline automático que detecta cambios en Git → genera embeddings → actualiza índice vectorial.

**Capa 3: Catálogo de Conocimiento**

- Contenido: Metadatos de cada artefacto (ID, versión, fuente primaria, fecha, responsable, estado).
- Tecnología: Base de datos relacional (PostgreSQL) o sistema de catálogo (CKAN adaptado).

### Flujo de Actualización de Conocimiento

1. **Sourcing:** Identificación de fuente de conocimiento (ley nueva, normativa actualizada, procedimiento modificado).
2. **Staging:** Creación/actualización de artefacto STS en rama de staging de Git.
3. **Audit:** Revisión de calidad (sintaxis STS, exactitud, completitud) por curador senior.
4. **Publishing:** Merge a rama main de Git → trigger de pipeline de embeddings.
5. **Registration:** Actualización de catálogo de conocimiento.
6. **Maintenance:** Monitoreo de vigencia, re-audit periódico (cada 6-12 meses según criticidad).

---

## E.7. Modelo Semántico Unificado (Glosario y Ontología)

ID: PTD-DATOS-MODELO-SEMANTICO-01

### Propósito

Garantizar que todos los sistemas, documentos y conversaciones del GORE utilicen una terminología consistente y definiciones inequívocas. Esto es crítico para:

- Interoperabilidad entre sistemas.
- Calidad de asistentes de IA (evitar ambigüedad).
- Claridad en comunicaciones ciudadanas.

### Glosario Maestro del GORE Ñuble (Extracto)

Fnd: kb_gn_014_glosario_gore_nuble_sts.md (referencial).

Req: Se establecerá un glosario formal con definiciones autorizadas de términos clave.

| Término | Definición Oficial | Fuente Legal/Técnica | Sinónimos Aceptados | Sinónimos Prohibidos |
|:---|:---|:---|:---|:---|
| **IPR** | Intervención Pública Regional: Término paraguas que engloba proyectos (IDI) y programas (PPR) financiados por el GORE. | kb_gn_019_gestion_ipr_sts.md | Iniciativa | "Proyecto" (ambiguo, no distingue de IDI) |
| **IDI** | Iniciativa de Inversión: Proyecto de gasto de capital (Subt. 31/33) evaluado por SNI. | DL 1.263, Art. 19 bis | Proyecto de Inversión | - |
| **PPR** | Programa Público Regional: Iniciativa de gasto corriente/mixto (Subt. 24) evaluada por DIPRES/SES o GORE. | Glosa 06, Ley de Presupuestos | Programa | - |
| **FNDR** | Fondo Nacional de Desarrollo Regional: Principal fuente de financiamiento de inversión regional. | Ley 19.175, Art. 74 | - | "Fondo Regional" (ambiguo) |
| **FRPD** | Fondo Regional para la Productividad y el Desarrollo: Recursos de Royalty Minero para innovación y competitividad. | Ley 21.591 | Fondo Royalty | - |
| **RS** | Recomendación Satisfactoria: Resultado positivo de evaluación técnico-económica del MDSF que habilita financiamiento de un proyecto. | SNI, MDSF | - | "Aprobación" (no es aprobación, es recomendación) |
| **RF** | Recomendación Favorable: Resultado positivo de evaluación de diseño de DIPRES/SES que habilita financiamiento de un programa de ejecución directa GORE. | Glosa 06, Of. Circ. 22 DIPRES | - | - |

Req: El glosario completo se mantiene como artefacto de conocimiento en el RUC y se publica en el Observatorio Ñuble 360 para consulta ciudadana.

### Ontología de Dominio IPR (Simplificada)

Def: Modelo conceptual que define las entidades principales del dominio de gestión de IPR y sus relaciones.

**Entidades Principales:**

- **IPR:** Entidad raíz.
  - Atributos: ID, nombre, tipo (IDI/PPR), estado, monto, etc.
  - Relaciones:
    - `tiene_un` Ejecutor (Municipio, Servicio Público, GORE).
    - `pertenece_a` Programa Presupuestario.
    - `se_financia_con` Fuente (FNDR, FRPD, Sectorial).
    - `contribuye_a` Trazo Ñuble 250.
    - `tiene_muchos` Hitos.
    - `genera_muchas` Rendiciones.

- **Ejecutor:** Entidad que implementa la IPR.
  - Atributos: RUT, nombre, tipo (Público/Privado).

- **Hito:** Evento o entregable dentro del ciclo de vida de IPR.
  - Atributos: nombre, fecha programada, fecha real, estado.

- **Rendición:** Documento de justificación de uso de fondos.
  - Atributos: período, monto rendido, estado (aprobada, observada, pendiente).
  - Relaciones: `corresponde_a` IPR, `revisada_por` Funcionario.

Req: Esta ontología se implementa como esquema de base de datos relacional en NEXO GORE, asegurando consistencia de datos.

---

## E.8. Protocolo de Calidad de Datos

ID: PTD-DATOS-CALIDAD-PROTOCOLO-01

Fnd: Marco MGDE, ISO 8000 (Calidad de Datos).

### Dimensiones de Calidad

Todo dataset crítico será evaluado trimestralmente según 6 dimensiones:

| Dimensión | Definición | Métrica | Meta |
|:---|:---|:---|:---|
| **Completitud** | % de campos obligatorios llenos (sin nulos) | (registros completos / total) * 100 | >=95% |
| **Exactitud** | % de datos correctos (validados contra fuente primaria) | Medido por auditoría de muestra aleatoria | >=98% |
| **Consistencia** | % de datos sin contradicciones entre sistemas | Medido por reglas de validación cruzada | 100% |
| **Frescura** | % de datos actualizados dentro del SLA | (registros actualizados / total) * 100 | >=90% |
| **Unicidad** | % de registros sin duplicados | (registros únicos / total) * 100 | 100% |
| **Validez** | % de datos que cumplen reglas de negocio y formatos | Medido por validaciones automáticas | >=99% |

### Reporte Trimestral de Calidad

Req: En cada CVC, los Dueños de Datos de datasets críticos reportan:

- Estado de las 6 dimensiones de calidad de su dataset.
- Problemas identificados y plan de mejora.

Res: Datasets con calidad <90% en dimensiones críticas se marcan como "en mejora" en el catálogo y se establecen alertas para sus consumidores.

---

**Fin del Anexo E**

Este anexo ha establecido la Política de Gobierno de Datos del GORE, el catálogo de datasets críticos con estándares de metadatos (generales e ISO para geoespaciales), la guía de anonimización/seudonimización, la política de datos abiertos, la arquitectura del Repositorio Único de Conocimiento, el modelo semántico unificado y el protocolo de calidad de datos.

Ref: Las estrategias de comunicación sobre datos y IA hacia la ciudadanía se encuentran en el Anexo F.
