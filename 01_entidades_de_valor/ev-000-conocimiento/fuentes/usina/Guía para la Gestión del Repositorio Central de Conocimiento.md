# Guía para la Gestión del Repositorio Central de Conocimiento

## **1. Filosofía y Principios Fundamentales**

* **Propósito:** Establecer los principios fundamentales para la administración del Centro de Conocimiento (`Knowledge Hub`) como un sistema de ingeniería, en lugar de una simple colección de documentos.
* **Misión:** Asegurar que todos los activos de conocimiento sean localizables, auditables, versionables y reutilizables a través de todo el ecosistema de asistentes de inteligencia artificial del Gobierno Regional.

A continuación se detallan los principios rectores:

* **Principio 1 – El Conocimiento como un Activo Gestionado:** Cada artefacto de conocimiento es tratado con el mismo rigor que el código de software. Posee un ciclo de vida definido, está sujeto a estrictos controles de calidad y se administra en un sistema de control de versiones.
* **Principio 2 – Centro Unificado, Dominios Federados:** Todo el conocimiento reside en un único repositorio maestro (el `Hub`), pero se organiza de manera estricta en dominios separados y autocontenidos (ej. `core`, `gore_nuble`). Esta estructura previene la contaminación cruzada de información y simplifica la gobernanza y el mantenimiento.
* **Principio 3 – Composición por sobre Ramificación:** Las bases de conocimiento específicas para cada asistente se construyen mediante la "composición" de artefactos granulares e independientes. Se prohíbe explícitamente el uso de ramas de Git para gestionar variaciones de contenido para diferentes asistentes, ya que se considera un anti-patrón crítico que compromete la integridad del sistema.
* **Principio 4 – Gobernanza Explícita:** La estructura, la nomenclatura y el ciclo de vida de cada activo de conocimiento están gobernados exclusivamente por las reglas contenidas en esta guía y deben estar registrados en el Catálogo de Conocimiento.
* **Principio 5 – Integración con el Ciclo de Vida del Asistente:** Esta guía sirve como la implementación detallada de la capa de gestión del conocimiento descrita en el `Marco Metodológico para el Ciclo de Vida de Asistentes de IA`.

## **2. Arquitectura de Directorios**

* **Propósito:** Definir la estructura de directorios estandarizada y obligatoria para todos los activos relacionados con el conocimiento.
* **Requisito:** Esta estructura debe ser implementada en la raíz del repositorio de código.

* `/knowledge/`: Directorio raíz que contiene todos los artefactos de conocimiento validados, curados y listos para ser consumidos por los asistentes.
  * **Requisito:** Solo los archivos ubicados en este directorio pueden ser referenciados en la directiva de configuración de un asistente.
  * `knowledge/core/`: Contiene conocimiento fundacional y transversal a toda la organización, como las guías maestras de estándares y metodologías.
  * `knowledge/domains/{nombre_dominio}/`: Contiene conocimiento específico de un área de negocio o contexto particular (ej. `gore_nuble/`, `juridico/`).
  * `knowledge/catalog/`: Contiene el inventario maestro de todos los activos de conocimiento.

* `/sources/`: Repositorio para materiales en bruto y sin procesar (ej. archivos PDF, documentos de Word, borradores). Estos archivos son los insumos para el proceso de curación y transformación.

* `/staging/`: Área de trabajo temporal donde los artefactos de conocimiento son transformados y refactorizados a los formatos `STS` o `SFD` antes de ser auditados y publicados.

* `/agents/`: Contiene los archivos de definición (`agent.yaml`) de todos los asistentes de IA. Cada asistente reside en su propio subdirectorio.

## **3. Convención de Nomenclatura de Activos**

* **Propósito:** Definir una convención estricta y legible por máquina para nombrar los archivos de artefactos de conocimiento dentro del directorio `/knowledge/`.
* **Modelo:** `{tipo}_{dominio}_{id-num}_{descripcion-corta}_{formato}.md`

* **Componentes del Nombre:**
  * `tipo`: Indica la naturaleza del artefacto (`kb` para base de conocimiento, `guide` para guías de gobernanza, `sfd` para formularios).
  * `dominio`: Abreviatura del dominio al que pertenece (`core` para transversal, `gn` para GORE Ñuble).
  * `id-num`: Identificador secuencial de 3 dígitos dentro de su tipo y dominio (ej. `001`, `042`).
  * `descripcion-corta`: De 2 a 4 palabras en minúsculas y separadas por guiones que describen el contenido (ej. `contexto-regional`).
  * `formato`: El estándar estructural aplicado al contenido (`sts` o `sfd`).
  * `extensión`: El nombre final debe incluir el formato como un sufijo antes de la extensión `.md` (ej. `_sts.md`).

* **Ejemplos de Nombres Válidos:**
  * `kb_gn_001_contexto-regional_sts.md`
  * `guide_core_001_alm-master_sts.md`
  * `sfd_gn_005_formulario-postulacion_sfd.md`

## **4. El Catálogo de Conocimiento**

* **Propósito:** Especificar la estructura, el propósito y el mantenimiento del catálogo maestro de conocimiento.
* **Fundamento:** El catálogo es la única fuente de verdad para descubrir y comprender los activos de conocimiento disponibles en la organización.

* **Archivo Maestro:** El catálogo reside en el archivo `knowledge/catalog/catalog_master_sts.md`, cuya existencia y mantenimiento son obligatorios.

* **Estructura de Entrada:** Cada entrada en el catálogo representa un único artefacto de conocimiento y debe proveer metadatos clave para su rápida identificación:
  * `ID`: Identificador único del catálogo.
  * `Purp`: Propósito del artefacto.
  * `Cpt: Skeleton`: Un esquema o esqueleto del contenido del artefacto, listando sus encabezados principales para permitir una evaluación rápida de su estructura sin necesidad de abrir el archivo.

## **5. Ciclo de Vida del Conocimiento y Proceso de Curación**

* **Propósito:** Detallar el proceso auditable de extremo a extremo para la creación, validación y publicación de un artefacto de conocimiento.
* **Proceso:** El ciclo consta de 6 fases.

1. **Fase 1 - Abastecimiento (Sourcing):** Se identifican los materiales fuente en bruto necesarios y se almacenan en el directorio `/sources/`.
2. **Fase 2 - Puesta en Escena y Transformación (Staging):** El archivo fuente se copia al directorio `/staging/`, donde se le aplica la metodología de refactorización definida en la `Norma para la Elaboración de Artefactos de Conocimiento Institucional` (STS) o en el `Estándar para la Digitalización Estructurada de Formularios` (SFD).
3. **Fase 3 - Auditoría:** Se realiza una auditoría de cumplimiento utilizando la lista de verificación definida en la normativa correspondiente (`Norma para la Elaboración de Artefactos de Conocimiento Institucional` o `Estándar para la Digitalización Estructurada de Formularios`). El artefacto debe superar el 100% de los controles para proceder.
4. **Fase 4 - Publicación:** Se determina el nombre de archivo final según la convención de nomenclatura y el archivo validado se mueve desde `/staging/` a su destino final en el directorio `/knowledge/`. Si es necesario, se ejecuta el Protocolo de Sincronización de KB definido en el `Marco Metodológico para el Ciclo de Vida de Asistentes de IA`.
5. **Fase 5 - Registro:** Se actualiza el catálogo maestro (`catalog_master_sts.md`), añadiendo una nueva entrada para el artefacto recién publicado.
6. **Fase 6 - Mantenimiento:** Cualquier actualización a un artefacto existente inicia un nuevo miniciclo. El archivo se mueve de vuelta a `/staging` para su modificación, es re-auditado, y luego se mueve nuevamente a `/knowledge`, sobrescribiendo la versión anterior. El protocolo de sincronización debe ser re-ejecutado para actualizar las plataformas de despliegue.

## **6. Estrategia de Versionamiento con Git**

* **Propósito:** Establecer el uso correcto y obligatorio de Git para el control de versiones de los activos de conocimiento.
* **Fundamento:** Se basa en el principio de "Composición por sobre Ramificación".

* **El Anti-Patrón (Práctica Prohibida):** Se prohíbe la creación de ramas de Git para gestionar diferentes configuraciones de conocimiento para distintos asistentes. Esta práctica genera conflictos de fusión inmanejables, destruye la única fuente de verdad y hace imposible la auditoría.

* **El Patrón Correcto (Composición a Nivel de Agente):**
  * **Instrucción:** La base de conocimiento para cualquier asistente se define explícitamente ("se compone") en su archivo de configuración `agent.yaml`.
  * **Mecanismo:** La directiva `KB.GOVERNANCE.SOURCE_FILES` lista el conjunto exacto de artefactos de conocimiento que el asistente utilizará.
  * **Resultado:** Este enfoque es declarativo, auditable y mantiene la integridad de cada artefacto individual. Git se utiliza para versionar la historia de cada archivo, no para gestionar conjuntos de configuración.

* **Convención de Mensajes de Commit:**
  * **Requisito:** Todos los commits deben adherirse a la especificación de "Commits Convencionales", detallada en el `Marco Metodológico para el Ciclo de Vida de Asistentes de IA`.
  * **Instrucción:** Para los cambios que afecten exclusivamente a artefactos de conocimiento, se debe utilizar el tipo `kb`.
  * **Ejemplo:** `kb(gn_001): actualizar contexto regional con datos del censo 2024`
