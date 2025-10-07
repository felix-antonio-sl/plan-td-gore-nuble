# Anexo C: Marco de IA Responsable

ID: PTD-ANEXO-C-IA-RESPONSABLE-01
Version: 1.0.0
Status: Published
Parent-Document: plan_td_gore_nuble_2026-2028.md
Creation-Date: 2025-10-06
Ref-STS-Guide: GUIDE-STS-MASTER-01

---

## C.1. Política de Uso Responsable de Inteligencia Artificial del GORE Ñuble

ID: PTD-IA-POLITICA-01

### Preámbulo

El Gobierno Regional de Ñuble reconoce el potencial transformador de la Inteligencia Artificial (IA) para mejorar la eficiencia de la gestión pública, la calidad de los servicios ciudadanos y la toma de decisiones basada en evidencia. Al mismo tiempo, reconoce los riesgos asociados al uso de estas tecnologías: sesgos algorítmicos, vulneración de derechos fundamentales, opacidad en las decisiones y erosión de la confianza ciudadana.

Esta Política establece los principios, roles, procesos y controles para asegurar que todo uso de IA en el GORE se realice de manera **responsable, ética, transparente, auditable y centrada en el bienestar de las personas**.

Fnd:

- Recomendaciones del Consejo para la Transparencia sobre Transparencia Algorítmica (2024).
- Proyecto de Ley que regula los sistemas de inteligencia artificial (Boletín N° 16.821-19, en tramitación).
- Ley N° 21.719 sobre Protección de Datos Personales.
- Política Nacional de Inteligencia Artificial de Chile.
- Guía de Formulación Ética de Proyectos de Ciencias de Datos (Gobierno Digital & UAI, 2022).

### Artículo 1: Ámbito de Aplicación

Esta Política se aplica a todo sistema, aplicación o herramienta que utilice técnicas de Inteligencia Artificial (incluyendo, pero no limitado a: aprendizaje automático, procesamiento de lenguaje natural, visión por computadora, sistemas de recomendación, modelos generativos) desarrollada, adquirida u operada por el Gobierno Regional de Ñuble o por terceros en su nombre, que sea utilizada para:

a) Apoyar, asistir o reemplazar la toma de decisiones administrativas que produzcan efectos jurídicos o afecten significativamente a personas (Sistemas de Decisión Automatizada - SDA).
b) Procesar datos personales de ciudadanos, funcionarios o beneficiarios de programas del GORE.
c) Proveer servicios o información a la ciudadanía en nombre del GORE.
d) Analizar datos institucionales para la generación de inteligencia de negocio o evaluación de políticas públicas.

### Artículo 2: Principios Rectores

Todo uso de IA en el GORE se regirá por los siguientes principios no negociables:

**Principio 1: Centralidad de la Persona Humana**

- Def: La IA es una herramienta al servicio de las personas, no un fin en sí misma.
- Req: Todo sistema de IA debe mejorar el bienestar humano, facilitar el ejercicio de derechos o aumentar la eficiencia en la provisión de servicios públicos.
- Prohib: Usos de IA que vulneren la dignidad humana o derechos fundamentales.

**Principio 2: Supervisión y Control Humano**

- Def: La decisión final siempre debe recaer en una persona humana, especialmente en decisiones que afectan derechos.
- Req: Todo SDA de Alto Riesgo debe contar con un mecanismo de supervisión humana efectiva (Humano-en-el-Bucle o Humano-sobre-el-Bucle).
- Req: Toda decisión automatizada debe ser revisable y apelable por una persona.

**Principio 3: Transparencia y Explicabilidad**

- Def: El funcionamiento de los sistemas de IA debe ser comprensible y comunicable.
- Req: Todo SDA que afecte derechos o acceso a servicios debe contar con una Ficha de Transparencia (Ficha SDA) pública.
- Req: Los ciudadanos afectados por una decisión de IA deben poder obtener una explicación en lenguaje claro de los factores que influyeron en esa decisión.

**Principio 4: Equidad y No Discriminación**

- Def: Los sistemas de IA no deben perpetuar ni amplificar sesgos o discriminaciones.
- Req: Todo sistema de IA debe ser evaluado para detectar sesgos antes de su despliegue.
- Req: Especial cuidado con sistemas que afectan a grupos vulnerables (personas en situación de pobreza, adultos mayores, pueblos originarios, personas con discapacidad).

**Principio 5: Privacidad y Protección de Datos**

- Def: El diseño y operación de sistemas de IA debe respetar el derecho a la privacidad.
- Req: Cumplimiento estricto de la Ley N° 21.719 (principios de finalidad, proporcionalidad, seguridad).
- Req: Minimización de datos: solo se recolectarán y procesarán datos estrictamente necesarios.
- Req: Anonimización o seudonimización cuando sea técnicamente posible y no afecte la finalidad.

**Principio 6: Seguridad y Robustez**

- Def: Los sistemas de IA deben ser seguros, resilientes y confiables.
- Req: Cumplimiento de la Norma Técnica de Seguridad (DS N°7).
- Req: Evaluación de vulnerabilidades específicas de IA (ataques adversariales, envenenamiento de datos, fugas de información).

**Principio 7: Rendición de Cuentas (Accountability)**

- Def: Siempre debe existir una persona o entidad responsable del funcionamiento y las consecuencias de un sistema de IA.
- Req: Todo sistema de IA debe tener un Responsable del Sistema designado formalmente.
- Req: Trazabilidad completa: logs de decisiones, versiones de modelos, datos de entrenamiento utilizados.

**Principio 8: Beneficio Social y Sostenibilidad**

- Def: La adopción de IA debe generar un retorno social neto positivo.
- Req: Evaluación ex-ante de impactos sociales (no solo económicos).
- Req: Consideración de impacto ambiental (eficiencia energética de modelos de IA).

### Artículo 3: Clasificación de Riesgo de Sistemas de IA

Fnd: Enfoque basado en riesgo del proyecto de Ley de IA chilena, inspirado en AI Act de la UE.

El Subcomité de IA clasificará todo sistema de IA según su nivel de riesgo, lo cual determinará los controles y obligaciones aplicables:

**Nivel 1: Riesgo Inaceptable (Prohibido)**

- Def: Usos de IA incompatibles con el respeto a derechos fundamentales.
- Prohib: Están absolutamente prohibidos en el GORE.
- Ejemplos (según proyecto de Ley de IA):
  - Manipulación subliminal que cause daño.
  - Categorización masiva basada en datos sensibles que resulte en discriminación.
  - "Social scoring" (calificación social generalizada).
  - Identificación biométrica remota en tiempo real sin orden judicial.

**Nivel 2: Alto Riesgo**

- Def: Sistemas cuyo uso presenta un riesgo significativo de afectar derechos fundamentales o acceso a servicios/beneficios esenciales.
- Req: Controles estrictos, supervisión humana obligatoria, auditoría externa.
- Ejemplos en contexto GORE:
  - Sistema de IA que prioriza automáticamente postulantes a subsidios o beneficios sociales.
  - Sistema de IA que apoya decisión de aprobación/rechazo de proyectos de inversión.
  - Sistema de IA para detección de fraude en rendiciones de cuentas (si genera decisiones automáticas de rechazo).
  - Analítica de video con identificación de personas (si se implementara en futuro).

**Nivel 3: Riesgo Limitado**

- Def: Sistemas con riesgos de manipulación o engaño, pero no de afectación significativa de derechos.
- Req: Obligaciones de transparencia (Ficha SDA), deber de informar al usuario que interactúa con IA.
- Ejemplos en contexto GORE:
  - Chatbots y asistentes conversacionales para consultas ciudadanas.
  - Asistentes de IA que ayudan a funcionarios a redactar documentos (copilotos jurídicos, de comunicaciones).
  - Sistemas de recomendación de contenido en aplicaciones.

**Nivel 4: Riesgo Bajo o Mínimo**

- Def: Sistemas de IA sin riesgos significativos para derechos o bienestar.
- Req: Controles mínimos, no requieren Ficha SDA (salvo decisión del Subcomité).
- Ejemplos:
  - IA para optimización interna de procesos (ej. enrutamiento de correos, clasificación de documentos para archivo).
  - Modelos predictivos para planificación de recursos (ej. estimación de demanda de servicios).

### Artículo 4: Obligaciones Diferenciadas por Nivel de Riesgo

| Obligación | Riesgo Inaceptable | Alto Riesgo | Riesgo Limitado | Riesgo Bajo |
|:---|:---:|:---:|:---:|:---:|
| **Prohibición de uso** | ✓ | ✗ | ✗ | ✗ |
| **Aprobación del Subcomité IA** | N/A | ✓ (obligatoria) | ✓ (obligatoria) | ✓ (recomendada) |
| **Ficha SDA pública** | N/A | ✓ | ✓ | ✗ (salvo decisión Subcomité) |
| **EIPD (Evaluación de Impacto en Protección de Datos)** | N/A | ✓ (si procesa datos personales) | Según DPO | ✗ |
| **Evaluación de Sesgos** | N/A | ✓ (obligatoria) | ✓ (recomendada) | ✗ |
| **Supervisión Humana (HITL/HOTL)** | N/A | ✓ (obligatoria) | ✗ | ✗ |
| **Auditoría Externa** | N/A | ✓ (anual) | ✗ | ✗ |
| **Logs y Trazabilidad** | N/A | ✓ (obligatoria, retención 3 años) | ✓ (retención 1 año) | Según diseño |
| **Explicabilidad de decisiones** | N/A | ✓ (obligatoria) | ✓ (recomendada) | ✗ |

### Artículo 5: Roles y Responsabilidades

**Responsable del Sistema de IA:**

- Def: Persona designada formalmente como responsable de un sistema de IA específico.
- Resp: Velar por el cumplimiento de esta Política, coordinar evaluaciones, mantener actualizada la Ficha SDA, gestionar incidentes.
- Req: Debe ser un funcionario del GORE con conocimiento del sistema y de la normativa.

**Subcomité de IA y Ética Digital:**

- Resp: Evaluar, aprobar y supervisar todos los sistemas de IA.
- Comp: Ver Anexo A, Artículos 5-8 de Resolución Constitutiva.

**Delegado de Protección de Datos (DPO):**

- Resp: Asegurar cumplimiento de Ley 21.719 en sistemas de IA que procesan datos personales.

**Oficial de Seguridad de la Información (CISO):**

- Resp: Evaluar y supervisar seguridad de sistemas de IA.

**Coordinador de Transformación Digital:**

- Resp: Presidir el Subcomité de IA, mantener el Catálogo de SDA, gestionar el Registro de Incidentes.

### Artículo 6: Prohibiciones Absolutas

Están absolutamente prohibidos en el Gobierno Regional de Ñuble los siguientes usos de IA:

a) Sistemas de IA para manipulación subliminal o explotación de vulnerabilidades que causen daño físico o psicológico.
b) Sistemas de categorización o "social scoring" de personas basados en datos sensibles que resulten en trato discriminatorio.
c) Sistemas de identificación biométrica en tiempo real en espacios públicos, salvo orden judicial específica para persecución penal.
d) Sistemas de evaluación de emociones en contextos sensibles (decisiones laborales, evaluación de postulantes a beneficios) sin consentimiento explícito y justificación fundada.
e) Sistemas de IA que procesen datos de niños, niñas y adolescentes sin autorización de padres/tutores y sin un análisis de impacto aprobado.

Warn: La violación de estas prohibiciones constituye una infracción grave y será causal de investigación administrativa y potencial responsabilidad funcionaria.

---

## C.2. Plantilla de Ficha SDA (Ficha de Transparencia de Sistemas de Decisión Automatizada)

ID: PTD-IA-FICHA-SDA-PLANTILLA-01

Fnd: Recomendaciones del Consejo para la Transparencia sobre Transparencia Algorítmica.

### Propósito de la Ficha SDA

La Ficha SDA es un documento público, conciso y en lenguaje claro que informa a la ciudadanía sobre la existencia, propósito, funcionamiento y gobernanza de un sistema de Inteligencia Artificial o decisión automatizada utilizado por el GORE.

Req: Toda sistema de IA de Riesgo Limitado o Alto Riesgo que afecte derechos o acceso a servicios debe tener una Ficha SDA aprobada por el Subcomité de IA y publicada en el sitio web de Transparencia Activa del GORE, sección "Transparencia Algorítmica".

### Plantilla de Ficha SDA

---

**FICHA DE TRANSPARENCIA DE SISTEMA DE DECISIÓN AUTOMATIZADA (SDA)**

**Gobierno Regional de Ñuble**
**Fecha de Publicación:** [DD/MM/AAAA]
**Versión de la Ficha:** [X.Y]

---

#### 1. Identificación del Sistema

**1.1. Nombre del SDA:**
[Nombre oficial del sistema o asistente de IA]

**1.2. Identificador Interno:**
[Código único, ej. SDA-GORE-001]

**1.3. Versión del SDA:**
[Versión del software/modelo, ej. v1.2.0]

**1.4. Fecha de Versión:**
[DD/MM/AAAA]

**1.5. Estado:**
☐ En Desarrollo (Piloto)
☐ En Producción
☐ Descontinuado

---

#### 2. Responsabilidad y Contacto

**2.1. División/Unidad Responsable:**
[Nombre de la división del GORE responsable del sistema]

**2.2. Responsable del Sistema:**
[Nombre y cargo del funcionario designado]

**2.3. Canal de Consultas o Reclamos:**
☐ Sí, existe un canal específico para este SDA.

- **Cómo acceder:** [Email, formulario web, teléfono]
☐ No, se aplican los canales generales del organismo (OIRS).

**2.4. Derecho de Oposición a Decisiones Automatizadas:**
☐ Sí, el ciudadano puede oponerse y solicitar revisión humana (conforme Art. 8 bis, Ley 21.719).
☐ No aplica (el sistema no toma decisiones sobre personas).

---

#### 3. Propiedad y Desarrollo

**3.1. Titularidad de Derechos:**
☐ Propiedad del GORE Ñuble / del Estado de Chile.
☐ Licenciado de tercero proveedor.

**3.2. Proveedor (si aplica):**

- **Nombre:** [Razón social]
- **RUT:** [RUT]
- **Contrato/Licitación:** [Código de Mercado Público o referencia]

---

#### 4. Objetivo y Propósito del SDA

**4.1. ¿Por qué existe este sistema? ¿Qué problema resuelve?**
[Descripción en lenguaje claro del propósito del sistema, dirigida a un ciudadano sin conocimientos técnicos. Máximo 200 palabras.]

Ejemplo:
"Este asistente fue creado para ayudar a las organizaciones comunitarias a postular de forma más simple al Concurso 8% FNDR. Responde preguntas frecuentes sobre requisitos, plazos y procedimientos, guía en el llenado de formularios y reduce los errores en las postulaciones."

**4.2. ¿A quién está dirigido? ¿Quién lo usa?**
[Descripción de los usuarios del sistema]

---

#### 5. Funcionamiento del Sistema

**5.1. ¿Cómo funciona? ¿Qué hace el sistema?**
[Descripción funcional en lenguaje claro, explicando el flujo de operación. Máximo 300 palabras.]

Ejemplo:
"El asistente utiliza inteligencia artificial para comprender las preguntas de los usuarios en lenguaje natural. Busca la respuesta en una base de conocimiento que contiene las bases del concurso, las preguntas frecuentes históricas y la normativa aplicable. Luego genera una respuesta en lenguaje simple. Si la pregunta es muy compleja o ambigua, deriva al usuario a un funcionario humano del GORE."

**5.2. ¿Apoya, asiste o reemplaza la toma de decisiones humanas?**
☐ Apoya (provee información para que una persona decida).
☐ Asiste (pre-filtra, recomienda, pero decisión final es humana).
☐ Reemplaza (toma la decisión automáticamente, sujeta a revisión humana posterior).

**5.3. ¿El sistema categoriza, clasifica o elabora perfiles de personas?**
☐ Sí.

- **Categorías o Perfiles:** [Listar, ej. "Postulante Apto / No Apto", "Riesgo Alto / Medio / Bajo"]
- **¿Por qué estas categorías son relevantes?** [Justificación]
- **¿Cómo se asignan las categorías?** [Metodología en lenguaje claro]
- **¿Qué variables o factores tienen mayor peso?** [Explicación]
☐ No.

**5.4. ¿Qué consecuencias puede tener para una persona el procesamiento de sus datos por este sistema?**
[Explicación de efectos, ej. "Recibir o no un subsidio", "Ser contactado por una institución de seguridad", "Acceder o no a un beneficio"]

**5.5. Si este sistema puede generar una decisión negativa (ej. rechazo de una solicitud), ¿qué factores influyen en esa decisión?**
[Explicación de criterios, ej. "No cumplir con requisito de antigüedad de organización", "Puntaje de evaluación técnica bajo"]

**5.6. Método o Modelo de IA Utilizado:**
[Descripción técnica de alto nivel, ej. "Modelo de lenguaje grande (LLM) con recuperación aumentada (RAG)", "Red neuronal convolucional para visión por computadora", "Árbol de decisión supervisado"]

---

#### 6. Datos Utilizados

**6.1. ¿El sistema utiliza datos personales?**
☐ Sí.
☐ No.

**6.2. ¿El sistema utiliza datos personales sensibles?**
☐ Sí. [Especificar tipos: salud, origen étnico, afiliación política, etc.]
☐ No.

**6.3. Categorías o clases de datos utilizados:**
[Listar, ej. "Nombre, RUT, comuna de residencia, edad, género, ingresos del hogar (RSH)"]

**6.4. ¿Se realizó una Evaluación de Impacto en la Protección de Datos Personales (EIPD)?**
☐ Sí. [Enlace al resumen público de la EIPD]
☐ No aplica (no procesa datos personales o es de bajo riesgo).

**6.5. Conjuntos de datos de entrenamiento, validación y prueba (si el sistema fue entrenado con datos):**
[Descripción de la fuente y naturaleza de los datos. Si son datos abiertos, enlace. Si son datos institucionales, descripción genérica respetando privacidad.]

Ejemplo:
"El asistente fue entrenado utilizando:

- Las bases oficiales del Concurso 8% FNDR (años 2022-2024).
- 500 preguntas frecuentes históricas de ciudadanos (anonimizadas).
- Normativa aplicable (Glosa 07 Ley de Presupuestos, Instructivo del GORE)."

**6.6. Política de Privacidad:**
[Enlace a la política de privacidad del GORE o sección específica del sistema]

---

#### 7. Medidas de Seguridad y Mitigación de Riesgos

**7.1. Principales riesgos identificados y cómo se mitigan:**
[Listar riesgos y controles, ej.:

- "Riesgo de sesgo en contra de organizaciones rurales → Mitigación: Evaluación de equidad en dataset de entrenamiento, inclusión balanceada de casos rurales y urbanos."
- "Riesgo de respuesta incorrecta → Mitigación: Validación humana de respuestas críticas, opción de derivación a funcionario."]

**7.2. ¿El sistema ha sido auditado?**
☐ Sí. [Fecha de última auditoría: DD/MM/AAAA, Entidad auditora: XXXX]
☐ No, aún no (sistema reciente, auditoría planificada para: [fecha]).

---

#### 8. Información Adicional

**8.1. Enlace a Información Complementaria:**
[URL del sitio web del GORE con documentación técnica adicional, manuales de usuario, etc.]

**8.2. Fecha de Próxima Revisión de la Ficha:**
[DD/MM/AAAA - Las fichas se revisan al menos anualmente]

---

**Fin de la Ficha SDA**

Documento público del Gobierno Regional de Ñuble, disponible en [URL].
Para consultas o reclamos: [email/formulario].

---

## C.3. Protocolo de Evaluación de Riesgos de IA

ID: PTD-IA-EVALUACION-RIESGOS-01

### Fase 1: Clasificación de Riesgo (Obligatoria para Todo Sistema de IA)

Resp: Responsable del Sistema + Subcomité de IA.

Mech: El Responsable del Sistema completa el siguiente cuestionario. El Subcomité de IA revisa y asigna la clasificación final.

**Cuestionario de Clasificación de Riesgo:**

**Pregunta 1: ¿El sistema toma o apoya decisiones que producen efectos jurídicos o afectan significativamente a personas?**

- Ejemplos: Aprobar/rechazar subsidios, priorizar acceso a servicios, determinar elegibilidad.
- ☐ Sí → Potencial Alto Riesgo, continúe a P2.
- ☐ No → Potencial Riesgo Limitado o Bajo, continúe a P5.

**Pregunta 2: ¿La decisión afecta derechos fundamentales o acceso a servicios esenciales (salud, educación, vivienda, seguridad social)?**

- ☐ Sí → **Alto Riesgo confirmado.**
- ☐ No → Continúe a P3.

**Pregunta 3: ¿La decisión es revisada y puede ser modificada por una persona humana antes de aplicarse?**

- ☐ Sí, siempre hay supervisión humana efectiva → Riesgo Limitado.
- ☐ No, o la supervisión es nominal → Alto Riesgo.

**Pregunta 4: ¿El sistema procesa datos personales sensibles (salud, origen étnico, afiliación política, datos biométricos)?**

- ☐ Sí, y las decisiones se basan significativamente en estos datos → Alto Riesgo.
- ☐ Sí, pero son datos auxiliares → Riesgo Limitado.
- ☐ No → Continúe a P5.

**Pregunta 5: ¿El sistema interactúa directamente con personas (chatbot, asistente conversacional, interfaz de usuario)?**

- ☐ Sí → Riesgo Limitado (obligación de informar que es IA).
- ☐ No, es proceso interno → Riesgo Bajo.

**Resultado:**

- Si alguna pregunta llevó a "Alto Riesgo": Clasificación Final = **Alto Riesgo**.
- Si solo se alcanzó "Riesgo Limitado": Clasificación Final = **Riesgo Limitado**.
- Si solo se alcanzó "Riesgo Bajo": Clasificación Final = **Riesgo Bajo**.

### Fase 2: Evaluación de Sesgos (Obligatoria para Alto Riesgo, Recomendada para Riesgo Limitado)

Resp: Responsable del Sistema + Experto en IA (interno o externo).

Obj: Detectar y mitigar sesgos que puedan resultar en discriminación o inequidad.

**Protocolo de Evaluación:**

1. **Análisis del Dataset de Entrenamiento:**
   - Act: Examinar la representatividad del dataset.
   - Preguntas:
     - ¿Están todos los grupos de interés representados proporcionalmente?
     - ¿Hay sub-representación de grupos vulnerables (rurales, adultos mayores, pueblos originarios)?
   - Métrica: Calcular distribución de clases/grupos, comparar con distribución poblacional de Ñuble.

2. **Análisis de Resultados Desagregados:**
   - Act: Evaluar el desempeño del modelo por subgrupos.
   - Métricas:
     - Tasa de falsos positivos/negativos por grupo (ej. por género, por comuna rural vs urbana).
     - Paridad estadística: ¿La tasa de decisiones positivas es similar entre grupos?
   - Herramienta: Usar biblioteca open-source (ej. Fairlearn, AI Fairness 360) o servicio de GobLab UAI.

3. **Prueba de Casos Extremos:**
   - Act: Generar casos sintéticos de personas de distintos perfiles y evaluar si el sistema produce resultados razonables y equitativos.

4. **Documentación:**
   - Res: Informe de Evaluación de Sesgos (5-10 páginas).
   - Contenido: Metodología, hallazgos, medidas de mitigación implementadas.
   - Dest: Se anexa a la Ficha SDA (puede ser versión simplificada para publicación).

### Fase 3: Diseño de Supervisión Humana (Obligatoria para Alto Riesgo)

Resp: Responsable del Sistema + División Patrocinante.

Obj: Asegurar que una persona humana capacitada puede intervenir, revisar y modificar decisiones de IA.

**Modalidades de Supervisión:**

**Humano-en-el-Bucle (Human-in-the-Loop, HITL):**

- Def: La decisión de IA es una recomendación. Una persona revisa y aprueba/rechaza antes de que se aplique.
- Uso: Sistemas de Alto Riesgo donde la decisión es crítica e irreversible.
- Ejemplo: Sistema de IA que pre-evalúa postulaciones a subsidios → Funcionario revisa top recomendados y rechazados antes de formalizar resultado.

**Humano-sobre-el-Bucle (Human-over-the-Loop, HOTL):**

- Def: El sistema toma la decisión automáticamente, pero una persona supervisa el proceso y puede intervenir ante anomalías. La decisión es auditable y reversible.
- Uso: Sistemas de Alto Riesgo donde el volumen es alto pero el riesgo individual es moderado.
- Ejemplo: Pre-auditor de rendiciones que rechaza documentos con errores → DAF revisa muestra aleatoria + todos los rechazos, puede corregir.

**Sin Supervisión Directa (Para Riesgo Limitado/Bajo):**

- Def: El sistema opera autónomamente, pero con logging completo y posibilidad de auditoría ex-post.
- Req: Debe existir un canal de reclamos para casos de error.

**Especificación de Supervisión:**

- Req: Definir quién supervisa (rol), con qué frecuencia, qué métricas monitorea.
- Req: Protocolo de escalamiento si el supervisor detecta patrón de errores.

---

## C.4. Catálogo de Asistentes y SDA Existentes

ID: PTD-IA-CATALOGO-ASISTENTES-01

### Propósito del Catálogo

Proveer un inventario completo y actualizado de todos los sistemas de IA y asistentes en operación o desarrollo en el GORE Ñuble, su clasificación de riesgo, estado de cumplimiento y responsables.

| ID | Nombre del Asistente/SDA | División Responsable | Responsable del Sistema | Propósito | Nivel de Riesgo | Estado Ficha SDA | Estado Operativo | Evidencia de Valor |
|:---|:---|:---|:---|:---|:---|:---|:---|:---|
| **SDA-001** | Formuevaluador (Formulación y Evaluación IPR) | DIPIR / Transversal | [Coordinador TD] | Guiar formuladores en selección de vía de financiamiento, elaboración de IPR y simulación de evaluación ex-ante | Limitado | ✓ Publicada (v1.1, 10/10/2025) | **Producción** | **1.500+ consultas en 8% FNDR 2024-2025** |
| **SDA-002** | Comunicon (Comunicaciones Institucionales) | Comunicaciones | [Jefa de Comunicaciones] | Asesor en estrategia comunicacional, redacción de comunicados, minutas y documentos oficiales | Bajo | ☐ No requiere | **Producción** | **Uso diario por Jefatura, adoptante comprometida** |
| **SDA-003** | Digitrans (Experto TDE y Cumplimiento) | ODIA / Transversal | [Coordinador TD] | Experto en Ley 21.180, 6 Normas Técnicas, Estrategia GD 2030, motor de cumplimiento normativo | Bajo | ☐ No requiere | **Producción** | Motor de diseño de este Plan TD |
| **SDA-004** | Goreólogo (Experto Institucional GORE) | ODIA / Transversal | [Coordinador TD] | Consultor de conocimiento profundo sobre GORE (marco legal, gestión presupuestaria, ciclo IPR, contexto Ñuble) | Bajo | ☐ No requiere | **Producción** | Onboarding de funcionarios, consultas técnicas |
| **SDA-005** | Jano (Asesor Jurídico y Conformidad CGR) | Asesoría Jurídica / DAF | [Asesor Jurídico] | Copiloto jurídico: análisis de legalidad, co-producción de actos administrativos, simulación de auditoría CGR | Limitado | En elaboración | **Piloto Interno** | Uso en co-producción de convenios |
| **SDA-006** | Chat GORE Ciudadano (Atención 24/7) | Comunicaciones | [Coordinador TD] | Responder consultas ciudadanas generales sobre GORE | Limitado | ✓ Publicada (v1.0, 15/10/2025) | Beta Pública | En testeo, capacidad multicanal |
| **SDA-007** | Pre-Auditor de Rendiciones (A desarrollar) | DAF | [Jefe DAF] | Validar documentos de respaldo de rendiciones vs Res. 30 CGR | Alto | En elaboración | Diseño (H2) | Planificado para Q2-2026 |
| **SDA-008** | Analista Predictivo de Cartera (A desarrollar) | DIPIR | [Jefe DIPIR] | Predecir retrasos en proyectos basado en patrones históricos | Bajo | ☐ No requiere | Diseño (H2) | Planificado para Q3-2026 |
| **SDA-009** | Copiloto de Fomento en Mi Ñuble (A desarrollar) | DIFOI / Comunicaciones | [Jefe DIFOI] | Guiar emprendedores y organizaciones a fondos regionales | Limitado | En elaboración | Diseño (H2-H3) | Planificado para Q4-2026 |

**Nota:** Los asistentes SDA-001 a SDA-006 (exceptuando SDA-007 y posteriores) son **activos ya existentes y en operación o piloto**, no propuestas futuras. Este es un diferenciador crítico del GORE Ñuble: **parte con una flota operativa de IA, no con promesas.**

Req: El Coordinador TD es responsable de mantener este catálogo actualizado y publicarlo mensualmente en el Observatorio Ñuble 360.

---

## C.5. Protocolo de Gestión de Incidentes de IA

ID: PTD-IA-PROTOCOLO-INCIDENTES-01

### Definición de Incidente de IA

Def: Un incidente de IA es cualquier evento donde un sistema de IA:

- Genera un resultado incorrecto, sesgado o discriminatorio.
- Falla técnicamente de forma que afecta la operación o la experiencia de usuario.
- Es utilizado de manera indebida por un funcionario o ciudadano.
- Experimenta una brecha de seguridad o fuga de datos.
- Genera una consecuencia no prevista que afecta negativamente a personas.

### Canal de Reporte

Mech: Cualquier persona (funcionario, ciudadano, stakeholder) puede reportar un incidente de IA mediante:

- Formulario web en el sitio de Transparencia del GORE (sección "Reporte de Incidentes de IA").
- Email a: <incidentes-ia@gorenuble.cl> (atendido por Coordinador TD).
- Presencialmente en OIRS del GORE.

Req: El reporte debe incluir:

- Identificación del sistema (nombre o ID del SDA).
- Descripción del incidente.
- Fecha y hora.
- Evidencia (capturas de pantalla, transcripción de conversación, etc.).
- Impacto percibido.

### Proceso de Gestión

**Paso 1: Recepción y Triage (24 horas)**

- Resp: Coordinador TD.
- Act: Registrar el incidente en el Registro Centralizado.
- Act: Clasificar severidad:
  - **Crítica:** Afecta derechos fundamentales o seguridad de datos de múltiples personas. Impacto inmediato.
  - **Alta:** Afecta a una persona o genera error sistemático en decisiones.
  - **Media:** Error aislado sin afectación de derechos, pero afecta experiencia de usuario.
  - **Baja:** Sugerencia de mejora, no un error propiamente tal.

**Paso 2: Escalamiento según Severidad**

- **Crítica:** Notificación inmediata al Subcomité de IA, CISO, DPO, Administradora Regional.
  - Decisión: Suspensión precautoria del sistema hasta investigación.
- **Alta:** Notificación al Subcomité de IA (sesión extraordinaria en 48 hrs).
- **Media/Baja:** Asignación al Responsable del Sistema para investigación y respuesta.

**Paso 3: Investigación y Resolución (Plazos según severidad)**

- Crítica: Resolución en 72 horas.
- Alta: Resolución en 7 días.
- Media: Resolución en 15 días.
- Baja: Resolución en 30 días.

Proc: El Responsable del Sistema investiga causa raíz, implementa corrección (re-entrenamiento de modelo, ajuste de prompt, corrección de bug) y documenta en Registro.

**Paso 4: Comunicación y Cierre**

- Act: Notificar al reportante sobre resultado de investigación y acciones tomadas.
- Act: Si el incidente reveló un problema sistémico, actualizar Ficha SDA y comunicar a usuarios afectados.
- Act: Si hubo afectación de derechos, escalar a DPO para gestionar según Ley 21.719.

**Paso 5: Aprendizaje**

- Act: Presentar incidentes significativos en siguiente sesión del Subcomité de IA.
- Obj: Identificar patrones, proponer mejoras a políticas y protocolos.

### Registro Centralizado de Incidentes

Resp: Coordinador TD mantiene registro en plataforma del GORE (puede ser módulo de NEXO GORE).

Cpt: Información registrada por incidente:

- ID único de incidente.
- Fecha de reporte.
- Sistema afectado.
- Descripción.
- Severidad.
- Responsable asignado.
- Acciones tomadas.
- Fecha de cierre.
- Estado (abierto, en investigación, resuelto, cerrado).

Req: Reporte trimestral de incidentes se presenta en CVC como indicador de salud de la cartera de IA.

---

## C.6. Checklist de Pre-Despliegue para Sistemas de IA

ID: PTD-IA-CHECKLIST-PREDESPLIEGUE-01

Req: Todo sistema de IA debe superar este checklist antes de pasar a producción. Es parte del Gate G3 (IA Responsable).

| Criterio | Alto Riesgo | Riesgo Limitado | Riesgo Bajo | Verificación |
|:---|:---:|:---:|:---:|:---|
| **1. Clasificación de riesgo asignada por Subcomité IA** | ✓ | ✓ | ✓ | Acta del Subcomité |
| **2. Ficha SDA elaborada y aprobada** | ✓ | ✓ | ✗ | Ficha publicada en web |
| **3. Evaluación de sesgos realizada** | ✓ | Recomendado | ✗ | Informe de Evaluación |
| **4. EIPD aprobada por DPO (si procesa datos personales)** | ✓ | Según DPO | ✗ | Documento EIPD firmado |
| **5. Mecanismo de supervisión humana diseñado e implementado** | ✓ (HITL o HOTL) | ✗ | ✗ | Documentación del mecanismo |
| **6. Logs y trazabilidad de decisiones habilitados** | ✓ (retención 3 años) | ✓ (retención 1 año) | Recomendado | Configuración de logging |
| **7. Plan de explicabilidad (cómo se justificarán decisiones)** | ✓ | Recomendado | ✗ | Documento de diseño |
| **8. Canal de reclamos identificado y operativo** | ✓ | ✓ | ✗ | URL/email verificado |
| **9. Evaluación de seguridad aprobada por CISO** | ✓ | ✓ | ✓ | Informe de seguridad |
| **10. Documentación técnica completa (arquitectura, modelo, datos)** | ✓ | Recomendado | Recomendado | Repositorio de documentación |
| **11. Pruebas de aceptación de usuario (UAT) superadas** | ✓ | ✓ | Recomendado | Informe de UAT |
| **12. Plan de monitoreo post-despliegue definido** | ✓ | ✓ | ✗ | Plan de monitoreo |

Proc: El Responsable del Sistema completa el checklist y adjunta evidencia de cada criterio. El Subcomité de IA verifica y aprueba (o rechaza con observaciones).

---

## C.7. Directrices para Comunicación del Uso de IA a Ciudadanos

ID: PTD-IA-COMUNICACION-CIUDADANA-01

Fnd: Art. 11, Proyecto de Ley de IA (deber de informar que se interactúa con IA); Oficio Circular N°711 (uso de IA en interacción ciudadana).

Req: Todo sistema de IA de Riesgo Limitado que interactúe directamente con ciudadanos debe informar claramente que el usuario está conversando o siendo atendido por un sistema de IA.

### Buenas Prácticas de Comunicación

**1. Identificación Clara y Temprana:**

- El sistema debe identificarse como IA en el primer mensaje o en un lugar visible de la interfaz.
- Ejemplo (Chatbot):
  - ✓ Correcto: "Hola, soy el Asistente Virtual del GORE Ñuble, un sistema de inteligencia artificial. Estoy aquí para ayudarte a postular al Concurso 8% FNDR. ¿En qué puedo asistirte?"
  - ✗ Incorrecto: "Hola, soy Asistente GORE Ñuble, ¿en qué puedo ayudarte?" (no informa que es IA).

**2. Transparencia sobre Capacidades y Limitaciones:**

- Informar qué puede y qué no puede hacer el sistema.
- Ejemplo: "Puedo responder preguntas sobre requisitos, plazos y procedimientos del concurso. Para consultas sobre el estado de tu postulación específica, te derivaré a un funcionario."

**3. Opción de Atención Humana:**

- Ofrecer siempre la posibilidad de ser derivado a una persona humana.
- Ejemplo: "Si prefieres hablar con una persona, escribe 'derivar' o llama al [teléfono]."

**4. Lenguaje Claro y Empático:**

- Usar lenguaje simple (Guía de Voz y Tono, kb_tde_073_voz_tono_sts.md).
- Evitar tecnicismos.
- Tono: servicial, respetuoso, institucional pero cercano.

**5. Gestión de Expectativas:**

- No prometer lo que el sistema no puede cumplir.
- Si el sistema no entiende una pregunta, reconocerlo honestamente y ofrecer alternativas.

---

## C.8. Protocolo de Auditoría Externa de IA

ID: PTD-IA-AUDITORIA-EXTERNA-01

Req: Los sistemas de IA de Alto Riesgo deben someterse a una auditoría externa anual, realizada por una entidad independiente (universidad, consultora especializada, organismo de certificación).

### Alcance de la Auditoría

La auditoría externa evaluará:

1. **Cumplimiento de esta Política de IA Responsable.**
2. **Calidad y Representatividad de Datos:** Revisión de datasets de entrenamiento.
3. **Evaluación de Sesgos:** Validación independiente de equidad y no-discriminación.
4. **Robustez y Seguridad:** Pruebas de adversarial attacks, análisis de vulnerabilidades.
5. **Transparencia:** Verificación de completitud y exactitud de Fichas SDA.
6. **Supervisión Humana:** Evaluación de efectividad de mecanismos HITL/HOTL.
7. **Trazabilidad:** Revisión de logs, capacidad de auditar decisiones históricas.

### Proceso

**Paso 1: Selección de Auditor (Mes previo a auditoría):**

- Resp: CTD selecciona y contrata auditor externo mediante proceso de Ley 19.886.
- Req: El auditor debe ser independiente (sin conflictos de interés) y con experiencia demostrable en IA ética.

**Paso 2: Ejecución de Auditoría (1-2 meses):**

- El auditor tiene acceso completo a documentación, código fuente (si aplica), datasets, logs (con resguardo de datos sensibles).
- El Responsable del Sistema y el Subcomité de IA colaboran, proveyendo información y respondiendo consultas.

**Paso 3: Informe de Auditoría:**

- El auditor emite Informe con hallazgos, nivel de cumplimiento y recomendaciones.
- Informe se presenta al Subcomité de IA y al CTD.

**Paso 4: Plan de Acción Correctivo:**

- Si la auditoría identifica incumplimientos o riesgos:
  - Resp: El Responsable del Sistema elabora Plan de Acción Correctivo con plazos.
  - Act: El Subcomité de IA supervisa implementación de correcciones.
  - Cond: Si los hallazgos son críticos, el sistema puede ser suspendido hasta corregir.

**Paso 5: Publicación:**

- Req: Un resumen ejecutivo del Informe de Auditoría (sin información técnica sensible) se publica en el sitio de Transparencia Activa.

---

**Fin del Anexo C**

Este anexo ha establecido el marco completo de IA Responsable para el GORE Ñuble: la Política que rige todo uso de IA, la plantilla de Ficha SDA para transparencia, los protocolos de evaluación de riesgos y sesgos, el catálogo de sistemas existentes, la gestión de incidentes y el proceso de auditoría externa.

Ref: Los aspectos de gestión de datos específicos (políticas, catálogo, metadatos) se detallan en el Anexo E. La estrategia de comunicación ciudadana sobre IA se detalla en el Anexo F.
