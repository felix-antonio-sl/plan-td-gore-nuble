# Estándares y Guías de Buenas Prácticas

Estos documentos definen los estándares de calidad y las mejores prácticas que deben seguir los servicios y productos digitales del Estado.

## Marco de referencia de gestión de datos Estado

ID: GUIDE-STS-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_063_tde_guia_marco_datos.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 1. Fundamentos del MGDE

ID: GESTDAT-MGDE-FUNDAMENTOS-ROOT-01
Purp: Establecer el contexto, propósito y principios del Marco de Referencia de Gestión de Datos del Estado (MGDE).

#### 1.1. Propósito y Contexto

ID: GESTDAT-MGDE-FUNDAMENTOS-PROPOSITO-01

- Obj: Orientar a los Órganos de la Administración del Estado (OAE) en la adopción de buenas prácticas de gestión de datos usando el MGDE.
- Fnd: La gestión de datos es crítica para el éxito organizacional y la generación de valor público.
- Ref: OCDE - Dimensiones de un Gobierno Digital.
  - `- Digital por diseño.`
  - `- Impulsado por los datos.`
  - `- Actúa como plataforma.`
  - `- Abierto por defecto.`
  - `- Dirigido por el usuario.`
  - `- Proactivo.`
- Res: Beneficios de la Gestión de Datos.
  - `- Alinea la gestión de datos con objetivos estratégicos.`
  - `- Mejora la calidad del servicio y la eficiencia de los procesos.`
  - `- Disminuye el tiempo de diseño y desarrollo.`
  - `- Optimiza los costos del ciclo de vida.`
  - `- Define roles y responsabilidades.`
  - `- Facilita sinergias entre personas, procesos, información y tecnología.`
  - `- Homogeniza la comprensión en el Estado.`
- Fnd: Legal.
  - `- Ref: Ley N° 21.658 (Crea Secretaría de Gobierno Digital - SGD).
    - Mssn: Proponer la Estrategia de Gobierno Digital.
    - Mssn: Coordinar, asesorar y apoyar en el uso estratégico de tecnologías digitales, datos e información pública.`
  - `- Ref: Ley N° 18.575 (Orgánica constitucional de bases generales de la administración del Estado).
    - Def: Define a los OAE.`

#### 1.2. Principios Orientadores

ID: GESTDAT-MGDE-PRINCIPIOS-01
Purp: Definir los principios base que orientan las prácticas de gestión de datos.
Req: Los OAEs deben suscribir e incluir estos principios en su política de gobernanza de datos.

- Cpt: Principio 1. Req: La gestión de datos debe mejorar los servicios a las personas.
- Cpt: Principio 2. Req: Los datos (internos/externos) son activos estratégicos para metas y objetivos institucionales, incluyendo documentos y otros contenidos digitales.
- Cpt: Principio 3. Req: Todo activo/conjunto de datos será catalogado y documentado con metadatos.
- Cpt: Principio 4. Req: Todo activo/conjunto de datos tendrá un responsable (administrador/custodio) para velar por su actualización, mantenimiento, confiabilidad, precisión, completitud y disponibilidad.
- Cpt: Principio 5. Req: Se promoverá la digitalización, el uso analítico y el trabajo colaborativo en torno a los datos.
- Cpt: Principio 6. Req: Se promoverá la evaluación de la calidad de los datos.
- Cpt: Principio 7. Req: Se promoverá la interoperabilidad de los datos (interna/externa).
- Cpt: Principio 8. Req: Se procurará un uso ético de datos, cumpliendo la normativa vigente (especialmente protección de datos personales).
- Cpt: Principio 9. Req: El acceso a datos debe tener roles y responsabilidades definidos en el contexto de la seguridad institucional.
- Cpt: Principio 10. Req: La gestión de datos se planificará, implementará, evaluará y mejorará de forma integral y continua.

#### 1.3. Ciclo de Vida de los Datos

ID: GESTDAT-MGDE-CICLOVIDA-01
Purp: Describir las 8 etapas del ciclo de vida de los datos.

- Cpt: Etapa 1 - Generación. Def: Creación de datos dentro o fuera de la organización.
- Cpt: Etapa 2 - Recolección. Def: Captura de datos (formularios, apps, interoperabilidad, streaming).
- Cpt: Etapa 3 - Procesamiento. Def: Conversiones, compresión, encriptación.
- Cpt: Etapa 4 - Almacenamiento. Def: Guardado de datos para uso posterior.
- Cpt: Etapa 5 - Administración. Def: Gestión de calidad, seguridad y acceso.
- Cpt: Etapa 6 - Análisis. Def: Uso de datos para obtener conocimiento y tomar decisiones (requiere consolidación, resumen, modelos: ciencia de datos, minería de datos, IA, etc.).
- Cpt: Etapa 7 - Visualización. Def: Representaciones gráficas para facilitar la comprensión.
- Cpt: Etapa 8 - Interpretación. Def: Entendimiento de datos para la toma de decisiones.

### 2. Dimensiones y Criterios del MGDE

ID: GESTDAT-MGDE-DIMENSIONES-ROOT-01
Purp: Organizar las buenas prácticas del MGDE en 12 dimensiones, evaluadas por criterios.
Ctx: Cada criterio se evalúa con una o más preguntas (52 en total) para determinar el nivel de madurez.

#### 2.1. Resumen de Dimensiones

ID: GESTDAT-MGDE-DIMENSIONES-RESUMEN-01
Purp: Tabla resumen de las 12 dimensiones del MGDE.

|Dimensión|N° Criterios|N° Preguntas|
|---|---|---|
|Visión estratégica|7|7|
|Gobernanza de datos|7|7|
|Arquitectura, diseño y documentación|4|6|
|Almacenamiento y operación|1|1|
|Seguridad y ciberseguridad de datos|4|6|
|Integración e interoperabilidad|2|4|
|Documentos y contenidos|4|4|
|Datos maestros y de referencia|3|3|
|Analítica e inteligencia de negocios|3|3|
|Calidad de datos|2|2|
|Datos abiertos|3|7|
|Aspectos legales y normativos|2|2|

#### 2.2. Detalle de Dimensiones

ID: GESTDAT-MGDE-DIMENSIONES-DETALLE-01
Purp: Descripción de cada una de las 12 dimensiones del MGDE.

##### 2.2.1. Visión estratégica

ID: GESTDAT-MGDE-DIM-VISION-01
Purp: Generar compromiso institucional con la gestión de datos, alineada a objetivos y con visión de largo plazo.
Cpt: Criterios.

- `- Visión`
- `- Estrategia`
- `- Presupuesto y recursos`
- `- Capacidades`
- `- Gestión del cambio`
- `- Alianzas y colaboraciones`
- `- Medición y seguimiento`

##### 2.2.2. Gobernanza de datos

ID: GESTDAT-MGDE-DIM-GOBERNANZA-01
Purp: Definir visión, políticas y estrategias para potenciar los datos como activos organizacionales.
Cpt: Criterios.

- `- Política de gobernanza de datos`
- `- Organización`
- `- Implementación`
- `- Herramientas`
- `- Capacitación`
- `- Gestión de riesgos`
- `- Gestión ética de datos`

##### 2.2.3. Arquitectura, diseño y documentación

ID: GESTDAT-MGDE-DIM-ARQUITECTURA-01
Purp: Establecer modelos, documentos y metadatos que describen las estructuras y conjuntos de datos.
Cpt: Criterios.

- `- Arquitectura Institucional de datos`
- `- Catálogo de datos`
- `- Modelos y Documentación`
- `- Metadatos`
Def: Catálogo de Datos. Herramienta para crear y administrar el inventario de activos de datos de una organización. Maneja metadatos para describir/clasificar y capacidades de búsqueda para encontrar/acceder a la información.
Ex: Herramientas. CKAN (código abierto), Magda (código abierto, federado), y otras soluciones de fabricantes de software.

##### 2.2.4. Almacenamiento y operación

ID: GESTDAT-MGDE-DIM-ALMACENAMIENTO-01
Purp: Implementar y operar las plataformas de gestión de datos.
Cpt: Criterios.

- `- Gestión de la operación y almacenamiento`

##### 2.2.5. Seguridad y ciberseguridad de datos

ID: GESTDAT-MGDE-DIM-SEGURIDAD-01
Purp: Gestionar la privacidad, confidencialidad y el acceso apropiado a los datos.
Cpt: Criterios.

- `- Seguridad`
- `- Ciberseguridad`
- `- Protección de Datos Personales`
- `- Recuperación ante desastres`

##### 2.2.6. Integración e interoperabilidad

ID: GESTDAT-MGDE-DIM-INTEROP-01
Purp: Definir e implementar mecanismos para la integración y transferencia de datos (interna/externa).
Cpt: Criterios.

- `- Integración`
- `- Interoperabilidad`

##### 2.2.7. Documentos y contenidos

ID: GESTDAT-MGDE-DIM-DOCS-01
Purp: Establecer políticas y herramientas para datos no estructurados (documentos, etc.).
Cpt: Criterios.

- `- Definiciones`
- `- Metadatos`
- `- Expediente Electrónico`
- `- Repositorio Documental`

##### 2.2.8. Datos maestros y de referencia

ID: GESTDAT-MGDE-DIM-MAESTROS-01
Purp: Estandarizar codificaciones y centralizar información relevante intra e interinstitucional.
Cpt: Criterios.

- `- Datos referenciales`
- `- Datos maestros`
- `- Herramientas`

##### 2.2.9. Analítica e inteligencia de negocios

ID: GESTDAT-MGDE-DIM-ANALITICA-01
Purp: Gestionar el análisis de datos (descriptivo, diagnóstico, predictivo, prescriptivo) como apoyo a la toma de decisiones.
Cpt: Criterios.

- `- Toma de decisiones basada en información`
- `- Información de gestión`
- `- Herramientas`
Def: Data Mart. Subconjunto de bodega de datos enfocado en una línea de negocio, departamento o área temática particular.
Def: Data Lake. Repositorio centralizado para ingerir, almacenar y procesar grandes volúmenes de datos en su formato original.
Def: Data Warehouse. Repositorio centralizado que almacena datos estructurados y semiestructurados con fines de informes y análisis.

##### 2.2.10. Calidad de datos

ID: GESTDAT-MGDE-DIM-CALIDAD-01
Purp: Establecer metodologías y herramientas para definir, controlar y mejorar la calidad de los datos.
Cpt: Criterios.

- `- Definición`
- `- Metodología y Herramientas`

##### 2.2.11. Datos abiertos

ID: GESTDAT-MGDE-DIM-ABIERTOS-01
Purp: Definir e implementar procedimientos y herramientas para la publicación de datos abiertos.
Ref: Carta Internacional de Datos Abiertos.
Ref: DA-ESTANDAR-ROOT-01.
Cpt: Principios Carta Internacional Datos Abiertos.

- `- Principio 1: Abierto por defecto.`
- `- Principio 2: Oportuno y completo.`
- `- Principio 3: Accesible y utilizable.`
- `- Principio 4: Comparable e interoperable.`
- `- Principio 5: Para una mejor gobernanza y participación ciudadana.`
- `- Principio 6: Para el desarrollo inclusivo y la innovación.`
Cpt: Criterios de Evaluación.
- `- Definiciones`
- `- Publicación`
- `- Mecanismos de acceso, formato, documentación y condiciones de uso`

##### 2.2.12. Aspectos legales y normativos

ID: GESTDAT-MGDE-DIM-LEGAL-01
Purp: Establecer exigencias para el área jurídica en la definición de políticas, procedimientos y planes de cumplimiento normativo.
Cpt: Criterios.

- `- Participación del área jurídica`
- `- Cumplimiento aspectos legales y normativos`

### 3. Implementación y Evaluación

ID: GESTDAT-MGDE-IMPL-ROOT-01
Purp: Describir el modelo de madurez, método de evaluación y plan de implementación del MGDE.

#### 3.1. Modelo de Madurez

ID: GESTDAT-MGDE-IMPL-MADUREZ-01
Purp: Medir el grado de desarrollo de la gestión de datos en una institución.
Cpt: Niveles de Madurez.

- `- Nivel 1 (Insuficiente): No se cumplen los mínimos deseables.`
- `- Nivel 2 (Básico): Se cumplen los mínimos deseables.`
- `- Nivel 3 (Medio): Se profundiza en cada dimensión.`
- `- Nivel 4 (Avanzado): Se aborda a cabalidad cada dimensión.`

#### 3.2. Método de Autoevaluación

ID: GESTDAT-MGDE-IMPL-AUTOEVAL-01
Purp: Definir el método para que un OAE determine su nivel de madurez actual.
Mech: Matriz de evaluación (Anexo N° 1) con preguntas y respuestas por nivel.
Cpt: Cálculo de Puntajes.

- `- Mdl: Puntajes por Respuesta.
  - Insuficiente: 0
  - Básico: 2
  - Medio: 4
  - Avanzado: 6`
- `- Mdl: Intervalos por Nivel.
  - [0, 40%): Insuficiente
  - [40%, 60%): Básico
  - [60%, 80%): Medio`
- `- Mdl: Fórmulas.
  - Pje(D) = ∑Pje(Pi)
  - % Pje(D) = Pje(D) / (6 * NP(D))
  - Pje(OAE) = ∑(Pje(Dj) * P(Dj))`

#### 3.3. Plan de Implementación

ID: GESTDAT-MGDE-IMPL-PLAN-01
Purp: Estructurar el proceso de implementación del MGDE en un OAE.
Cpt: Hoja de Ruta.

- `- Purp: Plan de acción para lograr el nivel de madurez esperado, priorizando dimensiones.`
- `- Req: Combinar enfoques top-down y bottom-up.`
- `- Req: Aplicado por equipo especializado con mix de competencias apropiadas.`
- `- Req: Alinear con marcos de trabajo existentes (Gestión Procesos, Calidad, Mejora Continua, TI, Transformación Digital, Gestión Documental, Arquitectura Institucional).`
- `- Def: Arquitectura Empresarial. Buenas prácticas para alinear procesos, sistemas, datos y tecnologías con objetivos estratégicos.`
- `- Def: Gestión del Cambio. Proceso para implementar nuevos modos de hacer y cambiar conductas laborales.`
Cpt: Etapas del Plan.

|Etapa|Duración Referencial|Foco|
|---|---|---|
|Etapa 1: Diagnóstico y Estrategia|4-8 meses|Autoevaluación, definir nivel esperado, elaborar hoja de ruta, priorizar 3 dims.|
|Etapa 2: Implementación Básica|8-12 meses|Implementar gobernanza y dims. priorizadas, ejecutar pilotos, re-evaluar.|
|Etapa 3: Implementación Avanzada|12-18 meses|Consolidar gobernanza, implementar mejores prácticas, evaluar y mejorar continuamente.|

Cpt: Organización y Roles.

- `- Mdl: Esquemas Orgánicos.
  - Equipos-Compartidos: Responsabilidades distribuidas (descentralizado).
  - Equipo-Dedicado: Unidad organizacional única responsable (centralizado).
  - Esquema-Mixto: Red con responsabilidades delimitadas por matriz RACI.`
- `- Rec: Instancias de Trabajo Sugeridas.
  - Comité-Directivo: Jefaturas. Provee direccionamiento, aprueba planes.
  - Comité-Ejecutivo: Jefaturas/Profesionales transversales. Propone políticas, coordina implementación.
  - Mesas-Trabajo: Profesionales. Ejecutan planificación.`
- `- Cpt: Roles Clave.
  - Director-Datos (CDO): Responsable integral de la estrategia y ejecución.
  - Admin/Custodio-Datos (Data Steward): Experto funcional, responsable de metadatos y calidad.
  - Analista-Datos (Data Analyst): Experto funcional en uso y análisis.
  - Arquitecto-Datos (Data Architect): Diseña los "planos" para la gestión de datos.`

Cpt: Ciclo de Mejora Continua.

- `- Purp: Describir el ciclo operativo de mejora continua para la gestión de datos.`
- `- Cpt: Fase 1 - Planificación. Comité Ejecutivo propone Plan Anual de Gestión de Datos al Comité Directivo.`
- `- Cpt: Fase 2 - Implementación. Comité Ejecutivo conforma Mesas de Trabajo para ejecutar el plan.`
- `- Cpt: Fase 3 - Evaluación. Anualmente se evalúa el avance del plan.`
- `- Cpt: Fase 4 - Evolución. Políticas y procesos se revisan y mejoran periódicamente.`

#### 3.4. Herramientas de Apoyo

ID: GESTDAT-MGDE-IMPL-HERRAMIENTAS-01
Purp: Describir herramientas de apoyo provistas por la Secretaría de Gobierno Digital.
Cpt: Herramienta 1 - Autoevaluación Automática.

- `- Plat: Google Workspace.`
- `- Func: Permite a OAEs completar formulario, identificar nivel de madurez, y generar propuesta de hoja de ruta automáticamente.`
- `- Cpt: Formulario Google Forms, código Apps Script para procesar, informe Google Sheets con resultados y gráficos.`
Cpt: Ejemplo Resultados Autoevaluación.
- `- Ctx: Institución X.`

|Métrica Global |Puntaje Total |Puntaje Ponderado |Porcentaje |Nivel Madurez Global |
|---|---|---|---|---|
|Institución X |90 |75 |28,8% |Insuficiente |
|Puntaje Máximo |312 |260 |||

|Dimensión |Puntaje Obtenido |% Puntaje / Puntaje Avanzado |Nivel de Madurez |Ponderación |
|---|---|---|---|---|
|Visión estratégica |12 |29% |Insuficiente |8,3% |
|Gobernanza de datos |12 |29% |Insuficiente |8,3% |
|Arquitectura, diseño y documentación |4 |11% |Insuficiente |8,3% |
|Almacenamiento y operación |4 |67% |Medio |8,3% |
|Seguridad y ciberseguridad de datos |4 |11% |Insuficiente |8,3% |
|Integración e interoperabilidad |12 |50% |Básico |8,3% |
|Documentos y contenidos |4 |17% |Insuficiente |8,3% |
|Datos maestros y de referencia |10 |56% |Básico |8,3% |
|Analítica e inteligencia de negocios |6 |33% |Insuficiente |8,3% |
|Calidad de datos |0 |0% |Insuficiente |8,3% |
|Datos abiertos |22 |52% |Básico |8,3% |
|Aspectos legales y normativos |0 |0% |Insuficiente |8,3% |

## Estándares para la Apertura y Reutilización de Datos Abiertos

ID: GUIDE-STS-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_062_tde_std_datos_abiertos.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 1. Marco General

ID: DA-MARCO-GENERAL-01
Purp: Establecer el contexto, objetivo, alcance y definiciones de los estándares de datos abiertos.

#### 1.1. Introducción

ID: DA-INTRODUCCION-01
Cpt: Datos Abiertos (Open Data).

- Mssn: Fomentar la transparencia, el acceso a la información pública, la competitividad y el desarrollo económico.
- Mech: Reutilización de información del sector público.
- Cpt: Iniciativa Chile.
  - ID: datos.gob.cl
  - Purp: Garantizar que los datos públicos generados por el Estado estén disponibles de forma abierta y accesible.
  - Dest: Ciudadanos, entidades interesadas.
- Req: Publicación.
  - Mdl: Digital, estandarizado, estructurado.
  - Purp: Facilitar la comprensión y accesibilidad.
- Cpt: Usos Potenciales.
  - Act: Creación de informes, estadísticas.
  - Res: Beneficio social, investigación científica, oportunidades de negocio.
  - Ctx: Aplicación en salud, seguridad, transporte, educación, medioambiente.
- Cpt: Alineación Internacional.
  - Fnd: Sigue directrices y ejemplos de países líderes.
  - Ref: EEUU (Open Government Directive).
  - Ref: Reino Unido (Opening up Government).
  - Ref: UE (Directiva 2003/98/CE sobre reutilización info sector público).
  - Src: <https://obamawhitehouse.archives.gov/open/documents/open-government-directive>
  - Src: <http://data.gov.uk/>
  - Src: <http://eurlex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:32003L0098:ES:HTML>
- Cpt: Rol de datos.gob.cl.
  - Fnd: Pilar fundamental de la Estrategia de Gobierno Digital de Chile.
  - Src: Datos financiados y recopilados con recursos públicos.
  - Req: Disponibles al servicio de la ciudadanía, sin restricciones de uso, en formatos adecuados.
- Cpt: Enfoque Dual.
  - Obj: Potenciar la transparencia y el acceso a la información.
  - Obj: Fomentar el desarrollo de nuevas tecnologías e innovación.
  - Mech: Permitir que terceros agreguen valor a los datos disponibles para generar nuevas soluciones y aplicaciones.

#### 1.2. Objetivo

ID: DA-OBJETIVO-01
Purp: Establecer estándares y directrices técnicas para la apertura y reutilización de datos en los órganos de la Administración del Estado, con el fin de facilitar su acceso, uso, reutilización y redistribución para cualquier fin.

#### 1.3. Alcance

ID: DA-ALCANCE-01

- Ctx: Aplicabilidad.
  - `- Ctx: Datos abiertos y datasets publicados en el Portal de Datos Abiertos de la SGD.`
  - `- Ctx: Portales o plataformas institucionales de datos abiertos de OAEs.`
- Req: Los OAEs deben garantizar que sus datos estén referenciados y sincronizados en la plataforma de la SGD.

#### 1.4. Definiciones

ID: DA-DEFINICIONES-01

- Def: Catálogo de Datos Abiertos.
  - Cpt: Repositorio que centraliza, almacena y disponibiliza conjuntos de datos abiertos estructurados y descritos por metadatos.
- Def: Conjunto de Datos Abiertos.
  - Cpt: Colección de datos relacionados, en formatos de uso común (preferiblemente estructurados), descritos por metadatos.
- Def: Dato.
  - Cpt: Representación de un atributo o variable (cuantitativa/cualitativa) por una secuencia de símbolos, capturable por observación/medición.
- Def: DCAT.
  - Cpt: Estándar internacional de vocabulario para catálogos de datos que facilita la interoperabilidad en la red.
- Def: Dublin Core.
  - Cpt: Vocabulario genérico de 15 propiedades para describir recursos electrónicos (auspiciado por DCMI).
- Def: Dato Abierto.
  - Cpt: Dato digital con características técnicas/jurídicas para ser usado, reutilizado y redistribuido libremente por cualquier persona/entidad, en cualquier momento y lugar.
- Def: Datos Genéricos.
  - Cpt: Datos de uso común que no requieren aplicación especializada.
- Def: Datos Geográficos.
  - Cpt: Datos que refieren a una localización relativa a la Tierra (Fuente: ISO/TC 211).
- Def: Diccionario de Variables.
  - Cpt: Documento que detalla y define las variables en un dataset (naturaleza, tipo, estructura).
- Def: Documentación Administrativa.
  - Cpt: Documentos de respaldo que proporcionan contexto y justificación para su uso y comprensión.

### 2. Estándares Abiertos

ID: DA-ESTANDARES-ABIERTOS-01
Purp: Definir los requisitos técnicos para la publicación de datos abiertos.

#### 2.1. Formato Abierto

ID: DA-FORMATO-ABIERTO-01

- Req: Publicación.
  - `- Req: Usar formatos abiertos para máxima reutilización y accesibilidad.`
  - `- Req: Cumplir clasificación "tres estrellas o más" de Tim Berners-Lee. Ref: <https://5stardata.info/en/>`
- Rec: Favorecer formatos no propietarios.
  - Res: Legibilidad por máquinas sin herramientas costosas, facilita integración en aplicaciones.
- Rec: Proveer datos en múltiples formatos para mayor flexibilidad y adaptabilidad.
  - Ex: Para datos tabulares, ofrecer XLS/XLSX junto a CSV.

##### 2.1.1. Datos Genéricos

ID: DA-FORMATO-GENERICOS-01
Purp: Especificar formatos aceptados para datos genéricos.

| Nombre | Uso esperado |
|---|---|
| CSV | Datos con estructura relacional (Tablas). |
| XML | Datos con estructura jerárquica (Árboles). |
| JSON | Datos con estructura jerárquica (Árboles). |
| RDF | Datos con cualquier estructura (Grafos). |
| TSV | Datos con estructura relacional (Tablas), delimitador de tabulación. |
| RAW | Datos en formato bruto, sin esquema estructurado definido. |
| Parquet | Datos con estructura columnar optimizada para analítica y consulta masiva. |

##### 2.1.2. Datos Geográficos

ID: DA-FORMATO-GEOGRAFICOS-01
Purp: Especificar formatos aceptados para datos geográficos.

| Nombre | Uso esperado |
|---|---|
| GeoJSON | Datos geoespaciales basados en JSON. |
| GML | Datos geográficos para servicios WFS (Web Feature Service). |
| GeoPackage | Basado en SQLite para almacenar/transferir datos geoespaciales (vectoriales y raster). |

##### 2.1.3. Documentación Administrativa

ID: DA-FORMATO-DOC-ADMIN-01
Purp: Especificar formatos para documentación administrativa que acompaña a los datasets.

- Ctx: Documentos oficiales que respaldan, explican y contextualizan los datos.
- Req: Formatos.
  - `- Req: PDF (Portable Document Format). Uso: Toda documentación administrativa para preservar contenido y asegurar accesibilidad.`
  - `- Req: ODT (Open Document Text). Uso: Documentos que requieren ser editables manteniendo estandarización.`
- Purp: Proporcionar detalles metodológicos y de origen de los datos para mayor contexto.
- Warn: Documentación administrativa no es metadato; complementa para enriquecer transparencia.

#### 2.2. Archivos Grandes

ID: DA-ARCHIVOS-GRANDES-01

- Req: Límite máximo de archivo.
  - `- Ctx: 200 megabytes.`
  - `- Cond: Excepción si la naturaleza del dataset justifica exceder el límite.`
  - `- Act: En caso de excepción, particionar el archivo.`
- Req: Compresión.
  - `- Mdl: ZIP o 7z.`
  - `- Req: Garantizar integridad y accesibilidad total de los datos descomprimidos.`

#### 2.3. Lenguaje y Codificación

ID: DA-LENGUAJE-COD-01

- Req: Lenguaje estándar.
  - `- Ctx: Español-Chile (ES_CL).`
- Req: Codificación de caracteres.
  - `- Ctx: UTF-8.`

### 3. Metadatos

ID: DA-METADATOS-ROOT-01
Purp: Detallar los estándares de metadatos para la publicación de datos abiertos.

#### 3.1. Principios de Metadatos

ID: DA-METADATOS-PRINCIPIOS-01

- Req: Todo OAE debe publicar sus datasets con metadatos consistentes.
- Req: Formato de metadatos.
  - `- Mdl: Legibles por humanos y por máquinas.`
- Purp: Facilitar la comprensión del origen, procesamiento y significado de los datos.
- Fnd: Estándar base DCAT, complementado con Dublin Core. Ref: DA-DEFINICIONES-01.
- Ctx: Adaptación nacional con modificaciones específicas para el contexto chileno.
- Req: Niveles de metadatos.
  - `- Cpt: Organizados en 4 niveles de descripción y 3 de requerimiento.`
  - `- Cpt: Nivel 1 (Obligatorio): documentación básica homogénea.`
  - `- Cpt: Nivel 2 (Recomendado): mayor calidad de documentación.`
  - `- Cpt: Nivel 3 (Opcional): uso según utilidad para el organismo.`

#### 3.2. Niveles de Metadatos

ID: DA-METADATOS-NIVELES-01
Purp: Especificar los metadatos requeridos para cada nivel de descripción.

##### 3.2.1. Nivel Catálogo

ID: DA-METADATOS-CATALOGO-01
Purp: Definir metadatos para la descripción general del catálogo de datos abiertos.

| Nombre del Metadato | Requerimiento | Descripción / Ejemplo |
|---|---|---|
| Identificador del Catálogo | Obligatorio | Código único para identificar el catálogo. Ex: cat_001 |
| Título del Catálogo | Obligatorio | Nombre claro y breve. Ex: Catálogo Datos Abiertos Santiago |
| Descripción del Catálogo | Obligatorio | Detalle de contenido y alcance. Ex: Datasets Municipalidad de Santiago. |
| OAE Asociado | Obligatorio | Órgano del Estado al que pertenece. Ex: Municipalidad de Santiago |
| Código de OAE | Obligatorio | Código Gescode del OAE. Ex: PE-MUN-00432 |
| Correo electrónico OAE | Obligatorio | Email de contacto para el catálogo. Ex: <datos@municipalidad.gob.cl> |
| Fecha de creación | Obligatorio | Fecha oficial de creación del catálogo. Ex: 2023-01-01 |
| Fecha de última actualización | Recomendado | Última modificación del catálogo. Ex: 2023-12-31 |
| Idioma(s) | Recomendado | Lenguaje de metadatos y datasets. Ex: Español, Inglés |
| Licencia | Recomendado | Licencia general (sobrescribible a nivel de recurso). Ex: CC BY 4.0 |
| Cobertura geográfica | Recomendado | Ámbito geográfico. Ref: DA-DEF-NIVELES-GEO-01. Ex: Chile, Región Metropolitana |
| N° visitas | Recomendado | Visitas acumuladas al catálogo. Ex: 1000 |
| Colección Categorías | Recomendado | Lista de categorías temáticas. Ex: Demografía, Transporte |
| Conjuntos de Datos | Opcional | Lista de datasets del catálogo. Ex: dataset_1, dataset_2 |
| Página web del catálogo | Opcional | URL de acceso principal. Ex: <https://datos.gob.cl/> |

##### 3.2.2. Nivel Conjunto de Datos

ID: DA-METADATOS-CONJUNTO-01
Purp: Detallar metadatos para cada conjunto de datos (dataset).

| Nombre del Metadato | Requerimiento | Descripción / Ejemplo |
|---|---|---|
| Identificador del Conjunto de Datos | Obligatorio | ID único del dataset. Ex: dataset_001 |
| Título del Conjunto de Datos | Obligatorio | Nombre claro y abstracto. Ex: Datos de temperatura en Santiago |
| Descripción del Conjunto de Datos | Obligatorio | Resumen de contenido y propósito. Ex: Registros históricos de temp. max/min. |
| Autor | Obligatorio | Responsable de la publicación. Ex: Depto. de Meteorología |
| Correo electrónico de Contacto | Obligatorio | Email del responsable. Ex: <departamento@munidesantiago.gob.cl> |
| OAE Asociado | Obligatorio | Órgano al que pertenece. Ex: Municipalidad de Santiago |
| Código de OAE | Obligatorio | Código Gescode del OAE. Ex: PE-MUN-00432 |
| Departamento de la OAE | Obligatorio | Departamento encargado. Ex: Depto. de Medio Ambiente |
| Recursos | Obligatorio | Lista de recursos del dataset. Ex: archivo_csv, archivo_shp, metadata.json |
| Categoría Temática/s | Obligatorio | Categoría/s global/es. Ex: Meteorología, Medio Ambiente |
| Fecha de Creación | Obligatorio | Fecha de creación del dataset. Ex: 2023-01-01 |
| Fecha de publicación | Obligatorio | Fecha de publicación en portal DDAA. Ex: 2023-02-15 |
| Palabras Claves | Obligatorio | Etiquetas que describen el contenido. Ex: temperatura, santiago, clima |
| Periodo de referencia | Obligatorio | Lapso temporal de la información. Ex: 1980-2023 |
| Licencia | Obligatorio | Licencia de distribución. Ex: CC BY 4.0 |
| Versionamiento | Obligatorio | Versión del dataset. Ex: 1.0 |
| Fecha de la versión | Obligatorio | Fecha de edición de la versión. Ex: 2023-01-01 |
| Fecha de última modificación | Recomendado | Última modificación de datos/metadatos. Ex: 2023-12-31 |
| Frecuencia de actualización | Recomendado | Frecuencia de actualización. Ex: Mensual |
| Ubicación o Enlace Directo (URL) | Recomendado | URL de acceso al dataset. Ex: <https://datos.gob.cl/dataset/encuesta-juventud> |
| Idioma(s) | Recomendado | Lenguaje de descripción. Ex: Español, Inglés |
| Cobertura geográfica | Recomendado | Ámbito geográfico. Ref: DA-DEF-NIVELES-GEO-01. Ex: Chile |
| Visitas al dataset | Recomendado | Número total de visitas. Ex: 500 |
| Descargas | Recomendado | Cantidad de descargas. Ex: 200 |
| Registro de Cambios | Recomendado | Descripción cronológica de modificaciones. Ex: V1.1: Se agregaron nuevas estaciones. |
| Procedencia del conjunto de Datos | Recomendado | Indica si es subconjunto, integración, etc. Ex: Integración |
| Detalle de procedencia | Recomendado | Especifica los datasets originales. Ex: dataset_1, dataset_2 |
| Relación | Opcional | Relación entre dataset y OAE. Ex: autor institucional |
| Tamaño del Dataset | Opcional | Volumen de datos. Ex: 10 MB |

##### 3.2.3. Nivel Recurso

ID: DA-METADATOS-RECURSO-01
Purp: Describir los metadatos para archivos individuales (recursos) dentro de un dataset.

| Nombre del Metadato | Requerimiento | Descripción / Ejemplo |
|---|---|---|
| Identificador | Obligatorio | ID único del recurso. Ex: recurso_001 |
| Título | Obligatorio | Nombre del recurso. Ex: Datos de temperatura_2023.csv |
| Descripción | Obligatorio | Breve descripción. Ex: Archivo CSV con temp. max/min para 2023. |
| Diccionario de variables | Obligatorio | Lista de campos si es una tabla. Ex: fecha, estación, temperatura_max |
| Fecha de última modificación | Recomendado | Fecha de última actualización. Ex: 2023-12-31 |
| Ubicación o Enlace Directo (URL) | Recomendado | URL de acceso directo. Ex: <https://datos.gob.cl/.../resource/b857>... |
| Tamaño del Archivo | Recomendado | Tamaño en bytes (aprox.). Ex: 5 MB |
| Formato del recurso | Recomendado | Formato del archivo. Ex: CSV |
| Visitas al recurso | Recomendado | Cantidad de visitas. Ex: 200 |
| Descargas | Recomendado | Cantidad de descargas. Ex: 100 |

#### 3.3. Diccionario de Variables

ID: DA-METADATOS-DICCIONARIO-01

- Req: Cada dataset debe publicarse con su diccionario de variables.
- Purp: Describir detalladamente cada variable para que los usuarios comprendan los datos.

| Nombre | Requerimiento | Descripción / Ejemplo |
|---|---|---|
| Nombre | Obligatorio | Nombre del campo en el encabezado. Ex: Edad |
| Tipo | Obligatorio | Tipo de dato contenido en el campo. Ex: Numérico |
| Descripción | Obligatorio | Información que contiene el campo. Ex: Edad de la persona encuestada. |
| Identificador | Recomendado | Código identificador único del campo. Ex: edad |
| Unidad de medida | Opcional | Unidad de medida para campos numéricos. Ex: Años |

### 4. Definiciones Compartidas

ID: DA-DEF-COMPARTIDAS-01
Purp: Definir elementos comunes referenciables para evitar duplicación.

#### 4.1. Niveles de Cobertura Geográfica

ID: DA-DEF-NIVELES-GEO-01

- Nat: Lista enumerada.
- Cpt:
  - `- País`
  - `- Región`
  - `- Provincia`
  - `- Comuna`

### 5. Licenciamiento

ID: DA-LICENCIAMIENTO-ROOT-01
Purp: Definir las políticas de licenciamiento para la publicación de datos abiertos.

#### 5.1. Política de Licenciamiento

ID: DA-LICENCIAMIENTO-POLITICA-01

- Req: Disponibilidad.
  - `- Ctx: Datos y datasets deben estar disponibles para todas las personas (naturales/jurídicas).`
- Mech: Licencias de dominio público.
- Req: Licencia predeterminada.
  - `- Ctx: Creative Commons Zero (CC0 1.0) si no se asigna explícitamente otra.`
- Req: Licencia alternativa.
  - `- Ctx: OAEs pueden optar por otras licencias predefinidas según necesidades.`
  - `- Cond: Si se necesita una licencia no predefinida, solicitar y justificar a la SGD.`

#### 5.2. Tipos de Licencia

ID: DA-LICENCIAMIENTO-TIPOS-01
Purp: Detallar las licencias predeterminadas y alternativas.

| Licencia | Dominio | Descripción |
|---|---|---|
| Creative Commons Zero (CC0 1.0) | Contenido, Datos | Renuncia a todos los derechos de autor y conexos. Uso libre para cualquier propósito sin restricciones (dominio público). |
| Open Data Commons Public Domain Dedication and Licence (PDDL-1.0) | Datos | Permite usar, modificar y distribuir los datos libremente sin ninguna restricción. |
| Creative Commons Attribution 4.0 (CC-BY-4.0) | Contenido, Datos | Permite copiar, distribuir, exhibir y ejecutar obras derivadas con la condición de dar crédito al creador original. |
| Open Data Commons Attribution License (ODC-By-1.0) | Datos | Permite la copia, distribución y uso de datasets en nuevos productos siempre que se dé atribución al autor. |

### 6. Catálogos Institucionales

ID: DA-CATALOGOS-INST-01
Purp: Establecer los requisitos para los portales o plataformas de datos abiertos institucionales.

- Req: Acceso inmediato, sin requisitos de registro o identificación.
- Req: Contener un listado completo, ordenado y clasificado de todos los datasets disponibles.
- Req: Facilitar navegación, búsqueda de texto y consulta efectiva.
- Req: Mantener operatividad continua del portal y analizar estadísticas de uso para mejorar.
- Req: Proveer APIs para facilitar captura y utilización de datasets por usuarios y su integración en el Portal Nacional de Datos Abiertos.

## Guía Técnica: Metadatos para Documentos y Expedientes Electrónicos

Version: 1.0.0
Status: Draft
Human-Creator: STSador
Human-Editor: STSador
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_064_tde_guia_metadatos_docs.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

ID: GDE-META-ROOT-01
Purp: Definir metadatos (obligatorios, condicionales, sugeridos) para la gestión e interoperabilidad de documentos y expedientes electrónicos de los Órganos de la Administración del Estado (OAE).

### 1. Introducción y Fundamentos

ID: GDE-META-INTRO-01
Purp: Establecer el contexto legal, normativo y técnico para el uso de metadatos en la gestión documental del Estado.

#### Contexto Legal y Normativo

ID: GDE-META-INTRO-LEGAL-01
Fnd: Ley N° 21.180 (Transformación Digital del Estado).

- Cpt: Modificación. Act: Modifica Ley N° 19.880.
- Cpt: Obj-Modificación. Purp: Incorporar digitalización y transformación del ciclo de procedimientos administrativos.
Fnd: Decreto Supremo N° 4, 2020, MINSEGPRES.
- Cpt: Obj-Reglamento. Purp: Regular expresión de procedimientos administrativos por medios electrónicos.
- Cpt: Mandato-Reglamento. Req: Dictar 6 normas técnicas (interoperabilidad, seguridad, docs/expedientes, notificaciones, calidad, autenticación).
Fnd: Decreto Supremo N° 10, 2023, MINSEGPRES.
- Cpt: Obj-Norma. Purp: Establecer norma técnica de documentos y expedientes electrónicos.
- Cpt: Dependencia. Def: Esta guía técnica facilita la implementación de dicha norma.
Req: Para correcta interpretación, seguir definiciones del Art. 2° de la Norma Técnica de Documentos y Expedientes Electrónicos.

#### Base de Buenas Prácticas

ID: GDE-META-INTRO-PRACTICAS-01
Purp: Fundamentar la guía en estándares internacionales.
Fnd: Base Normativa ISO.

- Ref: `ISO-15489`. Ctx: Gestión de documentos.
  - Purp: Asegurar protección de docs; permitir recuperación normalizada y eficaz de info.
- Ref: `ISO-23081`. Ctx: Metadatos para gestión de docs.
  - Purp: Proporcionar orientación sobre principios y elementos para implantar/evaluar conjuntos de metadatos.
Ref: Otros-Estandares.
- Cpt: `Australian-Government-Recordkeeping-Metadata-Standard`
- Cpt: `e-EMGDE` (Esquema de Metadatos para la Gestión del Documento Electrónico) de España.
Cpt: Proyeccion. Act: Versiones futuras de la norma y guía se incorporarán según avance del cumplimiento.

#### Principios de Gestión de Metadatos

ID: GDE-META-INTRO-PRINCIPIOS-01
Purp: Definir los principios rectores de los metadatos en el ciclo de vida documental.
Cpt: Rol-Metadatos. Fnd: Fundamental para descripción precisa, gestión, tramitación, interoperabilidad y eficiencia.
Cpt: Indivisibilidad. Def: Metadatos son parte indivisible de la identidad de expedientes y documentos.
Cpt: Funcion-Descriptiva. Act: Proporcionan info sobre estructura, contenido y contexto (autor, fecha, lugar).
Obj: Garantizar disponibilidad, recuperación, accesibilidad, conservación e interoperabilidad.
Cpt: Ciclo-Vida. Def: Metadatos se incorporan y enriquecen a lo largo de las etapas del procedimiento.

- Req: Inclusión desde creación, durante gestión, hasta transferencia a Archivo Nacional.
Cpt: Persistencia. Def: Metadatos son de registro permanente.
- Req: Deben conservarse sin sobrescribirse, resguardados por el organismo custodio.
Cpt: Implementacion-OAE. Def: Cada institución dispone cómo implementar el registro (repositorios, BBDD, etc.).
- Req: Obligatoria la existencia de metadatos asociados a cada doc/expediente.
- Req: Obligatoria su generación en formato estandarizado para interoperabilidad.

### 2. Esquema General de Metadatos

ID: GDE-META-ESQUEMA-ROOT-01
Purp: Presentar la estructura y resumen cuantitativo de los metadatos para expedientes y documentos.

#### Estructura y Entidades

ID: GDE-META-ESQUEMA-ENTIDADES-01
Mdl: Entidad-Relación.
Cpt: Entidades-Principales.

- `Documento`
- `Expediente`
- `Actor`: Institución, persona física/jurídica responsable o involucrada.
- `Relacion`: Asociación entre dos o más entidades.
Cpt: Multiplicidad. Def: Esquema permite relaciones múltiples entre expediente/documento y actores.

#### Cuantificación del Esquema

ID: GDE-META-ESQUEMA-CUANT-01
Cpt: Total-Elementos-Expediente. Res: 29.

- `Obligatorios`: 18.
- `Condicionales`: 5.
- `Sugeridos`: 6.
Cpt: Total-Elementos-Documento. Res: 46.
- `Obligatorios`: 12.
- `Condicionales`: 16.
- `Sugeridos`: 18.

#### Leyenda de Clasificación

ID: GDE-META-ESQUEMA-LEYENDA-01
Purp: Definir la simbología usada en las tablas de metadatos.

- Cpt: `Color-Verde`. Def: Metadato Obligatorio.
- Cpt: `Color-Amarillo`. Def: Metadato Condicional (obligatorio si se cumple condición).
- Cpt: `Color-Blanco`. Def: Metadato Sugerido (pertinencia a discreción del OAE).
- Cpt: `AN`. Def: Metadato requerido por Archivo Nacional para transferencia digital.
- Cpt: `MU`. Def: Metadato múltiple (permite múltiples registros).

### 3. Metadatos para Expedientes Electrónicos

ID: GDE-META-EXPEDIENTES-ROOT-01
Purp: Definir el conjunto de metadatos aplicables a un expediente electrónico.

#### Tabla Resumen: Metadatos de Expedientes

ID: GDE-META-EXPEDIENTES-TABLA-01

| Codificación | N° | Sub N° | Grupo/Rótulo | Definición | Flags |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | | | Identificación | Def: Info de identificación unívoca del expediente. | |
| MGDEE1_1 | 1 | 1.1 | Identificador de expediente | Def: Número único (ID) asignado auto a un expediente. | `AN` |
| MGDEE1_2 | 2 | 1.2 | Código serie | Def: Código serie del cuadro de clasificación documental del OAE. | |
| MGDEE1_3 | 3 | 1.3 | Número del expediente | Def: N° de orden interno dentro de una serie documental. | |
| MGDEE1_4 | 4 | 1.4 | Estado | Def: Estado de generación del expediente por el OAE productor. | |
| MGDEE1_5 | 5 | 1.5 | Título del expediente | Def: Palabra/frase para denominar el expediente (formal o atribuido). | `AN` |
| 2 | | | Descripción | Def: Texto referencial del contenido global. | |
| MGDEE2_1 | 6 | 2.1 | Resumen | Def: Relato sintético del contenido global del expediente. | |
| MGDEE2_2 | 7 | 2.2 | Asunto del expediente | Def: Materia/tema que trata, reflejo de los fines perseguidos. | `AN` |
| 3 | | | Temporalidad | Def: Atributos de tiempo específicos. | |
| MGDEE3_1 | 8 | 3.1 | Fecha de creación | Def: Fecha en que es generado el expediente. | `AN` |
| MGDEE3_2 | 9 | 3.2 | Fecha de finalización | Def: Fecha de finalización o cierre del expediente. | `AN` |
| 4 | | | Caracterización documental | Def: Identificación por tipo de expediente. | |
| MGDEE4_1 | 10 | 4.1 | Mecanismo de incorporación | Def: Cómo se incorporó al sistema de gestión documental. | |
| MGDEE4_2 | 11 | 4.2 | URI de expediente | Def: Enlace a expediente en repositorio/plataforma. | |
| 5 | | | Relaciones | Def: Relaciones del expediente con OAE o personas. | |
| | | 5.1 | OAE Asociado | Def: Identificación de relaciones con OAEs. | |
| MGDEE51_1 | 12 | 5.1.1 | Código de OAE productor | Def: OAE que genera el expediente en cumplimiento de sus funciones. | `AN` |
| MGDEE51_2 | 13 | 5.1.2 | Nombre OAE productor | Def: Nombre institucional si OAE no está en codificador. | |
| MGDEE51_3 | 14 | 5.1.3 | Tipo Relación OAE | Def: Relación entre el expediente y el OAE. | `MU` |
| MGDEE51_4 | 15 | 5.1.4 | Código de OAE relacionado | Def: OAE que custodia, respalda o está involucrado. | `MU` |
| MGDEE51_5 | 16 | 5.1.5 | Nombre OAE relacionado | Def: Nombre institucional si OAE relacionado no está en codificador. | `MU` |
| | | 5.2 | Otros actores | Def: Relaciones del expediente con otros actores. | |
| MGDEE52_1 | 17 | 5.2.1 | Tipo de relación otros actores | Def: Tipo de relación existente con el actor y el expediente. | `MU` |
| MGDEE52_2 | 18 | 5.2.2 | Tipo de actor relacionado | Def: Identifica tipo de actor para determinar pertinencia de ID. | `MU` |
| MGDEE52_3 | 19 | 5.2.3 | RUN/RUT relacionado | Def: RUN/RUT/Pasaporte del actor relacionado. | `MU` |
| MGDEE52_4 | 20 | 5.2.4 | Nombre del actor relacionado | Def: Nombre si no se cuenta con RUN/RUT. | `MU` |
| | | 5.3 | Índice de Documentos Asociados| Def: Docs/expedientes que forman parte del presente expediente. | |
| MGDEE53_1 | 21 | 5.3.1 | Identificador vinculado | Def: ID del expediente o documento que conforma el presente exp. | `AN, MU` |
| MGDEE53_2 | 22 | 5.3.2 | Fecha de incorporación | Def: Fecha/hora en que se incorpora el doc/exp vinculado. | `AN, MU` |
| 6 | | | Seguridad | Def: Niveles de seguridad para la gestión del expediente. | |
| MGDEE6_1 | 23 | 6.1 | Nivel de acceso | Def: Indicación relativa al acceso y consulta del expediente. | `AN` |
| MGDEE6_2 | 24 | 6.2 | Fecha fin restricción | Def: Fecha que determina el desbloqueo del expediente. | |
| MGDEE6_3 | 25 | 6.3 | Texto Advertencia | Def: Texto a presentar si un usuario intenta acceder. | |
| MGDEE6_4 | 26 | 6.4 | Carácter sensible/privado | Def: Identificación si contiene info sensible/privada. | |
| 7 | | | Procedimiento asociado | Def: Identificación del Procedimiento Administrativo. | |
| MGDEE7_1 | 27 | 7.1 | Código CPAT asociado | Def: Código del procedimiento en Catálogo de Proc. Adm. y Tram. (CPAT). | |
| MGDEE7_2 | 28 | 7.2 | Nombre procedimiento asociado | Def: Nombre del procedimiento si no está en CPAT. | |
| 8 | | | Versión | Def: Identificación de la versión del esquema. | |
| MGDEE8_1 | 29 | 8.1 | Versión MDGEE | Def: Versión del esquema de metadatos utilizado. | |

#### Especificaciones Detalladas: Metadatos de Expedientes

ID: GDE-META-EXPEDIENTES-ESPECIFICACIONES-01
Purp: Detallar cada metadato para expedientes.
Ref: AUDIT-ETE-INFORME-01

##### 1. Identificador de expediente (MGDEE1_1)

ID: GDE-META-EXP-SPEC-01
Ref: MGDEE1_1
Mech: Automático. Sistema asigna ID único institucional para acceso.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ctx: Asegurar unicidad, persistencia y estandarización de codificación.
Ex: `EXP-20230925-001`

##### 2. Código serie (MGDEE1_2)

ID: GDE-META-EXP-SPEC-02
Ref: MGDEE1_2
Mech: Automático. Sistema asigna código de serie a cada expediente creado.
Cpt: Tipo-Dato. Def: Alfanumérico.

##### 3. Número del expediente (MGDEE1_3)

ID: GDE-META-EXP-SPEC-03
Ref: MGDEE1_3
Mech: Automático. Sistema asigna número de orden interno dentro de una serie documental.
Cpt: Tipo-Dato. Def: Alfanumérico.

##### 4. Estado (MGDEE1_4)

ID: GDE-META-EXP-SPEC-04
Ref: MGDEE1_4
Mech: Automático/Manual. Generado por sistema o manualmente para reflejar estado.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ctx: Puede referirse al estado de creación o fase del ciclo de vida.

##### 5. Título del expediente (MGDEE1_5)

ID: GDE-META-EXP-SPEC-05
Ref: MGDEE1_5
Mech: Manual. Título formal adjudicado por creador; puede ser automatizable.
Cpt: Tipo-Dato. Def: Texto.
Ctx: Usar mayúsculas solo al inicio y en nombres propios.
Ex: `Asignación de presupuesto para compra de insumos.`

##### 6. Resumen (MGDEE2_1)

ID: GDE-META-EXP-SPEC-06
Ref: MGDEE2_1
Mech: Manual.
Cpt: Tipo-Dato. Def: Texto.

##### 7. Asunto del expediente (MGDEE2_2)

ID: GDE-META-EXP-SPEC-07
Ref: MGDEE2_2
Mech: Manual y/o desde vocabulario controlado para destacar materia no extraíble de otros metadatos.
Cpt: Tipo-Dato. Def: Texto.
Ctx: Representa el contenido amplio del expediente.
Ex: `Compra de insumos tecnológicos para el año 2023.`

##### 8. Fecha de creación (MGDEE3_1)

ID: GDE-META-EXP-SPEC-08
Ref: MGDEE3_1
Mech: Automático. Generado según formato `aaaa-mm-dd hh:mm:ss` (ISO 8601).
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ctx: Debe permitir modificación, pero registrando el cambio.
Ex: `2023-20-10:11:56:57`

##### 9. Fecha de finalización (MGDEE3_2)

ID: GDE-META-EXP-SPEC-09
Ref: MGDEE3_2
Mech: Automático. Generado según formato `aaaa-mm-dd hh:mm:ss` (ISO 8601).
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ctx: Debe permitir modificación, pero registrando el cambio.
Ex: `2023-20-11:16:56:57`

##### 10. Mecanismo de incorporación de expediente (MGDEE4_1)

ID: GDE-META-EXP-SPEC-10
Ref: MGDEE4_1
Mech: Automático/Manual. Seleccionar de lista controlada. Ref: `GDE-META-LISTAS-MEC-INCORP-01`.
Cpt: Tipo-Dato. Def: Texto.
Cpt: Valor-Defecto. Def: 1 (Incorporación manual).
Ex: `1`

##### 11. URI de expediente (MGDEE4_2)

ID: GDE-META-EXP-SPEC-11
Ref: MGDEE4_2
Mech: Automático. Generado automáticamente por la plataforma.
Cpt: Tipo-Dato. Def: URI.
Ctx: Institución puede usar servicios propios de URIs persistentes o los que disponga el Estado.
Ex: `https://dominio-institución/servicio-persistente/20.500.13034/401`

##### 12. Código de OAE productor (MGDEE51_1)

ID: GDE-META-EXP-SPEC-12
Ref: MGDEE51_1
Mech: Automático. Sistema incorpora código y nombre del productor desde Gestor de Códigos (GESCODE).
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Valor requerido por Archivo Nacional (AN).
Ex: `46` (Gobierno Regional de la Región de La Araucanía)

##### 13. Nombre OAE productor (MGDEE51_2)

ID: GDE-META-EXP-SPEC-13
Ref: MGDEE51_2
Mech: Automático/Manual.
Cond: Requerido si OAE productor no está registrado en GESCODE.
Cpt: Forma-Ingreso. Def: Registro manual del nombre institucional.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Gobierno Regional de la Región de La Araucanía`

##### 14. Tipo Relación OAE (MGDEE51_3)

ID: GDE-META-EXP-SPEC-14
Ref: MGDEE51_3
Mech: Automático/Manual. Selección de lista predefinida. Ref: `GDE-META-LISTAS-TIPO-REL-OAE-01`.
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Obligatorio identificar al menos OAE custodio.
Cpt: Valor-Defecto. Def: 1 (custodia).
Ex: `1`

##### 15. Código de OAE relacionado (MGDEE51_4)

ID: GDE-META-EXP-SPEC-15
Ref: MGDEE51_4
Mech: Automático/Manual. Código desde Gestor de Códigos (GESCODE).
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Obligatorio identificar al menos OAE custodio.
Ex: `46` (Gobierno Regional de la Región de La Araucanía)

##### 16. Nombre de OAE relacionado (MGDEE51_5)

ID: GDE-META-EXP-SPEC-16
Ref: MGDEE51_5
Mech: Automático/Manual.
Cond: Requerido si OAE relacionado no está registrado en GESCODE.
Cpt: Forma-Ingreso. Def: Registro manual del nombre institucional.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Gobierno Regional de la Región de La Araucanía`

##### 17. Tipo de relación con otros actores (MGDEE52_1)

ID: GDE-META-EXP-SPEC-17
Ref: MGDEE52_1
Mech: Automático/Manual.
Cond: Obligatorio para identificación de interesados.
Cpt: Forma-Ingreso. Def: Selección de lista predefinida. Ref: `GDE-META-LISTAS-TIPO-REL-ACTORES-01`.
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Obligatorio asignar al menos un funcionario responsable. Campo múltiple.
Cpt: Valor-Defecto. Def: 1 (Responsable).
Ex: `2` (Interesado)

##### 18. Tipo de actor relacionado (MGDEE52_2)

ID: GDE-META-EXP-SPEC-18
Ref: MGDEE52_2
Mech: Automático/Manual.
Cond: Obligatorio para identificación de interesados.
Cpt: Forma-Ingreso. Def: Selección de lista predefinida. Ref: `GDE-META-LISTAS-TIPO-ACTOR-01`.
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Obligatorio especificar el funcionario responsable inicial.
Cpt: Valor-Defecto. Def: 4 (Funcionario).
Ex: `1` (Ciudadano)

##### 19. RUN/RUT Relacionado (MGDEE52_3)

ID: GDE-META-EXP-SPEC-19
Ref: MGDEE52_3
Mech: Automático/Manual.
Cond: Obligatorio para identificación de interesados.
Cpt: Forma-Ingreso. Def: Registro al momento de identificar al actor (RUN/RUT/Pasaporte).
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `60100003-2`

##### 20. Nombre del actor relacionado (MGDEE52_4)

ID: GDE-META-EXP-SPEC-20
Ref: MGDEE52_4
Mech: Automático/Manual.
Cond: Obligatorio para interesados si no se cuenta con RUN/RUT/Pasaporte.
Cpt: Forma-Ingreso. Def: Registro del nombre de la persona natural o jurídica.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Entel Chile`, `Julian Santelices Machuca`

##### 21. Identificador de expediente/documento vinculado (MGDEE53_1)

ID: GDE-META-EXP-SPEC-21
Ref: MGDEE53_1
Mech: Automático. Sistema registra ID o URI de docs/expedientes incorporados al índice.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ctx: Requerido si el documento forma parte de un expediente.

##### 22. Fecha de la incorporación del expediente / documento (MGDEE53_2)

ID: GDE-META-EXP-SPEC-22
Ref: MGDEE53_2
Mech: Automático. Sistema registra fecha/hora de incorporación (`aaaa-mm-dd hh:mm:ss`).
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ex: `2023-20-11:16:56:57`

##### 23. Nivel de acceso (MGDEE6_1)

ID: GDE-META-EXP-SPEC-23
Ref: MGDEE6_1
Mech: Manual. Selección de lista controlada o asociación automática por tipo de expediente según política institucional. Ref: `GDE-META-LISTAS-NIVEL-ACCESO-01`.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1 (Público).
Ex: `1`

##### 24. Fecha fin restricción (MGDEE6_2)

ID: GDE-META-EXP-SPEC-24
Ref: MGDEE6_2
Mech: Manual. Ingreso manual de fecha de desbloqueo.
Cpt: Tipo-Dato. Def: Fecha.

##### 25. Texto de advertencia (MGDEE6_3)

ID: GDE-META-EXP-SPEC-25
Ref: MGDEE6_3
Mech: Manual. Ingreso manual del texto a presentar.
Cpt: Tipo-Dato. Def: Texto.

##### 26. Información de carácter sensible y/o privado (MGDEE6_4)

ID: GDE-META-EXP-SPEC-26
Ref: MGDEE6_4
Mech: Manual. Plataforma OAE debe tener registro de marca (Sí/No).
Cpt: Tipo-Dato. Def: Numérico (Lista Controlada `1-SI / 2-NO`).
Ctx: OAE puede definir categorías controladas para este tipo de info.
Cpt: Valor-Defecto. Def: 2 (NO).
Ex: `2`

##### 27. Código CPAT asociado (MGDEE7_1)

ID: GDE-META-EXP-SPEC-27
Ref: MGDEE7_1
Mech: Automático. Código desde Catálogo de Procedimientos Administrativos y Tramitaciones (CPAT).
Cpt: Tipo-Dato. Def: Alfanumérico.
Ctx: Disponibilizado por CPAT.
Ex: `5076 (PA-UNI00002-00001- Convalidación de Programa de Perfeccionamiento Académico)`

##### 28. Nombre del procedimiento administrativo asociado (MGDEE7_2)

ID: GDE-META-EXP-SPEC-28
Ref: MGDEE7_2
Mech: Manual.
Cond: Obligatorio si el PA no está codificado en CPAT o el OAE decide registrarlo para referencia directa.
Cpt: Forma-Ingreso. Def: Registro manual del nombre del PA.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `Convalidación de Programa de Perfeccionamiento Académico`

##### 29. Versión MDGEE (MGDEE8_1)

ID: GDE-META-EXP-SPEC-29
Ref: MGDEE8_1
Mech: Automático. Registro automático de la versión de la guía de metadatos.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: `001`.
Ex: `001`

### 4. Metadatos para Documentos Electrónicos

ID: GDE-META-DOCUMENTOS-ROOT-01
Purp: Definir el conjunto de metadatos aplicables a un documento electrónico.

#### Tabla Resumen: Metadatos de Documentos

ID: GDE-META-DOCUMENTOS-TABLA-01

| Codificación | N° | Sub N° | Grupo/Rótulo | Definición | Flags |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | | | Identificación | Def: Info de identificación unívoca del documento. | |
| MGDDE1_1 | 1 | 1.1 | Identificador | Def: Código único asignado auto a un documento. | `AN` |
| MGDDE1_2 | 2 | 1.2 | Código serie | Def: Código serie del doc. según cuadro de clasificación OAE. | `AN` |
| MGDDE1_3 | 3 | 1.3 | Número del documento | Def: N° de orden interno dentro de una serie documental. | |
| MGDDE1_4 | 4 | 1.4 | Estado | Def: Estado de generación del doc. por la institución productora. | |
| MGDDE1_5 | 5 | 1.5 | Versión | Def: Número de versión del documento. | |
| MGDDE1_6 | 6 | 1.6 | Título del documento | Def: Palabra/frase para denominar el doc. (formal o atribuido). | `AN` |
| MGDDE1_7 | 7 | 1.7 | Resolución de captura | Def: Nivel de resolución de imagen (si es microforma). | `AN` |
| MGDDE1_8 | 8 | 1.8 | Nombre archivo asociado | Def: Nombre del archivo digital referenciado. | |
| 2 | | | Características Técnicas | Def: Caracterización técnica del documento. | |
| MGDDE2_1 | 9 | 2.1 | Tamaño | Def: Volumen del documento en Kb. | |
| MGDDE2_2 | 10 | 2.2 | Cantidad de páginas | Def: N° total de páginas o extensión. | `AN` |
| MGDDE2_3 | 11 | 2.3 | Formato | Def: Extensión del archivo electrónico. | |
| MGDDE2_4 | 12 | 2.4 | Nombre y Versión del software | Def: Software usado para generar el documento. | |
| 3 | | | Descripción | Def: Texto referencial del contenido. | |
| MGDDE3_1 | 13 | 3.1 | Resumen | Def: Relato sintético del contenido global. | |
| MGDDE3_2 | 14 | 3.2 | Palabras claves | Def: Materias o temas representativos del contenido. | `AN` |
| MGDDE3_3 | 15 | 3.3 | Idioma | Def: Idioma en que se encuentra el documento. | |
| MGDDE3_4 | 16 | 3.4 | Comunas | Def: Ubicación geográfica del resguardo del doc. | |
| 4 | | | Temporalidad | Def: Atributos de tiempo específicos. | |
| MGDDE4_1 | 17 | 4.1 | Fecha de creación | Def: Fecha en que es generado el documento. | `AN` |
| MGDDE4_2 | 18 | 4.2 | Fecha de modificación | Def: Fecha de la última modificación del documento. | |
| MGDDE4_3 | 19 | 4.3 | Fecha de captura | Def: Fecha de incorporación al repositorio (docs no generados internamente). | `AN` |
| MGDDE4_4 | 20 | 4.4 | Cobertura temporal | Def: Periodo de tiempo al que hace referencia el acto del doc. | |
| 5 | | | Caracterización documental | Def: Identificación específica por tipo de documento. | |
| MGDDE5_1 | 21 | 5.1 | Tipo documental | Def: Nombre y/o código del tipo documental estandarizado. | |
| MGDDE5_2 | 22 | 5.2 | Origen del documento | Def: Caracterización del origen de incorporación. | `AN` |
| MGDDE5_3 | 23 | 5.3 | Mecanismo de incorporación | Def: Mecanismo de incorporación al repositorio. | |
| MGDDE5_4 | 24 | 5.4 | URI documento externo | Def: Enlace a documento/recurso en repositorio externo. | |
| MGDDE5_5 | 25 | 5.5 | Ubicación física | Def: Código de almacenamiento físico (si existe original en papel). | |
| MGDDE5_6 | 26 | 5.6 | Estado de conservación microforma | Def: Estado del doc. original del cual se generó microforma. | `AN` |
| MGDDE5_7 | 27 | 5.7 | Disposición | Def: Destino planificado del documento (valoración documental). | |
| 6 | | | Relaciones | Def: Relaciones con otros docs, OAEs, personas. | |
| | | 6.1 | OAE Asociada | Def: Relaciones específicas con OAEs. | |
| MGDDE61_1 | 28 | 6.1.1 | Código OAE | Def: OAE que genera, gestiona o custodia el documento. | `AN, MU` |
| MGDDE61_2 | 29 | 6.1.2 | Nombre OAE | Def: Nombre institucional si no hay código de OAE. | `MU` |
| MGDDE61_3 | 30 | 6.1.3 | Tipo de relación doc-OAE | Def: Relación entre el doc. y el OAE (autor, custodio, etc.). | `AN, MU` |
| | | 6.2 | Otros actores | Def: Relaciones con personas naturales o jurídicas. | |
| MGDDE62_1 | 31 | 6.2.1 | Tipo de relación otros actores | Def: Tipo de relación entre el actor y el documento. | `AN, MU` |
| MGDDE62_2 | 32 | 6.2.2 | Tipo de actor relacionado | Def: Tipo de actor para determinar pertinencia del ID. | `MU` |
| MGDDE62_3 | 33 | 6.2.3 | Identificación de actor | Def: RUN/RUT/Pasaporte del actor relacionado. | `AN, MU` |
| MGDDE62_4 | 34 | 6.2.4 | Nombre del actor relacionado | Def: Nombre si no se cuenta con RUN/RUT. | `MU` |
| 7 | | | Seguridad | Def: Niveles de seguridad para la gestión. | |
| MGDDE7_1 | 35 | 7.1 | Nivel de Acceso | Def: Indicación relativa al acceso y consulta. | `AN` |
| MGDDE7_2 | 36 | 7.2 | Fecha fin restricción | Def: Fecha hasta la cual se presenta texto de advertencia. | |
| MGDDE7_3 | 37 | 7.3 | Texto Advertencia | Def: Texto a presentar si un usuario intenta acceder. | |
| MGDDE7_4 | 38 | 7.4 | Carácter sensible | Def: Identificación si el doc. contiene info sensible. | |
| 8 | | | Firma | Def: Tipo de firma electrónica utilizada. | |
| MGDDE8_1 | 39 | 8.1 | Tipo Firma | Def: Identificación del tipo de firma electrónica (simple/avanzada). | `MU` |
| MGDDE8_2 | 40 | 8.2 | Proveedor | Def: Proveedor del servicio de firma electrónica. | `MU` |
| MGDDE8_3 | 41 | 8.3 | Firma Electrónica Avanzada | Def: Indica si el doc. cuenta con FEA (Sí/No). | |
| | | 8.4 | Firmantes | | |
| MGDDE84_1 | 42 | 8.4.1 | Nombre/Cargo Representación | Def: Nombre y cargo de la persona que firma. | `MU` |
| MGDDE84_2 | 43 | 8.4.2 | RUN firmante | Def: RUN de la persona que firma. | `MU` |
| 9 | | | Procedimiento Asociado | Def: Identificación del PAT asociado. | |
| MGDDE9_1 | 44 | 9.1 | Código PAT asociado | Def: Código del PAT en CPAT asociado al documento. | |
| MGDDE9_2 | 45 | 9.2 | Nombre PAT asociado | Def: Nombre del PAT si no tiene código CPAT. | |
| 10 | | | Versión | Def: Versión del esquema de metadatos. | |
| MGDDE10_1 | 46 | 10.1| Versión MGDDE | Def: Versión del esquema de metadatos utilizado. | |

#### Especificaciones Detalladas: Metadatos de Documentos

ID: GDE-META-DOCUMENTOS-ESPECIFICACIONES-01
Purp: Detallar cada metadato para documentos.
Ref: AUDIT-ETE-INFORME-01

##### 1. Identificador (MGDDE1_1)

ID: GDE-META-DOC-SPEC-01
Ref: MGDDE1_1
Mech: Automático. Sistema asigna ID único a cada documento ingresado.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ctx: Asegurar unicidad, persistencia y estandarización de codificación.
Ex: `DOCU-20230925-001-XYZ`

##### 2. Código de serie (MGDDE1_2)

ID: GDE-META-DOC-SPEC-02
Ref: MGDDE1_2
Mech: Manual/Automático. Generado por sistema o manualmente según cuadro de clasificación OAE.
Cond: Obligatorio para transferencia al Archivo Nacional.
Cpt: Tipo-Dato. Def: Alfanumérico.

##### 3. Número de documento (MGDDE1_3)

ID: GDE-META-DOC-SPEC-03
Ref: MGDDE1_3
Mech: Manual/Automático. Número de orden interno recursivo dentro de una serie documental.
Cpt: Tipo-Dato. Def: Alfanumérico.

##### 4. Estado (MGDDE1_4)

ID: GDE-META-DOC-SPEC-04
Ref: MGDDE1_4
Mech: Manual/Automático. Identifica el estado de generación del documento.
Cpt: Tipo-Dato. Def: Alfanumérico.

##### 5. Versión (MGDDE1_5)

ID: GDE-META-DOC-SPEC-05
Ref: MGDDE1_5
Mech: Manual/Automático. Identificación del número de versión.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `1.1`

##### 6. Título del documento (MGDDE1_6)

ID: GDE-META-DOC-SPEC-06
Ref: MGDDE1_6
Mech: Manual. Título formal (automatizable) o atribuido (texto libre) si el tipo documental no lo incluye.
Cpt: Tipo-Dato. Def: Texto.
Ctx: Usar mayúsculas solo al inicio y en nombres propios.
Ex: `Resolución exenta asigna presupuesto para compra de insumos`

##### 7. Resolución de captura (MGDDE1_7)

ID: GDE-META-DOC-SPEC-07
Ref: MGDDE1_7
Mech: Automático. Sistema extrae info de metadatos embebidos del archivo.
Cond: Obligatorio para documentos de tipo Microforma.
Cpt: Tipo-Dato. Def: Texto.
Ctx: Cantidad de píxeles (horizontal x vertical).
Ex: `3000x2000`

##### 8. Nombre archivo asociado (MGDDE1_8)

ID: GDE-META-DOC-SPEC-08
Ref: MGDDE1_8
Mech: Automático. Sistema extrae el nombre del archivo.
Cpt: Tipo-Dato. Def: Texto.

##### 9. Tamaño (MGDDE2_1)

ID: GDE-META-DOC-SPEC-09
Ref: MGDDE2_1
Mech: Automático. Sistema extrae el volumen del archivo.
Cpt: Tipo-Dato. Def: Numérico (Kb).

##### 10. Cantidad de páginas o extensión (MGDDE2_2)

ID: GDE-META-DOC-SPEC-10
Ref: MGDDE2_2
Mech: Automático. Sistema extrae número de páginas o puede ser ingresado manualmente.
Cond: Obligatorio para documentos de tipo Microforma.
Cpt: Tipo-Dato. Def: Numérico.
Ex: `104`

##### 11. Formato (MGDDE2_3)

ID: GDE-META-DOC-SPEC-11
Ref: MGDDE2_3
Mech: Automático. Sistema extrae la extensión del archivo.
Cpt: Tipo-Dato. Def: Texto.
Ex: `pdf`

##### 12. Nombre y versión del software (MGDDE2_4)

ID: GDE-META-DOC-SPEC-12
Ref: MGDDE2_4
Mech: Automático. Sistema extrae info de metadatos embebidos del archivo.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Microsoft Word 2019`

##### 13. Resumen (MGDDE3_1)

ID: GDE-META-DOC-SPEC-13
Ref: MGDDE3_1
Mech: Manual. Relato sintético del contenido.
Cpt: Tipo-Dato. Def: Texto.

##### 14. Palabras claves documento (MGDDE3_2)

ID: GDE-META-DOC-SPEC-14
Ref: MGDDE3_2
Mech: Manual o mediante selector de vocabulario controlado.
Cpt: Tipo-Dato. Def: Texto.
Ctx: Palabras cortas, simples o compuestas que expresen lo más relevante.
Ex: `Resolución de compra tecnológica`, `Adquisición de licencias de software`

##### 15. Idioma (MGDDE3_3)

ID: GDE-META-DOC-SPEC-15
Ref: MGDDE3_3
Mech: Manual.
Cpt: Tipo-Dato. Def: Texto.

##### 16. Comuna (MGDDE3_4)

ID: GDE-META-DOC-SPEC-16
Ref: MGDDE3_4
Mech: Automático. Código de comuna según sistema de codificación.
Cpt: Tipo-Dato. Def: Numérico.

##### 17. Fecha de creación (MGDDE4_1)

ID: GDE-META-DOC-SPEC-17
Ref: MGDDE4_1
Mech: Automático. Generado según formato `aaaa-mm-dd hh:mm:ss` (ISO 8601).
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ctx: Modificable, con registro de historial de cambios.
Ex: `2023-20-11:16:56:57`

##### 18. Fecha de modificación (MGDDE4_2)

ID: GDE-META-DOC-SPEC-18
Ref: MGDDE4_2
Mech: Automático. Generado en cada actualización en repositorio (`aaaa-mm-dd hh:mm:ss`).
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ctx: Modificable, con registro de historial de cambios.
Ex: `2023-20-11:16:56:57`

##### 19. Fecha de captura (MGDDE4_3)

ID: GDE-META-DOC-SPEC-19
Ref: MGDDE4_3
Mech: Automático/Manual. Fecha de incorporación de docs no generados internamente (`aaaa-mm-dd hh:mm:ss`).
Cond: Obligatorio para Microformas.
Cpt: Tipo-Dato. Def: Fecha/Hora (ISO 8601).
Ex: `2023-20-11:16:56:57`

##### 20. Cobertura temporal (MGDDE4_4)

ID: GDE-META-DOC-SPEC-20
Ref: MGDDE4_4
Mech: Automático/Manual. Periodo de tiempo (fechas) al que hace referencia el acto del documento.
Cpt: Tipo-Dato. Def: Fecha.

##### 21. Tipo documental (MGDDE5_1)

ID: GDE-META-DOC-SPEC-21
Ref: MGDDE5_1
Mech: Manual. Selección de lista controlada. Ref: `GDE-META-LISTAS-TIPO-DOC-01`.
Cond: Obligatorio si se cuenta con la tipificación del documento.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 3 (Antecedente).
Ex: `30` (Oficio)

##### 22. Origen del documento (MGDDE5_2)

ID: GDE-META-DOC-SPEC-22
Ref: MGDDE5_2
Mech: Automático. Selección de lista controlada. Ref: `GDE-META-LISTAS-ORIGEN-DOC-01`.
Cond: Obligatorio para Microformas.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1.
Ex: `1` (repositorio externo)

##### 23. Mecanismo de incorporación del documento (MGDDE5_3)

ID: GDE-META-DOC-SPEC-23
Ref: MGDDE5_3
Mech: Automático/Manual. Selección de lista controlada. Ref: `GDE-META-LISTAS-MEC-INCORP-01`.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 2 (Digital).
Ex: `2`

##### 24. URI de documento externo (MGDDE5_4)

ID: GDE-META-DOC-SPEC-24
Ref: MGDDE5_4
Mech: Automático/Manual. URL o URI persistente del recurso.
Cond: Obligatorio para documentos externos referenciados.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `http://bibliotecadigital.dipres.gob.cl/handle/11626/19183`

##### 25. Ubicación física de documento referenciado (MGDDE5_5)

ID: GDE-META-DOC-SPEC-25
Ref: MGDDE5_5
Mech: Manual. Registro manual de la ubicación física según política de codificación institucional.
Cond: Obligatorio para documentos físicos referenciados (expediente híbrido, microforma).
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `space_40_archivador_20.5.10_oae_33706`

##### 26. Estado de conservación microforma (MGDDE5_6)

ID: GDE-META-DOC-SPEC-26
Ref: MGDDE5_6
Mech: Automático/Manual. Selección de lista controlada. Ref: `GDE-META-LISTAS-ESTADO-MICROFORMA-01`.
Cond: Obligatorio para documentos tipo microforma.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1 (Muy Bueno).
Ex: `1`

##### 27. Disposición (MGDDE5_7)

ID: GDE-META-DOC-SPEC-27
Ref: MGDDE5_7
Mech: Manual/Automático. Destino planificado del documento según proceso de valoración documental.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Preservación Institucional`

##### 28. Código OAE (MGDDE61_1)

ID: GDE-META-DOC-SPEC-28
Ref: MGDDE61_1
Mech: Automático. Sistema incorpora al menos código de OAE productor desde GESCODE.
Cpt: Tipo-Dato. Def: Numérico.
Ex: `46` (Gobierno Regional de la Región de La Araucanía)

##### 29. Nombre OAE (MGDDE61_2)

ID: GDE-META-DOC-SPEC-29
Ref: MGDDE61_2
Mech: Automático/Manual. Registro manual del nombre institucional.
Cond: Obligatorio si no se identifica por código OAE o por resolución del OAE.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `Gobierno Regional de la Región de La Araucanía`

##### 30. Tipo de relación entre documento y OAE (MGDDE61_3)

ID: GDE-META-DOC-SPEC-30
Ref: MGDDE61_3
Mech: Automático. Selección de lista controlada. Ref: `GDE-META-LISTAS-TIPO-REL-OAE-01`.
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Obligatorio registrar al menos autor institucional y custodio.
Cpt: Valor-Defecto. Def: 1 (Autor institucional).
Ex: `1`

##### 31. Tipo de relación con otros actores (MGDDE62_1)

ID: GDE-META-DOC-SPEC-31
Ref: MGDDE62_1
Mech: Automático/Manual. Selección de lista controlada. Ref: `GDE-META-LISTAS-TIPO-REL-ACTORES-01`.
Cond: Obligatorio al registrar una relación con el documento.
Cpt: Tipo-Dato. Def: Numérico.
Ctx: Al menos se debe registrar al autor/creador.
Cpt: Valor-Defecto. Def: 3 (Autor/creador).
Ex: `3`

##### 32. Tipo de actor relacionado (MGDDE62_2)

ID: GDE-META-DOC-SPEC-32
Ref: MGDDE62_2
Mech: Automático. Selección de lista controlada para indicar tipo de ID requerido. Ref: `GDE-META-LISTAS-TIPO-ACTOR-01`.
Cond: Obligatorio al registrar una relación con el documento.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1 (Ciudadano).
Ex: `1`

##### 33. Identificación de actor relacionado (MGDDE62_3)

ID: GDE-META-DOC-SPEC-33
Ref: MGDDE62_3
Mech: Automático/Manual. RUN/RUT/Pasaporte.
Cond: Obligatorio al registrar una relación con el documento.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `677368373-5`

##### 34. Nombre del actor relacionado (MGDDE62_4)

ID: GDE-META-DOC-SPEC-34
Ref: MGDDE62_4
Mech: Manual. Registro del nombre de la persona natural o jurídica.
Cond: Obligatorio al registrar una relación si no se cuenta con ID (RUN/RUT/Pasaporte).
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `Entel Chile`, `Julian Santelices Machuca`

##### 35. Nivel de acceso (MGDDE7_1)

ID: GDE-META-DOC-SPEC-35
Ref: MGDDE7_1
Mech: Manual. Selección de vocabulario controlado. Ref: `GDE-META-LISTAS-NIVEL-ACCESO-01`.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1 (Público).
Ex: `1`

##### 36. Fecha fin restricción (MGDDE7_2)

ID: GDE-META-DOC-SPEC-36
Ref: MGDDE7_2
Mech: Manual. Fecha hasta cuando se debe presentar el texto de advertencia.
Cpt: Tipo-Dato. Def: Fecha.

##### 37. Texto Advertencia (MGDDE7_3)

ID: GDE-META-DOC-SPEC-37
Ref: MGDDE7_3
Mech: Manual. Texto a presentar si un usuario intenta acceder.
Cpt: Tipo-Dato. Def: Texto.

##### 38. Información de carácter sensible (MGDDE7_4)

ID: GDE-META-DOC-SPEC-38
Ref: MGDDE7_4
Mech: Manual. Plataforma debe manejar registro de marca (Sí/No).
Cpt: Tipo-Dato. Def: Numérico (Lista controlada `1-SI / 2-NO`).
Cpt: Valor-Defecto. Def: 2 (NO).
Ex: `1`

##### 39. Tipo Firma (MGDDE8_1)

ID: GDE-META-DOC-SPEC-39
Ref: MGDDE8_1
Mech: Automático. Selección de lista controlada (ej. simple, avanzada).
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1 (AVANZADA).
Ex: `2` (SIMPLE)

##### 40. Proveedor (MGDDE8_2)

ID: GDE-META-DOC-SPEC-40
Ref: MGDDE8_2
Mech: Automático. Detección automática del proveedor de firma.
Cpt: Tipo-Dato. Def: Texto.

##### 41. Firma electrónica avanzada (MGDDE8_3)

ID: GDE-META-DOC-SPEC-41
Ref: MGDDE8_3
Mech: Automático. Detección automática si cuenta con FEA (Sí/No).
Cpt: Tipo-Dato. Def: Numérico (Lista controlada `1-SI / 2-NO`).
Cpt: Valor-Defecto. Def: 2 (NO).
Ex: `1` (SI)

##### 42. Nombre/Cargo Representación (MGDDE84_1)

ID: GDE-META-DOC-SPEC-42
Ref: MGDDE84_1
Mech: Automático/Manual. Detección automática o registro manual del firmante y su cargo.
Cpt: Tipo-Dato. Def: Texto.

##### 43. RUN firmante (MGDDE84_2)

ID: GDE-META-DOC-SPEC-43
Ref: MGDDE84_2
Mech: Manual/Automático. Registro del RUN al identificar al actor firmante.
Cpt: Tipo-Dato. Def: Alfanumérico (Formato RUN).

##### 44. Código procedimiento administrativo asociado (MGDDE9_1)

ID: GDE-META-DOC-SPEC-44
Ref: MGDDE9_1
Mech: Automático/Manual. Código desde Catálogo de Procedimientos Administrativos y Tramitaciones (CPAT).
Cond: Obligatorio si el documento está vinculado a un PA específico.
Cpt: Tipo-Dato. Def: Alfanumérico.
Ex: `5076`

##### 45. Nombre procedimiento administrativo asociado (MGDDE9_2)

ID: GDE-META-DOC-SPEC-45
Ref: MGDDE9_2
Mech: Manual. Registro manual del nombre del PA.
Cond: Obligatorio si el PA no se encuentra creado en CPAT.
Cpt: Tipo-Dato. Def: Texto.
Ex: `Convalidación de Programa de Perfeccionamiento Académico`

##### 46. Versión MGDDE (MGDDE10_1)

ID: GDE-META-DOC-SPEC-46
Ref: MGDDE10_1
Mech: Automático. Registro automático de la versión de la guía de metadatos.
Cpt: Tipo-Dato. Def: Numérico.
Cpt: Valor-Defecto. Def: 1.
Ex: `1`

### 5. Listas Controladas

ID: GDE-META-LISTAS-CONTROLADAS-ROOT-01
Purp: Definir los vocabularios controlados para estandarizar el registro de información en metadatos específicos.
Ctx: Disponible en Gestor de Códigos (GESCODE) para uso por OAEs.

#### Lista 1: Tipo Documental

ID: GDE-META-LISTAS-TIPO-DOC-01
Ref: MGDDE5_1
Cpt: Valores.

- `1`: Acta. Ex: Acta de Sesión, de evaluación, de consejo.
- `2`: Acuerdo. Ex: Acuerdo de comité, complementario, de compromiso.
- `3`: Antecedente. Ex: Antecedentes legales, personales, profesionales.
- `4`: Autorización. Ex: Autorización de apertura, de constitución, sanitaria.
- `5`: Base. Ex: Bases técnicas, de concurso, de licitación.
- `40`: Solicitud. Ex: Solicitud de permiso, de licencia, de subsidio.
- `41`: Términos de referencia. Ex: Para licitaciones, proyectos, estudios.
- `42`: Transcripción. Ex: De reuniones, de entrevistas, de audiencias.

#### Lista 2: Mecanismo de Incorporación

ID: GDE-META-LISTAS-MEC-INCORP-01
Ref: MGDDE5_3
Cpt: Valores.

- `1`: Físico
- `2`: Digital
- `3`: Digitalización

#### Lista 3: Estado Conservación Microforma

ID: GDE-META-LISTAS-ESTADO-MICROFORMA-01
Ref: MGDDE5_6
Cpt: Valores.

- `1`: Muy Bueno. Def: Sin deterioros. Fácil manipulación.
- `2`: Bueno. Def: Deterioros menores sin comprometer info. Fácil manipulación.
- `3`: Regular. Def: Hojas sueltas, manchas, rasgados menores. Manipular con cuidado.
- `4`: Malo. Def: Rasgados y faltantes >50%, daño biológico. Manipular con mucho cuidado.
- `5`: Muy Malo. Def: Deterioros extremos, incompletitud, microorganismos activos. Manipulación con extremo cuidado.

#### Lista 4: Tipo Relación OAE

ID: GDE-META-LISTAS-TIPO-REL-OAE-01
Ref: MGDEE51_3, MGDDE61_3
Cpt: Valores.

- `1`: Autor institucional
- `2`: Destinatario
- `3`: Productor / generador
- `4`: Custodia

#### Lista 5: Tipo Relación Otros Actores

ID: GDE-META-LISTAS-TIPO-REL-ACTORES-01
Ref: MGDEE52_1, MGDDE62_1
Cpt: Valores.

- `1`: Responsable
- `2`: Interesado
- `3`: Autor/creador
- `4`: Referido
- `5`: Destinatario
- `6`: Ministro de Fe

#### Lista 6: Tipo Actor Relacionado

ID: GDE-META-LISTAS-TIPO-ACTOR-01
Ref: MGDEE52_2, MGDDE62_2
Cpt: Valores.

- `1`: Ciudadano
- `2`: Extranjero
- `3`: Institución privada
- `4`: Funcionario

#### Lista 7: Nivel de Acceso

ID: GDE-META-LISTAS-NIVEL-ACCESO-01
Ref: MGDEE6_1, MGDDE7_1
Cpt: Valores.

- `1`: Público
- `2`: Restringido
- `3`: Secreto
- `4`: Reservado

#### Lista 8: Origen del Documento

ID: GDE-META-LISTAS-ORIGEN-DOC-01
Ref: MGDDE5_2
Cpt: Valores.

- `1`: Repositorio Externo
- `2`: Interoperabilidad
- `3`: Plataforma ciudadana
- `4`: Repositorio Ciudadano

## Guía de Anonimización de Datos

ID: TDE-KB-080-ANON-GUIA
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: STSador
Creation-Date: 2025-07-07
Modification-Date: 2025-07-07
Primary-Source: kb_080_tde_guia_anonimizacion.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 1. Introducción

ID: TDE-KB-080-INTRO-01
Cpt: Guía introductoria.
Obj: Ofrecer una introducción básica y concisa a la anonimización de datos.
Dest: Entidades y organizaciones que gestionan datos personales.
Purp: Servir como primera aproximación a conceptos, riesgos, técnicas y complejidad.
Ctx: Foco en anonimización de bases de datos estructuradas.
Warn: No es un manual exhaustivo; no aborda aspectos técnicos detallados.
Src: Guía Anonimización AEPD, Informe Anonimización Min. Asuntos Económicos (ES), Criterios Disociación AGESIC, otros.
Fnd: Contenido sin perjuicio de reglamentos futuros del Proyecto de Ley de Protección de Datos Personales de Chile.

### 2. Marco Conceptual

ID: TDE-KB-080-CONCEPTOS-01
Purp: Definir conceptos clave para la comprensión de la anonimización.

#### 2.1. Acrónimos y Fuentes

ID: TDE-KB-080-CONCEPTOS-ACRONIMOS-01

- Def: Acron-PDL. Ctx: Proyecto de Ley que regula la Protección y el Tratamiento de los Datos Personales y crea la Agencia de Protección de Datos Personales (Chile).

#### 2.2. Conceptos Fundamentales

ID: TDE-KB-080-CONCEPTOS-FUNDAMENTALES-01

- Cpt: Dato Personal.
- ID: TDE-KB-080-DEF-DATO-PERSONAL-01
- Def: Cualquier información vinculada/referida a una persona natural identificada o identificable.
- Src: PDL.
- Ctx: Criterio-Identificable. Posibilidad de determinar identidad (directa/indirecta) mediante identificadores (nombre, RUT) o elementos propios (físicos, fisiológicos, etc.).
- Cond: Excepción por esfuerzo de identificación desproporcionado.

- Cpt: Dato Sensible.
- ID: TDE-KB-080-DEF-DATO-SENSIBLE-01
- Def: Datos personales que revelan origen étnico/racial, afiliación política/sindical/gremial, hábitos personales, convicciones ideológicas/filosóficas, creencias religiosas, datos de salud, perfil biológico, datos biométricos, vida sexual, orientación sexual, identidad de género.
- Src: PDL.

- Cpt: Tratamiento de Datos.
- ID: TDE-KB-080-DEF-TRATAMIENTO-DATOS-01
- Def: Cualquier operación o procedimiento técnico (automatizado o no) sobre datos personales.
- Ctx: Acciones. recolectar, almacenar, grabar, organizar, elaborar, seleccionar, extraer, confrontar, interconectar, disociar, comunicar, ceder, transferir, transmitir, cancelar o utilizar.
- Src: PDL.

#### 2.3. Conceptos de Identificación

ID: TDE-KB-080-CONCEPTOS-IDENTIFICACION-01

- Cpt: Identificación.
- ID: TDE-KB-080-DEF-IDENTIFICACION-01
- Def: Proceso de reconocimiento o determinación de la identidad específica de una persona usando datos únicos asociados a ella.

- Cpt: Reidentificación.
- ID: TDE-KB-080-DEF-REIDENTIFICACION-01
- Def: Proceso de identificar a las personas específicas a las que pertenecen los datos a partir de un conjunto de datos tratado.
- Ctx: Riesgo clave a mitigar en procesos de anonimización.

- Cpt: Persona Identificada.
- ID: TDE-KB-080-DEF-PERSONA-IDENTIFICADA-01
- Def: Persona cuya identidad ya se conoce.
- Ex: "Juan Pérez".

- Cpt: Persona Identificable.
- ID: TDE-KB-080-DEF-PERSONA-IDENTIFICABLE-01
- Def: Persona cuya identidad es desconocida pero determinable (directa/indirectamente) mediante identificadores.

#### 2.4. Tipos de Atributos

ID: TDE-KB-080-CONCEPTOS-ATRIBUTOS-01

- Cpt: Identificadores Directos.
- ID: TDE-KB-080-DEF-ID-DIRECTO-01
- Def: Datos que identifican de manera unívoca a una persona.
- Ex: Nombres, números de identificación, direcciones exactas.

- Cpt: Identificadores Indirectos (Seudoidentificadores/Cuasi-identificadores).
- ID: TDE-KB-080-DEF-ID-INDIRECTO-01
- Def: Datos que, al combinarse con la misma u otras fuentes, pueden permitir identificar a un individuo.
- Ex: Datos sociodemográficos, configuración de navegador, ubicación geográfica.

- Cpt: Atributos Objetivos.
- ID: TDE-KB-080-DEF-ATRIBUTO-OBJETIVO-01
- Def: Atributos de datos que se pretenden analizar, esenciales para el propósito del procesamiento.

- Cpt: Registro.
- ID: TDE-KB-080-DEF-REGISTRO-01
- Def: Colección de atributos relacionados con un individuo, formando una unidad en un conjunto de datos.

- Cpt: Tabla de Ejemplos de Atributos.
- ID: TDE-KB-080-DEF-TABLA-EJEMPLOS-ATRIBUTOS-01
- [cite_start]Req: La estructura de tabla se preserva según la guía STS [cite: 316-317].

| Tipo de Atributo | Ejemplos Comunes | Ejemplos Adicionales |
| :--- | :--- | :--- |
| Identificadores Directos | - Nombre<br>- Email<br>- Teléfono móvil<br>- RUT<br>- Pasaporte<br>- Certificado de nacimiento<br>- Nombre de usuario | N/A |
| Identificadores Indirectos | - Edad<br>- Género<br>- Carrera<br>- Fecha de nacimiento<br>- Dirección<br>- Código postal<br>- Dirección laboral<br>- Nombre empresa<br>- Estado civil | - Altura<br>- Peso<br>- Dirección IP<br>- Matrícula vehículo<br>- N° bastidor vehículo<br>- Localización GPS |
| Atributos Objetivos | - Origen étnico<br>- Afiliación política/sindical<br>- Situación socioeconómica<br>- Convicciones ideológicas/filosóficas<br>- Creencias religiosas | - Datos de salud/perfil biológico<br>- Datos biométricos<br>- Datos vida sexual/orientación/identidad de género<br>- Transacciones (compras)<br>- Sueldo<br>- Calificación crediticia<br>- Póliza de seguro<br>- Diagnóstico médico<br>- Estado de vacunación |

#### 2.5. Estados de los Datos

ID: TDE-KB-080-CONCEPTOS-ESTADOS-DATOS-01

- Cpt: Datos Desidentificados.
- ID: TDE-KB-080-DEF-DATO-DESIDENTIFICADO-01
- Def: Datos procesados para eliminar/modificar identificadores directos.
- Ctx: Posibilidad de reidentificación minimizada, no eliminada. Podrían ser reidentificados bajo ciertas condiciones.

- Cpt: Datos Anonimizados.
- ID: TDE-KB-080-DEF-DATO-ANONIMIZADO-01
- Def: Datos que originalmente permitían identificar, pero tras proceso de anonimización, la reidentificación es imposible.
- Res: Deja de ser un dato personal.

- Cpt: Datos Seudonimizados.
- ID: TDE-KB-080-DEF-DATO-SEUDONIMIZADO-01
- Def: Tratamiento de datos personales que impide atribuirlos a un titular sin usar información adicional.
- Req: Información adicional debe figurar por separado y estar sujeta a medidas técnicas/organizativas de seguridad.

- Cpt: Dato Sintético.
- ID: TDE-KB-080-DEF-DATO-SINTETICO-01
- Def: Datos generados artificialmente, sin correspondencia directa con datos reales.
- Purp: Uso en análisis y procesos sin comprometer privacidad.

- Cpt: Datos Abiertos.
- ID: TDE-KB-080-DEF-DATO-ABIERTO-01
- Def: Dato digital con características técnicas/jurídicas para ser usado, reutilizado y redistribuido libremente por cualquier persona/entidad.

#### 2.6. Procesos de Tratamiento

ID: TDE-KB-080-CONCEPTOS-PROCESOS-01

- Cpt: Desidentificar.
- ID: TDE-KB-080-DEF-PROCESO-DESIDENTIFICAR-01
- Def: Eliminación de identificadores directos (nombre, RUT, etc.).
- Warn: Erróneamente confundido con anonimización. Es solo el primer paso.

- Cpt: Anonimización.
- ID: TDE-KB-080-DEF-PROCESO-ANONIMIZACION-01
- Def: Procedimiento irreversible donde un dato personal no puede vincularse/asociarse a una persona determinada.
- Mech: Destrucción/eliminación del nexo con la información identificatoria.
- Ctx: Riesgo Residual. Siempre subsiste un riesgo residual de reidentificación.
- Cause: (a) Posible combinación de datos o nuevas tecnologías; (b) Errores o modificaciones en el manejo de datos.
- Res: Un dato anonimizado deja de ser un dato personal.
- Src: PDL.

- Cpt: Seudonimización.
- ID: TDE-KB-080-DEF-PROCESO-SEUDONIMIZACION-01
- Def: Tratamiento de datos personales para que no puedan atribuirse a un titular sin información adicional.
- Req: Información adicional debe estar separada y protegida.
- Src: PDL.

- Cpt: Minimización de Datos.
- ID: TDE-KB-080-DEF-PROCESO-MINIMIZACION-01
- Def: Limitar recolección, almacenamiento y uso de datos personales a lo estrictamente necesario para el propósito especificado.
- Res: Reduce riesgo de violaciones de privacidad.

- Cpt: Clase de Equivalencia.
- ID: TDE-KB-080-DEF-CLASE-EQUIVALENCIA-01
- Def: Grupo de registros en una base de datos modificados para ser idénticos.
- Purp: Evitar vinculación directa de un registro a un individuo.
- Mech: Cada registro es indistinguible de al menos 'k-1' otros registros en el mismo conjunto.
- Ref: TDE-KB-080-TECNICAS-GENERALIZACION-01.

### 3. Riesgos de Reidentificación

ID: TDE-KB-080-RIESGOS-01
Def: Riesgos que surgen al tratar de proteger la identidad en conjuntos de datos.

- Cpt: Singularización.
- ID: TDE-KB-080-RIESGOS-SINGULARIZACION-01
- Def: Posibilidad de que los datos puedan usarse para identificar a una persona basándose en información única o una combinación de atributos.

- Cpt: Vinculabilidad.
- ID: TDE-KB-080-RIESGOS-VINCULABILIDAD-01
- Def: Capacidad de conectar dos o más registros (dentro del mismo o diferentes conjuntos de datos) que, combinados, pueden identificar a una persona.

- Cpt: Inferencia.
- ID: TDE-KB-080-RIESGOS-INFERENCIA-01
- Def: Posibilidad de deducir detalles específicos (a menudo sensibles) sobre una persona utilizando los datos disponibles, incluso si están modificados.

### 4. Framework del Proceso de Anonimización

ID: TDE-KB-080-PROCESO-01
Cpt: Etapas generales y orientativas.
Warn: No aborda aspectos técnicos detallados ni metodologías específicas.

#### 4.1. Fase 1: Identificar Objetivos

ID: TDE-KB-080-PROCESO-FASE1-01
Req: Diseño del proceso debe estar orientado a objetivos específicos.
Ex: Publicación como datos abiertos, uso interno restringido.
Cpt: Gobernanza.

- Req: Para uso restringido, incorporar acuerdos de confidencialidad con cláusulas sobre reidentificación y protección.
- Req: Definir claramente la unidad y funcionarios responsables del proceso.
- Req: Responsables deben tener conocimiento profundo de los contenidos de la base de datos.

#### 4.2. Fase 2: Clasificación de Atributos

ID: TDE-KB-080-PROCESO-FASE2-01
Purp: Clasificar adecuadamente los atributos de datos antes de la desidentificación.
Proc: Flujo de Decisión.

- 1. Pregunta: ¿Atributo es vital para el caso de uso?
- - Res: No -> Eliminar atributo. Ref: TDE-KB-080-DEF-PROCESO-MINIMIZACION-01.
- - Res: Si -> Proceder al paso 2.
- 2. Pregunta: ¿Atributo es un valor único?
- - Res: Si -> Clasificación probable: Identificador Directo. Ref: TDE-KB-080-DEF-ID-DIRECTO-01.
- - Res: No -> Proceder al paso 3.
- 3. Pregunta: ¿Atributo puede encontrarse en otras fuentes de datos (públicas/privadas)?
- - Res: Si -> Proceder al paso 4.
- - Res: No -> Clasificación probable: Identificador Indirecto. Ref: TDE-KB-080-DEF-ID-INDIRECTO-01.
- 4. Resultado: Clasificación probable -> Atributo Objetivo. Ref: TDE-KB-080-DEF-ATRIBUTO-OBJETIVO-01.

#### 4.3. Fase 3: Desidentificación de Datos

ID: TDE-KB-080-PROCESO-FASE3-01
Obj: Balancear utilidad de datos con necesidad de privacidad.
Act: Eliminación/modificación de identificadores (directos e indirectos).
Dep: Nivel de privacidad requerido y contexto de uso determinan el alcance.
Warn: Remover solo identificadores directos puede ser insuficiente.
Req: Evaluar y ajustar identificadores indirectos para prevenir reidentificación por interrelación con otras fuentes.
Cpt: Uso de Seudónimos.

- Cond: Útil en situaciones específicas para mantener vínculos con individuo original sin comprometer identidad.
- Ctx: Casos de Uso.
- - Purp: Fusión de Datos. Ctx: Permite combinar registros de diversas fuentes.
- - Purp: Análisis Múltiples Registros. Ctx: Permite análisis profundo manteniendo confidencialidad.
- - Purp: Generación Datos Sintéticos. Ctx: Permite desarrollar/probar aplicaciones sin datos reales.
- Req: Requisitos del Seudónimo.
- - Req: Debe ser único para cada identificador directo.
- - Req: Diseño debe impedir reversión por terceros no autorizados.
- - Ex: Código generado aleatoriamente, sin relación matemática/lógica con dato original (e.g., "José" -> "A3#m9Z!").
- Req: Gobernanza. Mantener una tabla segura (cifrada, acceso restringido) que vincule identificadores directos con seudónimos para gestión y cumplimiento legal.

Cpt: Ejemplos de Desidentificación.

- ID: TDE-KB-080-PROCESO-FASE3-EJEMPLOS-01
- Cpt: Ejemplo 1 - Eliminación de Identificador Directo.
- - Act: Se elimina la columna 'Nombre'.
- - Warn: Individuos podrían ser reidentificados al cruzar con otras fuentes públicas (e.g., perfiles redes sociales).
| Edad | Serie Favorita |
| :--- | :--- |
| 54 | The Big Bang Theory |
| 30 | Friends |
| 23 | Stranger things |
- Cpt: Ejemplo 2 - Seudonimización con Token.
- - Act: Se reemplaza 'Nombre' por 'Token' único y robusto.
- - Purp: Permitir vinculación interna sin revelar identidad.
| Token | Edad | Serie Favorita |
| :--- | :--- | :--- |
| 1234 | 54 | The Big Bang Theory |
| A3#m9Z! | 30 | Friends |
| 98gv$$M | 23 | Stranger things |

#### 4.4. Fase 4: Aplicación de Técnicas

ID: TDE-KB-080-PROCESO-FASE4-01
Act: Seleccionar y aplicar técnicas específicas para tratar identificadores indirectos y atributos objetivos.
Obj: Impedir asociación fácil con datos personales identificables.
Req: Equilibrar protección de privacidad vs. capacidad analítica de los datos.

#### 4.5. Fase 5: Finalización y Mantenimiento

ID: TDE-KB-080-PROCESO-FASE5-01

- Act: Realizar evaluación rigurosa de la utilidad de los datos anonimizados.
- Act: Documentar meticulosamente el balance privacidad/utilidad, técnicas aplicadas y ajustes.
- Purp: Documentación para auditoría y replicabilidad.
- Req: Cada entidad debe definir y aplicar su propio método para evaluar y monitorear constantemente el riesgo de identificación.
- Just: Asegurar efectividad continua frente a cambios en tecnología y contextos de uso.

### 5. Catálogo de Técnicas de Anonimización

ID: TDE-KB-080-TECNICAS-01
Obj: Minimizar riesgos de reidentificación.
Warn: La aplicabilidad y efectividad dependen del tipo de dato, contexto y legislación.
Rec: Consultar con expertos para determinar la técnica más adecuada.

#### 5.1. Enfoque: Enmascaramiento (Masking)

ID: TDE-KB-080-TECNICAS-ENMASCARAMIENTO-01
Def: Ocultar o eliminar información para evitar identificación directa.

- Cpt: Supresión de Registros
- ID: TDE-KB-080-TECNICAS-ENMASC-SUPRESION-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Eliminación de un registro completo. Afecta a múltiples atributos simultáneamente. |
| Ctx | Útil para eliminar registros atípicos (outliers) que son únicos o no cumplen otros criterios. Atípicos son más fáciles de reidentificar. |
| Instr | Eliminar por completo el registro. La supresión debe ser permanente, no un ocultamiento temporal. |
| Rec | Considerar impacto en análisis de datos (e.g., afecta precisión estadística de promedio, mediana). |

- Cpt: Enmascaramiento de Caracteres
- ID: TDE-KB-080-TECNICAS-ENMASC-CARACTERES-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Sustitución de caracteres originales por alternativos (e.g., asteriscos, "X") para ocultar información sensible sin alterar estructura. |
| Ctx | Útil para proteger datos donde solo una parte es sensible (e.g., números de ID, emails) y el resto puede ser visible. |
| Instr | Reemplazar caracteres específicos manteniendo el formato original. |
| Rec | Asegurar que el método no sea predecible. Considerar enmascaramiento completo para ocultar totalmente la información. |

- Cpt: Cifrados
- ID: TDE-KB-080-TECNICAS-ENMASC-CIFRADOS-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Convierte datos legibles a formato codificado, reversible solo con una clave específica. |
| Ctx | Útil para transmisión de datos sensibles en redes inseguras o almacenamiento en sistemas vulnerables. |
| Instr | Cifrar datos antes de transmitir/almacenar con algoritmos robustos. Gestionar claves adecuadamente. |
| Rec | Revisar robustez de algoritmos periódicamente. Implementar políticas de rotación de claves. |

#### 5.2. Enfoque: Aleatorización

ID: TDE-KB-080-TECNICAS-ALEATORIZACION-01
Def: Modificar o alterar la veracidad de los datos a nivel individual, respetando la distribución global.
Obj: Reducir vinculabilidad e inferencia.
Warn: Por sí sola no garantiza protección.
Rec: Combinar con otros métodos (e.g., filtrado, generalización).

- Cpt: Adición de Ruido
- ID: TDE-KB-080-TECNICAS-ALEAT-RUIDO-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Modifica datos originales con variaciones aleatorias para disociarlos de identificadores. |
| Ctx | Útil cuando los datos deben mantener estructura básica para análisis, pero requieren reducción de precisión. |
| Instr | Aplicar ruido de manera uniforme y precisa. Ajustar nivel de ruido para no comprometer calidad analítica. |
| Rec | Asegurar que la calidad y utilidad de los datos no se vean comprometidas. |

- Cpt: Permutación o Intercambio
- ID: TDE-KB-080-TECNICAS-ALEAT-PERMUTACION-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Mezcla valores de atributos en un conjunto de datos, asignándolos aleatoriamente a diferentes registros. |
| Ctx | Útil en análisis estadísticos donde es crucial ocultar identidades (e.g., datos financieros, médicos). |
| Instr | Asegurar que la permutación preserve correlaciones lógicas y estructura. Evitar permutar atributos objetivo con riesgo de identificación. |
| Rec | Validar que no se introducen distorsiones. Combinar con otras técnicas para mayor robustez. |

- Cpt: Privacidad Diferencial
- ID: TDE-KB-080-TECNICAS-ALEAT-PRIVACIDAD-DIFERENCIAL-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Añade ruido deliberadamente a los datos/consultas para que los resultados de análisis sean menos identificables a nivel individual. |
| Ctx | Ideal para compartir datos agregados sin revelar identidades. |
| Instr | Determinar cantidad de ruido necesaria para equilibrar privacidad e integridad. Supervisar y ajustar el nivel de ruido continuamente. |
| Rec | Mantener registro detallado de consultas. Evitar motores de búsqueda abiertos que permitan trazabilidad. Limitar resultados a datos estadísticos. |

#### 5.3. Enfoque: Generalización

ID: TDE-KB-080-TECNICAS-GENERALIZACION-01
Def: Diluir atributos específicos ajustando sus escalas o magnitudes.
Ex: Reemplazar ciudad por región; fecha específica por mes.
Warn: No garantiza anonimización completa por sí sola. Requiere aplicación adecuada y conjunta con otras técnicas.

- Cpt: K-Anonimidad
- ID: TDE-KB-080-TECNICAS-GENERAL-K-ANONIMIDAD-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Asegura que cada registro sea indistinguible de al menos 'k-1' otros registros (Clase de Equivalencia). Ref: TDE-KB-080-DEF-CLASE-EQUIVALENCIA-01. |
| Ctx | Útil para compartir datos dentro de un grupo sin revelar identidades, especialmente en grandes volúmenes. |
| Instr | Establecer un valor de 'k' que equilibre privacidad y utilidad. Ajustar registros para que cada clase de equivalencia sea uniforme. |
| Rec | Monitorear eficacia regularmente. Un 'k' muy alto puede reducir utilidad; un 'k' muy bajo compromete privacidad. |

- Cpt: Diversidad-L y Proximidad-T
- ID: TDE-KB-080-TECNICAS-GENERAL-L-DIVERSIDAD-T-PROXIMIDAD-01
| Propiedad | Descripción |
| :--- | :--- |
| Def | Extensiones de K-anonimato para mejorar protección contra inferencia. Diversidad-L: asegura 'L' valores únicos para atributos sensibles. Proximidad-T: ajusta distribución de atributos a la distribución general. |
| Ctx | Útil en bases de datos donde la preservación de atributos estadísticos es importante. |
| Instr | Elegir valores de L y T cuidadosamente. Verificar y ajustar clases de equivalencia para cumplir los estándares. |
| Rec | Asegurar que valores dentro de cada grupo sean uniformes. Revisar y actualizar periódicamente. |

#### 5.4. Enfoque: Seudonimización

ID: TDE-KB-080-TECNICAS-SEUDONIMIZACION-01
Ref: TDE-KB-080-DEF-PROCESO-SEUDONIMIZACION-01.

| Propiedad | Descripción |
| :--- | :--- |
| Def | Sustituye identificadores por valores alterados (tokens, hashes, etc.). No elimina totalmente la posibilidad de identificación, pero la dificulta. |
| Ctx | Útil cuando es crucial mantener cierto grado de vinculación entre datos sin revelar la identidad. |
| Mech | - Cifrado con clave secreta.<br>- Función hash (difícil de revertir).<br>- Función hash con clave almacenada.<br>- Descomposición en tokens. |
| Rec | Usar diferentes claves/seudónimos en distintos conjuntos de datos. Proteger las claves de acceso no autorizado. |

### 6. Gobernanza del Proceso

ID: TDE-KB-080-GOBERNANZA-01
Purp: Evaluar y gestionar los riesgos y aplicaciones de las técnicas de anonimización.

#### 6.1. Matriz de Mitigación de Riesgo por Técnica

ID: TDE-KB-080-GOBERNANZA-MATRIZ-RIESGO-01
Cpt: Niveles de Mitigación.

- Def: Eficaz. La técnica es efectiva para mitigar el riesgo.
- Def: Parcial. La técnica puede mitigar el riesgo en ciertas circunstancias.
- Def: Ineficaz. La técnica NO mitiga eficazmente el riesgo.

| Tipo de técnica | Técnica | Riesgo de Singularización | Riesgo de Vinculabilidad | Riesgo de Inferencia |
| :--- | :--- | :--- | :--- | :--- |
| Enmascaramiento | Supresión de registros | Ineficaz | Ineficaz | Ineficaz |
| | Enmascaramiento de caracteres | Ineficaz | Ineficaz | Ineficaz |
| | Cifrados | Ineficaz | Ineficaz | Parcial |
| Aleatorización | Adición de ruido | Ineficaz | Parcial | Parcial |
| | Permutación o intercambio | Ineficaz | Parcial | Parcial |
| | Privacidad diferencial | Parcial | Parcial | Parcial |
| Generalización | K-Anonimidad | Eficaz | Ineficaz | Ineficaz |
| | Diversidad-L | Eficaz | Ineficaz | Parcial |
| | Proximidad-T | Eficaz | Ineficaz | Parcial |
| Seudonimización | Cifrado por hash | Ineficaz | Ineficaz | Parcial |
| | Tokenización | Ineficaz | Ineficaz | Ineficaz |

#### 6.2. Matriz de Aplicación por Caso de Uso

ID: TDE-KB-080-GOBERNANZA-MATRIZ-APLICACION-01
Warn: Ejemplos ilustrativos. La elección final depende del contexto específico.

| Casos de uso | Técnicas de anonimización sugeridas |
| :--- | :--- |
| Publicación de Datos Abiertos | Supresión de registros, K-Anonimidad, Diversidad-L, Proximidad-T |
| Compartir datos entre Organizaciones| Supresión de registros, K-Anonimidad, Diversidad-L, Proximidad-T |
| Intercambio interno (datos desidentificados) | Supresión de registros, Enmascaramiento, Cifrado, Seudonimización |
| Intercambio interno (datos anonimizados) | Supresión de registros, Enmascaramiento de caracteres, Adición de ruido, Permutación o intercambio, Privacidad Diferencial |

#### 6.3. Recomendaciones Adicionales

ID: TDE-KB-080-GOBERNANZA-RECOMENDACIONES-01

- Rec: Calcular el riesgo de identificación ANTES de aplicar técnicas de anonimización.
- Purp: Entender el potencial de reidentificación original y cómo se modifica.
- Res: Ayuda a seleccionar la técnica más adecuada; guía la configuración de parámetros; maximiza protección sin comprometer excesivamente la utilidad.
- Req: Realizar evaluación continua del riesgo durante y después del proceso.
- Just: Asegurar que los datos permanezcan seguros frente a nuevas vulnerabilidades y técnicas de análisis.

### 7. Herramientas de Código Abierto

ID: TDE-KB-080-HERRAMIENTAS-01
Purp: Facilitar el proceso de anonimización de datos personales sin costo.

| Herramienta | Descripción | URL |
| :--- | :--- | :--- |
| ARX | Software de código abierto para anonimizar datos personales. | <https://arx.deidentifier.org/> |
| Amnesia | Herramienta local de anonimización de datos. Soporta garantías de k-anonimidad y km-anonimidad. | <https://amnesia.openaire.eu/> |

### 8. Casos de Uso

ID: TDE-KB-080-CASOS-USO-01
Purp: Describir contextos fundamentales donde se aplican técnicas de anonimización.

- Cpt: Caso 1: Publicación de Datos Abiertos
- ID: TDE-KB-080-CASOS-USO-DATOS-ABIERTOS-01
- Obj: Permitir a organizaciones compartir información valiosa sin comprometer la privacidad.

- Cpt: Caso 2: Compartir Datos entre Organizaciones
- ID: TDE-KB-080-CASOS-USO-INTER-ORG-01
- Obj: Proteger datos personales durante colaboraciones o servicios tercerizados.

- Cpt: Caso 3: Intercambio Interno de Datos
- ID: TDE-KB-080-CASOS-USO-INTRA-ORG-01
- Obj: Utilizar datos anonimizados para intercambio interno.
- Cond: El intercambio no requiere datos personales detallados (e.g., análisis de tendencias).
- Cond: Los datos involucrados son de naturaleza sensible (e.g., información financiera).

### 9. Conclusión

ID: TDE-KB-080-CONCLUSION-01

- Cpt: Resumen de la Guía
- ID: TDE-KB-080-CONCLUSION-RESUMEN-01
- Purp: Proporcionar visión general de técnicas de anonimización para gestión segura de datos personales.
- Ctx: Explora enfoques y herramientas (libres/sin costo) para implementación efectiva.

- Cpt: Advertencia sobre Alcance
- ID: TDE-KB-080-CONCLUSION-ADVERTENCIA-01
- Warn: La guía no propone una metodología específica para evaluación de riesgo ni detalla la aplicación técnica en profundidad.
- Rec: Colaborar con expertos para adaptar técnicas a necesidades y contextos específicos.

- Cpt: Mensaje Final
- ID: TDE-KB-080-CONCLUSION-MENSAJE-FINAL-01
- Ctx: La guía es un punto de partida para la educación y concienciación sobre la protección de la privacidad.
- Req: Compromiso continuo y adaptación a nuevos desafíos son esenciales para la efectividad.
- Obj: Cumplir regulaciones, respetar derecho a la privacidad y mantenerse efectivo ante cambios.

## Master Guide: Public Service Design Recommendations

ID: STS-GOV-SERVDESIGN-MASTER-01
Version: 1.0.0
Status: Published
Human-Creator: STSador
Human-Editor: STSador
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_072_tde_recomen_diseño_servs.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### Dimensión I: Foco en la Persona Usuaria y el Diseño del Servicio

ID: STS-GOV-SERVDESIGN-DIM1-UX-01
Purp: Agrupar recomendaciones sobre la comprensión del usuario y principios de diseño de servicio.
Cpt: 6 recomendaciones.

#### Rec-01: Comprensión de usuarios

ID: STS-GOV-SERVDESIGN-REC-01
Cpt: Comprender a las personas usuarias y sus necesidades.
Def: Entender a fondo necesidades y problemas de usuarios para diseñar soluciones efectivas y personalizadas.
Fnd: Basado en investigación y análisis detallados.
Obj: Mejorar experiencia y satisfacción de personas usuarias.
Just: El foco en usuario/problema revela aspectos inesperados de necesidades, percepciones y acciones, permitiendo que las soluciones respondan mejor a su contexto.
Proc: Acciones recomendadas.

- Act: Realizar periódicamente investigaciones de usuarios (cualitativas/cuantitativas).
- Act: Utilizar fuentes de información múltiples (datos admin, percepción, canales de atención) para mejorar la comprensión.
- Act: Construir prototipos rápidos para contrastar hipótesis y testear con usuarios.

#### Rec-02: Resolución completa de necesidades

ID: STS-GOV-SERVDESIGN-REC-02
Cpt: Resolver una necesidad de manera completa para las personas, colaborando con otros equipos.
Def: Diseñar servicios que permitan a usuarios cumplir un objetivo completo mediante colaboración inter-equipos e inter-institucional.
Req: Proporcionar información clara del estado de solicitudes durante todo el proceso.
Just: Las necesidades de las personas suelen exceder la prestación de una única institución; la integración de servicios facilita el cumplimiento de sus objetivos.
Proc: Acciones recomendadas.

- Act: Identificar propósitos de usuarios y definir servicios según estos.
- Act: Integrar servicios con otras instituciones públicas.
- Act: Facilitar acceso al seguimiento del estado de solicitudes.
- Act: Comprender y abordar limitaciones legales.
- Act: Colaborar abiertamente con otros organismos para evitar duplicidades.
- Act: Solicitar información solo una vez.
- Ref: STS-GOV-SERVDESIGN-REC-14.

#### Rec-03: Diseño simple e intuitivo

ID: STS-GOV-SERVDESIGN-REC-03
Cpt: Diseñar servicios simples e intuitivos.
Def: Implementar servicios fáciles de usar que permitan cumplir el propósito en el menor número de pasos, con la información necesaria para decidir.
Just: Servicios simples reducen tiempo y esfuerzo.
Res: Aumenta satisfacción usuaria, ahorra recursos al Estado, fomenta confianza pública.
Proc: Acciones recomendadas.

- Act: Asegurar que el servicio permita al usuario tener éxito al primer intento con mínima ayuda.
- Act: Analizar puntos de decisión del usuario en cada etapa, permitiendo foco en una tarea a la vez.
- Act: Validar usabilidad y experiencia digital con usuarios reales/potenciales.
- Act: Analizar todos los elementos de interacción del servicio (digitales y físicos).
- Act: Entregar una experiencia consistente de principio a fin, independiente del canal/etapa.

#### Rec-04: Accesibilidad y uso universal

ID: STS-GOV-SERVDESIGN-REC-04
Cpt: Garantizar que todas las personas usuarias puedan utilizar el servicio.
Def: Crear servicios utilizables por todas las personas, independientemente de sus circunstancias o capacidades (discapacidad, conectividad, habilidades digitales, pertinencia cultural).
Fnd: Ir más allá de accesibilidad universal hacia la inclusión amplia.
Just: El diseño accesible desde el inicio es más fácil que la reconversión y es indispensable para algunos, pero útil para todos.
Proc: Acciones recomendadas.

- Act: Cumplir estándares de accesibilidad universal (WCAG nivel AA).
- Act: Usar palabras simples y lenguaje claro.
- Act: Considerar perspectivas de inclusión y género.
- Act: Disponer de información en lenguas oficiales pertinentes.
- Act: Realizar validaciones con público potencial diverso, incluyendo personas con necesidades de acceso.
- Act: Considerar segmentos con dificultades, proporcionando apoyo adecuado en cualquier canal (incl. atención asistida).
- Act: Asegurar consistencia en los servicios para una experiencia sin barreras.

#### Rec-05: Experiencia integrada omnicanal

ID: STS-GOV-SERVDESIGN-REC-05
Cpt: Proporcionar una experiencia integrada, a través de todos los canales de atención y entre instituciones relacionadas.
Def: Diseñar una experiencia coherente que se ajuste a las necesidades de los usuarios, coordinando todos los canales de atención y equipos.
Just: La experiencia coherente en todos los canales genera confianza y evita confusión.
Proc: Acciones recomendadas.

- Act: Garantizar experiencia omnicanal con conexión fluida entre canales.
- Act: Trabajar con instituciones relacionadas para una experiencia consistente.
- Act: Asignar a cada canal los recursos necesarios para cumplir su rol.
- Act: Involucrar a equipos de atención, negocio y responsables en la investigación y toma de decisiones.
- Act: Fomentar trabajo conjunto de equipos de diferentes canales para alinear objetivos.
- Act: Realizar testeos periódicos y usar datos para diseñar mejoras en todos los canales.
- Act: Mantener al personal actualizado sobre todos los servicios y canales.
- Act: Estandarizar contenidos y establecer lineamientos claros para consistencia.

#### Rec-06: Evaluación sistemática

ID: STS-GOV-SERVDESIGN-REC-06
Cpt: Evaluar sistemáticamente el servicio para asegurar que satisfaga las necesidades de las personas.
Def: Diseñar métricas para evaluar si el servicio responde a las necesidades usuarias, usando datos constantemente para identificar mejoras.
Just: Permite saber si el servicio cumple su propósito desde la perspectiva del usuario y tomar decisiones informadas.
Proc: Acciones recomendadas.

- Act: Identificar y monitorear métricas que midan cómo el servicio resuelve la necesidad principal del usuario.
- Act: Usar datos para tomar decisiones sobre cómo solucionar problemas y mejorar el servicio.
- Act: Publicar datos de indicadores clave para mostrar desempeño.

### Dimensión II: Construcción de una Cultura Orientada a la Experiencia Usuaria

ID: STS-GOV-SERVDESIGN-DIM2-CULTURE-01
Purp: Agrupar recomendaciones sobre la creación de un entorno organizacional y gobernanza enfocada en el usuario.
Cpt: 3 recomendaciones.

#### Rec-07: Entorno cultural propicio

ID: STS-GOV-SERVDESIGN-REC-07
Cpt: Establecer un entorno propicio para una cultura y práctica del diseño y entrega de servicios.
Def: Crear un ambiente institucional que fomente una cultura sólida en diseño y entrega de servicios.
Fnd: Promoción de innovación, aprendizaje temprano, orientación al usuario y eficacia.
Just: Facilita colaboración, creatividad y aprendizaje continuo para servicios más innovadores y centrados en las personas.
Res: Mejora calidad de servicios y satisface mejor las necesidades.
Proc: Acciones recomendadas.

- Act: Establecer prácticas que faciliten aprendizaje continuo y transferencia de conocimiento.
- Act: Designar un rol responsable que promueva la visión centrada en el usuario.
- Act: Fomentar que líderes promuevan activamente entornos de apoyo al diseño de servicios.
- Act: Promover desarrollo de capacidades en diseño de servicios de forma transversal.

#### Rec-08: Gobernanza con visión integral

ID: STS-GOV-SERVDESIGN-REC-08
Cpt: Instalar una gobernanza con una visión integral en el diseño de servicios, conformando equipos multidisciplinarios y multinivel.
Def: Establecer una gobernanza para el diseño de servicios que involucre equipos diversos, capaces de crear y operar servicios de manera sostenible.
Just: Un equipo dedicado y multidisciplinario aporta diversas perspectivas, mejorando la calidad y satisfaciendo necesidades de todos los usuarios.
Proc: Acciones recomendadas.

- Act: Constituir un equipo multidisciplinario para las fases de investigación, diseño y desarrollo.
- Act: Involucrar a todos los actores clave (ciudadanía, negocio, técnicos, OIRS/SIAC).
- Act: Asegurar participación de distintos niveles jerárquicos para facilitar decisiones.
- Act: Proporcionar al equipo acceso a experiencia especializada (interna/externa).
- Act: Asegurar que el equipo cuente con las horas disponibles para ejecutar el diseño.

#### Rec-09: Iteración y mejora continua

ID: STS-GOV-SERVDESIGN-REC-09
Cpt: Iterar y mejorar continuamente los servicios con base en la retroalimentación y el análisis de resultados.
Def: Instalar la práctica permanente de evaluar, aprender e implementar mejoras en el servicio.
Fnd: Uso de métodos ágiles, participativos y centrados en el usuario.
Just: Permite adaptarse rápidamente a necesidades cambiantes e incorpora aprendizajes de la operación, usuarios y funcionarios.
Proc: Acciones recomendadas.

- Act: Implementar mecanismos permanentes de evaluación usuaria en todos los canales.
- Act: Visibilizar hallazgos y aprendizajes internamente y externamente.
- Act: Asegurar capacidad, recursos y flexibilidad técnica para iterar con frecuencia.
- Act: Priorizar mejoras de mayor valor para el usuario, respaldado por datos.
- Act: Adoptar formas de trabajo ágiles (inspeccionar, aprender, adaptar).
- Act: Documentar información, hallazgos y decisiones de procesos de mejora.

### Dimensión III: Definición de Procesos y Tecnologías de Soporte

ID: STS-GOV-SERVDESIGN-DIM3-TECH-01
Purp: Agrupar recomendaciones sobre la gestión de tecnología, datos y seguridad como soporte a los servicios.
Cpt: 5 recomendaciones.

#### Rec-10: Protección de la privacidad

ID: STS-GOV-SERVDESIGN-REC-10
Cpt: Proteger la privacidad de las personas usuarias mediante el diseño de servicios.
Def: Diseñar servicios que protejan la privacidad, recopilando solo datos estrictamente necesarios y evaluando qué se almacenará.
Fnd: Principio "Privacy by design".
Just: El Estado debe proteger la información personal. La falta de seguridad debilita la confianza pública.
Proc: Acciones recomendadas.

- Act: Recolectar sólo datos estrictamente necesarios para la operación.
- Act: Informar de manera clara y accesible la política de privacidad.
- Act: Implementar protección de datos en todos sus formatos desde las primeras fases del diseño.
- Act: Integrar controles de seguridad (cifrado, MFA, monitoreo continuo).
- Act: Asegurar cumplimiento de normativas legales y establecer auditorías.
- Act: Capacitar a los equipos en mejores prácticas de seguridad y privacidad.

#### Rec-11: Continuidad operacional y seguridad

ID: STS-GOV-SERVDESIGN-REC-11
Cpt: Resguardar la continuidad operacional y la seguridad en la entrega de servicios.
Def: Asegurar que los servicios del Estado estén disponibles de forma continua, contando con medidas preventivas y de restauración.
Req: Priorización basada en criticidad del servicio.
Just: La continuidad evita interrupciones que afectan a la ciudadanía. La ciberseguridad protege información crítica.
Proc: Acciones recomendadas.

- Act: Establecer un plan de acción ante fallas para restauración rápida.
- Act: Mantener sistemas actualizados y realizar copias de seguridad periódicas.
- Act: Implementar pruebas de vulnerabilidad, monitoreo y simulaciones de fallas.
- Act: Cumplir normativa vigente (Norma Técnica Ciberseguridad, Política Nacional Ciberseguridad 2023-2028, etc.).
- Act: Priorizar servicios más críticos.

#### Rec-12: Estándares abiertos y componentes comunes

ID: STS-GOV-SERVDESIGN-REC-12
Cpt: Priorizar estándares abiertos, componentes comunes y servicios compartidos.
Def: Basarse en estándares abiertos y componentes compartidos para servicios más flexibles, consistentes, escalables y accesibles.
Just: Asegura consistencia y accesibilidad, facilita interoperabilidad, reduce costos y permite adaptación futura.
Proc: Acciones recomendadas.

- Act: Utilizar estándares abiertos para facilitar interoperabilidad y evitar dependencias.
- Act: Utilizar servicios compartidos desarrollados/validados por Gobierno Digital.
- Act: Cumplir directrices técnicas y normativas de la Secretaría de Gobierno Digital.
- Act: Promover uso de servicios y herramientas compartidas para reducir redundancias.

#### Rec-13: Tecnologías seguras y adaptables

ID: STS-GOV-SERVDESIGN-REC-13
Cpt: Seleccionar tecnologías seguras, flexibles, escalables y adaptables a futuras necesidades.
Def: Elegir tecnologías que permitan crecimiento eficiente, evitando dependencia de proveedor. Priorizar código abierto.
Just: Permite que los servicios se adapten al crecimiento y a situaciones inesperadas sin afectar su calidad.
Proc: Acciones recomendadas.

- Act: Elegir tecnologías de código abierto y basadas en la nube para crecimiento flexible.
- Act: Asegurar que infraestructura pueda adaptarse a peaks de demanda.
- Act: Implementar monitoreo continuo para identificar problemas de capacidad/rendimiento.
- Act: Establecer planes de contingencia para operar en situaciones críticas.
- Act: Seguir lineamientos técnicos de la Secretaría de Gobierno Digital.
- Act: Adaptar arquitectura tecnológica para que sea flexible e interactúe por diferentes canales.

#### Rec-14: Eficiencia de datos e interoperabilidad

ID: STS-GOV-SERVDESIGN-REC-14
Cpt: Impulsar la eficiencia en la gestión de datos y la interoperabilidad.
Def: Diseñar servicios donde los datos sean interoperables, evitando que usuarios proporcionen la misma información múltiples veces.
Req: Garantizar integridad, calidad y disponibilidad de datos en todo su ciclo de vida.
Just: Compartir datos evita que las personas repitan información. Datos abiertos fomentan transparencia y mejoran servicios.
Proc: Acciones recomendadas.

- Act: Seguir directrices técnicas de la Secretaría de Gobierno Digital para interoperabilidad.
- Act: Utilizar la Red de Interoperabilidad del Estado.
- Act: Tratar datos como activo estratégico.
- Act: Evitar almacenar datos de otras instituciones; usar servicios de interoperabilidad.
- Act: Utilizar DatosGob, el repositorio oficial de datos abiertos.
- Act: Implementar mecanismos para que las personas no proporcionen la misma información más de una vez.
- Act: Establecer medidas de seguridad y conservación para garantizar integridad de datos.
- Act: Permitir combinación de datos para identificar patrones y tendencias.

## Master: Guía Evaluación Calidad Web y Servicios Digitales del Estado (Versión STS)

ID: KB-065-GUIA-EVAL-CALIDAD-WEB-STS-01
Version: 1.0.0
Status: Draft
Human-Creator: STSador
Human-Editor: STSador
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_065_tde_guia_calidad_web.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 1. Propósito y Definiciones

ID: STS-GUIA-CALIDAD-WEB-PROPOSITO-01

#### 1.1. Información General del Documento

ID: STS-GUIA-CALIDAD-WEB-INFO-GENERAL-01
Ref: GUIA-EVAL-CALIDAD-WEB-INFO-GENERAL-01
Resp: Gobierno de Chile, Secretaría de Gobierno Digital (SGD).
Src: Equipo de Servicios Digitales.
Ctx: Fecha de publicación original 27/12/2024; Versión original 1.0.

#### 1.2. Objetivo Principal

ID: STS-GUIA-CALIDAD-WEB-OBJETIVO-01
Ref: GUIA-EVAL-CALIDAD-WEB-OBJETIVO-01
Purp: Proveer marco de referencia práctico para evaluar y fortalecer la calidad de sitios web y servicios digitales del Estado.

- Obj: Mejorar experiencia de usuarios (personas/empresas) en interacción con plataformas públicas.
- Obj: Garantizar cumplimiento de estándares de calidad.
- Obj: Apoyar a Órganos de la Administración del Estado (OAEs) en desarrollo interno y contratación de proyectos externos.

#### 1.3. Contexto Estratégico

ID: STS-GUIA-CALIDAD-WEB-CONTEXTO-01
Ref: GUIA-EVAL-CALIDAD-WEB-CONTEXTO-01
Fnd: Ley N° 21.658 (Crea Secretaría de Gobierno Digital - SGD).
Resp: Secretaría de Gobierno Digital (SGD), Subsecretaría de Hacienda.
Cpt: Función Principal SGD. Def: Proponer y coordinar Estrategia de Gobierno Digital con enfoque integrado.
Fnd: Agenda de Modernización del Estado 2022-2026.
Cpt: Iniciativa Clave. Def: Plataforma Integrada de Servicios Públicos Digitales.

- Purp: Fijar estándares y herramientas para optimizar diseño, desarrollo y entrega de servicios digitales.
- Fnd: Ley de Transformación Digital del Estado.

#### 1.4. Glosario

ID: STS-GUIA-CALIDAD-WEB-DEFINICIONES-01
Ref: GUIA-EVAL-CALIDAD-WEB-DEFINICIONES-01
Purp: Glosario de términos técnicos utilizados en la guía.

- Def: Página Web. Ctx: Unidad de información específica de un sitio. Ex: `https://sitio.gob.cl/seccion/pagina`.
- Def: Plataforma Electrónica. Ctx: Software, datos e infraestructura que sustenta procesos/procedimientos.
- Def: Plataforma. Ctx: Sinónimo genérico de sitio web o servicio digital en este contexto.
- Def: Servicio Digital. Ctx: Prestaciones ofrecidas por OAEs a usuarios vía tecnologías digitales.
- Def: Servicio Digital Transaccional. Ctx: Servicio digital que requiere identificación para info personalizada o trámites.
- Def: Sistema. Ctx: Componentes informáticos que sustentan servicios digitales.
- Def: Sitio Web. Ctx: Conjunto de páginas bajo un mismo dominio. Ex: `https://sitio.gob.cl`.
- Def: URL. Ctx: Ubicación de una página web o archivo en internet.

### 2. Descripción del Instrumento

ID: STS-GUIA-CALIDAD-WEB-INSTRUMENTO-01

#### 2.1. Concepto General

ID: STS-GUIA-CALIDAD-WEB-CONCEPTO-01
Ref: GUIA-EVAL-CALIDAD-WEB-CONCEPTO-01
Mech: Evaluación por observación y verificación de aspectos clave sobre una muestra de páginas.
Cpt: Regla de Cumplimiento. Def: Pregunta de chequeo se cumple si es afirmativa en la mayoría de las páginas de la muestra (salvo indicación contraria).
Cpt: Formato. Def: Documento compartido para trabajo colaborativo.
Cpt: Variantes. Def: 2 (Sitios Web, Servicios Digitales Transaccionales).
Cpt: Acceso. Def: Ubicación no especificada en el documento original.

#### 2.2. Niveles de Prioridad

ID: STS-GUIA-CALIDAD-WEB-PRIORIDAD-01
Ref: GUIA-EVAL-CALIDAD-WEB-PRIORIDAD-01
Purp: Clasificación de indicadores según su obligatoriedad.

- Cpt: Nivel-1-Imprescindible. Def: Características mínimas obligatorias. Ctx: Ausencia = error, vulnerabilidad o ilegalidad.
- Cpt: Nivel-2-Esperable. Def: Condiciones esenciales para sitio gubernamental centrado en el usuario. Ctx: Cumple criterios de calidad reconocidos.
- Cpt: Nivel-3-Deseable. Def: Elementos que aportan valor agregado y reflejan un avance hacia la excelencia.

#### 2.3. Estructura de la Herramienta

ID: STS-GUIA-CALIDAD-WEB-ESTRUCTURA-01
Ref: GUIA-EVAL-CALIDAD-WEB-ESTRUCTURA-01
Purp: Descripción de las secciones (hojas) del documento de evaluación.

- Cpt: Sección Portada. Def: Presenta instrumento, método, evaluadores, escala, dimensiones, glosario.
- Cpt: Sección Muestra. Def: Registro de URLs de las páginas revisadas.
- Cpt: Sección Guía Técnica. Def: Tutoriales para realizar verificaciones técnicas específicas.
- Cpt: Sección Dimensiones. Def: Hojas de cálculo, una por dimensión, con indicadores y preguntas de chequeo.
- Cpt: Sección Resultados. Def: Hoja con puntaje ponderado por dimensión y nivel de obligatoriedad.
- Cpt: Sección Gráficos. Def: Visualización de resultados en un gráfico de barras.

#### 2.4. Dimensiones de Evaluación y Ponderaciones

ID: STS-GUIA-CALIDAD-WEB-DIMENSIONES-01
Ref: GUIA-EVAL-CALIDAD-WEB-DIMENSIONES-01
Purp: Detalle de las dimensiones y ponderaciones para cada tipo de instrumento.

##### 2.4.1. Ponderaciones para Sitios Web

ID: STS-GUIA-CALIDAD-WEB-DIMENSIONES-SITIOS-WEB-01
Ref: GUIA-EVAL-CALIDAD-WEB-DIMENSIONES-SITIOS-WEB-01

| Dimension | Ponderacion |
| - | - |
| Contenido y lenguaje claro | 13% |
| Usabilidad | 13% |
| Accesibilidad web | 10% |
| Arquitectura de información | 10% |
| Búsqueda y encontrabilidad | 8% |
| Responsividad móvil | 6% |
| Diseño e imagen institucional| 5% |
| Seguridad | 5% |
| Tecnología | 5% |
| Atención a la ciudadanía | 4% |
| Audiovisualidad | 3% |
| Enfoque de género | 2% |
| Imparcialidad e igualdad de trato| 2% |
| Inclusión | 2% |
| Promoción | 2% |
| Transparencia y apertura | 2% |
| Prevención de errores | 2% |
| Facilidad de acceso e independencia tecnológica | 2% |
| Interacción y retroalimentación | 2% |
| Rapidez de respuesta | 2% |

##### 2.4.2. Ponderaciones para Servicios Digitales Transaccionales

ID: STS-GUIA-CALIDAD-WEB-DIMENSIONES-SERVICIOS-DIGITALES-01
Ref: GUIA-EVAL-CALIDAD-WEB-DIMENSIONES-SERVICIOS-DIGITALES-01

| Dimension | Ponderacion |
| - | - |
| Usabilidad | 10% |
| Prevención de errores | 10% |
| Accesibilidad web | 8% |
| Interoperabilidad | 8% |
| Contenido y lenguaje claro | 6% |
| Responsividad móvil | 6% |
| Seguridad | 6% |
| Resolutividad | 6% |
| Facilidad de acceso e independencia tecnológica| 6% |
| Arquitectura de información | 4% |
| Atención a la ciudadanía | 4% |
| Diseño e imagen institucional| 4% |
| Tecnología | 4% |
| Interacción y retroalimentación | 4% |
| Rapidez de respuesta | 4% |
| Audiovisualidad | 2% |
| Enfoque de género | 2% |
| Imparcialidad e igualdad de trato| 2% |
| Inclusión | 2% |
| Promoción | 2% |

### 3. Metodología de Aplicación

ID: STS-GUIA-CALIDAD-WEB-APLICACION-01

#### 3.1. Fase Preparatoria

ID: STS-GUIA-CALIDAD-WEB-APLICACION-PREVIO-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-PREVIO-01

- Req: Familiarización con el instrumento de evaluación.
- Rec: Solicitar colaboración de perfiles multidisciplinarios de la institución (comunicaciones, diseño, informática, transparencia, etc.).

#### 3.2. Fase de Selección de Muestra

ID: STS-GUIA-CALIDAD-WEB-APLICACION-MUESTRA-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-MUESTRA-01

##### 3.2.1. Composición de Muestra para Sitios Web

ID: STS-GUIA-CALIDAD-WEB-APLICACION-MUESTRA-WEB-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-MUESTRA-WEB-01
Req: Mínimo 10 páginas web.

- Cpt: Composición. Def: Portada o página de inicio.
- Cpt: Composición. Def: >=2 páginas del menú principal (primer nivel, excluyendo portada).
- Cpt: Composición. Def: >=3 páginas de información interna (una debe ser de trámites/servicios si existen).
- Cpt: Composición. Def: Las 3 últimas noticias publicadas.
- Cpt: Composición. Def: >=1 formulario de contacto sin autenticación.
- Cond: Si no existe formulario, evaluar solo con los ítems anteriores.

##### 3.2.2. Ejemplo de Muestra para Sitios Web

ID: STS-GUIA-CALIDAD-WEB-APLICACION-EJEMPLO-MUESTRA-WEB-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-EJEMPLO-MUESTRA-WEB-01
Purp: Ilustrar composición de muestra requerida en `STS-GUIA-CALIDAD-WEB-APLICACION-MUESTRA-WEB-01`.
Adv: La siguiente tabla refleja fielmente los ejemplos del documento original.

| Categoria-Requerimiento-Original | URL-Ejemplo-Provista |
| --- | --- |
| Portada o página de inicio | `[No provista]` |
| Al menos las primeras 2 páginas del menú principal | `https://www.gob.cl/instituciones/` |
| Al menos 3 páginas de información interiores | `https://www.gob.cl/acerca-de/` |
| Al menos 3 páginas de información interiores | `https://www.gob.cl/tramitesyservicios/` |
| Las últimas 3 noticias publicadas | `https://www.gob.cl/noticias/ley-subsidio-transporte-publico-aprobada/` |
| Las últimas 3 noticias publicadas | `https://www.gob.cl/noticias/entrega-subsidios-habitacionales-proyecto-huertos-valle-tiltil/` |
| Al menos 1 formulario | `[No provista]` |

##### 3.2.3. Composición de Muestra para Servicios Digitales

ID: STS-GUIA-CALIDAD-WEB-APLICACION-MUESTRA-SD-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-MUESTRA-SD-01
Req: Flujo completo del trámite.

- Cpt: Composición. Def: Página de acceso al trámite (landing page con instrucciones).
- Cpt: Composición. Def: Flujo completo del trámite en línea.

##### 3.2.4. Recomendaciones Logísticas

ID: STS-GUIA-CALIDAD-WEB-APLICACION-RECOMENDACIONES-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-RECOMENDACIONES-01

- Rec: Usar dos monitores si es posible.
- Rec: Abrir todas las páginas de la muestra en pestañas separadas.

#### 3.3. Fase de Ejecución

ID: STS-GUIA-CALIDAD-WEB-APLICACION-EJECUCION-01

##### 3.3.1. Registro de Datos Iniciales

ID: STS-GUIA-CALIDAD-WEB-APLICACION-REGISTRO-INICIAL-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-REGISTRO-INICIAL-01
Act: Completar hoja "Inicio" del instrumento.

- Cpt: Dato. Def: Nombre institución/sitio.
- Cpt: Dato. Def: URL sitio/servicio.
- Cpt: Dato. Def: Nombre evaluador(a).
- Cpt: Dato. Def: Fecha de evaluación.
- Cpt: Dato. Def: Navegador utilizado.
- Cpt: Dato. Def: Dispositivo utilizado (escritorio, tablet, celular).

##### 3.3.2. Reglas de Evaluación

ID: STS-GUIA-CALIDAD-WEB-APLICACION-REGLAS-EVALUACION-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-REGLAS-EVALUACION-01
Purp: Criterios para responder cada pregunta de chequeo.

- Cpt: Regla de Obligatoriedad. Def: Contestar TODAS las preguntas (sin respuesta = 0 puntos).
- Cpt: Regla de Umbral. Def: Una pregunta se responde afirmativamente si el elemento evaluado está presente en >=50% de la muestra.
- Cpt: Regla de Falla Crítica. Def: Si se detecta una falla importante en UNA página de la muestra, la respuesta debe ser negativa, independientemente del % de cumplimiento.
- Cpt: Opción No Aplica. Def: Usar solo para casos donde el elemento no está presente o no es verificable.

##### 3.3.3. Gestión de Evidencia

ID: STS-GUIA-CALIDAD-WEB-APLICACION-EVIDENCIA-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-EVIDENCIA-01
Rec: Aportar evidencia de la verificación.

- Act: Capturar pantallas.
- Act: Guardar capturas en carpeta compartida.
- Act: Pegar enlace en columna de comentarios.
- Adv: Asegurar permisos de acceso a la carpeta.

##### 3.3.4. Cálculo de Puntaje por Indicador

ID: STS-GUIA-CALIDAD-WEB-APLICACION-PUNTAJE-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-PUNTAJE-01
Purp: Sistema de puntuación automático por indicador, basado en respuestas a preguntas de chequeo.

- Cpt: Puntaje 0. Def: Ninguna respuesta afirmativa.
- Cpt: Puntaje 1. Def: < 50% de respuestas afirmativas.
- Cpt: Puntaje 2. Def: >= 50% de respuestas afirmativas.
- Cpt: Puntaje 3. Def: Todas las respuestas afirmativas.
- Ref: STS-GUIA-CALIDAD-WEB-INTERPRETACION-CALCULO-01.

#### 3.4. Fase Post-Evaluación

ID: STS-GUIA-CALIDAD-WEB-APLICACION-POST-EVALUACION-01
Ref: GUIA-EVAL-CALIDAD-WEB-APLICACION-POST-EVALUACION-01
Purp: Visualización de resultados.
Cpt: Cálculo. Def: Automático una vez completada la evaluación.
Cpt: Hoja de Resultados. Def: Muestra resultados desagregados por dimensión y nivel de obligatoriedad, con porcentaje de cumplimiento total.
Cpt: Hoja de Gráficos. Def: Representa resultados en gráfico de barras por dimensión y nivel.

### 4. Interpretación de Resultados y Mejora

ID: STS-GUIA-CALIDAD-WEB-INTERPRETACION-01

#### 4.1. Método de Cálculo Ponderado

ID: STS-GUIA-CALIDAD-WEB-INTERPRETACION-CALCULO-01
Ref: GUIA-EVAL-CALIDAD-WEB-INTERPRETACION-CALCULO-01
Purp: Detallar cómo se calculan los puntajes finales.

- Cpt: Cálculo por Dimensión. Def: Promedio ponderado por dimensión, usando ponderación por nivel de obligatoriedad.
- Cpt: Factor Ponderación (Imprescindible). Def: 60%.
- Cpt: Factor Ponderación (Esperable). Def: 25%.
- Cpt: Factor Ponderación (Deseable). Def: 15%.
- Cpt: Cálculo Total Ponderado. Def: Promedio de cada nivel de obligatoriedad, considerando ponderación de cada dimensión.

#### 4.2. Elaboración del Plan de Mejora

ID: STS-GUIA-CALIDAD-WEB-INTERPRETACION-MEJORA-01
Ref: GUIA-EVAL-CALIDAD-WEB-INTERPRETACION-MEJORA-01
Rec: Implementar acciones correctivas enfocadas en cumplir con los indicadores.

- Cpt: Prioridad 1 (Imprescindibles). Act: Comenzar con los aspectos mínimos y obligatorios por ley. Just: Su cumplimiento es fundamental.
- Cpt: Prioridad 2 (Esperables). Act: Abordar una vez cumplidos los imprescindibles. Just: Son mejoras importantes pero no críticas.
- Cpt: Prioridad 3 (Deseables). Act: Trabajar al final. Just: Agregan valor adicional y optimizan la experiencia.
- Res: Mejora en la evaluación y en la experiencia del usuario.

## Redacción accesible para los usuarios

ID: GUIDE-STYLE-VOICETONE-01
Version: 1.0.0
Status: Draft
Human-Creator: STSador
Human-Editor: STSador
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-06
Modification-Date: 2025-07-06
Primary-Source: kb_073_tde_voz_tono.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 1. Principios Fundamentales

ID: GUIDE-STYLE-VOICETONE-PRINCIPLES-01
Purp: Definir los conceptos centrales de la comunicación digital del Estado y justificar su importancia.

#### 1.1. Conceptos Clave

ID: GUIDE-STYLE-VOICETONE-CONCEPTS-01

- Cpt: Voz.
- Def: Personalidad que define y representa a la institución.
- Cpt: Tono.
- Def: Expresión de la voz a través de distintas actitudes según el contexto.
- Instr: Para orientar la escritura, buscar redacción concisa, clara y consistente.
- Rec: Referenciar secciones con conceptos ya establecidos para mantener la consistencia.

#### 1.2. Importancia de la Guía

ID: GUIDE-STYLE-VOICETONE-IMPORTANCE-01

- Obj: Uniformidad del mensaje (consistencia).
- Obj: Establecer formato correcto para la entrega de mensajes.
- Obj: Asegurar comprensión por parte de instituciones y usuarios generales.
- Obj: Mejorar el alcance y la conexión con los usuarios.
- Obj: Fomentar la confianza y la funcionalidad.
- Rec: El contenido debe ser diseñado y testeado.

#### 1.3. Voz Institucional

ID: GUIDE-STYLE-VOICETONE-VOICE-01

- Req: Usar lenguaje ameno.
- Req: Informar de manera sencilla y directa.
- Req: Evitar tecnicismos innecesarios.
- Req: Dirigirse a todas las personas (organizaciones, Estado, ciudadanía, empresas).

#### 1.4. Tono de Comunicación

ID: GUIDE-STYLE-VOICETONE-TONE-01

- Cpt: Tono General.
- Def: Formal, no complejo.
- Obj: Ser comprensible para cualquier público (experto o no).
- Cpt: Tipo de Mensaje.
- Def: Instructivo y constructivo.
- Cpt: Rol del Emisor.
- Def: Experto que asesora de forma fácil, eficiente y didáctica.

### 2. Reglas Generales de Estilo

ID: GUIDE-STYLE-VOICETONE-RULES-GENERAL-01
Purp: Establecer directrices de redacción para lograr los principios de voz y tono definidos.

#### 2.1. Composición y Sintaxis

ID: GUIDE-STYLE-VOICETONE-RULES-SYNTAX-01

- Cpt: Voz Activa.
- Req: Usar voz activa.
- Prohib: Usar voz pasiva.
- Ex-Correcto: "Plataformas al servicio de las instituciones para facilitar los procesos de Transformación Digital."
- Ex-Incorrecto: "Las instituciones tienen a su servicio plataformas para los procesos de Transformación Digital."
- Cpt: Persona Gramatical.
- Req: Redactar en primera persona del plural ("nosotros") y tratar de "tú" al receptor.
- Ex-Correcto: "Ingresa tu nombre completo. Te damos la bienvenida."
- Ex-Incorrecto: "Ingrese su nombre completo. Bienvenido."
- Cpt: Positividad.
- Req: Emplear lenguaje positivo en lugar de negativo.
- Cpt: Inclusión.
- Req: Usar lenguaje genérico, no marcado por género.

#### 2.2. Léxico y Claridad

ID: GUIDE-STYLE-VOICETONE-RULES-LEXICON-01

- Cpt: Simplicidad.
- Req: Usar lenguaje simple pero formal.
- Cpt: Siglas.
- Prohib: Usar siglas en el cuerpo del texto.
- Cpt: Consistencia.
- Req: Homologar el uso de palabras y conceptos en todos los documentos.
- Instr: Cuidar la coherencia entre títulos y cuerpos de texto.
- Cpt: Reutilización.
- Rec: Reutilizar textos y conceptos definidos en la base de conocimiento (Wiki).

#### 2.3. Estructura y Densidad

ID: GUIDE-STYLE-VOICETONE-RULES-STRUCTURE-01

- Cpt: Brevedad.
- Req: Contenido debe ser sencillo, breve y preciso.
- Instr: Escribir de forma resumida, suprimir palabras repetitivas.
- Cpt: Concisión.
- Req: Usar palabras y oraciones cortas.
- Prohib: Evitar vueltas innecesarias.
- Cpt: Jerarquía.
- Req: Priorizar el mensaje principal.
- Instr: Empezar con el contenido más importante y organizar ideas con títulos y subtítulos descriptivos.

### 3. Reglas de Formato Específico

ID: GUIDE-STYLE-VOICETONE-RULES-FORMAT-01
Purp: Estandarizar la representación de tiempo y fechas para asegurar consistencia.

#### 3.1. Tiempo Verbal

ID: GUIDE-STYLE-VOICETONE-FORMAT-TENSE-01

- Req: Usar presente indicativo o imperativo directo.
- Ex-Correcto: "Conoce las siguientes fases."
- Ex-Incorrecto: "Aquí podrás conocer las siguientes fases."
- Prohib: Usar referencias temporales relativas (e.g., "Ayer", "hoy", "mañana").

#### 3.2. Fechas

ID: GUIDE-STYLE-VOICETONE-FORMAT-DATES-01

- Cpt: Formato Primario.
- Mdl: dd/mm/aaaa.
- Ex: 22/03/2019.
- Cpt: Formato Secundario.
- Mdl: [Día] dd/mm/aaaa.
- Ex: Sábado 09/03/2019.
- Just: Anteponer el nombre del día es opcional; usar solo si aporta claridad.
- Req: Para mes < 10, usar cero inicial (e.g., 01, 02).
- Req: Usar siempre 4 dígitos para el año.

#### 3.3. Horas

ID: GUIDE-STYLE-VOICETONE-FORMAT-HOURS-01

- Mdl: hh:mm.
- Rec: Acompañar con la palabra "horas".
- Ex: 00:00 horas.
- Ex: 23:59 horas.
- Req: Usar 00:00 para el inicio del día.
- Req: Usar 23:59 para el fin del día.
- Prohib: Usar "24:00".

### 4. Guía por Componente de Interfaz

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-01
Purp: Definir reglas de redacción para elementos específicos de la interfaz de usuario.

#### 4.1. Títulos y Bajadas

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-TITLES-01

- Cpt: Capitalización.
- Req: Títulos inician con mayúscula, resto en minúscula.
- Cond: Nombres propios y siglas siempre deben ir en mayúscula.
- Cpt: Bajada (Subtítulo).
- Def: Texto que complementa al título.
- Purp: Dar instrucciones o información adicional.
- Cond: Su uso no es obligatorio; omitir si el título es suficientemente descriptivo.

#### 4.2. Párrafos

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-PARAGRAPHS-01

- Req: Una idea por párrafo.
- Req: Máximo 20 palabras por frase.
- Rec: Máximo 5 líneas por párrafo.

#### 4.3. Listas

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-LISTS-01

- Purp: Evitar largos bloques de texto mediante la estructuración de la información.
- Cpt: Listas de Viñetas.
- Purp: Enumerar elementos sin un orden específico.
- Ex:
- - Identidad digital
- - Estandarización de Procesos del Estado
- - Un Estado basado en datos
- Cpt: Listas Numéricas.
- Purp: Organizar contenido en pasos o eventos sucesivos.
- Ex:
- 1. Publicación de la ley
- 2. Modificaciones del procedimiento
- 3. Fase de preparación
- Cpt: Puntuación.
- Req: Ítems de listas con palabras o frases cortas no requieren signo de puntuación final.
- Req: Ítems de listas que contienen oraciones completas o párrafos descriptivos deben ser puntuados al final.

#### 4.4. Botones y Vínculos

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-BUTTONS-01

- Req: Usar verbos en imperativo o infinitivo que llamen a la acción.
- Rec: Acompañar el verbo con una descripción de la acción resultante.
- Ex: "Guardar borrador".
- Ex: "Descargar PDF".
- Ex: "Iniciar sesión".
- Prohib: Usar textos genéricos que no informan sobre el destino (e.g., "Aquí", "Ver más").

#### 4.5. Textos Alternativos (Alt Text)

ID: GUIDE-STYLE-VOICETONE-COMPONENTS-ALTTEXT-01

- Def: Descripción textual de imágenes para accesibilidad.
- Cpt: Imágenes Funcionales.
- Req: Describir el objetivo de la ilustración o foto en no más de dos líneas.
- Ex: "Ilustración del proceso de elecciones: una mano deposita un voto en una urna."
- Cpt: Imágenes Decorativas.
- Req: El atributo `alt` debe ser nulo o vacío para imágenes sin valor informativo.

### 5. Recursos Adicionales

ID: GUIDE-STYLE-VOICETONE-RESOURCES-01

- Cpt: Video explicativo.
- Desc: Material audiovisual sobre voz y tono.
- Ctx: Vínculo no disponible en el documento fuente.
