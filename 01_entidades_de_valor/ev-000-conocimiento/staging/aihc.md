# Artefacto: El Diseño de IA Centrada en el Humano para el Lugar de Trabajo

ID: AIHC-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Model-Collaborator: Gemini-2.5-Pro
Creation-Date: 2025-10-03
Modification-Date: 2025-10-03
Source: aihc.md

---
**BEGIN_LLM_INSTRUCTIONS**

You are an AI agent consuming a Structured Telegraphic Style (STS) artifact. Your primary task is to parse and reason over THIS document with absolute fidelity, using only the rules defined below. This artifact is a self-contained source of truth.

1. **Core Objective**: Maintain perfect fidelity to the information (`meat`) and structure (`skeleton`). Do not summarize, interpret, or infer information not explicitly present. Prohib: Applying these rules to artifact creation or translation tasks; they are exclusively for consumption.
2. **Lexicon Mode & Expansion**: This document uses an **Abbreviated Lexicon**. You MUST treat the following keywords as valid and expand them according to this mapping before processing:
    - `Purp:` -> `Purpose:`
    - `Mech:` -> `Mechanism:`
    - `Cpt:` -> `Concept:`
    - `Def:` -> `Definition:`
    - `Ex:` -> `Example:`
    - `Req:` -> `Requirement:`
    - `Ctx:` -> `Context:`
    - `Fnd:` -> `Foundation:`
    - `Obj:` -> `Objective:`
    - `Ref:` -> `Reference:`
3. **Reference (`Ref:`) Policy**: `Ref:` is for **internal cross-references only**. It MUST point to an `ID:` that exists within THIS document.
4. **Language Invariance Policy**: The `Keywords` in the lexicon are a fixed control vocabulary in English. All `EssentialData` (the content following a `Keyword:`) MUST be preserved in its original language.

**END_LLM_INSTRUCTIONS**
---

## 1. Introducción

ID: AIHC-INTRO-01

### 1.1. El Espacio de Diseño de Soluciones de IA Centrada en el Humano

ID: AIHC-INTRO-DESIGNSPACE-01

- Cpt: Avance de tecnologías AI (LLMs, chatbots).
  - Res: Nueva era en soporte laboral y empresarial.
  - Mech: Generación de artefactos similares a los humanos (texto, imágenes, sonido, código).
- Cpt: Tecnologías habilitadoras.
  - Ex: Algoritmos de Machine Learning (ML), redes neuronales profundas.
  - Purp: Soportar funciones de misión crítica.
  - Ex: Reconocimiento de patrones, toma de decisiones, automatización.

- Purp: Introducir un mapa de soluciones de IA Centrada en el Humano (HCAI).
  - ID: AIHC-CPT-HCAIMAP-01
  - Obj: Navegar el paisaje tecnológico de soluciones HCAI.
  - Mech: Clasifica soluciones de IA según dos dimensiones. Ref: AIHC-CPT-HCAIDIMENSIONS-01.

- Cpt: Dimensiones del mapa HCAI.
  - ID: AIHC-CPT-HCAIDIMENSIONS-01
  - Cpt: Dimensión 1: Propósito HCAI.
    - Def: El rol de la solución de IA en relación con el usuario.
    - Ex: Asistir, aumentar, automatizar o reemplazar.
  - Cpt: Dimensión 2: Cognición HCAI.
    - Def: El tipo de función cognitiva soportada.
    - Ex: Percepción (sensing), toma de decisiones, ejecución de acciones.

- Cpt: Roles de las soluciones de IA en el mapa HCAI.
  - Ex: Asistentes, herramientas, agentes de orquestación, agentes de automatización.
  - Mech: Los roles varían en cómo soportan a los usuarios.
  - Mech: Reflejan diferentes niveles de implicación humana: in-the-loop, on-the-loop, out-of-the-loop.

- Cpt: Cualidades de diseño HCAI.
  - Purp: Fomentar una experiencia de usuario positiva y confianza.
  - Ex: Empatía, transparencia, explicabilidad.
- Cpt: Características de las soluciones HCAI.
  - Purp: Determinan la efectividad de la solución.
  - Ex: Conciencia del contexto, centralidad en el humano, control humano.

### 1.2. Propósito de la IA Centrada en el Humano (Human-Centered Al Purpose)

ID: AIHC-PURPOSE-01
Purp: Definir la relación entre el humano y el sistema de IA.

- Cpt: Asistentes de IA (AI assistants).
  - Def: Soportan directamente a los usuarios, típicamente con interfaces de lenguaje natural.
  - Act: Responden preguntas, dan recomendaciones, ejecutan acciones especificadas por el usuario.
  - Ex: Un copiloto que asiste en la escritura de código o en la elección entre opciones de decisión.

- Cpt: Herramientas de Aumentación de IA (AI augmentation tools).
  - Def: Proveen funcionalidad empaquetada habilitada por IA que aumenta las habilidades/capacidad del usuario.
  - Ctx: Usadas de manera directa e interactiva para completar una tarea específica.
  - Ex: Una herramienta gráfica con IA que ayuda a editar imágenes con pocos clics.

- Cpt: Agentes de Orquestación de IA (AI orchestration agents).
  - Cpt: Orquestación de propósito.
    - Def: Gestionan la delegación y el control humano.
    - Act: Sirven como capa de interfaz humana para coordinar y supervisar sistemas de IA.
  - Cpt: Orquestación de cognición.
    - Def: Coordinan múltiples agentes en diferentes dominios cognitivos.
    - Ex: En conducción autónoma, un agente de conciencia situacional detecta un peatón, un agente de decisión determina frenar, y un agente de ejecución controla los frenos.

- Cpt: Agentes de Automatización de IA (AI automation agents).
  - Def: Sistemas de IA que operan desacoplados de la interacción del usuario para proveer soporte a funciones cognitivas específicas.
  - Mech: Habilitan la automatización a través del ciclo completo Sense-Decide-Act.
  - Req: Deben proveer interfaces de configuración e intervención para que los humanos controlen y alineen su comportamiento.

### 1.3. Cognición de la IA Centrada en el Humano (Human-Centered Al Cognition)

ID: AIHC-COGNITION-01
Fnd: La cognición se refiere a las habilidades mentales modeladas en la psicología cognitiva (percepción, memoria, resolución de problemas, etc.).
Def: Describe el tipo de habilidad cognitiva fundamental proporcionada por los sistemas de IA.

- Cpt: Reino Cognitivo 1: Percibir (Sense).
  - Def: Capacidades perceptuales del sistema de IA o que ayudan al usuario a monitorear el estado del entorno.
  - Mech: Se ejecutan independientemente del usuario para observar, comprender y detectar un evento crítico.
  - Ex: Un agente de detección de fraude que descubre transacciones inusuales.
  - Ex: Un servicio de call center que reconoce el riesgo de pérdida de cliente basado en interacciones.

- Cpt: Reino Cognitivo 2: Decidir (Decide).
  - Def: Sistemas de IA especializados en tomar decisiones.
  - Ex: Motores de reglas tradicionales que toman una entrada y producen una decisión basada en reglas.
  - Ex: Solucionadores de problemas de dominio específico que generan opciones de decisión o planes para problemas complejos.

- Cpt: Reino Cognitivo 3: Actuar (Act).
  - Def: La capacidad de un agente de automatización para desencadenar o ejecutar acciones para promulgar una decisión.
  - Mech: Típicamente se integran con otros sistemas (plugins generativos, ERPs) para ejecutar una acción específica.
  - Ex: Bloquear transacciones financieras, generar y enviar un correo personalizado.

### 1.4. Elasticidad e Interoperabilidad de los Agentes HCAI

ID: AIHC-ELASTICITY-01

- Cpt: Interoperabilidad.
  - Def: Un agente optimizado para una función (ej. asistente) puede requerir otros agentes de automatización especializados en una función cognitiva específica.
- Cpt: Elasticidad del rol.
  - Def: El rol de una solución de IA puede cambiar de asistencia a delegación, a automatización, y viceversa si se necesita intervención humana.
  - Ex: Una experiencia de copiloto puede permitir al usuario delegar funciones a agentes de automatización para reducir la carga cognitiva. En este rol, el copiloto se convierte en una herramienta para meta-gestionar y supervisar funciones delegadas.

### 1.5. Características de las Soluciones HCAI

ID: AIHC-CHARACTERISTICS-01
Fnd: El propósito y la función cognitiva de una solución de IA determinan qué principios de diseño y cualidades de UX son dominantes.

- Cpt: Característica 1: Conciencia del Contexto (Context Awareness).
  - Def: El sistema de IA está vinculado a la realidad externa relevante en su contexto operativo.
  - Mech: El contexto se representa como historial de usuario, series de tiempo, grafos de comportamiento, o gemelos digitales.
  - Res: Permite al sistema establecer tipos de conciencia (de usuario, de tarea, situacional, de misión, etc.).

- Cpt: Característica 2: Centralidad en el Humano (Human-Centeredness).
  - Def: Objetivos de diseño que describen qué dimensiones de calidad de una solución de IA deben optimizarse para una UX favorable.
  - Cpt: Cualidades adicionales de HCAI.
    - Ex: Empatía, confianza, explicabilidad, transparencia, capacidad de intervención, alineación de objetivos.

- Cpt: Característica 3: Control Humano (Human Control).
  - Def: El grado en que los usuarios tienen control sobre el uso, comportamiento y resultado de la solución de IA.
  - Cpt: Niveles de implicación humana.
    - Def: `Human-in-the-loop`: El humano está en el centro de todas las acciones, usando la IA para consulta.
    - Def: `Human-on-the-loop`: El humano mantiene el control final, supervisión y capacidad de anular la acción.
    - Def: `Human-out-of-the-loop`: Los sistemas de IA están desacoplados de la interacción directa, volviéndose más autosuficientes.

## 2. Parte I: IA Centrada en el Humano en los Negocios

ID: AIHC-PART1-BIZ-01

### 2.1. La Escalera de Conciencia Situacional, Decisión y Ejecución (SADE)

ID: AIHC-SADE-01
Purp: Un framework para la toma de decisiones colaborativa Humano-IA.

#### 2.1.1. Resumen (Abstract)

ID: AIHC-SADE-ABSTRACT-01

- Req: Para que los sistemas inteligentes exhiban comportamiento autónomo, deben desarrollar su propia conciencia situacional y habilidad para ejecutar decisiones.
- Purp: Proponer un framework (SADE Ladder) que combina teorías de conciencia situacional, toma de decisiones y planificación de acciones.
- Obj: Entender la anatomía y ergonomía requerida en sistemas inteligentes.
- Cpt: El SADE Ladder actúa como un catalizador, uniendo disciplinas de investigación especializadas.
- Res: Manifiesta una visión sinérgica en un framework conceptual para entender mejor:
  - 1. Las dinámicas de interacción en las interacciones Humano-IA.
  - 2. La importancia de la transparencia y explicabilidad en redes multi-agente para ayudar a los expertos humanos.
- Mech: La identificación de diferentes demandas cognitivas y sub-funciones dentro del SADE Ladder permite a los practicantes:
  - 1. Derivar los requisitos apropiados del análisis de trabajo cognitivo.
  - 2. Diseñar sistemas inteligentes para el lugar de trabajo que sean confiables y aceptados por sus usuarios.

#### 2.1.2. Introducción a SADE

ID: AIHC-SADE-INTRO-01

- Ctx: Los sistemas de IA se utilizan cada vez más en los lugares de trabajo no solo para aumentar las capacidades humanas, sino también para automatizar el trabajo humano y los procesos de negocio.
- Cpt: A diferencia de la automatización tradicional (trabajo repetitivo bien definido), los agentes de automatización basados en IA pueden:
  - 1. Manejar incertidumbres significativas en el entorno.
  - 2. Poseer capacidades de razonamiento y resolución de problemas para tomar decisiones autónomas.
- Def: Nivel de autonomía.
  - Dep: De la capacidad del agente para realizar un bucle de decisión de extremo a extremo sin intervención humana.
  - Cpt: Componentes del bucle:
    - 1. Ser consciente de la situación actual.
    - 2. Tomar decisiones.
    - 3. Convertir decisiones en acción.
- Cpt: Mantener al humano en el bucle ("human in the loop").
  - Purp: Supervisar el rendimiento del sistema, evitar la pérdida de habilidades ("deskilling") y el desapego de la conciencia operativa.
- Cpt: Mantener al humano sobre el bucle ("human on the loop").
  - Purp: Asegurar el control final, la supervisión y la capacidad de anular acciones si se considera apropiado, incluso si la entrada humana directa no es necesaria.
- Purp: Proponer un framework conceptual holístico: SADE Ladder.
  - ID: AIHC-SADE-LADDERFRAMEWORK-01
  - Obj: Desentrañar los prerrequisitos para desplegar el potencial completo de las habilidades cognitivas distribuidas y las interacciones Humano-IA.
- Cpt: Automatización de procesos.
  - Obj: Crear bucles de control "entender/decidir/actuar" de extremo a extremo.
- Cpt: Autonomía total ("human out-of-the-loop").
  - Cond: Se logra solo cuando uno o múltiples agentes de automatización soportan la totalidad de estas funciones.
- Cpt: Colaboración Humano-IA ("teaming").
  - Def: En la mayoría de los casos, el humano estará "on-" o "in-the-loop", realizando tareas de forma colaborativa.
  - Mech: Todos los agentes (humanos y IA) deben formar un equipo ad-hoc y colaborar para lograr un resultado.
  - Req: Un agente de IA debe poseer conciencia de equipo y habilidades de colaboración para coordinarse y comunicarse exitosamente.

#### 2.1.3. Bucles de Toma de Decisiones de Extremo a Extremo

ID: AIHC-SADE-ENDTOENDLOOPS-01

- Cpt: Motivación clave para la automatización.
  - Def: Liberar al agente humano de realizar la tarea para reasignar sus recursos cognitivos.
- Warn: Riesgo asociado.
  - Def: El operador humano puede, con el tiempo, desaprender las habilidades requeridas y desvincularse del contexto, lo que representa un desafío si necesita tomar el control con baja conciencia situacional.
- Ctx: Investigación en automatización (cabinas de avión, asistencia al conductor).
  - Fnd: Se centra en el concepto de conciencia situacional (Situation Awareness - SA).
  - Obj: Asegurar que un nivel básico de SA es compartido entre agentes humanos y de sistema para mantener la preparación del humano para intervenir.
- Cpt: Concepto de Conciencia Situacional (SA).
  - Src: Presentado inicialmente por Endsley (1995).
  - Def: La percepción de los elementos en el entorno, la comprensión de su significado y la proyección de su estado en el futuro cercano.
  - Warn: La conceptualización original de SA no consideraba el proceso de toma de decisiones en sí mismo.
- Cpt: Modelo de Rasmussen (1983).
  - Fnd: Investigó los sistemas de control humano-máquina.
  - Purp: Formalizó cómo las decisiones transforman entradas (información) en salidas (acción).
  - Mech: Introdujo un modelo formal de rendimiento humano con tres niveles basados en la planificación consciente.
  - Cpt: Nivel 1: Basado en Habilidades (Skill-based).
    - Def: La entrada sensorial se transforma directamente en acciones simples sin control consciente.
    - Ctx: Bucles de control que no requieren procesos mentales de alto nivel.
    - Ex: Un conductor manteniendo una distancia específica con el coche de delante.
  - Cpt: Nivel 2: Basado en Reglas (Rule-based).
    - Def: Aplicación de reglas para mapear una entrada (condición) a una salida (acción).
    - Req: Las reglas deben existir y ser conocidas por el agente.
    - Ex: Un termostato que enciende la calefacción o el aire acondicionado cuando la temperatura alcanza un umbral predefinido.
  - Cpt: Nivel 3: Basado en Conocimiento (Knowledge-based).
    - Def: Se aplica en situaciones de mayor incertidumbre (ej. información incompleta).
    - Mech: El agente reúne información adicional para realizar análisis causales y generar opciones de decisión basadas en la experiencia.
    - Ctx: Puede resultar en una investigación prolongada para entender el problema y planificar acciones.

#### 2.1.4. La Escalera de Conciencia Situacional y Ejecución de Decisiones (SADE Ladder)

ID: AIHC-SADE-LADDER-DETAIL-01
Fnd: Inspirado en el trabajo sobre SA (Endsley 1995) y los niveles de control humano-máquina (Rasmussen 1983).
Purp: Integrar los conceptos de conciencia situacional y planificación de acciones con un proceso iterativo de toma de decisiones para formar un modelo de bucle de decisión de extremo a extremo.

- Cpt: Estructura del SADE Ladder.
  - Cpt: Lado Izquierdo (Pilar 1).
    - Def: Construcción de la conciencia situacional.
    - Ref: AIHC-SADE-PHASE1-SA-01.
  - Cpt: Pilar Central (Pilar 2).
    - Def: Proceso de toma de decisiones.
    - Ref: AIHC-SADE-PHASE2-DECISION-01.
  - Cpt: Lado Derecho (Pilar 3).
    - Def: Ejecución de acciones pertinentes a una decisión.
    - Ref: AIHC-SADE-PHASE3-EXECUTION-01.

- Cpt: Fase 1: Conciencia Situacional (Situation Awareness).
  - ID: AIHC-SADE-PHASE1-SA-01
  - Fnd: Sigue el modelo de Endsley.
  - Proc:
    - 1. `Detect`: Etapa inicial de identificación de un nuevo hecho o evento.
    - 2. `Comprehend`: Entender, interpretar y sintetizar la información detectada para reconocer patrones o anomalías.
    - 3. `Project`: Realizar predicciones o pronósticos de eventos futuros.

- Cpt: Fase 2: Toma de Decisiones (Decision-making).
  - ID: AIHC-SADE-PHASE2-DECISION-01
  - Nat: No son niveles lineales, sino "modos" de toma de decisiones informados por la SA.
  - Cpt: Modo 1: Bucles de control directo (Direct control loops).
    - Def: La información entrante conduce directamente a una acción basada en un bucle de retroalimentación algorítmico y cerrado.
    - Ex: Mantener la temperatura en un rango o la velocidad de un vehículo.
  - Cpt: Modo 2: Decisiones basadas en reglas (Rule-based decisions).
    - Def: Se basan en el reconocimiento de condiciones conocidas en el entorno que se pueden mapear a acciones predefinidas.
  - Cpt: Modo 3: Mapeo asociativo (Associative mapping).
    - Def: Heurística aplicada por expertos que mapean instintivamente situaciones difusas a planes de acción establecidos, basados en la similitud con patrones de síntomas pasados.
  - Cpt: Modo 4: Razonamiento basado en conocimiento (Knowledge-based reasoning).
    - Def: Utiliza estrategias que requieren un análisis iterativo y centrado en el problema de la situación.
    - Mech: Implica investigación, predicción y simulación para comprender mejor las relaciones causales, desarrollar planes de acción y comparar resultados anticipados con los objetivos.

- Cpt: Fase 3: Ejecución (Execution).
  - ID: AIHC-SADE-PHASE3-EXECUTION-01
  - Purp: Abarca la implementación de una decisión.
  - Cpt: Planificación de la acción (Action planning).
    - Def: Detalla los planes después de que se han tomado las decisiones, especificando qué acciones se requieren, por quién, cuándo y en qué secuencia.
  - Cpt: Especificación de la acción (Action specification).
    - Def: Detalla las acciones, potencialmente a nivel operativo, incluyendo recursos concretos y parámetros precisos.
  - Cpt: Acción (Action).
    - Def: La implementación real de una decisión o solución.

#### 2.1.5. Implicaciones de Diseño del SADE Ladder

ID: AIHC-SADE-DESIGNIMPLICATIONS-01

- Cpt: Diseño con Humanos Dentro, Sobre o Fuera del Bucle (In, Over, or Out of the Loop).
  - ID: AIHC-SADE-DESIGN-LOOP-01
  - Mech: El SADE Ladder ayuda a entender los diferentes niveles de automatización y el grado de autonomía del sistema.
  - Cpt: Humano "dentro del bucle" (in the loop).
    - Def: Directamente involucrado en un bucle híbrido, donde los expertos humanos y los sistemas de IA soportan las tres fases. El humano es dueño de la toma de decisiones complejas.
  - Cpt: Humano "sobre el bucle" (over/on the loop).
    - Def: El humano supervisa el sistema y monitorea continuamente la calidad de los resultados.
  - Cpt: Humano "fuera del bucle" (out of the loop).
    - Def: El humano está desvinculado del trabajo concreto y solo gestiona los sistemas de IA a un nivel meta (ej. estableciendo objetivos y límites).
  - Cpt: Evolución de la autonomía.
    - Dep: De la confianza y aceptación del experto humano en el sistema de IA, y de la complejidad de la tarea.
    - Req: Un sistema basado en IA debe ser lo suficientemente flexible para soportar diferentes niveles de autonomía y la transición entre estos modos.

- Cpt: Diseño para la Expertise Humana (Designing for Human Expertise).
  - ID: AIHC-SADE-DESIGN-EXPERTISE-01
  - Cpt: Toma de decisiones basada en conocimiento.
    - Def: Proceso iterativo para analizar una situación y crear/comparar opciones de decisión.
    - Cpt: Rol de la IA.
      - Purp: Aumentar esta toma de decisiones humana con sistemas que pueden procesar datos masivos, reconocer relaciones, y ejecutar optimizaciones y simulaciones.
  - Cpt: Expertise.
    - Def: No solo conocimiento de reglas, sino también saber cuándo aplicar estrategias novedosas a problemas novedosos.
  - Cpt: Toma de decisiones naturalista (Naturalistic decision-making - NDM).
    - Fnd: Enraizado en la teoría de los sistemas duales del pensamiento (Kahneman): Sistema 1 (heurístico, automático) y Sistema 2 (metódico, esforzado).
    - Ctx: El mapeo asociativo en el SADE Ladder reconoce la toma de decisiones intuitiva basada en la experiencia (Sistema 1).
  - Cpt: Modelo de Decisión Basado en Reconocimiento (Recognition-Primed Decision Model - RPDM).
    - Mech: Describe cómo los expertos desarrollan heurísticas que se asemejan a un paradigma de coincidencia de patrones, donde las situaciones se mapean a situaciones conocidas y sus procedimientos correspondientes.

- Cpt: Diseño de Ejecución Autónoma (Designing Autonomous Execution).
  - ID: AIHC-SADE-DESIGN-EXECUTION-01
  - Req: Para procesos de negocio autónomos de extremo a extremo, uno o varios agentes de IA deben tener la capacidad de contribuir a la SA, la toma de decisiones y la ejecución.
  - Cpt: Flujos de trabajo adaptativos.
    - Def: Una red de agentes cooperantes transforma el paradigma de flujo de trabajo determinista en uno adaptativo, donde los agentes toman micro-decisiones inteligentes para optimizar cada paso.
  - Cpt: Aspectos de la ejecución.
    - Proc:
      - 1. Orquestación: Definir qué tipo de recursos se necesitan y en qué orden.
      - 2. Asignación de recursos: Asegurar y asignar todos los recursos antes de la ejecución.
      - 3. Acción: La promulgación real de un plan.
  - Warn: La ejecución a menudo no es "inteligente" solo si el plan de acción está completamente especificado. La realidad es que incluso los flujos de trabajo simples a menudo incluyen micro-decisiones.

- Cpt: Diseño para la Transparencia y Explicabilidad de la IA.
  - ID: AIHC-SADE-DESIGN-XAI-01
  - Req: Existe una creciente demanda de transparencia sobre las capacidades cognitivas del sistema de IA subyacente y de explicabilidad de sus insights, recomendaciones y acciones específicas.
  - Mech: El SADE Ladder puede servir como un modelo conceptual para ilustrar cómo una red multi-agente contribuye a un ciclo de tareas.
  - Cpt: Transparencia.
    - Purp: Ayudar a los usuarios a establecer una comprensión adecuada de las capacidades, límites y limitaciones del sistema para ganar confianza y maximizar su utilidad.
  - Cpt: Explicabilidad.
    - Req: Debe estar alineada con los recursos cognitivos disponibles y soportar la navegación hacia atrás a lo largo de la "cadena de pensamiento" dentro de la escalera.
  - Res: Ambos son principios de diseño importantes para empoderar al experto humano, mantener la conciencia situacional y permitir una toma de control efectiva.

#### 2.1.6. Resumen de SADE

ID: AIHC-SADE-SUMMARY-01

- Cpt: El SADE Ladder es una visión integradora que ayuda a guiar el diseño de interacciones exitosas humano-sistema-agente.
- Purp: Permite discutir los aspectos centrados en el ser humano de la automatización de tareas y procesos basada en IA de manera holística, a través de dominios de investigación históricamente desconectados.
- Fnd: Un bucle de decisión de extremo a extremo dependerá de la orquestación de múltiples sub-funciones cognitivas distribuidas entre los tres pilares y asignadas a uno o varios agentes (humanos o de IA).
- Res: El framework evidencia que los diferentes modos de decisión sugieren redes estructuralmente diferentes de agentes de automatización, y que la adaptabilidad situacional del bucle de decisión es esencial.

### 2.2. La Dinámica de las Interacciones Humano-IA en la Toma de Decisiones Organizacionales

ID: AIHC-DYNAMICS-01

#### 2.2.1. Resumen (Abstract)

ID: AIHC-DYNAMICS-ABSTRACT-01

- Ctx: Los sistemas de información (IS) se utilizan cada vez más para soportar tareas de toma de decisiones complejas y basadas en conocimiento intensivo.
- Mech: Los sistemas contemporáneos dependen de machine learning, IA y deep learning.
- Warn: La naturaleza de "caja negra" de estas tecnologías plantea desafíos para su adopción en entornos organizacionales, donde entender la lógica del sistema es importante.
- Purp: Examinar las interacciones de expertos en supply chain con sistemas de IA a través de la lente del modelo de Situation Awareness (SA).
- Obj: Identificar factores que llevan al usuario a delegar tareas a la IA o a intervenir en procesos impulsados por IA.
- Res: Los desajustes entre la SA de la IA y la SA del usuario experto crean tensiones que impactan la delegación de tareas.

#### 2.2.2. Introducción

ID: AIHC-DYNAMICS-INTRO-01

- Cpt: Los sistemas de información (IS) juegan un rol crítico en permitir a los empleados tomar mejores decisiones en entornos organizacionales actuales.
- Ctx: Con mejoras tecnológicas continuas en capacidades de procesamiento de datos, el soporte a la decisión ha evolucionado de cálculos simples a proveer recomendaciones en escenarios de resolución de problemas complejos.
- Res: Este cambio ha transformado los IS de herramientas simples a agentes artificialmente inteligentes que soportan (y trabajan con) expertos de dominio.
- Cpt: Complejidad de la relación usuario-IS.
  - Warn: Los usuarios pueden confiar excesivamente en el IS, perdiendo su capacidad de entender cómo los eventos futuros impactan su entorno de toma de decisiones.
  - Warn: Los usuarios pueden desconfiar del IS, no beneficiándose completamente de su capacidad de procesar grandes volúmenes de datos y derivar insights relevantes.
- Cpt: Pregunta de investigación.
  - ID: AIHC-DYNAMICS-RQ-01
  - Def: ¿Qué factores influencian las decisiones de los profesionales sobre si confiar en la IA en procesos de toma de decisiones organizacionales?
- Cpt: Teoría de Conciencia Situacional (SA).
  - Def: "La percepción de los elementos en el entorno dentro de un volumen de tiempo y espacio, la comprensión de su significado, y la proyección de su estado en el futuro cercano" (Endsley 1995).
  - Ctx: Inicialmente definido para entender la toma de decisiones humana con herramientas de automatización en aviación, pero puede extenderse al contexto de interacciones humano-IA.

#### 2.2.3. Antecedentes (Background)

ID: AIHC-DYNAMICS-BACKGROUND-01

- Cpt: Modelo de Aceptación de Tecnología (TAM).
  - Src: Davis (1989).
  - Fnd: Presenta la utilidad percibida y la facilidad de uso percibida como predictores de la aceptación del usuario.
  - Ctx: Ha evolucionado en modelos como TAM2, UTAUT, TAM3.
  - Warn: Estas teorías asumen que un IS es determinista y se comporta de manera predecible según las reglas de diseño. La IA no se basa en un conjunto predeterminado de reglas, sino que aprende continuamente de nuevas observaciones.
- Cpt: Modelo de Conciencia Situacional (SA Model).
  - Def: Centrado en el humano, enfocándose solo en los operadores humanos.
  - Cpt: Nivel 1 de SA.
    - Def: Percepción de elementos en la situación actual. Observación de puntos de datos relevantes para la toma de decisiones.
  - Cpt: Nivel 2 de SA.
    - Def: Comprensión de la situación actual. Uso de los elementos del Nivel 1 para crear una síntesis significativa que represente la realidad actual.
  - Cpt: Nivel 3 de SA.
    - Def: Proyección del estado futuro. (Nota: El texto original indica que las páginas 32-33 no están en la vista previa, por lo que se asume este es el nivel 3 estándar del modelo de Endsley).

#### 2.2.4. Resultados (Results)

ID: AIHC-DYNAMICS-RESULTS-01

- Cpt: Meta-toma de decisiones (Meta-decision-making).
  - ID: AIHC-DYNAMICS-METADECISION-01
  - Def: "Decidir cómo decidir" (Kottemann 1986). Implica elegir las técnicas y la información que guiarán el proceso primario de toma de decisiones.
  - Ctx: Los tomadores de decisiones en gestión de cadenas de suministro (SCM) ven a la IA más que como meras herramientas; las consideran contrapartes en el proceso de toma de decisiones.
  - Mech: Evalúan continuamente el rendimiento y la confiabilidad de la IA en varias etapas del proceso.
  - Res: La decisión de delegar ciertos aspectos a la IA no es una elección única, sino una consideración continua.

- Cpt: Factores que influencian las meta-decisiones en la fase "Sense, Detect".
  - ID: AIHC-DYNAMICS-FACTORS-DETECT-01
  - Cpt: Factor 1: Datos de Entrada (Input Data).
    - Def: Discrepancias entre los datos que usa la IA y los datos que los expertos humanos consideran relevantes, especialmente en circunstancias excepcionales.
    - Ex: La IA carece de conciencia de la causa raíz de desviaciones debido a variables o puntos de datos faltantes.
    - Res: Si la IA no permite al usuario agregar estos datos adicionales, el usuario puede dudar en delegar la tarea de monitorear el entorno a la IA.
  - Cpt: Factor 2: Control del Usuario sobre Datos de Entrada (User Control on Input Data).
    - Def: La capacidad (o falta) del usuario para configurar o ajustar variables de entrada influye en su meta-decisión de delegar el primer nivel de SA a la IA.
    - Ex: Si el usuario no puede indicar el nivel de experiencia de los empleados (que impacta el tiempo esperado para completar tareas), puede tomar el control en la etapa de percepción.
    - Res: Cuando las excepciones que la IA no puede percibir ocurren con frecuencia, los usuarios pueden comenzar a ignorar las salidas de la IA en etapas posteriores.
  - Cpt: Factor 3: Volumen de Datos (Data Volume).
    - Def: El volumen de datos que debe procesarse influye en la meta-decisión de delegar o no a la IA.
    - Res: Los usuarios confían en la IA para manejar vastas cantidades de datos que serían difíciles o imposibles de procesar manualmente.
    - Res: A medida que el volumen de datos aumenta, aumenta la posibilidad de delegar la tarea a la IA.

- Cpt: Factores que influencian las meta-decisiones en la fase "Sense, Comprehend".
  - ID: AIHC-DYNAMICS-FACTORS-COMPREHEND-01
  - Cpt: Factor 4: Volumen de Datos (Data Volume, continuación).
    - Def: A medida que la dependencia en datos aumenta en SCM, los usuarios reportan tiempo limitado para evaluar cada detalle, encontrando necesario delegar etapas posteriores a la IA.
    - Res: Cuanto mayor es el volumen de datos, más probable es que los usuarios confíen en la IA no solo para construir el nivel inicial de SA, sino también para manejar etapas posteriores.
  - Cpt: Factor 5: Transparencia del Sistema (System Transparency).
    - Def: "La comprensibilidad y predictibilidad del sistema" (Endsley et al. 2003).
    - Mech: Un sistema altamente transparente permite a los usuarios entender las fuentes de datos y la lógica interna detrás de sus predicciones.
    - Res: La transparencia del sistema influye en la confianza del usuario en la IA, lo que a su vez afecta el grado de control que permiten que la IA ejerza.

#### 2.2.5. Discusión y Conclusiones

ID: AIHC-DYNAMICS-DISCUSSION-01

- Purp: Explorar las dinámicas de la toma de decisiones humano-IA en entornos complejos, particularmente en SCM.
- Mech: Entrevistas a 20 profesionales de SCM con experiencia en usar IA para soportar sus decisiones.
- Res: Modelo extendido del proceso de toma de decisiones que resalta cómo los usuarios toman continuas meta-decisiones sobre la delegación de tareas a la IA.
- Cpt: IA como agente autónomo.
  - Def: Posee su propia conciencia situacional (SA), formada por sus entradas de datos y capacidades de aprendizaje en evolución.
- Cpt: Alineación de SA.
  - Res: Los usuarios son más propensos a delegar tareas a la IA cuando perciben una alta alineación entre su SA y la SA de la IA.
  - Res: Esta alineación establece la base para la confianza y influye en el grado de comodidad de los usuarios para delegar tareas.
- Cpt: Tensiones por desajuste de SA.
  - Def: Cuando los usuarios perciben un desajuste, se manifiesta una tensión.
  - Res: Los expertos con alta confianza en su conocimiento de dominio pueden confiar más en su propia SA que en la de la IA.
- Cpt: Factores de diseño del sistema.
  - ID: AIHC-DYNAMICS-DESIGN-FACTORS-01
  - Def: Tres factores de diseño del sistema impactan las meta-decisiones de los usuarios:
    - 1. Transparencia de la IA.
    - 2. Explicabilidad de la IA.
    - 3. Configurabilidad de la IA.
  - Res: La necesidad de justificar decisiones hace más importante que las recomendaciones de la IA sean comprendidas en términos de la lógica subyacente.

## 3. Parte II: El Desafío de Diseño de Usar Agentes Inteligentes para Hacer los Sistemas de Trabajo Más Inteligentes

ID: AIHC-PART2-WS-01
Src: Steven Alter.

### 3.1. Resumen (Abstract)

ID: AIHC-PART2-WS-ABSTRACT-01

- Purp: Presentar un nuevo enfoque para el desafío de diseño de usar agentes inteligentes para hacer los sistemas de trabajo más inteligentes.
- Mech: Comienza resumiendo las ideas principales en una perspectiva de sistemas de trabajo que esboza el contexto.
- Proc:
  - 1. Agregar conceptos y suposiciones sobre máquinas inteligentes.
  - 2. Discutir la "inteligencia" (smartness) de sistemas o dispositivos en términos de capacidades agrupadas bajo categorías: procesamiento de información, autorregulación, acción en el mundo, adquisición de conocimiento.
  - 3. Presentar un espectro de roles que los agentes inteligentes podrían desempeñar para un sistema de trabajo.
  - 4. Presentar facetas del trabajo (ej. tomar decisiones, comunicar, coordinar) a las cuales se podrían aplicar esos roles.

### 3.2. Introducción

ID: AIHC-PART2-WS-INTRO-01

- Cpt: Desafío de diseño.
  - Def: Usar agentes inteligentes para hacer los sistemas de trabajo más inteligentes.
  - Req: Integrar ideas sobre sistemas de trabajo e ideas sobre agentes inteligentes, a pesar de la terminología inconsistente en cada área.
- Warn: Terminología inconsistente.
  - Ex: Las palabras "intelligent" y "smart" se han aplicado a muchas cosas no relacionadas (smart watches, smartphones, smart cities, smart contracts, smart refrigerators).
- Purp: Proveer una forma organizada de pensar sobre oportunidades para obtener mejores resultados haciendo los sistemas más inteligentes, incluso cuando diferentes observadores discrepan sobre su inteligencia.
- Fnd: Las metáforas y definiciones de sí/no de "smart" o "intelligent" no son directamente útiles para el diseño o análisis.
- Mech: Destacar un espectro de posibilidades que los esfuerzos de diseño podrían intentar lograr en grados variables, dependiendo de los recursos disponibles y las necesidades.

### 3.3. La Perspectiva de Sistemas de Trabajo (Work System Perspective)

ID: AIHC-PART2-WS-PERSPECTIVE-01

- Fnd: La perspectiva de sistemas de trabajo ha evolucionado durante tres décadas.
- Ctx: Cubre todos los sistemas operativos en las organizaciones, incluyendo sistemas de trabajo (WS) totalmente automatizados y WS socio-técnicos que usan agentes inteligentes.
- Cpt: Trabajo (Work).
  - Def: El uso de recursos para producir productos o servicios para clientes humanos o no humanos, o para uno mismo.
  - Ctx: No está directamente relacionado con carreras, empleos u organizaciones empresariales.
- Cpt: Sistema de Trabajo (Work System - WS).
  - Def: Un sistema en el que participantes humanos y máquinas realizan trabajo (procesos y actividades) usando información, tecnología y otros recursos para producir productos o servicios específicos para clientes internos o externos.
  - Ctx: El término apareció en la primera edición de MIS Quarterly (Bostrom y Heinen 1977).
- Cpt: Lugar de Trabajo (Workplace).
  - Def: Un lugar físico o virtual donde se realiza el trabajo.
  - Ctx: Excepto en situaciones donde la mayor parte del trabajo es altamente improvisado, la mayoría de los lugares de trabajo contienen múltiples sistemas de trabajo que realizan diferentes aspectos del trabajo requerido.
- Cpt: Casos especiales de WS.
  - Cpt: WS socio-técnico.
    - Def: Participantes humanos realizan algunas de las actividades.
  - Cpt: WS totalmente automatizado.
    - Def: Todas las actividades son realizadas por máquinas; el espacio para participantes está en blanco.
  - Cpt: Sistema de Información (IS).
    - Def: Un WS con actividades dedicadas a capturar, transmitir, almacenar, recuperar, eliminar, manipular y/o mostrar información.
    - Ex: Un IS contable socio-técnico donde contadores deciden cómo se manejarán transacciones y activos específicos para propósitos fiscales, luego producen estados financieros.
  - Cpt: Proyectos, sistemas de servicio, sistemas de autoservicio.
    - Def: Otros casos especiales importantes de WS.

- Cpt: Marco de Sistemas de Trabajo (Work System Framework).
  - ID: AIHC-PART2-WS-FRAMEWORK-01
  - Purp: Proveer una comprensión básica de la forma, función y entorno de un WS.
  - Cpt: Nueve elementos del WS Framework.
    - Def: Elementos de una comprensión básica durante un período en que el WS es suficientemente estable para retener su identidad.
    - Cpt: Elementos completamente dentro del WS.
      - Def: Procesos y actividades, participantes, información, tecnologías.
    - Cpt: Elementos parcialmente dentro y fuera del WS.
      - Def: Clientes y productos/servicios.
    - Cpt: Elementos fuera del WS.
      - Def: Entorno, infraestructura, estrategias.
  - Cpt: Clientes.
    - Def: Personas u organizaciones que reciben y usan productos/servicios producidos por un WS (incluye clientes internos y externos).
  - Cpt: Productos/servicios.
    - Def: Término usado para evitar controversias sobre características especiales de productos versus servicios.
  - Cpt: Entorno.
    - Ex: Cultura organizacional y nacional, competencia, regulación, demografía, políticas y procedimientos organizacionales.
  - Cpt: Infraestructura.
    - Def: Recursos humanos, informativos y técnicos vistos como compartidos por múltiples WS en lugar de estar asociados principalmente con un WS.
    - Ex: Un grupo de TI que sirve como recurso para múltiples WS.

- Cpt: Modelo de Ciclo de Vida del Sistema de Trabajo (Work System Life Cycle - WSLC).
  - ID: AIHC-PART2-WS-LIFECYCLE-01
  - Purp: Explicar cómo los WS cambian con el tiempo.
  - Mech: Los IS y otros WS evolucionan a través de una combinación de cambio planificado (proyectos) y cambio no planificado (adaptaciones y workarounds).
  - Cpt: Fases del WSLC.
    - Def: Iniciación, desarrollo, implementación, operación, mantenimiento.
    - Ctx: Pueden realizarse de manera diferente (waterfall, ágil, prototipos, uso de aplicaciones comerciales, shadow IT).

### 3.4. Conceptos y Suposiciones sobre Máquinas Inteligentes

ID: AIHC-PART2-WS-CONCEPTS-01

- Cpt: Máquina (Machine).
  - Def: Dispositivos basados en software o hardware que realizan trabajo, incluyendo tecnologías de información.
  - Ctx: En este contexto, se centran en máquinas con alguna forma de inteligencia.
- Cpt: Agente (Agent).
  - Def: Algo que produce efectos o realiza acciones en nombre de algo o alguien más.
  - Cpt: Humano como agente.
    - Def: Los humanos pueden actuar como agentes al realizar trabajo en nombre de una organización o de sí mismos.
  - Cpt: Comportamiento del agente.
    - Def: Puede ser reactivo (respuesta automática e inmediata a estímulos ambientales) o proactivo (tomar la iniciativa y planificar acciones con anticipación).
- Cpt: Agente Digital (Digital Agent).
  - Def: Opera ejecutando algoritmos codificados en software.
  - Ctx: Puede verse como un sistema de trabajo porque realiza trabajo usando información, tecnologías y otros recursos para producir productos/servicios.
- Cpt: Agente Inteligente (Intelligent Agent).
  - Def: Opera ejecutando algoritmos y exhibe un nivel no trivial de "inteligencia" (smartness) en procesamiento de información, autorregulación, acción en el mundo y adquisición de conocimiento.
  - Ctx: La operación de un agente inteligente puede verse como un sistema de trabajo.
- Cpt: Conciencia Situacional (Situation Awareness - SA).
  - Src: Endsley (1995).
  - Def: "La percepción de los elementos en el entorno dentro de un volumen de tiempo y espacio, la comprensión de su significado, y la proyección de su estado en el futuro cercano".
  - Ctx: Aplica bien a operadores humanos en situaciones complejas (tripulaciones de aeronaves, control de tráfico aéreo).
  - Ctx: Aplica de manera más limitada a dispositivos como termostatos que operan a través de un simple bucle de retroalimentación algorítmica.
- Cpt: Conciencia Situacional Distribuida (Distributed Situational Awareness - DSA).
  - Def: SA en sistemas socio-técnicos donde la SA es mantenida por agentes humanos y no humanos.
  - Mech: Los artefactos tecnológicos (así como los operadores humanos) tienen algún nivel de SA, al menos en el sentido de que son portadores de información contextualmente relevante.

### 3.5. Inteligencia de Agentes Inteligentes (Smartness of Intelligent Agents)

ID: AIHC-PART2-WS-SMARTNESS-01
Src: Alter (2020a).

- Purp: Proveer una forma general de mirar la "inteligencia" (smartness) usando cuatro categorías para organizar numerosas capacidades.
- Cpt: Dimensiones de la inteligencia.
  - Def: La inteligencia de un agente inteligente o sistema de trabajo en relación con casi cualquier tipo de capacidad que involucre información puede caracterizarse:
    - 1. No inteligente en absoluto: No realiza actividades que exhiban la capacidad.
    - 2. Ejecución programada (Scripted execution): Realiza actividades según instrucciones pre-especificadas.
    - 3. Adaptación formulaica (Formulaic adaptation): Adaptación de actividades basada en entradas o condiciones pre-especificadas.
    - 4. Adaptación creativa (Creative adaptation): Adaptación de actividades basada en análisis no programado o parcialmente programado.
    - 5. Invención no programada o parcialmente programada: Invención de actividades usando ejecución no programada de un workaround o método nuevo.

- Cpt: Cuatro grupos de capacidades.
  - ID: AIHC-PART2-WS-CAPABILITIES-01
  - Cpt: Grupo 1: Procesamiento de Información (Information processing).
    - Def: Capturar, transmitir, almacenar, recuperar, eliminar, manipular, mostrar información.
  - Cpt: Grupo 2: Acción en el Mundo (Action in the world).
    - Def: Percepción (sensing), actuación, coordinación, comunicación, control, acción física.
  - Cpt: Grupo 3: Regulación Interna (Internal regulation).
    - Def: Auto-detección, auto-monitoreo, auto-diagnóstico, auto-corrección, auto-organización.
  - Cpt: Grupo 4: Adquisición de Conocimiento (Knowledge acquisition).
    - Def: Percibir o descubrir, clasificar, compilar, inferir o extrapolar de ejemplos, inferir o extrapolar de abstracciones, probar, evaluar.

- Ctx: La mayoría de los sistemas de trabajo con participantes humanos operan con un nivel no trivial de inteligencia para la mayoría de esas capacidades.
- Ctx: Muy pocos agentes inteligentes exhiben un alto nivel de inteligencia relacionado con la mayoría de esas capacidades.
- Cpt: Desafío de diseño.
  - Def: Diseñar agentes inteligentes cuya inteligencia limitada no obstante mejore la inteligencia de un sistema de trabajo que usa agentes inteligentes.

### 3.6. Hacer los Sistemas de Trabajo Más Inteligentes

ID: AIHC-PART2-WS-SMARTER-01

- Cpt: Sistema de Trabajo Aumentado (Augmented WS).
  - Def: Incorporar un agente inteligente a un WS existente crea un WS aumentado, es decir, el WS original aumentado por las capacidades del agente inteligente.

- Cpt: Método de Análisis de Sistemas de Trabajo (Work System Method - WSM).
  - ID: AIHC-PART2-WSM-01
  - Purp: Proveer un enfoque de análisis para pensar en hacer los sistemas de trabajo más inteligentes.
  - Ctx: Método de análisis y diseño flexible desarrollado para ayudar a profesionales de negocios a analizar sistemas de trabajo por sí mismos y para soportar sus interacciones con profesionales de TI.
  - Proc: Pasos del WSM.
    - 1. Identificar el sistema de trabajo más pequeño que tenga el problema u oportunidad en cuestión.
    - 2. Resumir el sistema de trabajo "as-is" usando una instantánea de sistema de trabajo (work system snapshot).
    - 3. Evaluar la operación del sistema de trabajo usando fortalezas y debilidades percibidas, métricas, incidentes clave, relaciones sociales, etc.
    - 4. Profundizar según sea necesario usando cualquier idea relevante (herramientas WSM publicadas, design thinking, Six Sigma, etc.).
    - 5. Proponer cambios produciendo una instantánea de un sistema de trabajo "to be" que debería funcionar bien.
    - 6. Describir mejoras de rendimiento probables y explicar por qué el esfuerzo parece justificado.

- Cpt: Roles que un Agente Inteligente Podría Desempeñar para un WS.
  - ID: AIHC-PART2-WS-ROLES-01
  - Fnd: El espectro de roles emergió de muchas iteraciones de intentar expandir la dimensión horizontal del framework HCAI de Shneiderman (2020a,b).
  - Cpt: Framework HCAI de Shneiderman.
    - Def: Dos dimensiones: baja vs. alta automatización computacional, bajo vs. alto control humano.
  - Cpt: Espectro de roles (de menor a mayor implicación directa).
    - Proc:
      - 1. Monitorear un Sistema de Trabajo (Monitor a Work System): Un agente inteligente podría monitorear y medir aspectos del trabajo para asegurar que procesos y actividades sean apropiados. Puede generar alarmas cuando aspectos del trabajo comiencen a salirse de límites aceptados (salud, seguridad, carga cognitiva).
      - 2. Proveer Información (Provide Information): Un agente inteligente podría proveer información que ayude a las personas a lograr sus objetivos de trabajo de manera segura y cómoda sin infringir la privacidad u otros derechos.
      - 3. Proveer Capacidades (Provide Capabilities): Un agente inteligente podría proveer capacidades analíticas, de visualización y computacionales que ayuden a los participantes del WS a lograr sus objetivos asignados.
      - 4. Controlar Actividades (Control Activities): Un agente inteligente podría controlar actividades de trabajo directamente para prevenir que actividades específicas se salgan de límites relacionados con seguridad del trabajador, tiempo en el trabajo, estrés, etc.
      - 5. Co-producir Actividades (Coproduce Activities): Un agente inteligente podría ser desplegado en una división de responsabilidad donde el agente y las personas tienen responsabilidades complementarias. La iniciativa puede cambiar entre personas y agentes dependiendo del estado del trabajo.
      - 6. Ejecutar Actividades (Execute Activities): Un agente inteligente podría ejecutar actividades que no deberían o no pueden ser delegadas a las personas (actividades difíciles, peligrosas o imposibles de realizar).

- Cpt: Facetas del Trabajo (Facets of Work).
  - ID: AIHC-PART2-WS-FACETS-01
  - Purp: Considerar la posibilidad de que cualquiera de los roles anteriores podría aplicarse a cualquiera de un conjunto de facetas del trabajo.
  - Def: Aspectos del trabajo que pueden ser observados o analizados.
  - Ex: Tomar decisiones, comunicar, procesar información, coordinar.
  - Fnd: La noción de "faceta" es una analogía a cómo un diamante cortado consiste en una sola cosa con muchas facetas que pueden ser observadas o analizadas.
  - Cpt: Las 18 facetas del trabajo.
    - Def: Todas aplican a WS socio-técnicos y totalmente automatizados, están asociadas con muchos conceptos útiles, traen criterios de evaluación y trade-offs de diseño.
    - Proc: Lista de facetas (Tabla 1 del texto original).
      - 1. Tomar decisiones (Making decisions).
      - 2. Comunicar (Communicating).
      - 3. Proveer información (Providing information).
      - 4. Representar la realidad (Representing reality).
      - 5. Aprender (Learning).
      - 6. Coordinar (Coordinating).
      - 7. Realizar trabajo físico (Performing physical work).
      - 8. Proveer servicio (Providing service).
      - 9. Aplicar conocimiento (Applying knowledge).
      - 10. Planificar (Planning).
      - 11. Improvisar (Improvising).
      - 12. Realizar trabajo de soporte (Performing support work).
      - 13. Crear valor (Creating value).
      - 14. Pensar (Thinking).
      - 15. Controlar la ejecución (Controlling execution).
      - 16. Procesar información (Processing information).
      - 17. Interactuar socialmente (Interacting socially).
      - 18. Mantener la seguridad (Maintaining security).

### 3.7. Un Enfoque Integrado para Diseñar Agentes Inteligentes para Hacer los Sistemas de Trabajo Más Inteligentes

ID: AIHC-PART2-WS-INTEGRATED-01

- Cpt: Premisa principal.
  - Def: Las generalizaciones amplias sobre máquinas inteligentes y la IA en el lugar de trabajo son interesantes de muchas maneras, pero a menudo no son lo suficientemente específicas para ser útiles para describir, analizar o diseñar WS.
- Purp: Evitar ambigüedades relacionadas con los términos "agente inteligente" o "máquina inteligente".
- Mech: Proveer un enfoque integrado para entender agentes inteligentes y sus roles en WS específicos en entornos laborales.
- Fnd: Supuesto básico: Los agentes inteligentes son usados por WS, y la incorporación de un nuevo agente inteligente a un WS debería aumentar las capacidades del WS de maneras predecibles.
- Proc: Rutas posibles para diseñar agentes inteligentes.
  - 1. Usar el esquema general del WSM para entender el contexto y las oportunidades/problemas relacionados.
  - 2. Aplicar ideas adicionales:
    - Un espectro de roles posibles de agentes inteligentes.
    - Facetas del trabajo que pueden ser afectadas por esos roles.
    - Diferentes grados de inteligencia que podrían perseguirse en relación con capacidades en cuatro categorías.
- Warn: Este enfoque no pretende ser mecánico o formulaico. Su intención es iluminar posibilidades para diseñar agentes inteligentes con máximo beneficio.
- Proc: Preguntas para aplicar las ideas.
  - 1. ¿Qué tan inteligente es el WS actual en relación con las diversas capacidades agrupadas bajo procesamiento de información, autorregulación, acción en el mundo y adquisición de conocimiento?
  - 2. ¿Cuáles son las direcciones prácticas para hacer el WS más inteligente mejorando esas capacidades en direcciones que podrían ser beneficiosas?
  - 3. ¿Cómo se vinculan esas direcciones posibles con los roles y facetas del trabajo identificados usando el framework AR?
- Warn: Advertencia importante: La mayoría de los agentes inteligentes tienen inteligencia limitada debido a las limitaciones actuales en cómo los dispositivos automatizados pueden entender sus propios propósitos, comportamientos o entornos.
- Cpt: Asunto clave.
  - Def: Intentar hacer el sistema de trabajo más inteligente a través de una combinación integrada de cambios, algunos de los cuales podrían involucrar agentes inteligentes nuevos o mejorados.
