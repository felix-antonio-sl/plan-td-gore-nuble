# **Guía Institucional Maestra: Estilo Telegráfico Estructurado (STS)**

## **0. Metacomentario: Cómo Interpretar este Documento**

* **Propósito:** Definir las distintas capas informativas de esta guía para asegurar su correcta interpretación y aplicación.

Esta guía se debe leer considerando las siguientes capas:

1. **Capa 1 - Definición del Estándar STS:** Corresponde a la especificación formal y normativa del estándar.
2. **Capa 2 - Auto-aplicación del Estándar:** Esta guía está escrita utilizando el mismo estándar STS que define, sirviendo como un ejemplo práctico de su aplicación.
3. **Capa 3 - Componentes Definidos:** Las secciones 1 y 2 de este documento definen los componentes que son obligatorios para que cualquier artefacto de conocimiento sea considerado compatible con el estándar STS.
4. **Capa 4 - Ejemplos Ilustrativos:** La sección 9 contiene contenido de ejemplo únicamente para fines de demostración y no debe considerarse parte de la norma.

## **1. Bloque de Metadatos de Control (Componente Obligatorio)**

* **Propósito:** Establecer un encabezado técnico obligatorio para cada documento STS que permita la gestión de versiones, autoría y fuentes.
* **Requisito:** Este bloque debe ser la primera sección de contenido en todo artefacto STS.

| Término Clave | Obligatorio | Definición |
| :--- | :--- | :--- |
| `Version:` | Sí | Versión del documento usando Versionamiento Semántico (MAYOR.MENOR.PARCHE). |
| `Status:` | Sí | Estado del ciclo de vida del documento (`Draft`, `Review`, `Published`, `Obsolete`). |
| `Human-Creator:` | Sí | Nombre o iniciales del autor humano de la primera versión. |
| `Model-Collaborator:`| Sí | Nombre del modelo de IA que colaboró en la última modificación. |
| `Creation-Date:` | Sí | Fecha de creación en formato `YYYY-MM-DD`. |
| `Modification-Date:`| Sí | Fecha de la última modificación en formato `YYYY-MM-DD`. |
| `Source:` | No | URI, ID de documento o descripción de la fuente original del artefacto. |

## **2. Instrucciones de Interpretación para LLM (Componente Obligatorio)**

* **Requisito:** Este bloque es obligatorio y debe seguir inmediatamente al Bloque de Metadatos. Su función es proporcionar un conjunto de reglas inmutables para que un Modelo de Lenguaje Grande (LLM) que "consume" (lee y razona sobre) el artefacto lo haga con perfecta fidelidad. Se prohíbe el uso de estas instrucciones para los LLM que participan en la *creación* o *traducción* de artefactos.

*(Nota: La siguiente sección es una explicación del contenido de las instrucciones para LLMs, adaptada para la comprensión humana).*

El bloque de instrucciones para LLMs contiene las siguientes directivas fundamentales:

1. **Objetivo Central:** Mantener una fidelidad absoluta a la información (`meat`) y a la estructura (`skeleton`) del documento, prohibiendo resúmenes, interpretaciones o inferencias.
2. **Metáforas Conceptuales:**
    * `meat` (carne): La información esencial, datos y hechos, que debe ser preservada sin ninguna pérdida.
    * `skeleton` (esqueleto): La estructura lógica (encabezados, IDs, listas), que también se considera `meat`.
    * `fat` (grasa): La verbosidad no esencial (palabras de relleno, prosa estilística), que debe ser ignorada.
3. **Léxico y Expansión:** Define el vocabulario de palabras clave que el LLM debe reconocer y expandir para su correcto razonamiento (ej. `Purp:` se expande a `Purpose:`).
4. **Política de Referencias (`Ref:`):** Las referencias se usan exclusivamente para hipervínculos *internos* a un `ID:` dentro del mismo documento. No deben interpretarse como enlaces a recursos externos.
5. **Política de Invariancia del Lenguaje:** Las palabras clave del protocolo están en inglés. Sin embargo, todo el contenido o "dato esencial" asociado a esas claves debe ser preservado en su idioma original, sin traducción.

## **3. Filosofía y Propósito**

* **Misión:** Gobernar el ciclo de vida de los artefactos de conocimiento para asegurar la máxima fidelidad, consistencia y densidad informacional.
* **Destinatario:** El estándar está diseñado para el procesamiento por parte de Modelos de Lenguaje Grandes (LLMs) y Asistentes de IA.
* **Propósito:** Facilitar que los modelos de IA razonen con la máxima precisión y cero ambigüedad, utilizando únicamente la información contenida dentro del propio artefacto.
* **Fundamento:** STS es un estándar fundacional para crear unidades de conocimiento portátiles y de alta fidelidad, sirviendo como un componente clave en estrategias más amplias de coherencia de datos.

## **4. Nomenclatura Oficial**

* **Nombre Completo:** Structured Telegraphic Style (Estilo Telegráfico Estructurado).
* **Acrónimo:** STS.
* **Naturaleza:** Es un estándar de **formato**, no de idioma. Se aplica a un documento manteniendo su idioma original; no es una herramienta para la traducción entre idiomas.

## **5. Principios Fundamentales**

1. **Fidelidad Absoluta:** La creación de un artefacto STS es una refactorización del formato, no un resumen del contenido. Todos los puntos de datos originales deben ser preservados. El resumen es un error crítico.
2. **Fuente de Verdad Autocontenida:** Un concepto o dato se define una sola vez con un `ID:` único dentro del artefacto. Se utilizan referencias internas (`Ref:`) para apuntar a esa única fuente, prohibiendo la repetición.
3. **La Estructura es Significado:** La jerarquía (encabezados), los identificadores, las referencias, las tablas y las listas son información esencial (`meat`), no meros elementos de estilo. Se prohíbe el uso de Markdown estilístico como negritas o cursivas; el énfasis debe ser explícito a través de palabras clave (`Warn:`, `Req:`).
4. **Cero Grasa y Máxima Densidad:** Se busca la máxima densidad de `meat` por token, eliminando radicalmente las palabras de relleno y traduciendo los matices del lenguaje humano a palabras clave explícitas.
5. **Optimización para RAG:** Cada sección de un documento (un "chunk") debe ser informativamente densa y tan autocontenida como sea posible para maximizar la "señal" de información en los sistemas de recuperación de IA.
6. **Invariancia del Lenguaje:** El lenguaje de control (el léxico de palabras clave) es un vocabulario fijo en inglés. El lenguaje de contenido (los datos esenciales) debe permanecer siempre en el idioma original del documento fuente.

## **6. Componentes del Estilo**

### **6.1. Microestructura: La Línea Telegráfica**

Es la unidad atómica de información y sigue el modelo `PalabraClave: DatoEsencial`.

* **PalabraClave (`Keyword`):** Un término del léxico oficial que define la naturaleza del dato (ej. `Obj:`, `Req:`).
* **DatoEsencial (`EssentialData`):** La información pura, despojada de verbosidad, pero sin omisiones.

### **6.2. Macroestructura: La Red de Conocimiento**

Busca hacer que el conocimiento sea navegable y contextual dentro del propio artefacto mediante tres elementos clave:

* Jerarquía de Encabezados (`#`, `##`, etc.).
* Identificadores Únicos (`ID:`).
* Referencias Cruzadas Internas (`Ref:`).

### **6.3. Estructuras Compuestas: Tablas y Listas**

Las estructuras que agrupan datos, como tablas y listas, deben mantener su formato original, ya que la relación inherente entre sus datos es parte del `meat`.

### **6.4. Bloques Embebidos**

Se define un mecanismo formal para incluir contenido que no es STS dentro de un documento STS, utilizando las directivas `BEGIN_EMBEDDED_BLOCK` y `END_EMBEDDED_BLOCK`. Esto permite que un documento STS actúe como un "contenedor" de alto nivel para otros formatos.

El caso de uso principal de este mecanismo es la inclusión de formularios, cuyo formato y contenido están rigurosamente definidos por el `Estándar para la Digitalización Estructurada de Formularios`.

### **6.5. Estándar de Identificadores Únicos (ID)**

Se define un formato obligatorio para todos los `ID:` (`GRUPO-SUBGRUPO-CONCEPTO-ID`) para asegurar la trazabilidad interna y la coherencia.

## **7. Metodología de Aplicación**

El proceso de creación de un artefacto STS sigue un ciclo iterativo de 4 fases:

1. **Fase 1: Arquitectura:** Crear el esqueleto lógico óptimo para el conocimiento, diseñando la jerarquía de secciones y asignando `ID`s únicos a cada nodo.
2. **Fase 2: Población de `Meat`:** Transferir toda la información esencial desde la fuente original al nuevo esqueleto, destilando el texto a formato telegráfico sin omitir datos.
3. **Fase 3: Sistema Nervioso:** Transformar el esqueleto estático en una red de conocimiento dinámica, conectando los nodos (`ID:`) con referencias internas (`Ref:`).
4. **Fase 4: Auditoría de Cumplimiento:** Utilizar una lista de chequeo formal para verificar que el artefacto cumple con todos los principios del estándar.

## **8. Gobernanza del Léxico**

El uso del léxico de palabras clave canónicas es obligatorio para evitar ambigüedades.

* **Reglas de Gobernanza:**
  * El léxico definido en esta guía es la única fuente de verdad.
  * Se prohíbe la creación unilateral de nuevos términos.
  * Las abreviaturas solo son válidas si se declaran en el bloque de instrucciones para LLMs.
  * El léxico (palabras clave) es un vocabulario de control en inglés; el contenido (`DatoEsencial`) permanece en el idioma original del documento.

* **Léxico Consolidado:** Se provee una tabla con todas las palabras clave canónicas, sus abreviaturas y notas de uso. El principio es que la especificidad debe residir en el `DatoEsencial`, no en la `PalabraClave`.

* **Anti-Patrón Crítico: Palabras Clave Secuenciadas:** Se prohíbe sufijar palabras clave con números o letras (ej. `Req-1:`, `Act-A:`). Esto rompe el estándar. El orden debe ser manejado por la estructura (listas), no modificando la palabra clave.

## **9. Ejemplos de Aplicación (Contenido Ilustrativo)**

* **Advertencia:** El siguiente contenido es estrictamente ilustrativo y no forma parte de la definición formal del estándar STS. Su único propósito es demostrar la aplicación práctica de los principios y reglas descritos en esta guía.

### **9.1. Ejemplo de Transcripción**

Este ejemplo muestra cómo un párrafo de texto en lenguaje natural se transforma en un artefacto STS conciso y estructurado.

* **Texto Humano (Fuente):**
    > "Para nuestra nueva estrategia de marketing de contenidos, que se detalla en el documento del plan general de marketing, proponemos la creación de una serie de tutoriales en vídeo. Creemos que esto es esencial porque nuestra última encuesta reveló que el 75% de los usuarios prefiere este formato. Sin embargo, no debemos olvidar que esto dependerá del presupuesto de marketing que se apruebe."

* **Transcripción a formato STS:**

    ```markdown
    ### Estrategia de Contenidos
    ID: GUIDE-STS-EXAMPLE-MKT-01
    Ctx: Basado en el plan general de marketing.
    
    - Purp: Crear una serie de tutoriales en video.
    - Just: Encuesta revela que el 75% de los usuarios prefiere el formato de video.
    - Dep: Presupuesto de marketing aprobado.
    ```

### **9.2. Ejemplo de Artefacto Completo**

Este ejemplo ilustra cómo se ve un documento STS completo y autocontenido, incluyendo el bloque de metadatos y las instrucciones para el LLM.

```markdown
 Artefacto: Requisitos del Módulo de Registro (Logging)
ID: REQ-LOG-MOD-01
Version: 1.0.0
Status: Draft
Human-Creator: Equipo-A
Model-Collaborator: Ninguno
Creation-Date: 2025-07-14
Modification-Date: 2025-07-14
Source: documento: AUDIT-SEC-2025-Q2

---
**BEGIN_LLM_INSTRUCTIONS**

Usted es un intérprete de artefactos en Estilo Telegráfico Estructurado (STS). Su tarea principal es interpretar ESTE documento con absoluta fidelidad según las reglas definidas a continuación. Este artefacto es autocontenido.
1. **Objetivo Central**: Mantener una fidelidad perfecta a la información (`meat`) y la estructura (`skeleton`). No resumir ni inferir.
2. **Modo de Léxico y Expansión**: Este documento utiliza un **Léxico Abreviado**. DEBE expandir las palabras clave según este mapeo:
    - `Purp:` -> `Purpose:`
    - `Fnd:` -> `Foundation:`
    - `Req:` -> `Requirement:`
    - `Cond:` -> `Condition:`
    - `Mech:` -> `Mechanism:`
3. **Política de Referencia (`Ref:`)**: `Ref:` es SÓLO para referencias cruzadas internas a un `ID:` dentro de este documento.
4. **Política de Invariancia del Lenguaje**: Preserve el idioma original de todos los `EssentialData`.

**END_LLM_INSTRUCTIONS**
---

## Requisitos Centrales
ID: REQ-LOG-MOD-CORE-01
Purp: Definir las características obligatorias para el módulo de registro del sistema.
Fnd: Basado en los hallazgos de la auditoría de seguridad.

- Req: Todas las entradas de registro deben estar estructuradas en formato JSON.
- Req: El nivel de registro (INFO, WARN, ERROR) debe ser un campo obligatorio.
- Cond: Los registros de nivel ERROR deben activar una alerta inmediata.
  - Mech: Enviar notificación al canal `canal-de-alertas`.
```

### **9.3. Ejemplo de Transcripción de Tabla**

Este ejemplo demuestra cómo se preserva la estructura de una tabla, traduciendo el contenido de cada celda al formato telegráfico para maximizar la densidad de la información.

* **Tabla en formato STS:**

| Característica | Opción A: Servidor Local | Opción B: SaaS en la Nube |
| :--- | :--- | :--- |
| **Costo Inicial** | Req: Alta inversión inicial. | Mdl: Suscripción. Ctx: Bajo costo inicial. |
| **Mantenimiento** | Resp: Equipo de TI interno. | Resp: Proveedor del servicio. |
| **Escalabilidad** | Mech: Compra de nuevo hardware. Proc: Lento, costoso. | Mech: Ajuste de la suscripción. Proc: Instantáneo. |
