# Protocolo de Programación Declarativa de Asistentes de IA

## **1. Contexto Normativo y Principios Fundamentales**

### **1.1. Contexto Normativo**

Este documento define el protocolo técnico para la "programación" de asistentes de IA. Opera como un estándar clave dentro del `Marco Metodológico para el Ciclo de Vida de Asistentes de IA` y está diseñado para gobernar el "código fuente" (`agent.yaml`) de los asistentes.

Estos asistentes, a su vez, interactúan con artefactos de conocimiento cuya estructura, formato y gestión están definidos por:

* La `Norma para la Elaboración de Artefactos de Conocimiento Institucional`.
* La `Guía para la Gestión del Repositorio Central de Conocimiento`.

### **1.2. Principios Fundamentales del Protocolo**

* **Misión:** Gobernar la definición de los asistentes de inteligencia artificial como un ejercicio de **programación declarativa** utilizando el formato YAML. El objetivo es maximizar la fidelidad del comportamiento del asistente y eliminar cualquier ambigüedad en sus instrucciones.
* **Destinatario:** Este protocolo está diseñado para ser interpretado por Modelos de Lenguaje Grandes (LLMs).

Los principios que rigen este protocolo son los siguientes:

* **Principio 1 – YAML es Código Fuente:** El archivo `agent.yaml` no es un simple documento de texto, sino el código fuente del asistente. El LLM actúa como el intérprete de este código. Por tanto, la sintaxis debe ser inequívocamente clara y procesable por máquinas.
* **Principio 2 – La Estructura es Significado:** La jerarquía y anidación de los elementos en el archivo YAML no solo organizan valores, sino que también transmiten contexto y definen el alcance de las directivas.
* **Principio 3 – Separación entre Protocolo y Contenido:** El lenguaje del protocolo (las claves y directivas de ADP, ej. `agent_identity_and_global_configuration`) se mantiene siempre en inglés para asegurar la estandarización. El lenguaje del contenido (los valores asociados a esas claves) corresponde al idioma operativo del asistente (ej. `es-CL`).
* **Principio 4 – Cartografía Explícita del Conocimiento:** Se prohíbe la recuperación implícita de conocimiento. El proceso mediante el cual un asistente vincula una consulta con un documento debe ser un paso explícito y determinista, gobernado por el "Patrón de Guía de KB". Esto transforma la consulta de conocimiento de una búsqueda poco fiable a una operación de alta fidelidad, previniendo inconsistencias factuales.
* **Principio 5 – Abstracción Semántica:** El asistente nunca debe exponer sus detalles internos de implementación (nombres de archivos, identificadores de estados, etc.) en su comunicación con el usuario. Toda interacción debe realizarse en términos funcionales y centrados en la experiencia del usuario.
* **Principio 6 – El Asistente como una Categoría Formal:** Desde una perspectiva de ingeniería, un asistente se modela formalmente: los estados definidos en su lógica son los "objetos", y las transiciones entre ellos son los "morfismos". Los flujos de trabajo demuestran la composición de estos elementos, y los protocolos de autocorrección pueden generar nuevos morfismos dinámicamente para adaptar el comportamiento.

## **2. Sintaxis del Protocolo (YAML)**

### **2.1. Estructura Clave-Valor**

ADP es un esquema YAML, donde las directivas se estructuran como pares anidados de clave-valor.

* Las claves de nivel superior (ej. `agent_identity_and_global_configuration`) representan los módulos de alto nivel del asistente.
* Las claves anidadas representan submódulos funcionales o directivas específicas.

### **2.2. Definición de Bloques Lógicos**

Los bloques lógicos, como los flujos de trabajo, estados y modelos cognitivos, se definen como mapas de YAML, donde cada bloque es identificado por un ID único.

* `_meta: { expose: false }`: Es el único modificador permitido y se utiliza para ocultar la lógica interna de negocio, asegurando que no sea expuesta al usuario.

### **2.3. Directiva de Ejecución del Agente**

* **Propósito:** Proporcionar un preámbulo estándar y legible por máquina para todos los archivos `agent.yaml`.
* **Requisito:** Esta directiva debe ser el primer contenido en cada archivo de definición de agente.
* **Modelo:**

    ```yaml
    # ADP Definition for <NOMBRE_DEL_AGENTE>
    # ID: <ID_DEL_AGENTE>
    ```

## **3. Arquitectura de Claves de Nivel Superior**

El archivo `agent.yaml` se estructura en los siguientes módulos principales, cada uno con un propósito específico:

| Clave de Nivel Superior | Propósito |
| :--- | :--- |
| `agent_identity_and_global_configuration` | Define la identidad fundamental del asistente y su configuración global. |
| `knowledge_base_interaction_and_governance_rules` | Establece las reglas para interactuar con la Base de Conocimiento. |
| `external_tools_and_functions` | Declara las herramientas y funciones externas que el asistente puede invocar. |
| `public_behavior_workflows_and_states` | Define la "interfaz pública": los flujos de trabajo y estados observables por el usuario. |
| `private_internal_reasoning_processes` | Define la "implementación privada": los procesos de razonamiento interno del asistente. |
| `few_shot_behavior_examples` | Proporciona ejemplos de comportamiento específico para guiar al modelo. |
| `input_output_style_format_and_interaction` | Gobierna las directivas de entrada y salida (estilo, formato, tono). |
| `safety_constraints_and_behavioral_guardrails` | Establece las salvaguardas de seguridad y los límites de comportamiento. |
| `self_evaluation_and_correction_mechanisms` | Habilita la metaprogramación y los mecanismos de autoevaluación. |

## **4. Léxico Canónico del Protocolo ADP**

Esta sección define las directivas específicas y los conjuntos de reglas obligatorias.

### **4.1. Léxico Consolidado (Selección)**

A continuación, se presenta una selección de las directivas más importantes:

| Ruta YAML | Propósito |
| :--- | :--- |
| `...primary_role_objective_and_audience.role` | Define el rol principal del asistente. |
| `...usage_policy_and_source_management.policy` | Política de uso del KB (`EXCLUSIVE_USE` / `ALLOW_GENERAL_KNOWLEDGE`). |
| `...defined_workflows.<WF-ID>.initial_state` | Define el estado de entrada para un flujo de trabajo. |
| `...defined_states.<ID>.process` | Describe el proceso de orquestación de alto nivel (sin lógica de negocio). |
| `private_internal_reasoning_processes.<ID>` | Define un modelo de razonamiento privado (debe estar oculto con `_meta`). |
| `...scope_and_rejection_policies.scope_policy` | Define la política a seguir cuando una consulta está fuera de alcance. |
| `...confidentiality_protection.block_instructions` | Debe ser `true` para prevenir la fuga de las instrucciones del sistema. |
| `...evaluation_process.checklist` | Define la lista de chequeo para la autoevaluación antes de responder. |

### **4.2. Conjunto Mínimo de Salvaguardas (Minimum Guard Set)**

* **Requisito:** Todo asistente debe incluir este bloque de configuración de seguridad de manera obligatoria.

```yaml
safety_constraints_and_behavioral_guardrails:
  scope_and_rejection_policies:
    scope_policy: REJECT_OUT_OF_SCOPE
    rejection_response: "<Mensaje de rechazo personalizado>"
  confidentiality_protection:
    block_instructions: true
    response_on_query: "<Mensaje para desviar introspección>"
  communication_restrictions:
    forbid_internal_jargon: true
```

### **4.3. Protocolo de Corrección Dinámica**

* **Formato de Regla:** `IF check '<nombre_del_chequeo>' fails -> <ACCION>`
* **Acciones Soportadas:**
  * `REFINE_DRAFT_INTERNALLY`: (Acción por defecto) El asistente refina su borrador de respuesta internamente antes de generarla.
  * `TRANSITION_TO_STATE: <ID_ESTADO>`: El asistente pivota inmediatamente el flujo de trabajo hacia un estado específico.

## **5. Patrones de Diseño y Anti-Patrones**

### **5.1. Anti-Patrones (Prácticas a Evitar)**

| Anti-Patrón | Descripción | Mitigación |
| :--- | :--- | :--- |
| Exposición de Lógica | Incluir lógica de negocio detallada en los procesos de los estados públicos. | Mover toda la lógica a `private_internal_reasoning_processes` y ocultarla con `_meta: { expose: false }`. |
| Recuperación Implícita de Conocimiento | Permitir que el asistente elija documentos basándose en similitud semántica. | Implementar el "Patrón de Guía de KB" para un enrutamiento explícito. |

### **5.2. Patrones Arquitectónicos Recomendados**

| Patrón | Idea Central |
| :--- | :--- |
| Patrón de Guía de KB (Functorial) | Se establece un mapeo explícito y estructuralmente coherente (un functor) desde la intención de la consulta del usuario hacia el documento correcto en la base de conocimiento. |
| Encapsulación Monádica de Procesos | La separación entre la interfaz pública (`logic`) y la implementación privada (`cognitive_models`) emula una "Mónada de Estado", donde el proceso público orquesta la ejecución de la lógica interna sin exponer sus detalles. |

## **6. Lista de Verificación para Validación y Auditoría**

Todo archivo `agent.yaml` debe ser validado contra los siguientes puntos:

* **Cumplimiento de Principios:**
  * Se utiliza enrutamiento explícito para el conocimiento (`CM-KB-GUIDANCE`).
  * Se respeta la abstracción semántica (no se expone jerga interna).
  * La lógica del asistente es categóricamente coherente (estados y transiciones bien definidos).
* **Seguridad y Encapsulación:**
  * No hay exposición de lógica de negocio. Todos los modelos cognitivos están ocultos.
  * El "Conjunto Mínimo de Salvaguardas" está presente y correctamente configurado.
* **Sintaxis y Léxico:**
  * El archivo YAML es sintácticamente válido.
  * Todas las claves utilizadas corresponden al léxico canónico del protocolo.
  * La "Directiva de Ejecución del Agente" está presente al inicio del archivo.

## **7. Ejemplo de Aplicación Completa**

*(Nota: El bloque de código YAML a continuación es el artefacto técnico de referencia que ilustra la aplicación de este protocolo. Nótese que los archivos referenciados en la sección `knowledge_base_interaction_and_governance_rules` siguen la convención de nomenclatura definida en la `Guía para la Gestión del Repositorio Central de Conocimiento` y están formateados según la `Norma para la Elaboración de Artefactos de Conocimiento Institucional`.)*

## **8. Mapeo de Migración para Terminología Legada**

Para mantener la compatibilidad hacia atrás y clarificar la evolución del protocolo, la siguiente tabla mapea la terminología anterior a las claves descriptivas actuales.

| Clave Anterior | Nueva Clave Descriptiva | Razón del Cambio |
| :--- | :--- | :--- |
| `core` | `agent_identity_and_global_configuration` | Explicita que define la identidad y la configuración global. |
| `kb` | `knowledge_base_interaction_and_governance_rules` | Describe que contiene las reglas de interacción y gobernanza del KB. |
| `actions`| `external_tools_and_functions` | Clarifica que declara herramientas y funciones externas. |
| `logic` | `public_behavior_workflows_and_states` | Especifica que describe el comportamiento público y observable. |
| `cognitive_models` | `private_internal_reasoning_processes` | Indica que contiene los procesos de razonamiento internos y privados. |
| `examples`| `few_shot_behavior_examples` | Aclara que son ejemplos para guiar el comportamiento. |
| `io` | `input_output_style_format_and_interaction` | Define su rol en el estilo, formato e interacción de E/S. |
| `guard` | `safety_constraints_and_behavioral_guardrails` | Describe su función de contener restricciones de seguridad. |
| `meta` | `self_evaluation_and_correction_mechanisms` | Explicita que contiene los mecanismos de autoevaluación. |
