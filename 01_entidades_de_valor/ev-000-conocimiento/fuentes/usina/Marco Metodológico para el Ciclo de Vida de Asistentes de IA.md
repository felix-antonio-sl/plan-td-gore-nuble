# Marco Metodológico para el Ciclo de Vida de Asistentes de IA

## **0. Preliminares**

### **0.1. Propósito y Audiencia**

El propósito de esta guía es establecer un marco de ingeniería unificado y estandarizado para el diseño, desarrollo, despliegue y mantenimiento de los asistentes de inteligencia artificial (IA) en el Gobierno Regional de Ñuble.

Este documento está dirigido a los siguientes perfiles profesionales: Arquitectos de Conocimiento, Ingenieros de IA, Desarrolladores de Agentes y Especialistas en la implementación de sistemas de Recuperación Aumentada de Información (RAG).

### **0.2. Prerrequisitos de Conocimiento**

Se requiere una comprensión funcional de los estándares y metodologías referenciados a continuación para la correcta aplicación de los principios aquí expuestos:

* `Norma para la Elaboración de Artefactos de Conocimiento Institucional`
* `Protocolo de Programación Declarativa de Asistentes de IA`
* `Estándar para la Digitalización Estructurada de Formularios`

### **0.3. Alcance de la Metodología**

* **Dentro del Alcance:** La presente metodología cubre el ciclo de vida completo para el desarrollo de asistentes de IA que integran capacidades de recuperación aumentada de información (RAG) y la ejecución de acciones predefinidas.
* **Fuera del Alcance:** No se abordan en este documento las técnicas avanzadas de ajuste fino (*fine-tuning*) de modelos de lenguaje ni el entrenamiento de modelos fundacionales desde cero.

## **1. Filosofía y Principios Arquitectónicos**

### **1.1. Misión Central**

La misión fundamental de este marco de trabajo es facilitar la transición desde la simple creación de instrucciones (*prompts*) hacia una disciplina formal de **ingeniería de asistentes**. Se establece que un asistente de IA debe ser tratado como un artefacto de software, con un ciclo de vida, controles de calidad y mantenibilidad definidos, en lugar de ser considerado un texto en lenguaje natural.

El objetivo principal es maximizar la predictibilidad de su comportamiento, la facilidad de su mantenimiento a largo plazo y la fidelidad con la que ejecuta las tareas encomendadas.

### **1.2. Principio Arquitectónico: Separación de Responsabilidades**

Para garantizar la robustez y escalabilidad de los asistentes, su arquitectura se basa en una estricta separación entre lo que el asistente *sabe* y lo que el asistente *hace*.

* **Componente de Lógica (`Código`):** Corresponde a la definición declarativa del comportamiento del asistente, formalizada en su archivo de configuración (`agent.yaml`). Este componente define **CÓMO** el asistente piensa y actúa.
* **Componente de Conocimiento (`Datos`):** Corresponde a la base de conocimiento estructurada (archivos `KB/*.md`) sobre la cual opera el asistente. Este componente define **QUÉ** es lo que el asistente sabe.

Esta separación se implementa a través de los siguientes sub-principios fundamentales:

* **Principio 1.2.1 – Interfaz Pública vs. Implementación Privada:** El comportamiento observable del asistente (su flujo de control, los pasos que declara seguir) se considera su "interfaz pública". La lógica de negocio compleja, el razonamiento detallado y los procesos internos constituyen su "implementación privada" y deben permanecer encapsulados. Esta separación, análoga a las prácticas estándar en ingeniería de software, minimiza la superficie de exposición de la lógica interna y maximiza la confidencialidad de los procesos.
* **Principio 1.2.2 – Abstracción Semántica en la Comunicación:** Toda comunicación del asistente con un usuario final debe abstraer los detalles de su implementación interna. El asistente debe describir sus capacidades en términos funcionales y centrados en el usuario, evitando cualquier tipo de jerga técnica interna (por ejemplo, identificadores de estados, nombres de archivos de conocimiento o acrónimos del marco de trabajo).
* **Principio 1.2.3 – Cartografía Explícita del Conocimiento:** El proceso mediante el cual un asistente vincula una consulta del usuario con un documento específico de su base de conocimiento debe ser un paso explícito, determinista y verificable, no una búsqueda semántica implícita. La dependencia de la interpretación semántica no acotada del modelo es una fuente primaria de inconsistencias factuales (conocidas como "alucinaciones"). Al implementar un mapa de enrutamiento explícito, la recuperación de conocimiento se transforma en una operación de consulta fiable y de alta fidelidad. Todo asistente que utilice una base de conocimiento debe, por tanto, implementar este patrón.
* **Principio 1.2.4 – Modelo de Ejecución Explícito:** El método para cargar las instrucciones que definen al asistente en el modelo de lenguaje debe ser una decisión de diseño explícita. Existen dos modelos: **Ejecución Directa**, donde las instrucciones se insertan directamente en la plataforma; y **Ejecución Indirecta**, donde una instrucción "cargador" (*bootloader*) instruye al modelo para que cargue y ejecute su configuración desde un archivo adjunto. Esta distinción es crítica para plataformas con limitaciones en la longitud de las instrucciones.

### **1.3. El Ecosistema Normativo**

La integridad y gobernanza del ciclo de vida de los asistentes se sustenta en la aplicación coordinada de un conjunto de normativas institucionales interconectadas:

* **Capa de Gobernanza del Conocimiento:** Se rige por la `Guía para la Gestión del Repositorio Central de Conocimiento`, que establece cómo se organizan y mantienen todos los activos de conocimiento.
* **Capa de Estructura del Conocimiento:** Se rige por la `Norma para la Elaboración de Artefactos de Conocimiento Institucional (STS)`, que define el formato estándar para todo el contenido documental.
* **Capa de Definición del Asistente:** Se rige por el `Protocolo de Programación Declarativa de Asistentes de IA (ADP)`, que estructura el código fuente del asistente.
* **Capa Especializada (Formularios):** Se rige por el `Estándar para la Digitalización Estructurada de Formularios (SFD)`, para la gestión de estructuras de datos y formularios.

### **1.4. Principio de Coherencia Categórica**

Los componentes de un asistente se gobiernan por relaciones estructurales lógicas y predecibles. Los flujos de trabajo se conciben como funtores, las transiciones entre estados como morfismos, y los propios estados como objetos. Toda composición de estos elementos debe respetar las leyes matemáticas de identidad y asociatividad.

*Nota Didáctica:* Este principio, derivado de la teoría de categorías, asegura que la "arquitectura" lógica del asistente sea coherente, componible y robusta, previniendo la existencia de estados inalcanzables o flujos de trabajo defectuosos.

### **1.5. Distinción Estratégica: Agente como Producto vs. Agente como Motor**

Una decisión de diseño preliminar y fundamental es definir la naturaleza del despliegue del asistente:

* **Agente como Producto:** Un asistente autocontenido que opera dentro de una plataforma existente (ej. Custom GPTs de OpenAI, Gems de Google). La plataforma proporciona la interfaz de usuario, la gestión de usuarios y las herramientas.
* **Agente como Motor:** Un asistente sin interfaz gráfica (*headless*) diseñado para ser integrado en aplicaciones externas a través de una API (ej. Assistants API de OpenAI, Gemini API de Google). Requiere la construcción de una aplicación a medida para su consumo.

Esta elección condiciona la totalidad del ciclo de vida, las herramientas a utilizar y la estrategia de despliegue.

## **2. Ciclo de Vida del Agente – 5 Fases**

El desarrollo y la gestión de un asistente de IA se articulan a través de un ciclo de vida estructurado en cinco fases secuenciales, diseñadas para garantizar un proceso ordenado, desde la idea inicial hasta el mantenimiento a largo plazo.

### **2.1. Fase 1: Concepción, Estrategia y Definición de Plataforma**

* **Objetivo:** Definir el propósito fundamental ("qué" y "por qué") y el entorno tecnológico ("dónde") en el que operará el asistente.

* **Actividades:**
  * **1.1 - Análisis y Selección de la Plataforma de Despliegue:**
    * **Procedimiento:** Realizar un inventario de las plataformas de destino disponibles y determinar el tipo de artefacto a construir (Producto vs. Motor).
    * **Procedimiento:** Analizar las implicaciones estratégicas asociadas a las características únicas de cada plataforma.
    * **Procedimiento:** Documentar de manera exhaustiva las restricciones y capacidades de la plataforma seleccionada, identificando límites técnicos (ej. longitud máxima de instrucciones, capacidad de carga de archivos) que impactarán directamente en la arquitectura del asistente.
    * **Procedimiento:** Identificar el modelo de gestión de conocimiento de la plataforma (ej. nativo de Git, basado en interfaz de usuario) como una restricción arquitectónica crítica.
    * **Resultado:** Elaboración de un "Informe de Capacidades de la Plataforma de Destino".
  * **1.2 - Elaboración del Acta de Constitución del Asistente:**
    * **Procedimiento:** Utilizar un marco de trabajo estructurado para definir los requerimientos de alto nivel del asistente.
    * **Resultado:** Creación del archivo de configuración `agent.yaml`, iniciando con la directiva de ejecución obligatoria y un borrador de las secciones de identidad (`core`) y seguridad (`guard`). Para las plataformas que requieran Ejecución Indirecta, se debe redactar también la instrucción "cargador" (*bootloader*).
  * **1.3 - Definición de la Estrategia de Adaptación del Modelo:**
    * **Procedimiento:** Evaluar la relación costo-beneficio entre utilizar un modelo de lenguaje de propósito general a través de RAG y la necesidad de desarrollar un modelo afinado (*fine-tuned*) para tareas específicas.
    * **Procedimiento:** Documentar los requerimientos de datos, costos asociados y las expectativas de rendimiento para cada opción.
    * **Resultado:** Un "Informe de Estrategia de Modelo" formal.

* **Punto de Control (Gate P1-GUARD):** En esta fase, es obligatoria la verificación automatizada de que el "Conjunto Mínimo de Salvaguardas" (`Minimum Guard Set`), definido en el `Protocolo de Programación Declarativa de Asistentes de IA`, esté presente y correctamente configurado en el archivo `agent.yaml`. No se podrá avanzar a la siguiente fase sin este control de seguridad fundamental.

### **2.2. Fase 2: Curación e Implementación de la Base de Conocimiento (KB)**

* **Objetivo:** Construir una base de datos y documentos optimizada para la plataforma de destino, que servirá como la fuente de verdad para el asistente.

* **Fundamento:** La capacidad de conocimiento de las plataformas modernas se basa en la técnica de Recuperación Aumentada de Información (RAG). El rendimiento de esta técnica es directamente proporcional a la calidad de los documentos fuente; por ello, la claridad, estructura y concisión son críticas.

* **Actividades:**
  * **2.1 - Transcripción y Refactorización del Conocimiento:**
    * **Procedimiento:** Aplicar la metodología `STS` para refactorizar todo el conocimiento textual existente en artefactos estandarizados (`.md`).
    * **Procedimiento:** Aplicar la metodología `SFD` para transcribir todo el conocimiento basado en formularios a artefactos estandarizados (`.md`).
  * **2.2 - Estrategia de Empaquetado y Consolidación del KB:**
    * **Procedimiento:** Diseñar la estructura de archivos `.md` basándose en las restricciones de la plataforma (número máximo de archivos, límites de tamaño, etc.).
    * **Procedimiento:** Para gestionar los límites en la cantidad de archivos, utilizar la directiva `EMBEDDED_BLOCK` de `STS` para consolidar múltiples artefactos en un único archivo.
    * **Procedimiento:** Para plataformas que utilicen el modelo de Ejecución Indirecta, el archivo `agent.yaml` debe ser incluido como parte del paquete de artefactos de conocimiento.
    * **Procedimiento:** Definir un Protocolo de Sincronización del Conocimiento en caso de que el repositorio de la plataforma no sea directamente el repositorio Git (ej. carga manual a una interfaz web). En este modelo, el KB de la plataforma se trata como un destino de despliegue, no como la fuente de verdad.
    * **Condición:** Si los requerimientos de conocimiento exceden las capacidades RAG de la plataforma, se debe activar un protocolo para acceder a una base de conocimiento externa mediante Acciones. Esta necesidad debe ser identificada y resuelta en esta fase.
  * **Resultado:** Un directorio `KB/` con artefactos validados en formato `STS` y `SFD`, y un Protocolo de Sincronización de Conocimiento definido.

### **2.3. Fase 3: Programación Declarativa del Asistente (ADP)**

* **Objetivo:** Escribir el "código fuente" del asistente de una manera que sea compatible con la plataforma y cumpla con los principios de diseño.

* **Fundamento:** La programación efectiva de asistentes se basa en principios avanzados de ingeniería de instrucciones: claridad extrema, uso de ejemplos (*few-shot*), estructuración del texto con etiquetas y la asignación de un rol y objetivo explícitos.

* **Actividades:**
  * **3.1 - Traducción del Diseño a Código:**
    * **Procedimiento:** Verificar que el archivo `agent.yaml` comience con la "Directiva de Ejecución del Agente" (`AGENT RUNTIME DIRECTIVE`), completa y sin modificaciones, según lo especificado en el `Protocolo de Programación Declarativa de Asistentes de IA`.
    * **Procedimiento:** Mapear sistemáticamente los conceptos de diseño de la Fase 1 a las claves y estructuras específicas del archivo `agent.yaml`.
  * **3.2 - Implementación de Lógica, Patrones y Reglas:**
    * **Procedimiento:** Definir los comportamientos complejos utilizando los módulos `logic.workflows`, `logic.states` y `cognitive_models`. Asegurar que las `actions` definidas sean compatibles con la plataforma de destino.
    * **Procedimiento:** Utilizar herramientas automáticas (*linters*) y revisiones de código para detectar y prevenir anti-patrones conocidos, como la exposición de lógica de negocio en la interfaz pública.
    * **Procedimiento:** Implementar los patrones arquitectónicos formales definidos en la metodología, como el "Patrón de Guía de KB" y la "Encapsulación Monádica de Procesos".
  * **3.3 - Implementación del Enrutamiento de Conocimiento:**
    * **Procedimiento:** Implementar el "Patrón de Guía de KB", mandatado por el Principio Arquitectónico 1.2.3. Esto se logra creando un modelo cognitivo dedicado (`CM-KB-GUIDANCE`) que actúa como un mapa de enrutamiento explícito entre el dominio de una consulta y el archivo fuente que contiene la respuesta.
    * **Justificación:** Esta técnica transforma la recuperación de conocimiento de una inferencia implícita y poco fiable en un paso de razonamiento explícito, auditable y de alta fidelidad.
  * **Resultado:** Un archivo `agent.yaml` completo y sintácticamente válido.

### **2.4. Fase 4: Pruebas, Despliegue y Refinamiento**

* **Objetivo:** Validar el comportamiento del asistente en un entorno controlado e implementar una observabilidad robusta para monitorear su funcionamiento.

* **Actividades:**
  * **4.1 - Diseño y Ejecución del Plan de Pruebas:**
    * **Componentes:** El plan debe incluir pruebas unitarias (para componentes individuales), pruebas de integración (para flujos de trabajo completos) y pruebas de regresión (para asegurar que los cambios no afecten funcionalidades existentes).
  * **4.2 - Implementación de la Estrategia de Observabilidad:**
    * **Procedimiento:** Definir métricas clave de rendimiento (KPIs) y una estrategia de registro de eventos (*logging*) que permita auditar y depurar el comportamiento del asistente en producción.
  * **4.3 - Ejecución del Ciclo de Refinamiento:**
    * **Procedimiento:** Depurar el comportamiento del asistente corrigiendo sistemáticamente el código (`agent.yaml`) y los datos (`KB/*.md`).
    * **Procedimiento:** Aplicar técnicas de depuración específicas para ingeniería de instrucciones, como la reformulación de directivas, la experimentación con el orden del contexto, la adición de ejemplos para casos de borde, o la instrucción explícita al modelo para que "piense paso a paso" y así poder auditar su cadena de razonamiento.
  * **4.5 - Despliegue:**
    * **Procedimiento:** Publicar el asistente en la plataforma de destino y versionar el estado final del código fuente utilizando Git.
    * **Procedimiento:** Para modelos de Ejecución Indirecta, el despliegue consta de dos pasos: 1) Pegar la instrucción "cargador" (*bootloader*) en el campo de instrucciones nativo de la plataforma. 2) Cargar el paquete de conocimiento completo, que incluye el archivo `agent.yaml`.
  * **Resultado:** Un asistente desplegado, estable y monitoreado.

* **Punto de Control (Gate 4.4 - Validación de Lista de Chequeo):** El sistema de integración y despliegue continuo (CI/CD) debe ejecutar de forma obligatoria la lista de validación `ADP-VALIDATION-CHECKLIST-02`. Esta lista incluye una verificación mandatoria de la presencia e integridad de la "Directiva de Ejecución del Agente". El despliegue será bloqueado si alguna de las verificaciones falla.

### **2.5. Fase 5: Mantenimiento y Evolución**

* **Objetivo:** Gestionar el asistente en producción, asegurando un rendimiento sostenido y planificando su evolución futura.

* **Actividades:**
  * **5.1 - Establecimiento del Control de Versiones:**
    * **Requisito:** Todos los repositorios de los asistentes deben seguir estrictamente el protocolo de gestión con Git detallado en la Sección 3 de esta guía.
  * **5.2 - Protocolo de Recolección y Análisis de Retroalimentación de Usuario:**
    * **Procedimiento:** Implementar mecanismos para recolectar retroalimentación, tanto explícita (encuestas) como implícita (análisis de logs), para identificar modos de falla y oportunidades de mejora.
  * **5.3 - Protocolo de Detección de Deriva y Monitoreo del Modelo:**
    * **Procedimiento:** Establecer métricas de base para detectar la degradación del rendimiento del modelo a lo largo del tiempo (*model drift*) o cambios en los patrones de consulta de los usuarios (*data drift*).
  * **5.4 - Auditoría de Mantenimiento Proactivo:**
    * **Requisito:** Ejecutar una auditoría trimestral recurrente contra la lista de validación `ADP-VALIDATION-CHECKLIST-02` y el "Conjunto Mínimo de Salvaguardas" para todos los agentes en producción, con el fin de prevenir la deriva en su configuración.
  * **5.5 - Protocolo de Gestión de Cambios:**
    * **Procedimiento:** Cualquier solicitud de cambio, ya sea correctiva o evolutiva, debe iniciar un nuevo ciclo ALM desde la fase que corresponda.

## **3. Control de Versiones y Gestión de Repositorios con Git**

* **Propósito:** Establecer una metodología estricta y estandarizada para gestionar el código fuente de los asistentes (`.adp.yaml`) y los artefactos de conocimiento (`KB/`) utilizando el sistema de control de versiones Git.

* **Fundamento:** El desarrollo de asistentes de IA debe ser tratado con la misma disciplina de ingeniería que el desarrollo de software tradicional. El control de versiones es un pilar fundamental de esta disciplina.

### **3.1. Estructura del Repositorio**

* **Requisito:** El sistema completo, incluyendo todos los asistentes y el conocimiento asociado, debe residir en un único mono-repositorio.

* **Fundamento:** Este enfoque centralizado asegura una única fuente de verdad para todos los artefactos de conocimiento, simplifica la gestión de dependencias entre asistentes y se alinea con el principio de "Centro de Conocimiento Centralizado, Dominios Federados".

* **Arquitectura de Directorios Canónica:**
  * `/agents/`: Contiene los archivos de definición de todos los asistentes de IA. Cada subdirectorio corresponde a un único asistente.
  * `/knowledge/`: Directorio raíz para todos los artefactos de conocimiento validados, curados y listos para ser utilizados por los asistentes.
  * `/sources/`: Repositorio para materiales fuente en bruto y sin procesar, que sirven de insumo para la creación de conocimiento.
  * `/staging/`: Un área de trabajo temporal para artefactos que están en proceso de transformación y curación.
  * `/tests/`: Contiene las pruebas automatizadas diseñadas para verificar la lógica de los asistentes y la integridad del conocimiento.

### **3.2. Estrategia de Ramificación (Branching)**

* **Propósito:** Proveer un modelo predecible para el desarrollo de nuevas funcionalidades, la corrección de errores y la publicación de nuevas versiones.
* **Modelo Adoptado:** Un modelo simplificado de GitFlow.

* **Componentes:**
  * **Rama `main`:** Representa el estado del asistente que está en producción y desplegado. Debe estar protegida contra escrituras directas. Solo se actualiza mediante la fusión de la rama `develop` para nuevas versiones.
  * **Rama `develop`:** Es la rama principal de integración para la próxima versión. Consolida una vista de todas las funcionalidades completadas y probadas.
  * **Ramas `feature/<nombre-funcionalidad>`:** Se utilizan para desarrollar nuevas funcionalidades o para añadir/actualizar artefactos de conocimiento de manera aislada. Se crean a partir de `develop` y se fusionan de vuelta a `develop` a través de una Solicitud de Integración (Pull Request).
  * **Ramas `hotfix/<nombre-incidencia>`:** Se utilizan para correcciones urgentes requeridas en la versión de producción (`main`). Se crean a partir de `main` y, una vez finalizadas, se fusionan tanto en `main` como en `develop` para asegurar la consistencia.

### **3.3. Convención para Mensajes de Commit**

* **Propósito:** Asegurar un historial de cambios claro, legible por máquinas y fácilmente trazable.
* **Requisito:** Todos los mensajes de commit deben adherirse a la especificación de "Commits Convencionales".
* **Modelo:** `tipo(alcance): descripción`
  * **Tipo:** Indica la naturaleza del cambio (`feat` para nuevas funcionalidades, `fix` para correcciones, `kb` para cambios en la base de conocimiento, `docs` para documentación, `refactor` para cambios que no alteran el comportamiento, `chore` para tareas de mantenimiento).
  * **Alcance (Opcional):** Especifica la parte del sistema afectada (ej. una ruta en el `agent.yaml` o el nombre de un archivo de conocimiento).
  * **Ejemplos:**
    * `feat(logic.states): agregar nuevo estado para validación de usuario`
    * `kb(kb_029_guia_circ33): actualizar circular 33 con nueva cláusula 2025`
    * `fix(core.identity): corregir error tipográfico en la definición del rol`

### **3.4. Estrategia de Etiquetado y Liberación de Versiones**

* **Requisito:** Cada fusión de código a la rama `main` constituye una nueva versión y debe ser marcada con una etiqueta (tag).
* **Requisito:** Las etiquetas deben seguir el estándar de Versionamiento Semántico (`MAYOR.MENOR.PARCHE`).

### **3.5. Ejemplo de Flujo de Trabajo Práctico**

* **Escenario:** "Añadir un nuevo formulario para la retroalimentación del usuario y un flujo de trabajo para procesarlo".

1. **Crear una nueva rama de funcionalidad:** A partir de la versión más reciente de `develop`, se crea una nueva rama llamada `feature/feedback-form-workflow`.
2. **Añadir el nuevo artefacto de conocimiento:** Se crea el archivo del formulario (`KB/forms/sfd_user_feedback.md`) y se confirma el cambio con un commit descriptivo: `kb(sfd_user_feedback): add user feedback form`.
3. **Actualizar la definición del asistente:** Se modifica el `agent.yaml` para añadir un nuevo flujo de trabajo que utilice el formulario recién creado. Se confirma el cambio con el commit: `feat(logic.workflows): add workflow for processing feedback form`.
4. **Publicar y solicitar revisión:** La rama de funcionalidad se sube al repositorio central y se abre una Solicitud de Integración (Pull Request) hacia la rama `develop`.
5. **Revisión de código y fusión:** El equipo revisa los cambios propuestos. Una vez aprobados, la Solicitud de Integración se fusiona en `develop`.
6. **Proceso de liberación:** En un momento posterior, como parte de un ciclo de liberación planificado, la rama `develop` (que ya contiene esta y otras funcionalidades) se fusiona en `main`. Se crea una nueva etiqueta de versión (ej. `v1.2.0`) y se publica.

## **4. Anexos**

### **Anexo A: Matriz de Capacidades de Plataformas (v1.2)**

* **Propósito:** Proveer una ficha técnica estandarizada para evaluar y seleccionar plataformas de despliegue de asistentes de IA.

La evaluación se basa en los siguientes criterios:

* **Límites de Conocimiento:**
  * `Max-Knowledge-Files`: Número máximo de archivos permitidos en la base de conocimiento RAG.
  * `Max-File-Size-MB`: Tamaño máximo por archivo individual.
  * `Max-Total-Size-MB`: Límite de tamaño combinado para todos los archivos.
* **Integración de Conocimiento Nativo:** Disponibilidad de conectores nativos con servicios externos para la recuperación dinámica de conocimiento (ej. Google Drive, Notion).
* **Capacidad de "Instrucción vía Archivo de Conocimiento":** Fiabilidad de la plataforma para seguir una instrucción "cargador" (*bootloader*) y tratar un archivo adjunto como su código fuente primario (Evaluación: Sí / No / Inestable).
* **Herramientas Nativas:**
  * `Web-Search`: Disponibilidad y tipo de navegación web integrada.
  * `Image-Generation`: Disponibilidad y modelo utilizado para la generación de imágenes.
  * `Data-Analysis`: Disponibilidad de un intérprete de código para tareas de análisis de datos.
* **Acciones Personalizadas:**
  * `OpenAPI-Support`: Versión del esquema OpenAPI soportada para definir acciones.
  * `Domain-Restrictions`: Capacidad para restringir las llamadas de acciones a dominios específicos.
* **Opciones de Modelo:**
  * `Model-Selection`: Capacidad del desarrollador para elegir el LLM subyacente.
  * `User-Facing-Model-Selection`: Capacidad del usuario final para cambiar el modelo.
* **Gobernanza y Seguridad:**
  * `Access-Control`: Mecanismos para compartir el asistente (público, solo con enlace, solo organización).
  * `Ownership-Transfer`: Protocolo para reasignar la propiedad de un asistente.
  * `API-Lifecycle`: Madurez de la API de orquestación (Beta, Disponibilidad General) y política de obsolescencia.
  * `Security`: Soporte para el "Conjunto Mínimo de Salvaguardas" (Sí / No).

### **Anexo B: Ejemplo de Asistente IPR (Actualizado)**

* **Propósito:** Este ejemplo canónico del asistente de Intervenciones Públicas Regionales (IPR) ha sido actualizado para incluir el "Conjunto Mínimo de Salvaguardas", ocultar toda la lógica de negocio privada, y servir como una demostración práctica del principio de Coherencia Categórica.
* **Recurso:** El archivo `agent.yaml` completo se proporciona como referencia canónica.

*(Nota: El bloque de código YAML del `agent.yaml` se mantiene en su formato original, ya que es un artefacto técnico).*

### **Anexo C: Mapa de Sincronización entre Teoría (ADP) y Práctica (ALM)**

* **Propósito:** Este anexo define el mapeo explícito que conecta los conceptos teóricos del `Protocolo de Programación Declarativa de Asistentes de IA` (ADP) con las actividades prácticas de este Marco Metodológico (ALM). Es el artefacto central que garantiza la coherencia y la gobernanza del proceso.

La siguiente tabla describe esta correspondencia:

| Objeto Teórico (ADP) | Mapeo en la Práctica (ALM) | Notas de Preservación Estructural |
| :--- | :--- | :--- |
| `Patrón: Encapsulación Monádica de Procesos` | `Principio 1.2.1 – Interfaz Pública/Privada` | Encapsula el razonamiento, ocultando la implementación. |
| `Patrón: Guía de KB (Functorial)` | `Actividad 3.3` + `Control 4.4` | Preserva la estructura explícita consulta↦documento. |
| `Anti-Patrón: Exposición de Lógica` | `Procedimiento 3.2.2` (detectado por linter) | Previene la violación del encapsulamiento. |
| `Lista de Validación ADP-VALIDATION-CHECKLIST-02` | `Control 4.4` y `Actividad 5.4` | Asegura la conformidad continua con los principios. |
| `Conjunto Mínimo de Salvaguardas` | `Control P1-GUARD` | Asegura la configuración de seguridad base. |

* **Reglas de Composición (Morfismos Permitidos):**
  * La aplicación conjunta del `Patrón de Guía de KB` y la `Encapsulación Monádica` es una composición válida y recomendada.
  * La `Exposición de Lógica` es una composición inválida, bloqueada por las herramientas de validación.

### **Anexo D: Glosario Conceptual para Desarrolladores**

* **Propósito:** Un micro-tutorial conceptual para aclarar los fundamentos teóricos en un lenguaje accesible.
* **Functor:** Un "traductor" que preserva la estructura. El Anexo C es la definición de este traductor entre el lenguaje de la teoría (ADP) y el de la práctica (ALM).
* **Objeto/Morfismo:** Un objeto es un "lugar" (un estado, un patrón). Un morfismo es un "camino" (una transición, una regla de composición). La teoría se enfoca en los caminos y cómo se conectan de forma fiable.
* **Mónada:** Una forma robusta de "empaquetar" una computación. En este contexto, se utiliza para empaquetar la lógica de negocio privada dentro de los `cognitive_models`, de modo que desde el exterior solo se observe la acción, no los detalles internos.

### **Anexo E: Catálogo de Patrones de Diseño**

* **Propósito:** Proveer una referencia canónica de patrones arquitectónicos y de implementación para construir asistentes de alta calidad.

**Parte 1: Patrones de Arquitectura de Agentes**

* `Patrón 1: Traducción de FTCF a ADP/YAML`: Muestra cómo convertir un análisis de alto nivel (`Función, Tarea, Contexto, Formato`) en la configuración `core`, `io` y `guard` del `agent.yaml`.
* `Patrón 2: Agente Validador de Entradas`: Utiliza un documento `SFD` como fuente de conocimiento para guiar a un usuario en el llenado de un formulario, validando cada campo.
* `Patrón 3: Agente de Flujo de Trabajo en Cadena de Valor`: Modela un proceso de negocio como una cadena de valor, transformando una entrada de bajo valor (una idea) en una salida de alto valor (una propuesta técnica validada). Cada estado representa una etapa de producción.
* `Patrón 4: Patrón de Encapsulación Estado-Cognición`: Conecta un estado público (`logic.states`) con un modelo cognitivo privado (`cognitive_models`) para ocultar la lógica de negocio.

**Parte 2: Patrones de Interacción y Razonamiento**

* `Patrón 6: Conductor de Interacción Multi-hilo`: Gestiona conversaciones complejas y no lineales, permitiendo al usuario cambiar entre múltiples temas sin que el asistente pierda el contexto.
* `Patrón 7: Patrón de Guía de KB`: Implementa el Principio Arquitectónico 1.2.3, transformando la recuperación de conocimiento implícita en un paso de razonamiento explícito y auditable para prevenir que el asistente consulte el documento equivocado.
* `Patrón 8: Patrón de Invocación de Cadena de Pensamiento (CoT)`: Mejora el razonamiento en tareas complejas forzando al modelo a articular su proceso de pensamiento paso a paso, usualmente dentro de etiquetas estructurales como `<thinking>`.
* `Patrón 9: Patrón de Comportamiento de Agente Autónomo`: Cambia al modelo de un rol pasivo de "chatbot" a un rol proactivo de "agente", inyectando instrucciones persistentes que incentivan el uso de herramientas, la planificación y la consecución de objetivos.
