# Artefacto: Centro Integrado de Emergencia y Seguridad (CIES) de Ñuble con Integración SITIA

ID: CIES-SITIA-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-10-06
Modification-Date: 2025-10-06
Source: documento: CIES SITIA.md
Ctx: Plan de Transformación Digital y IA para GORE Ñuble.

---
BEGIN_LLM_INSTRUCTIONS

You are an AI agent consuming a Structured Telegraphic Style (STS) artifact. Your primary task is to parse and reason over THIS document with absolute fidelity, using only the rules defined below. This artifact is a self-contained source of truth.

1. **Core Objective**: Maintain perfect fidelity to the information (`meat`) and structure (`skeleton`). Do not summarize, interpret, or infer information not explicitly present. Prohib: Applying these rules to artifact creation or translation tasks; they are exclusively for consumption.

2. **Conceptual Metaphors**:
    - `meat`: Essential information, data, and facts. Must be preserved with zero loss.
    - `skeleton`: Logical structure (headers, IDs, lists, tables). This is also `meat` and must be preserved.
    - `fat`: Non-essential verbiage (filler words, rhetoric, stylistic prose). Must be ignored during reasoning as it has no informational value.

3. **Lexicon Mode & Expansion**: This document uses an **Abbreviated Lexicon**. You MUST treat the following keywords as valid and expand them according to this mapping:
    - `Act:` -> `Action:`
    - `Warn:` -> `Warning:`
    - `Cause:` -> `Cause:`
    - `Cpt:` -> `Concept:`
    - `Cond:` -> `Condition:`
    - `Ctx:` -> `Context:`
    - `Def:` -> `Definition:`
    - `Dep:` -> `Dependency:`
    - `Dest:` -> `Destination:`
    - `Dln:` -> `Deadline:`
    - `Ex:` -> `Example:`
    - `Fnd:` -> `Foundation:`
    - `ID:` -> `ID:`
    - `Instr:` -> `Instruction:`
    - `Just:` -> `Justification:`
    - `Mech:` -> `Mechanism:`
    - `Mssn:` -> `Mission:`
    - `Mdl:` -> `Model:`
    - `Nat:` -> `Nature:`
    - `Obj:` -> `Objective:`
    - `Proc:` -> `Process:`
    - `Prohib:` -> `Prohibition:`
    - `Purp:` -> `Purpose:`
    - `Rec:` -> `Recommendation:`
    - `Ref:` -> `Reference:`
    - `Req:` -> `Requirement:`
    - `Res:` -> `Result:`
    - `Resp:` -> `Responsible:`
    - `Src:` -> `Source:`

4. **Reference (`Ref:`) Policy**:
    - `Ref:` is used for **internal cross-references only**.
    - It MUST point to an `ID:` that exists within THIS document.
    - You MUST NOT interpret a `Ref:` as a link to an external document or resource. Mentions of other documents are purely contextual (`Ctx:`).

5. **Language Invariance Policy**:
    - The `Keywords` in the lexicon are a fixed control vocabulary in English.
    - All `EssentialData` (the content following a `Keyword:`) MUST be preserved in its original language. Do not translate it.

END_LLM_INSTRUCTIONS
---

## 1. Descripción General

ID: CIES-SITIA-DESC-01

- Cpt: CIES-NUBLE.
  - Def: Centro Integrado de Emergencia y Seguridad de Ñuble.
  - Nat: Iniciativa estratégica del Gobierno Regional.
  - Purp: Fortalecer la seguridad pública y la gestión integral de riesgos.
  - Ctx: Aplicado a las 21 comunas de la región de Ñuble.
- Cpt: Funcionalidad-Principal.
  - Nat: Núcleo para vigilancia, coordinación y respuesta ante emergencias y delitos.
  - Mech: Utiliza tecnología de punta y colaboración interinstitucional.
- Cpt: Alianza-Estrategica.
  - Def: Colaboración con el Sistema Integrado de Teleprotección con Inteligencia Artificial (SITIA).
  - Resp: Subsecretaría de Prevención del Delito.
  - Purp: Potenciar capacidades del CIES.
  - Mech: Integrar capacidades locales del CIES con plataformas de analítica avanzada a nivel nacional.
- Cpt: Capacidades-Potenciadas.
  - Obj: Reforzar la detección de prófugos.
  - Obj: Reforzar la búsqueda de personas desaparecidas.
  - Obj: Reforzar la localización de vehículos con encargo de búsqueda.
- Cpt: Gobernanza-Datos.
  - Req: Gobernanza de datos transparente.
  - Fnd: Pleno respeto de la Ley N° 19.628.

## 2. Objetivos

ID: CIES-SITIA-OBJ-01

- Obj: Mejorar capacidad de prevención y respuesta ante emergencias y delitos en la región.
- Obj: Fortalecer coordinación interinstitucional para gestión efectiva de seguridad pública.
- Obj: Potenciar análisis de video con herramientas de IA de nivel nacional.
  - Purp: Anticipar riesgos.
  - Purp: Optimizar gestión de emergencias.
- Obj: Facilitar intercambio de evidencia digital con Ministerio Público y policías.
  - Mech: A través de plataformas unificadas.
- Obj: Contribuir al desarrollo social, económico y territorial de Ñuble.
  - Mech: Mediante la reducción de riesgos y amenazas.

## 3. Componentes Clave

ID: CIES-SITIA-COMP-01

### 3.1. Infraestructura Tecnológica y Física

ID: CIES-SITIA-COMP-INFRA-01

#### 3.1.1. Sala de Monitoreo Central

ID: CIES-SITIA-COMP-INFRA-SALA-01
Ctx: Ubicada en GORE Ñuble.

- Cpt: Diseño-Ergonomia.
  - Def: Sala de 77,03 m².
  - Fnd: Diseñada según norma ISO 11064.
  - Ctx: Incluye zonas operativas, técnicas, de supervisión y de descanso.
  - Purp: Garantizar rendimiento óptimo y bienestar del personal.
- Cpt: Visualizacion-Centralizada.
  - Def: Video Wall de 6x2 metros.
  - Ctx: Pantallas LED modulares 4K.
  - Mech: Capaz de mostrar hasta 16 vistas simultáneas.
  - Purp: Permitir monitoreo global y detallado de puntos críticos.
- Cpt: Estaciones-Trabajo.
  - Def: 7 estaciones de trabajo (6 operadores, 1 supervisor).
  - Ctx: 3 estaciones adicionales para Unidad Operativa de Control de Tránsito (UOCT).
  - Ctx: Cada estación equipada con monitor Full HD 32", teclado ergonómico, joystick.
  - Purp: Control preciso de cámaras PTZ.
- Cpt: Centro-Datos.
  - Def: Infraestructura robusta.
  - Ctx: Racks APC NetShelter SX.
  - Ctx: Servidores redundantes Dell PowerEdge R740.
  - Ctx: Sistemas de Alimentación Ininterrumpida (UPS).
  - Purp: Garantizar operación continua 24/7.

#### 3.1.2. Sistema Integrado de Cámaras y Red

ID: CIES-SITIA-COMP-INFRA-CAMNET-01

- Cpt: Cobertura-Regional.
  - Def: 209 puntos de vigilancia en 21 comunas.
  - Ctx: 140 cámaras PTZ 4K y 69 cámaras multisensor/panorámicas.
- Cpt: Conectividad.
  - Def: Red híbrida de alta velocidad con 316 nodos.
  - Ctx: 80% fibra óptica (100Mbps) y 20% enlaces inalámbricos (50Mbps).
- Cpt: Arquitectura-Federacion.
  - Def: Modelo federado para gestión centralizada con autonomía local.
  - Res: Garantiza resiliencia, robustez y escalabilidad.
- Cpt: Software-Gestion-VMS.
  - Def: Plataforma HikCentral.
  - Mech: Permite gestión centralizada, acceso a video grabado, notificaciones.
  - Ctx: Compatibilidad con estándar ONVIF.
- Cpt: Almacenamiento-Seguro.
  - Def: Capacidad para 60 días de grabaciones a máxima resolución.
  - Mech: Redundancia (RAID, ANR) y cifrado para proteger integridad de datos.

#### 3.1.3. Capacidades de Analítica Avanzada (CIES + SITIA)

ID: CIES-SITIA-COMP-INFRA-ANALITICA-01
Fnd: El sistema CIES cuenta con analítica de video (VCA) para funciones base (detección de movimiento, seguimiento, conteo, intrusión).
Cpt: La capacidad es potenciada por la integración con plataformas especializadas de SITIA.

- Cpt: SITIA-Patentes.
  - Purp: Complementar la lectura de placas local con una red integrada nacional (pórticos públicos y privados).
  - Mech: Datos contrastados en tiempo real con registro oficial de vehículos con encargo de búsqueda.
  - Res: Genera dashboards dinámicos sobre zonas críticas de robo y rutas probables.
- Cpt: SITIA-Evidencia.
  - Def: Plataforma digital para la gestión de evidencias.
  - Fnd: Basada en Genetec Clearance.
  - Purp: Facilitar solicitud, almacenamiento y compartición segura de pruebas audiovisuales.
  - Dest: Municipios, Policías, Fiscalía.
  - Res: Asegura cadena de custodia digital y reduce tiempos de investigación.
- Cpt: SITIA-Armas.
  - Mech: Implementa modelos de IA (basados en YOLOv11) en la red de cámaras.
  - Purp: Generar alertas automáticas en tiempo real al detectar un arma de fuego en la vía pública.
  - Res: Apoya labores de fiscalización y control.
- Cpt: SITIA-Unificacion-Videos.
  - Purp: Centralizar las señales de las cámaras del CIES en una interfaz única a nivel nacional.
  - Mech: Permite acceso a Carabineros de Chile.
  - Res: Refuerza la coordinación y la capacidad de respuesta ante emergencias.

### 3.2. Personal y Estructura Operativa

ID: CIES-SITIA-COMP-OPER-01

- Cpt: Equipo-Humano.
  - Def: 3 operadores y 1 supervisor por turno en la sala.
  - Ctx: Se integra personal de la UOCT.
- Cpt: Turnos-Operacion.
  - Def: Cobertura inicial de 16 horas diarias (08:00 a 00:00).
  - Ctx: Dos turnos rotativos.
  - Obj: Proyección de extenderse a 24/7.
- Cpt: Roles-Capacitacion.
  - Fnd: Personal capacitado conforme al Manual de Operaciones.
  - Cpt: Operadores.
    - Resp: Detección temprana, clasificación de incidentes, seguimiento en tiempo real.
  - Cpt: Supervisores.
    - Resp: Gestión de incidentes críticos, articulación de recursos, enlace interinstitucional.
  - Cpt: Soporte-Tecnico.
    - Resp: Mantenimiento preventivo y correctivo de la plataforma.
- Cpt: Enlaces-Interinstitucionales.
  - Def: Personal que actúa como facilitador de comunicación directa.
  - Dest: Carabineros, PDI, Bomberos, SAMU, 21 municipios.

### 3.3. Procesos y Protocolos (Marco Operativo y Legal)

ID: CIES-SITIA-COMP-PROC-01
Fnd: Todas las actuaciones se rigen por un estricto Manual de Operaciones.
Req: Garantizar el cumplimiento de la Ley N° 19.628 sobre Protección de la Vida Privada.

- Cpt: Protocolos-Vigilancia-Respuesta.
  - Def: Procedimientos estandarizados para monitoreo, detección, clasificación y escalamiento de incidentes.
  - Ctx: Clasificación por prioridad (alta, media, baja).
- Cpt: Cadena-Custodia-Digital.
  - Def: Las grabaciones son consideradas evidencia legal.
  - Proc: Su entrega se realiza únicamente bajo requerimiento formal (orden judicial o del Ministerio Público).
  - Req: Utilizar medios seguros y controlados para garantizar validez.
- Cpt: Gestion-Privacidad.
  - Proc: Grabaciones se almacenan por un máximo de 30 días.
  - Act: Eliminación segura e irreversible posterior al plazo.
  - Mech: Ciudadanos pueden solicitar cautela de una grabación por hasta 6 meses.
  - Cond: Si son víctimas o testigos de un delito.
- Cpt: Plan-Contingencia.
  - Def: Análisis de riesgos y plan de acción.
  - Purp: Enfrentar fallos técnicos, cortes de energía o desastres naturales.
  - Res: Asegurar la continuidad operativa.
- Cpt: Coordinacion-Interinstitucional.
  - Def: Canales de comunicación directos y protocolos de acción conjunta.
  - Ctx: Con todas las entidades de seguridad y emergencia.

## 4. Sostenibilidad y Modelo de Gestión

ID: CIES-SITIA-SOST-01

- Cpt: Financiamiento-Operativo.
  - Mech: Continuidad garantizada a través de presupuesto anual.
  - Purp: Cubrir gastos recurrentes (RR.HH., mantenimiento, servicios).
- Cpt: Mantenimiento-Garantia.
  - Def: Garantía técnica de 22 meses.
  - Ctx: Incluye mantenimiento preventivo trimestral.
- Cpt: Convenio-Colaboracion.
  - Mech: La relación con SITIA se formaliza a través de un convenio marco de colaboración.
  - Resp: Subsecretaría de Prevención del Delito y Gobierno Regional.
  - Purp: Establecer los ejes de cooperación en integración tecnológica, intercambio de datos y capacitación.

## 5. Beneficios para la Región

ID: CIES-SITIA-BENEF-01

- Res: Mayor seguridad y protección (disuasión y respuesta rápida).
- Res: Mejora en los tiempos de respuesta ante emergencias, minimizando daños.
- Res: Fortalecimiento de la coordinación interinstitucional, optimizando uso de recursos.
- Res: Generación de evidencia de alta calidad y estandarizada para apoyar procesos judiciales.
- Res: Acceso a una red de inteligencia nacional, mejorando capacidad de análisis y prevención.
- Res: Creación de un entorno más seguro para la inversión y la vida en comunidad en Ñuble.
