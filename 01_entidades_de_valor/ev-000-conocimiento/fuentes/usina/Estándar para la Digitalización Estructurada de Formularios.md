# Estándar para la Digitalización Estructurada de Formularios

## **0. Metacomentario: Cómo Interpretar este Documento**

* **Propósito:** Definir las dos perspectivas desde las cuales se debe interpretar esta guía para su correcta aplicación.

* **Perspectiva de Autoría (Para Humanos):** Dirigida a los desarrolladores y arquitectos de conocimiento encargados de transcribir formularios físicos o digitales al formato SFD. Esta perspectiva se centra en las reglas prescriptivas para la creación del contenido.

* **Perspectiva de Interpretación (Para Máquinas):** Dirigida a los Asistentes de IA y LLMs que deben leer, interpretar y razonar sobre el contenido SFD. Un asistente debe primero identificar un bloque de contenido SFD dentro de un documento anfitrión y solo entonces aplicar las reglas de interpretación específicas de SFD aquí descritas.

## **1. Rol y Relación con la Norma Institucional de Conocimiento**

* **Propósito:** Definir la posición de este estándar en relación con la `Norma para la Elaboración de Artefactos de Conocimiento Institucional`.

* **SFD como una Extensión:** SFD no es un estándar de documento independiente, sino un formato de contenido especializado diseñado para operar *dentro* de un artefacto de conocimiento. Por requisito, todo contenido SFD debe estar encapsulado dentro de un `EMBEDDED_BLOCK` en un documento anfitrión que siga dicha norma.

* **Jerarquía de Interpretación:** Un intérprete compatible con la norma de conocimiento primero identifica la existencia de un bloque SFD. A continuación, un intérprete especializado en SFD procesa el contenido de dicho bloque. Las palabras clave y estructuras definidas en esta guía SFD solo son válidas dentro de ese contexto encapsulado.

## **2. Filosofía y Propósito**

* **Misión:** Gobernar la transcripción de formularios y documentos rígidamente estructurados en artefactos de conocimiento de alta fidelidad, diseñados para ser procesados por LLMs para tareas de análisis, completado automático, guía al usuario y validación.

* **Concepto Clave: Fidelidad Funcional:** El principio rector es la preservación completa y sin pérdidas de la estructura original de un formulario, incluyendo sus metadatos, reglas de validación y lógica condicional. Una transcripción SFD no es un resumen; es una re-arquitectura funcional del formulario a un formato estructurado y legible por máquinas.

## **3. Modelo de Uso de SFD: Artefacto Embebido**

* **Propósito:** Definir el único contexto obligatorio en el que puede existir un artefacto SFD.

* **Modelo Exclusivamente Embebido:** El contenido SFD siempre debe ser un componente dentro de un documento STS más amplio que le proporciona el contexto narrativo o estructural. Este es el único caso de uso válido. El bloque SFD no contiene sus propios metadatos o instrucciones, ya que los hereda del documento STS padre.

## **4. Principios Fundamentales**

Los principios de SFD están alineados y heredados directamente de los definidos en la `Norma para la Elaboración de Artefactos de Conocimiento Institucional` para garantizar la consistencia.

* **Principio 1 – Fidelidad Absoluta:** Se debe transcribir cada regla, restricción, opción e instrucción del formulario original. Omitir o abstraer detalles funcionales corrompe la utilidad del artefacto.
* **Principio 2 – Fuente de Verdad Autocontenida:** Cada característica de un elemento del formulario debe ser definida explícitamente utilizando los términos del léxico oficial de SFD para garantizar una interpretación inequívoca por parte de las máquinas.
* **Principio 3 – La Estructura es Significado:** La jerarquía del formulario (secciones, campos, subgrupos) es información fundamental ("meat") y debe ser representada mediante el uso de encabezados Markdown y etiquetas de `ID:` únicas.
* **Principio 4 – Cero Grasa y Máxima Densidad:** Se deben eliminar radicalmente las palabras de relleno, convirtiendo todo el significado funcional en términos del léxico SFD.
* **Principio 5 – Optimización para RAG:** Cada sección del formulario debe ser un bloque de información denso y tan autocontenido como sea posible para optimizar su recuperación por parte de los sistemas de IA.
* **Principio 6 – Invariancia del Lenguaje:** SFD preserva el idioma original del contenido del formulario. Se prohíbe la traducción de etiquetas, instrucciones u opciones.

## **5. Componentes Arquitectónicos**

Un artefacto SFD es una jerarquía de los siguientes componentes:

* **Sección de Formulario (`Form-Section`):** Una agrupación lógica de campos, representada por un encabezado de nivel 3 (`###`).
* **Campo de Formulario (`Form-Field`):** La unidad atómica de información. Representa una única entrada, etiqueta o elemento interactivo. Se define como un bloque de pares `Clave: Valor` bajo un encabezado de nivel 4 (`####`).

### **5.1. El Componente `Form-Field` y el Léxico SFD**

* **Propósito:** Describir exhaustivamente un único elemento de formulario utilizando un léxico controlado y obligatorio.

| Término Clave | Obligatorio | Definición y Uso |
| :--- | :--- | :--- |
| `ID:` | Sí | Identificador único para una sección o campo. |
| `Field-Label:` | Sí | El texto de la etiqueta visible asociada al campo. |
| `Field-Type:` | Sí | El tipo de dato o control (ej. `Text`, `Date`, `Select`). Debe usar el vocabulario controlado. |
| `Field-Instr:` | No | Instrucciones específicas para el usuario sobre cómo completar el campo. |
| `Field-Constraint:`| No | Reglas de validación (ej. obligatorio, longitud máxima, formato). Utiliza un mini-lenguaje. |
| `Field-Placeholder:`| No | Texto de ejemplo que aparece dentro de un campo vacío. |
| `Field-Option:` | Condicional | Una opción disponible por línea. Requerido para campos de tipo `Radio`, `Select`, etc. |
| `Field-Logic:` | No | Lógica condicional que define la visibilidad o requerimientos basados en otros campos. |
| `Field-Group:` | No | Un sub-encabezado para agrupar múltiples `Field-Option`. |

### **5.2. Vocabulario Controlado para `Field-Type`**

Se deben utilizar únicamente los siguientes valores para la clave `Field-Type:`:

* `Text`, `TextArea`, `Number`, `Date`, `Checkbox`, `Checkbox-Group`, `Radio`, `Select`, `File`, `Static-Text`, `Repeater`.

### **5.3. Mini-Lenguaje para `Field-Constraint`**

Las restricciones se definen como una lista de reglas separadas por puntos.

* **Ejemplo:** `Field-Constraint: "Req: mandatory. Max-Len: 50."`
* **Reglas comunes:** `Req: mandatory`/`optional`, `Max-Len: <num>`, `Min-Len: <num>`, `Max-Val: <num>`, `Min-Val: <num>`, `Format: <tipo>`, `Pattern: <regex>`.

## **6. Metodología de Aplicación (Para Autores)**

El proceso de transcripción de un formulario a SFD sigue un ciclo iterativo de 5 fases:

1. **Fase 1: Deconstrucción:** Analizar el formulario original, inventariando todas sus secciones, campos y reglas.
2. **Fase 2: Transcripción:** Convertir cada elemento del formulario en un bloque `Form-Field` utilizando el léxico SFD.
3. **Fase 3: Ensamblaje:** Agrupar los bloques `Form-Field` bajo los encabezados `Form-Section` correspondientes, asegurando `ID`s únicos.
4. **Fase 4: Conexión:** Codificar las dependencias entre campos utilizando la directiva `Field-Logic:`.
5. **Fase 5: Auditoría de Cumplimiento:** Utilizar la lista de chequeo de conformidad del estándar STS para validar el artefacto.

## **7. Cumplimiento**

La validación de un artefacto SFD se realiza utilizando la lista de chequeo de cumplimiento definida en la `Norma para la Elaboración de Artefactos de Conocimiento Institucional`.

## **8. Ejemplo de Aplicación**

* **Advertencia:** El siguiente contenido es estrictamente ilustrativo.
* **Contexto:** Este ejemplo muestra un formulario SFD embebido dentro de un documento STS más amplio, lo cual representa el único caso de uso correcto.

```plain
 Documento de Análisis de Proyecto
ID: PLAN-PROJ-ANALYSIS-01
Version: 1.0.0
...

## Sección 3: Evaluación de Riesgos
ID: PLAN-PROJ-ANALYSIS-S3-RISK-01
Purp: Documentar la evaluación inicial de riesgos para el proyecto.
Fnd: Un riesgo clave está relacionado con el cumplimiento legal, que debe ser declarado formalmente.

BEGIN_EMBEDDED_BLOCK:: SFD RISK-DECLARATION-FORM-01

## Declaración de Cumplimiento Legal
ID: FORM-RISKDEC-S1-LEGAL-01

### Requiere Revisión Legal
ID: FORM-RISKDEC-S1-LEGALREV-01
Field-Label: "¿Requiere Revisión Legal?"
Field-Type: Checkbox
Field-Constraint: "Req: mandatory."

### Justificación para la Revisión Legal
ID: FORM-RISKDEC-S1-JUSTIFY-01
Field-Label: "Justificación para la Revisión Legal"
Field-Type: TextArea
Field-Logic: "Cond: (Ref: FORM-RISKDEC-S1-LEGALREV-01.Value == 'true') -> Req: mandatory."
Field-Constraint: "Req: optional."

END_EMBEDDED_BLOCK:: RISK-DECLARATION-FORM-01

## Sección 4: Próximos Pasos
ID: PLAN-PROJ-ANALYSIS-S4-NEXT-01
Act: Enviar la declaración para revisión formal.
Dep: Completitud del formulario en RISK-DECLARATION-FORM-01.
```
