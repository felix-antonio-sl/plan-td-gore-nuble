# Artefacto: Marco Integrado de Seguridad de la Información GORE Ñuble

ID: GORE-NUBLE-SI-MARCO-INTEGRADO-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-10-06
Modification-Date: 2025-10-06
Source: documentacion sistemas gore nuble.md
Ctx: Estrategia integral y unificada del GORE Ñuble para la protección de sus activos de información.

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

## 1. Fundamentos de la Política de Seguridad de la Información

ID: GORE-NUBLE-SI-FUNDAMENTOS-01
Purp: Establecer las bases conceptuales, legales y administrativas del sistema de gestión de seguridad de la información del GORE Ñuble.
Cpt: Define propósito, alcance, marco normativo y gobernanza de la política.

### 1.1 Principios y Objetivos Generales

ID: GORE-NUBLE-SI-PRINCIPIOS-01
Fnd: Formalizar el uso correcto de sistemas y aplicar buenas prácticas para proteger la información generada y gestionada.

- Cpt: 1.1.1 Propósito y Resumen de la Política
  - ID: GORE-NUBLE-SI-PROPOSITO-01
  - Obj: Definir un marco que asegure una infraestructura informática robusta para facilitar las misiones del servicio (comunicación, tareas administrativas).
  - Req: Todos los usuarios de la infraestructura TIC deben respetar la integridad de los recursos.
  - Prohib: Realizar accesos no autorizados.
  - Req: Usar de manera responsable los recursos compartidos.
  - Req: Respetar licencias de software y propiedad intelectual.

- Cpt: 1.1.2 Alcance y Ámbito de Aplicación
  - ID: GORE-NUBLE-SI-ALCANCE-01
  - Nat: Aplicación universal dentro de la institución.
  - Dest: Personal de planta, a contrata y a honorarios.
  - Ctx: Se extiende a cualquier entidad externa que utilice los recursos informáticos del Gobierno Regional.
  - Ctx: Procedimientos de respaldo y respuesta a incidentes aplican a todos los equipos y servidores con datos críticos y a todos los usuarios del GORE Ñuble.

- Cpt: 1.1.3 Recursos y Activos Cubiertos por la Política
  - ID: GORE-NUBLE-SI-ACTIVOS-CUBIERTOS-01
  - Def: El marco de seguridad abarca todos los sistemas de información (individuales o compartidos) y toda la infraestructura de comunicaciones propiedad del servicio o administrada por su Unidad de Informática.
  - Cpt: Inclusiones explícitas.
    - - Equipos: estaciones de trabajo, notebooks, servidores.
    - - Periféricos: impresoras, dispositivos Wi-Fi.
    - - Software.
    - - Servicios informáticos: correo electrónico, web, videoconferencias.

### 1.2 Marco Legal y Normativo

ID: GORE-NUBLE-SI-MARCO-LEGAL-01
Fnd: La política se sustenta en legislación chilena vigente y estándares técnicos reconocidos.
Purp: Asegurar un cumplimiento normativo riguroso.

- Cpt: 1.2.1 Adhesión a Leyes y Decretos Chilenos
  - ID: GORE-NUBLE-SI-LEYES-DECRETOS-01
  - Fnd: Decreto Supremo N°83, que establece normas técnicas sobre seguridad y confidencialidad de documentos electrónicos para órganos de la Administración del Estado.

- Cpt: 1.2.2 Legislación Clave
  - ID: GORE-NUBLE-SI-LEGISLACION-CLAVE-01
  - Req: Aplicación estricta de las siguientes leyes chilenas:
    - - Ley 19.223: Delitos informáticos (destrucción de sistemas, acceso indebido, alteración/difusión maliciosa de datos).
    - - Ley 17.336: Propiedad intelectual.
    - - Ley 19.628: Protección de la vida privada y datos de carácter personal.
    - - Ley 19.799: Documentos y firma electrónica.

- Cpt: 1.2.3 Normas Técnicas Aplicables
  - ID: GORE-NUBLE-SI-NORMAS-TECNICAS-01
  - Fnd: El diseño se alinea con estándares internacionales y nacionales.
  - Cpt: Referencias explícitas.
    - - Norma ISO 27001:2013 y 27002:2013: Referencia para política general y procedimientos de respaldo/respuesta a incidentes.
    - - Norma Chilena NCh 2777: Referencia a controles de seguridad informática.
    - - Política Nacional de Ciberseguridad.

### 1.3 Gobernanza y Mantenimiento de la Política

ID: GORE-NUBLE-SI-GOBERNANZA-01
Purp: Establecer mecanismos para mantener la política actualizada, difundida y con evolución documentada.

- Cpt: 1.3.1 Periodicidad de Evaluación y Revisión
  - ID: GORE-NUBLE-SI-REVISION-01
  - Req: La política debe ser revisada y evaluada formalmente con una periodicidad mínima de tres años.
  - Cond: La revisión puede ser anticipada si ocurren cambios significativos que afecten la evaluación de riesgos original (incidentes importantes, nuevas vulnerabilidades, cambios de infraestructura).

- Cpt: 1.3.2 Mecanismos de Difusión
  - ID: GORE-NUBLE-SI-DIFUSION-01
  - Mech: La difusión se realiza principalmente a través del correo electrónico institucional.
  - Dest: Todos los funcionarios y funcionarias del Gobierno Regional de Ñuble.

- Cpt: 1.3.3 Historial y Control de Versiones
  - ID: GORE-NUBLE-SI-VERSIONES-01
  - Req: Se mantiene un estricto control de versiones para documentar la evolución.
  - Ex: Política de Seguridad de la Información actualizada a v3.0 en agosto de 2020.
  - Ex: Procedimientos de respaldo y respuesta a incidentes en v1.0 en 2019.

## 2. Estructura Organizativa, Roles y Responsabilidades

ID: GORE-NUBLE-SI-ESTRUCTURA-ORG-01
Purp: Garantizar la correcta implementación y mantenimiento del marco de seguridad mediante una estructura organizativa clara, con roles y responsabilidades definidos.

### 2.1 Definición de Roles Clave en Seguridad

ID: GORE-NUBLE-SI-ROLES-CLAVE-01
Fnd: La política define roles fundamentales con deberes específicos para una gestión eficaz y compartida de la seguridad.

- Cpt: 2.1.1 Responsable Administrativo del Equipamiento
  - ID: GORE-NUBLE-SI-ROL-RESP-ADMIN-01
  - Def: Persona responsable de los equipos informáticos instalados en el servicio y a su cargo.
  - Mech: La responsabilidad se formaliza al firmar el acta de entrega del equipamiento.
  - Req: Sus obligaciones deben estar indicadas en su contrato.

- Cpt: 2.1.2 Administrador del Sistema
  - ID: GORE-NUBLE-SI-ROL-ADMIN-SISTEMA-01
  - Resp: Gestión técnica y administración de sistemas a su cargo; supervisar cumplimiento de la política de uso.
  - Ctx: Rol generalmente desempeñado por el informático a cargo del sistema. La Unidad de Informática asume este rol para recursos globales.
  - Cpt: Deberes.
    - - Prevenir daños físicos a componentes del sistema.
    - - Respetar licencias de hardware y software.
    - - Proteger la seguridad de datos, red y equipos.
    - - Garantizar procedimientos de recuperación de información en servidores bajo su responsabilidad.

- Cpt: 2.1.3 Encargado de Seguridad
  - ID: GORE-NUBLE-SI-ROL-ENC-SEGURIDAD-01
  - Nat: Figura central para la gobernanza de la seguridad.
  - Resp: Dirigir medidas y acciones para hacer cumplir la política; su interpretación, control y resolución de problemas.
  - Cpt: Responsabilidades principales.
    - - Redactar y proponer la Política de Seguridad.
    - - Interpretar la política y resolver conflictos.
    - - Asegurar el cumplimiento de la política, colaborando con otras unidades.
    - - Diseñar y monitorizar la arquitectura de seguridad.
    - - Colaborar con el responsable del Programa de Mejoramiento de la Gestión de Seguridad de la Información.

- Cpt: 2.1.4 Profesional de la Unidad de Informática
  - ID: GORE-NUBLE-SI-ROL-PROF-INFO-01
  - Nat: Brazo ejecutor de tareas técnicas de seguridad.
  - Cpt: Responsabilidades transversales.
    - - General: Preparar respuesta ante incidentes y velar por cumplimiento de procedimientos.
    - - Respaldo de información: Ejecutar respaldo de servidores y equipos; realizar pruebas de restauración mensuales.
    - - Respuesta a incidentes: Realizar análisis técnico, reparación/eliminación del incidente y su cierre.

- Cpt: 2.1.5 Usuarios y Funcionarios del Gobierno Regional
  - ID: GORE-NUBLE-SI-ROL-USUARIOS-01
  - Def: Todos los funcionarios, sin importar tipo de contrato.
  - Resp: Cumplir con lo establecido en la política y procedimientos.
  - Cpt: Deberes.
    - - Identificar la información a respaldar.
    - - Informar oportunamente a la Unidad de Informática sobre cualquier evento o incidente detectado.
    - - Aplicar políticas y normas de seguridad en sus tareas.

### 2.2 El Comité de Seguridad de la Información (CSI)

ID: GORE-NUBLE-SI-COMITE-CSI-01
Def: Órgano colegiado responsable de la supervisión y gestión estratégica de la seguridad de la información.

- Cpt: 2.2.1 Composición, Presidencia y Secretaría Ejecutiva
  - ID: GORE-NUBLE-SI-CSI-COMPOSICION-01
  - Resp: Presidente: Encargado de Seguridad de la Información.
  - Resp: Secretario Ejecutivo: Jefe de la Unidad de Informática (lleva registro de actas, controla asistencia).

- Cpt: 2.2.2 Miembros Departamentales
  - ID: GORE-NUBLE-SI-CSI-MIEMBROS-01
  - Nat: Composición multidisciplinaria para visión integral.
  - Cpt: Conformado por jefes o encargados de:
    - - Jefa Depto. Recursos Humanos.
    - - Jefa Depto. de Finanzas y Presupuesto.
    - - Jefe Unidad de Auditoría.
    - - Jefa Depto. Jurídico.
    - - Encargada de Riesgos.
    - - Presidente(a) Comité Paritario.
    - - Jefe Unidad de Adquisiciones.
    - - Encargada Unidad de Archivos.

- Cpt: 2.2.3 Quórum de Funcionamiento, Suplencias y Toma de Decisiones
  - ID: GORE-NUBLE-SI-CSI-QUORUM-01
  - Cpt: Normas de operación.
    - - Suplencias: Cada titular tiene un suplente designado con derecho a voz y voto.
    - - Quórum: Mínimo para sesionar es de seis integrantes.
    - - Toma de Decisiones: Acuerdos por mayoría de votos. En caso de empate, decide el voto del Encargado de Seguridad.

### 2.3 Responsabilidades Jerárquicas en la Gestión de Seguridad

ID: GORE-NUBLE-SI-RESP-JERARQUICAS-01
Purp: Definir una clara cadena de mando y responsabilidad, asegurando compromiso desde el más alto nivel.

- Cpt: 2.3.1 Jefe Superior del Servicio
  - ID: GORE-NUBLE-SI-RESP-JEFE-SERVICIO-01
  - Resp: Máximo responsable; liderar el proceso.
  - Act: Aprobar políticas de seguridad; validar estrategias y mecanismos de control; asignar recursos.

- Cpt: 2.3.2 Comité de Seguridad
  - ID: GORE-NUBLE-SI-RESP-COMITE-01
  - Resp: Supervisar la implementación de la política, procedimientos y estándares.
  - Act: Proponer estrategias y soluciones; arbitrar conflictos; reportar a la dirección sobre mejoras e incidentes.

- Cpt: 2.3.3 Secretario Ejecutivo del CSI (Jefe de Informática)
  - ID: GORE-NUBLE-SI-RESP-SEC-EJECUTIVO-01
  - Resp: Coordinador de actividades de gestión e implementación de la política.
  - Act: Seguimiento y control del PMG de Seguridad de la Información; llevar registro de actas; subrogar al presidente; comunicar acuerdos.

- Cpt: 2.3.4 Auditoría Interna
  - ID: GORE-NUBLE-SI-RESP-AUDITORIA-01
  - Nat: Órgano de control independiente.
  - Act: Monitorear el avance de cada etapa de la implementación del Proceso de Gestión de Seguridad; reportar periódicamente hallazgos al Jefe Superior del Servicio.

## 3. Gestión de Activos y Clasificación de la Información

ID: GORE-NUBLE-SI-GESTION-ACTIVOS-01
Fnd: Establece cómo el GORE Ñuble identifica, controla y protege sus recursos de información y los sistemas que la procesan.

### 3.1 Definición y Control de Activos

ID: GORE-NUBLE-SI-CONTROL-ACTIVOS-01
Purp: Establecer principios y procedimientos para identificar, inventariar y asignar responsabilidades sobre los activos de información.

- Cpt: 3.1.1 Concepto de Activo de la Información
  - ID: GORE-NUBLE-SI-CONCEPTO-ACTIVO-01
  - Def: Todo aquello que la organización considera importante o de alto valor.
  - Cpt: Incluye:
    - - Información en sí (bases de datos, contraseñas, etc.).
    - - Componentes que la soportan (servidores, switches, documentación, equipos, UPS).
  - Purp: La política define lineamientos para proteger estos activos contra accesos no autorizados que afecten su confidencialidad, disponibilidad e integridad.

- Cpt: 3.1.2 Procedimiento de Inventario de Activos
  - ID: GORE-NUBLE-SI-INVENTARIO-ACTIVOS-01
  - Req: El GORE Ñuble debe contar con un procedimiento formal para administrar un inventario de activos.
  - Just: Permite tener una visión clara de todos los activos a proteger.
  - Req: Cada activo informático del inventario debe tener un responsable asignado para su mantenimiento y soporte.

- Cpt: 3.1.3 Asignación de Propiedad y Responsabilidad de los Activos
  - ID: GORE-NUBLE-SI-PROPIEDAD-ACTIVOS-01
  - Req: Toda la información y activos asociados deben tener un propietario designado que sea parte del GORE Ñuble.
  - Resp: El propietario es el principal responsable de la protección del activo.
  - Cpt: Deberes del propietario:
    - - Asegurar la clasificación adecuada de la información y activos.
    - - Definir y revisar periódicamente las restricciones de acceso y la clasificación.

### 3.2 Tratamiento y Manejo de la Información

ID: GORE-NUBLE-SI-MANEJO-INFO-01
Purp: Establecer un sistema para el manejo y protección de activos, basado en una clasificación formal que determina sensibilidad y controles.

- Cpt: 3.2.1 Clasificación de la Información
  - ID: GORE-NUBLE-SI-CLASIFICACION-INFO-01
  - Mdl: Por defecto, toda la información se considera "Pública", a menos que se asigne una clasificación superior.
  - Cpt: Niveles de Clasificación.
    - - "Pública"
    - - "Reservada"
    - - "Secreta"
  - Req: La clasificación debe ser revisada periódicamente para mantenerla o modificarla.

- Cpt: 3.2.2 Protección de la Información Interna
  - ID: GORE-NUBLE-SI-PROT-INFO-INTERNA-01
  - Fnd: La información es un activo vital y debe ser protegida consistentemente con su importancia, valor y criticidad.
  - Req: El GORE debe proveer los recursos para implementar los controles de protección adecuados.
  - Ctx: La institución se reserva el derecho de revocar privilegios de acceso si las condiciones lo ameritan.

- Cpt: 3.2.3 Protección de Datos de Usuarios Externos
  - ID: GORE-NUBLE-SI-PROT-DATOS-EXTERNOS-01
  - Cond: Si la institución procesa datos de usuarios externos calificados como personales y/o sensibles.
    - - Req: Se compromete a asegurar que dicha información no será divulgada sin previa autorización.
    - - Req: Será protegida con el mismo rigor que la información interna.
  - Cond: Si la información de usuarios externos no es catalogada como personal o sensible.
    - - Ctx: Podrá ser divulgada sin autorización previa.

- Cpt: 3.2.4 Intercambio de Información con Terceros
  - ID: GORE-NUBLE-SI-INTERCAMBIO-TERCEROS-01
  - Cond: Al compartir información de usuarios externos con otras instituciones (e.g., externalización de servicios).
  - Req: Es indispensable que los terceros firmen un contrato de confidencialidad y no divulgación antes de la entrega de la información.

## 4. Seguridad Ligada a los Recursos Humanos y Usuarios

ID: GORE-NUBLE-SI-SEGURIDAD-RRHH-01
Fnd: El factor humano es un componente crítico; se definen políticas y procedimientos que abarcan todo el ciclo de vida del empleado para minimizar riesgos.

### 4.1 Seguridad Durante el Ciclo de Empleo

ID: GORE-NUBLE-SI-CICLO-EMPLEO-01
Purp: Integrar la seguridad en los procesos de RRHH para garantizar que el personal esté consciente de sus responsabilidades y sea idóneo para manejar la información.

- Cpt: 4.1.1 Inclusión de la Seguridad en la Definición de Puestos de Trabajo
  - ID: GORE-NUBLE-SI-PUESTOS-TRABAJO-01
  - Req: Las funciones y responsabilidades en seguridad deben ser documentadas formalmente para cada puesto.
  - Ctx: Incluye responsabilidades generales y tareas específicas de protección de activos.

- Cpt: 4.1.2 Proceso de Selección y Verificación de Personal
  - ID: GORE-NUBLE-SI-SELECCION-PERSONAL-01
  - Req: Los candidatos deben ser evaluados rigurosamente.
  - Cpt: Proceso de verificación incluye:
    - - Presentación de cartas de recomendación o referencias.
    - - Revisión de la veracidad y exactitud del currículum vitae.
    - - Corroboración de identidad mediante identificación oficial.
    - - Presentación de evidencia de carrera académica y experiencia laboral.

- Cpt: 4.1.3 Acuerdos y Contratos de Confidencialidad
  - ID: GORE-NUBLE-SI-CONTRATOS-CONFID-01
  - Req: Todos los empleados deben firmar un Contrato de Confidencialidad como parte de sus términos de contratación.
  - Ctx: El requisito se extiende a empleados eventuales o de outsourcing, quienes deben firmar antes de acceder a instalaciones o información.
  - Req: Los acuerdos deben revisarse si cambian las condiciones del contrato y al término de la relación laboral.

- Cpt: 4.1.4 Términos y Condiciones de Empleo Relativos a la Seguridad
  - ID: GORE-NUBLE-SI-TERMINOS-EMPLEO-01
  - Req: Los términos y condiciones de empleo deben establecer claramente las obligaciones del personal en seguridad.
  - Ctx: Estas responsabilidades continúan vigentes por un tiempo predeterminado después de finalizado el contrato.
  - Req: Deben definirse claramente las acciones a tomar si un empleado viola los acuerdos de seguridad.

### 4.2 Políticas de Uso Aceptable (ANEXOS)

ID: GORE-NUBLE-SI-USO-ACEPTABLE-01
Purp: Establecer reglas claras para regular el buen uso de recursos informáticos, prevenir abusos y garantizar un entorno digital seguro.

- Cpt: 4.2.1 Integridad y Disponibilidad de los Recursos
  - ID: GORE-NUBLE-SI-INTEGRIDAD-RECURSOS-01
  - Req: Los usuarios deben respetar la integridad de los sistemas de información.
  - Prohib:
    - - Intervenir, eliminar o dañar hardware, software o periféricos de otros.
    - - Absorber recursos compartidos de forma excesiva (e.g., correos masivos o en cadena).
    - - Desarrollar o usar intencionadamente programas maliciosos.

- Cpt: 4.2.2 Prohibición de Accesos no Autorizados y Suplantación de Identidad
  - ID: GORE-NUBLE-SI-ACCESOS-NO-AUTORIZADOS-01
  - Prohib: Intentar acceder a sistemas o recursos no autorizados, o facilitar que otros lo hagan.
  - Resp: Cada usuario es responsable de mantener en secreto su contraseña y de todo lo ejecutado desde su cuenta.
  - Req: Cualquier anomalía de seguridad detectada debe ser reportada de inmediato a la Unidad de Informática.

- Cpt: 4.2.3 Uso de la Infraestructura de Comunicaciones
  - ID: GORE-NUBLE-SI-USO-COMUNICACIONES-01
  - Prohib: Utilizar la red del GORE Ñuble para fines privados, personales, lúdicos o no relacionados con actividades del servicio.
  - Prohib: Instalar servicios (servidores web, FTP) o dispositivos de comunicación (módems, routers) sin autorización expresa de la Unidad de Informática.
  - Ctx: El correo electrónico es una herramienta de trabajo y debe usarse para propósitos laborales, con lenguaje respetuoso y evitando contenido ofensivo.

- Cpt: 4.2.4 Respeto a las Licencias de Software y Copyright
  - ID: GORE-NUBLE-SI-LICENCIAS-SOFTWARE-01
  - Req: Todo el software utilizado en equipos del GORE Ñuble debe estar debidamente licenciado.
  - Req: Los usuarios y administradores deben respetar las condiciones de licencia y derechos de autor.
  - Prohib: Usar medios del servicio para copiar software protegido o romper sus protecciones.
  - Prohib: La instalación de software por parte de los usuarios.
  - Proc: Si se requiere un programa, debe ser solicitado y gestionado a través de la Unidad de Informática.

### 4.3 Capacitación y Concienciación en Ciberseguridad

ID: GORE-NUBLE-SI-CAPACITACION-01
Fnd: La formación es un pilar para mitigar el riesgo humano.

- Cpt: 4.3.1 Inducción Formal y Educación Continua
  - ID: GORE-NUBLE-SI-INDUCCION-EMPLEADOS-01
  - Proc: La concienciación comienza con una inducción formal para nuevos empleados antes de otorgarles acceso.
  - Ctx: La capacitación es un proceso continuo que debe incluir requerimientos de seguridad, responsabilidades legales y uso correcto de herramientas.

- Cpt: 4.3.2 Oferta de Capacitación del CSIRT Nacional
  - ID: GORE-NUBLE-SI-CAPACITACION-CSIRT-01
  - Ctx: El CSIRT de Gobierno ofrece capacitación complementaria en ciberseguridad a funcionarios públicos.
  - Cpt: 4.3.2.1 Cursos Básicos y Avanzados.
    - ID: GORE-NUBLE-SI-CSIRT-CURSOS-01
    - Ctx: Charlas mensuales online sobre temas como "5 consejos básicos de ciberseguridad", "¿Cómo crear buenas claves?", y "5 consejos avanzados de ciberseguridad". También actividades avanzadas para equipos de TI.
  - Cpt: 4.3.2.2 Requisitos de Inscripción.
    - ID: GORE-NUBLE-SI-CSIRT-REQUISITOS-01
    - Req: Ser funcionario público e inscribirse con el correo electrónico institucional.
  - Cpt: 4.3.2.3 Plataforma y Condiciones.
    - ID: GORE-NUBLE-SI-CSIRT-PLATAFORMA-01
    - Mech: Las charlas se realizan a través de la plataforma Zoom.
    - Ctx: Zoom registra datos de participantes (nombre, correo, tiempo de conexión) que pueden ser compartidos con encargados de ciberseguridad de las instituciones solicitantes.

### 4.4 Proceso Disciplinario

ID: GORE-NUBLE-SI-PROCESO-DISCIPLINARIO-01
Purp: Asegurar el cumplimiento de la política mediante un proceso formal para abordar violaciones de seguridad.

- Cpt: 4.4.1 Proceso Formal ante Violaciones
  - ID: GORE-NUBLE-SI-VIOLACIONES-PROCESO-01
  - Mech: Existe un proceso disciplinario formal para empleados que violen las políticas.
  - Fnd: Se aplica según lo establecido en el reglamento del GORE Ñuble, respetando derechos del empleado y sustentando acusaciones con evidencia.

- Cpt: 4.4.2 Acciones Correctivas y Medidas Disciplinarias
  - ID: GORE-NUBLE-SI-ACCIONES-CORRECTIVAS-01
  - Cond: Si un administrador de sistema detecta un mal uso.
    - Act: Puede tomar medidas para proteger a otros, como notificar al usuario o suspender temporalmente el acceso.
  - Resp: Corresponde al Jefe de Servicio, informado por el Encargado de Seguridad, la adopción de medidas disciplinarias hacia el infractor.

## 5. Controles de Seguridad Técnicos y Operacionales

ID: GORE-NUBLE-SI-CONTROLES-TECNICOS-01
Purp: Describir las medidas y herramientas específicas implementadas para proteger la infraestructura tecnológica del GORE Ñuble.

### 5.1 Seguridad Física y del Entorno

ID: GORE-NUBLE-SI-SEGURIDAD-FISICA-01
Purp: Establecer barreras físicas y controles ambientales para proteger activos críticos contra accesos no autorizados, daños o interferencias.

- Cpt: 5.1.1 Seguridad Perimetral y Control de Acceso
  - ID: GORE-NUBLE-SI-SEG-PERIMETRAL-01
  - Mech: El acceso físico a áreas sensibles está controlado.
  - Ctx: Oficinas de la Unidad de Informática con puerta de acceso con llave.
  - Ctx: Acceso independiente y restringido para la sala de servidores y equipos de comunicaciones.

- Cpt: 5.1.2 Acceso Restringido al Data Center / Sala de Servidores
  - ID: GORE-NUBLE-SI-ACCESO-DATACENTER-01
  - Ctx: Servidores, equipos de comunicaciones y patch panels alojados en dependencias propias.
  - Req: El acceso al Data Center es estrictamente restringido.
  - Cond: Solo funcionarios de la Unidad de Informática tienen permiso de ingreso.
  - Cond: Técnicos externos pueden acceder únicamente si están acompañados y supervisados por un funcionario de la Unidad de Informática.

- Cpt: 5.1.3 Seguridad Climática y de Energía Eléctrica
  - ID: GORE-NUBLE-SI-SEG-CLIMATICA-01
  - Mech: Climatización.
    - Ctx: El Data Center está equipado con aire acondicionado para mantener una temperatura adecuada.
  - Mech: Energía.
    - Ctx: Ambos Data Centers cuentan con grandes equipos UPS que proporcionan autonomía eléctrica y protegen de fluctuaciones de voltaje.

### 5.2 Seguridad de Redes y Comunicaciones

ID: GORE-NUBLE-SI-SEGURIDAD-REDES-01
Purp: Proteger la red institucional contra amenazas internas y externas.

- Cpt: 5.2.1 Firewall de Hardware
  - ID: GORE-NUBLE-SI-FIREWALL-01
  - Resp: La seguridad perimetral de la red está a cargo de un firewall de hardware.
  - Act: Monitorea activamente el tráfico de red y los sitios web visitados.
  - Ctx: Cuenta con sistema integrado de antivirus y antispam.

- Cpt: 5.2.2 Autenticación de Usuarios
  - ID: GORE-NUBLE-SI-AUTENTICACION-01
  - Fnd: Acceso a recursos basado en el principio de identidad verificada.
  - Req: Todos los usuarios de la red deben ser autenticados para acceder a sistemas y recursos.

- Cpt: 5.2.3 Seguridad a Nivel de Usuario
  - ID: GORE-NUBLE-SI-SEG-USUARIO-01
  - Ctx: Cada estación de trabajo está protegida individualmente.
  - Mech: Se provee un antivirus licenciado en cada PC que se actualiza automáticamente una vez al día.
  - Act: El software realiza un chequeo automático de todos los archivos manejados en el equipo.

- Cpt: 5.2.4 Seguridad en la Navegación a Internet
  - ID: GORE-NUBLE-SI-SEG-NAVEGACION-01
  - Ctx: Todos los funcionarios tienen acceso a Internet con restricciones.
  - Mech: La Unidad de Informática administra perfiles de usuario que restringen el acceso a páginas consideradas peligrosas.
  - Act: La Unidad de Informática monitorea el tráfico para detectar usos indebidos y puede restringir la navegación.

- Cpt: 5.2.5 Seguridad del Servicio de Correo Electrónico
  - ID: GORE-NUBLE-SI-SEG-CORREO-01
  - Resp: El servicio es administrado por la Unidad de Informática.
  - Mech: El firewall de hardware posee un detector de spam que verifica cada correo antes de ser depositado en la casilla.
  - Ctx: La medida minimiza significativamente el ingreso de spam, aunque no lo elimina al 100%.

### 5.3 Relaciones con Terceros y Servicios Externos

ID: GORE-NUBLE-SI-RELACION-TERCEROS-01
Purp: Establecer controles estrictos para gestionar riesgos asociados a la colaboración con personal y proveedores externos.

- Cpt: 5.3.1 Identificación y Control de Riesgos con Contrapartes Externas
  - ID: GORE-NUBLE-SI-RIESGOS-TERCEROS-01
  - Req: La institución debe identificar los riesgos asociados al acceso de terceros a la información.
  - Req: En la contratación, se debe establecer que la información a manejar es de acceso restringido y no puede ser divulgada.
  - Req: Los terceros deben firmar un acuerdo de confidencialidad.

- Cpt: 5.3.2 Inclusión de Requisitos de Seguridad en Contratos con Terceros
  - ID: GORE-NUBLE-SI-CONTRATOS-TERCEROS-01
  - Cond: Al contratar servicios de un tercero o outsourcing.
  - Req: Los requerimientos de seguridad deben ser incluidos explícitamente en el acuerdo o contrato.

- Cpt: 5.3.3 Control de Acceso Físico y Lógico para Personal Externo
  - ID: GORE-NUBLE-SI-ACCESO-EXTERNO-01
  - Req: Todo acceso de terceros a activos informáticos debe ser controlado y vigilado.
  - Req: Cualquier acceso (físico o lógico) debe estar justificado y autorizado por el GORE Ñuble.
  - Req: Cualquier persona externa que requiera acceso en sitio deberá estar acompañada y vigilada en todo momento por personal autorizado.

## 6. Gestión de Incidentes de Seguridad de la Información

ID: GORE-NUBLE-SI-GESTION-INCIDENTES-01
Purp: Establecer un enfoque sistemático para manejar brechas y eventos de seguridad, definiendo procedimientos de respuesta, monitoreo y registro.

### 6.1 Procedimiento de Respuesta a Incidentes (Control SSI A.16.01.05)

ID: GORE-NUBLE-SI-RESP-INCIDENTES-01
Fnd: Se ha formalizado un procedimiento específico para asegurar una respuesta coordinada, eficiente y eficaz.

- Cpt: 6.1.1 Objetivo y Alcance del Procedimiento
  - ID: GORE-NUBLE-SI-OBJ-PROCEDIMIENTO-01
  - Obj: Establecer un procedimiento formal para responder ante incidentes de seguridad que afecten a usuarios o sistemas del GORE Ñuble.
  - Ctx: Su alcance es de aplicación general, cubriendo a todos los usuarios identificados de la institución.

- Cpt: 6.1.2 Definición de Eventos de Seguridad de la Información
  - ID: GORE-NUBLE-SI-DEF-EVENTO-SEGURIDAD-01
  - Def: Cualquier suceso que indique una posible violación de la política de seguridad o una falla en los controles.
  - Cpt: Incluye:
    - - Controles de seguridad ineficaces.
    - - Incumplimiento de la integridad, confidencialidad o disponibilidad de la información.
    - - Errores humanos.
    - - Incumplimiento de políticas o procedimientos institucionales.
    - - Incumplimiento de las disposiciones de seguridad física.
    - - Cambios no controlados en el sistema.
    - - Fallas en el software o hardware.
    - - Accesos no autorizados.

- Cpt: 6.1.3 Modo de Operación y Fases de la Respuesta
  - ID: GORE-NUBLE-SI-FASES-RESPUESTA-01
  - Mdl: El procedimiento se estructura en un ciclo de vida de cinco actividades con responsabilidades específicas.
  - Cpt: 6.1.3.1. Actividad 1 y 2: Detección y Aviso
    - ID: GORE-NUBLE-SI-FASE-DETECCION-01
    - Resp: Funcionarios del GORE Ñuble.
    - Act: Detectar eventos/incidentes en sus equipos y comunicarlos oportunamente a la Unidad de Informática (señalando tipo, características, fecha).
  - Cpt: 6.1.3.2. Actividad 3: Análisis técnico
    - ID: GORE-NUBLE-SI-FASE-ANALISIS-01
    - Resp: Profesional de la Unidad de Informática.
    - Act: Analizar técnicamente el incidente para comprender su naturaleza, alcance e impacto, recopilando evidencia.
  - Cpt: 6.1.3.3. Actividad 4: Revisión, eliminación o reparación
    - ID: GORE-NUBLE-SI-FASE-REPARACION-01
    - Resp: Profesional de la Unidad de Informática.
    - Act: Adoptar medidas de corrección y protección para contener el incidente.
  - Cpt: 6.1.3.4. Actividad 5: Cierre del Incidente
    - ID: GORE-NUBLE-SI-FASE-CIERRE-01
    - Resp: Profesional de la Unidad de Informática.
    - Act: Cerrar formalmente el incidente, asegurando su resolución y registrando fecha y observaciones.

### 6.2 Monitoreo, Auditoría y Registros

ID: GORE-NUBLE-SI-MONITOREO-REGISTROS-01
Purp: Permitir la detección temprana de incidentes y facilitar investigaciones mediante requisitos estrictos de registro y monitoreo.

- Cpt: 6.2.1 Creación y Mantenimiento de Bitácoras de Auditoría
  - ID: GORE-NUBLE-SI-BITACORAS-01
  - Req: Deben existir registros completos (bitácoras) de todas las excepciones y eventos relevantes para la seguridad.
  - Req: Los registros deben conservarse por un período mínimo de seis meses.
  - Req: Como mínimo, deben incluir fecha y hora de acceso al sistema.

- Cpt: 6.2.2 Monitoreo del Uso de los Sistemas
  - ID: GORE-NUBLE-SI-MONITOREO-USO-01
  - Req: El GORE Ñuble debe establecer procedimientos para monitorear el uso de sus sistemas y garantizar que los usuarios solo realicen actividades autorizadas.
  - Cpt: El monitoreo debe prestar especial atención a:
    - - Accesos no autorizados (registrando ID de usuario, fecha, hora, tipo de evento).
    - - Operaciones con privilegios (uso de cuentas de administrador, inicio/cierre del sistema).
    - - Alertas o fallas del sistema (mensajes de consola, alarmas de red).

- Cpt: 6.2.3 Protección y Sincronización de Bitácoras
  - ID: GORE-NUBLE-SI-PROT-BITACORAS-01
  - Req: La información de las bitácoras debe estar protegida contra accesos no autorizados y modificaciones.
  - Prohib: Alteración, edición o eliminación de los registros.
  - Req: Para garantizar exactitud, los relojes de los servidores deben estar sincronizados.
  - Req: Los equipos de PC deben estar configurados con la zona horaria (GMT-04:00) Santiago.

- Cpt: 6.2.4 Bitácoras de Operador, Administrador y de Fallas
  - ID: GORE-NUBLE-SI-BITACORAS-ESPECIFICAS-01
  - Req: Personal operativo y administradores deben registrar todas sus actividades en los sistemas.
  - Req: Todas las fallas en la infraestructura deben ser reportadas y registradas para asegurar su resolución.

### 6.3 Registro de Operación de Incidentes

ID: GORE-NUBLE-SI-REGISTRO-INCIDENTES-01
Purp: Formalizar y estandarizar la documentación de incidentes en un registro digital centralizado.

- Cpt: 6.3.1 Registro Digital "REGISTRO DE EVENTOS SEGURIDAD DE LA INFORMACION"
  - ID: GORE-NUBLE-SI-REGISTRO-DIGITAL-01
  - Mech: Se utiliza un archivo digital específico con este nombre para registrar la información de eventos reportados.
  - Resp: La Unidad de Informática es responsable de la producción, mantención y revisión del registro.

- Cpt: 6.3.2 Contenido del Registro
  - ID: GORE-NUBLE-SI-CONTENIDO-REGISTRO-01
  - Req: El registro debe contener, como mínimo, los siguientes campos:
    - - Nombre del Usuario
    - - Evento Informado
    - - Tipo de Equipo
    - - Serie
    - - Fecha de Incidente
    - - Fecha Solución
    - - Análisis / Observaciones

## 7. Continuidad Operacional: Respaldo y Recuperación de Información

ID: GORE-NUBLE-SI-CONTINUIDAD-OP-01
Purp: Detallar las medidas y procedimientos para asegurar la preservación y disponibilidad de información crítica ante fallas, desastres o pérdidas de datos.

### 7.1 Procedimiento de Respaldo de Información (Control SSI A.12.03.01)

ID: GORE-NUBLE-SI-PROC-RESPALDO-01
Fnd: Procedimiento formal que estandariza las actividades de respaldo, alineado con ISO 27001:2013 y la Política de Respaldo institucional.

- Cpt: 7.1.1 Objetivo y Alcance del Procedimiento
  - ID: GORE-NUBLE-SI-OBJ-RESPALDO-01
  - Obj: Mantener respaldada la información institucional contenida en sistemas y equipos del GORE Ñuble.
  - Ctx: Cubre toda la información en servidores y equipos que albergan datos, configuraciones, aplicativos y servicios críticos. Aplica a todos los equipos de los usuarios del GORE Ñuble.

- Cpt: 7.1.2 Responsabilidades
  - ID: GORE-NUBLE-SI-RESP-RESPALDO-01
  - Cpt: Asignación de responsabilidades:
    - - Profesional Unidad Informática: Velar por el cumplimiento del procedimiento y ejecutar el respaldo de servidores y equipos de usuario.
    - - Jefe Departamento de Finanzas: Solicitar respaldos de información de usuarios en caso de desvinculación de funcionarios.
    - - Funcionarios(as) GORE Ñuble: Cumplir con el procedimiento, especialmente en la identificación de la información a respaldar en sus equipos.

- Cpt: 7.1.3 Frecuencia y Método de Respaldo
  - ID: GORE-NUBLE-SI-FRECUENCIA-RESPALDO-01
  - Req: Toda información institucional relevante debe ser respaldada con una periodicidad de una vez al mes.
  - Mech: El respaldo se realiza a todos los equipos de usuarios vía remota desde la Unidad de Informática.

- Cpt: 7.1.4 Almacenamiento y Seguridad de los Respaldos
  - ID: GORE-NUBLE-SI-ALM-RESPALDOS-01
  - Mech: Los respaldos se almacenan en discos duros externos.
  - Ctx: Los discos son custodiados en una caja fuerte ubicada en la División de Administración y Finanzas.

### 7.2 Verificación de la Efectividad de los Respaldos

ID: GORE-NUBLE-SI-VERIF-RESPALDOS-01
Purp: Garantizar que los respaldos sean útiles en caso de contingencia.

- Cpt: 7.2.1 Realización de Pruebas de Restauración
  - ID: GORE-NUBLE-SI-PRUEBAS-RESTAURACION-01
  - Req: Se deben realizar pruebas de restauración de respaldo para comprobar la efectividad de las acciones.
  - Req: Las pruebas deben ejecutarse con una periodicidad de una vez al mes.

- Cpt: 7.2.2 Resolución de Fallas Detectadas
  - ID: GORE-NUBLE-SI-RESOLUCION-FALLAS-01
  - Cond: Si una prueba de restauración presenta fallas.
  - Req: Las fallas deberán ser resueltas de manera prioritaria.

### 7.3 Registros de Operación de Respaldos

ID: GORE-NUBLE-SI-REGISTROS-RESPALDOS-01
Purp: Mantener control y trazabilidad de todas las actividades de respaldo y prueba mediante registros digitales específicos.

- Cpt: 7.3.1 Registro Digital "BITÁCORA DE RESPALDOS"
  - ID: GORE-NUBLE-SI-BITACORA-RESPALDOS-01
  - Mech: Se utiliza un archivo digital en formato Excel para registrar la información de los respaldos.
  - Req: Debe contener como mínimo las columnas: "Código", "Fecha de respaldo", "Equipo Usuario" y "Medio de almacenamiento".

- Cpt: 7.3.2 Registro Digital "BITÁCORA DE PRUEBAS DE RESTAURACIÓN"
  - ID: GORE-NUBLE-SI-BITACORA-PRUEBAS-01
  - Mech: Se emplea un archivo digital en Excel para documentar las pruebas de restauración.
  - Req: Debe incluir los campos: "Código", "Fecha de prueba", "Equipo Usuario", "Presenta incidente (Si/No)", "Descripción de incidente", "Estado de incidente" y "Resultado de Prueba de Restauración".

## 8. Formulario: Registro de Iniciativa de Inversión, Desarrollo e Innovación (IDI)

Sobre estructura implementada en una planilla de google sheet se almacenan los registros de las IDIs del Gore de Ñuble

### Sección 1: Identificación de la Iniciativa

ID: FORM-IDI-S1-IDENTIFICACION-01

#### Código Único de Iniciativa

ID: FORM-IDI-S1-CODIGO-UNICO-01
Field-Label: "Código Único"
Field-Type: Text
Field-Constraint: "Req: mandatory; Format: unique_id."
Field-Instr: "Identificador único de la iniciativa (ej. CVC-AD-39-2025)."

#### Año Presupuestario

ID: FORM-IDI-S1-ANO-PPTAL-01
Field-Label: "Año Presupuestario"
Field-Type: Number
Field-Constraint: "Req: mandatory; Format: aaaa."

#### Nombre de la Iniciativa

ID: FORM-IDI-S1-NOMBRE-01
Field-Label: "Nombre de la Iniciativa"
Field-Type: Text
Field-Constraint: "Req: mandatory."

#### Código BIP

ID: FORM-IDI-S1-CODIGO-BIP-01
Field-Label: "Código BIP"
Field-Type: Text
Field-Constraint: "Req: optional."

#### Clasificación y Localización

ID: FORM-IDI-S1-CLASIFICACION-01
Field-Label: "Clasificación y Localización"
Field-Type: Group

- Field: "Unidad Técnica" (Text)
- Field: "Origen" (Text)
- Field: "Tipología" (Text)
- Field: "Provincia" (Select)
- Field: "Comuna" (Select)

#### Asignación Presupuestaria

ID: FORM-IDI-S1-ASIGNACION-PPTAL-01
Field-Label: "Asignación Presupuestaria"
Field-Type: Group

- Field: "Subtítulo" (Text)
- Field: "Ítem" (Text)
- Field: "Asignación" (Text)

### Sección 2: Financiamiento

ID: FORM-IDI-S2-FINANCIAMIENTO-01

#### Montos (en M$)

ID: FORM-IDI-S2-MONTOS-01
Field-Label: "Montos (en M$)"
Field-Type: Group

- Field: "Monto Total Proyecto" (Currency)
- Field: "Monto Sectorial" (Currency)
- Field: "Monto FNDR Postulado" (Currency)
- Field: "Monto FNDR Adjudicado" (Currency)
- Field: "Aumentos" (Currency)

### Sección 3: Gestión Administrativa y Estado

ID: FORM-IDI-S3-GESTION-01

#### Certificación y Aprobación

ID: FORM-IDI-S3-CERTIFICACION-01
Field-Label: "Certificación y Aprobación"
Field-Type: Group

- Field: "Certificado CORE o RS" (Text)
- Field: "Fecha Certificado" (Date: dd-mm-aaaa)
- Field: "Resolución Crea Asignación" (Text)
- Field: "N° Resolución Aprueba Convenio" (Text)
- Field: "Fecha Resolución Aprueba Convenio" (Date: dd-mm-aaaa)

#### Estado y Seguimiento

ID: FORM-IDI-S3-ESTADO-01
Field-Label: "Estado y Seguimiento"
Field-Type: Group

- Field: "Estado de Avance" (Select)
- Field: "Fecha Firma de Convenio" (Date: dd-mm-aaaa)
- Field: "Observación" (TextArea)

### Sección 4: Adjudicación y Ejecución

ID: FORM-IDI-S4-EJECUCION-01

#### Licitación y Adjudicación

ID: FORM-IDI-S4-LICITACION-01
Field-Label: "Licitación y Adjudicación"
Field-Type: Group

- Field: "ID Licitación" (Text)
- Field: "Empresa Adjudicada" (Text)
- Field: "RUT Empresa Adjudicada" (Text)

#### Plazos y Terreno

ID: FORM-IDI-S4-PLAZOS-01
Field-Label: "Plazos y Terreno"
Field-Type: Group

- Field: "Acta Entrega Terreno" (Text)
- Field: "Plazo (días)" (Number)
- Field: "Aumento de Plazo (Paralización)" (Number)

### Sección 5: Responsables

ID: FORM-IDI-S5-RESPONSABLES-01

- Field: "Profesional Responsable Presupuesto" (Text)
- Field: "Profesional Responsable Iniciativa" (Text)
- Field: "División Vinculada" (Text)

### Sección 6: Ejecución Presupuestaria (Formato Normalizado)

ID: FORM-IDI-S6-EJECUCION-PPTAL-01
Field-Label: "Registros de Ejecución Presupuestaria"
Field-Type: List-of-Objects
Field-Instr: "Cada objeto representa un registro mensual, transformando el formato ancho original en uno largo y manejable."

#### Objeto: Registro Mensual

ID: FORM-IDI-S6-REGISTRO-MENSUAL-01

- Field: "Año" (Number: aaaa)
- Field: "Mes" (Select: Enero, Febrero, ...)
- Field: "Monto Proyectado" (Currency)
- Field: "Monto Real" (Currency)

#### Gasto Acumulado y Arrastre

ID: FORM-IDI-S6-ACUMULADO-01
Field-Label: "Gasto Acumulado y Arrastre"
Field-Type: Group

- Field: "Gasto Ejecutado Año" (Currency)
- Field: "Gasto a Ejecutar Año" (Currency)
- Field: "Arrastre Siguiente Año" (Currency)
