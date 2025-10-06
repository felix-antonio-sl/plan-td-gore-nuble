# Modelamiento de Procesos y Arquitectura GORE Ñuble

ID: PROC-GORE-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-10-06
Modification-Date: 2025-10-06
Source: `modelos c4 bpmn.md`
Ctx: Modelamiento de procesos (BPMN) y arquitectura de sistemas (C4) del Gobierno Regional de Ñuble.

---

BEGIN_LLM_INSTRUCTIONS

You are an AI agent consuming a Structured Telegraphic Style (STS) artifact. Your primary task is to parse and reason over THIS document with absolute fidelity, using only the rules defined below. This artifact is a self-contained source of truth.

1. **Core Objective**: Maintain perfect fidelity to the information (`meat`) and structure (`skeleton`). Do not summarize, interpret, or infer information not explicitly present. Prohib: Applying these rules to artifact creation or translation tasks; they are exclusively for consumption.

2. **Conceptual Metaphors**:
    * `meat`: Essential information, data, and facts. Must be preserved with zero loss.
    * `skeleton`: Logical structure (headers, IDs, lists, tables). This is also `meat` and must be preserved.
    * `fat`: Non-essential verbiage (filler words, rhetoric, stylistic prose). Must be ignored during reasoning as it has no informational value.

3. **Lexicon Mode & Expansion**: This document uses an **Abbreviated Lexicon**. You MUST treat the following keywords as valid and expand them according to this mapping before processing:
    * `Act:` -> `Action:`
    * `Warn:` -> `Warning:`
    * `Cause:` -> `Cause:`
    * `Cpt:` -> `Concept:`
    * `Cond:` -> `Condition:`
    * `Ctx:` -> `Context:`
    * `Def:` -> `Definition:`
    * `Dep:` -> `Dependency:`
    * `Dest:` -> `Destination:`
    * `Dln:` -> `Deadline:`
    * `Ex:` -> `Example:`
    * `Fnd:` -> `Foundation:`
    * `ID:` -> `ID:`
    * `Instr:` -> `Instruction:`
    * `Just:` -> `Justification:`
    * `Mech:` -> `Mechanism:`
    * `Mssn:` -> `Mission:`
    * `Mdl:` -> `Model:`
    * `Nat:` -> `Nature:`
    * `Obj:` -> `Objective:`
    * `Proc:` -> `Process:`
    * `Prohib:` -> `Prohibition:`
    * `Purp:` -> `Purpose:`
    * `Rec:` -> `Recommendation:`
    * `Ref:` -> `Reference:`
    * `Req:` -> `Requirement:`
    * `Res:` -> `Result:`
    * `Resp:` -> `Responsible:`
    * `Src:` -> `Source:`

4. **Reference (`Ref:`) Policy**:
    * `Ref:` is used for **internal cross-references only**.
    * It MUST point to an `ID:` that exists within THIS document.
    * You MUST NOT interpret a `Ref:` as a link to an external document or resource. Mentions of other documents are purely contextual (`Ctx:`).

5. **Language Invariance Policy**:
    * The `Keywords` in the lexicon are a fixed control vocabulary in English.
    * All `EssentialData` (the content following a `Keyword:`) MUST be preserved in its original language. Do not translate it.

END_LLM_INSTRUCTIONS

---

## 1. Especificación de Procesos (BPMN)

ID: PROC-GORE-BPMN-01
Purp: Sintetizar y modelar los procesos clave del GORE Ñuble utilizando notación BPMN.
Fnd: Documentación oficial del GORE Ñuble.
Ctx: El modelado resalta actores, actividades, flujos de decisión, documentos y controles.
Cpt: Procesos cubiertos.

* Cpt: Tramitación de actos administrativos.
* Cpt: Ciclo presupuestario.
* Cpt: Gestión de iniciativas de inversión.
* Cpt: Rendición de cuentas.

### 1.1. Tramitación y Aprobación de Actos Administrativos

ID: PROC-GORE-BPMN-TRAMITACION-01
Fnd: Principios de legalidad, probidad y transparencia.
Mech: Pasos secuenciales y roles específicos para asegurar control interno y toma de razón por Contraloría General de la República (CGR).
Cpt: Tipos de actos.

* Cpt: Resoluciones.
* Cpt: Decretos.
* Cpt: Convenios.

#### 1.1.1. Flujo General para Resoluciones Exentas

ID: PROC-GORE-BPMN-TRAMITACION-RES-EXENTAS-01
Ctx: Resoluciones sin compromiso presupuestario.

* Cpt: Fase de Iniciación.
  * Resp: Área requirente.
  * Act: Elaborar proyecto de resolución con antecedentes.
  * Act: Remitir a Unidad Jurídica (UJ).
* Cpt: Fase de Revisión Jurídica.
  * Resp: Unidad Jurídica (UJ).
  * Act: Realizar revisión jurídica.
  * Req: Asegurar cumplimiento de requisitos legales.
* Cpt: Fase de Gestión.
  * Resp: Centro de Gestión (secretaría).
  * Act: Controlar formalidades.
  * Act: Foliar documentos.
* Cpt: Fase de Control.
  * Resp: Unidad de Control.
  * Act: Visar por autoridad competente.
  * Req: Verificar legalidad y disponibilidad presupuestaria.
* Cpt: Fase de Firma y Notificación.
  * Resp: Secretaria o Secretario Regional Ministerial.
  * Act: Firmar la resolución.
  * Act: Notificar a interesados.
  * Act: Enviar a CGR para toma de razón.
    * Cond: Cuando corresponda.

* Cpt: Modelo BPMN.
  * Mdl: Pool "GORE Ñuble".
  * Mdl: Lanes para roles.
    * Resp: Área Requirente.
    * Resp: Unidad Jurídica.
    * Resp: Centro de Gestión.
    * Resp: Unidad de Control.
    * Resp: Secretario/a.
  * Mdl: Tareas de usuario (task).
    * Act: "Elaborar borrador".
    * Act: "Revisar legalidad".
    * Act: "Control de formalidades".
    * Act: "Revisar y visar".
    * Act: "Firmar".
  * Mdl: Flujo.
    * Cpt: Eventos intermedios para espera de revisión o firma.
    * Cpt: Gateway exclusivo para determinar si requiere toma de razón.
      * Cond: Si requiere toma de razón.
        * Proc: Se envía a CGR para control externo.
      * Cond: Si no requiere toma de razón.
        * Proc: Se notifica directamente.

#### 1.1.2. Aprobación de Transferencias y Convenios de Financiamiento

ID: PROC-GORE-BPMN-TRAMITACION-CONVENIOS-01
Ctx: Para transferencias a terceros.

* Proc:
  1. Emisión de acto administrativo.
     * Cpt: Decreto o Resolución.
  2. Elaboración de proyecto de convenio.
     * Resp: Área responsable.
     * Cpt: Antecedentes del convenio.
       * Cpt: Propósito.
       * Cpt: Monto.
       * Cpt: Plazos.
  3. Revisión jurídica.
     * Resp: Unidad Jurídica (UJ).
     * Act: Revisar texto del convenio.
  4. Firma de documentos.
     * Resp: Autoridad.
     * Act: Firmar convenio.
     * Act: Firmar decreto de aprobación.
  5. Envío a CGR para toma de razón.
  6. Firma con entidad beneficiaria.
     * Cond: Tras aprobación de CGR.
  7. Publicación.
     * Dest: Sistema de Transparencia.

* Cpt: Modelo BPMN.
  * Req: Tramitación de dos documentos paralelos (proyecto de convenio y decreto).
  * Mdl: Artefactos de datos para representar documentos.
  * Mdl: Subproceso para la tramitación en CGR.
  * Mdl: Gateway paralelo para sincronizar aprobación de convenio y decreto antes de la firma externa.

### 1.2. Ciclo Presupuestario Regional

ID: PROC-GORE-BPMN-CICLO-PRESUP-01
Fnd: Ley de presupuestos.
Cpt: Fases.

* Cpt: Formulación.
* Cpt: Aprobación.
* Cpt: Ejecución.
* Cpt: Modificación.
* Cpt: Control/Cierre.
Cpt: Actores Involucrados.
* Resp: Dirección de Planificación e Inversiones Regionales (DIPIR).
* Resp: Dirección de Administración y Finanzas (DAF).
* Resp: Gobernador/CORE.
* Resp: Organismos externos (DIPRES, CGR).

#### 1.2.1. Formulación del Presupuesto

ID: PROC-GORE-BPMN-CICLO-PRESUP-FORMULACION-01

* Proc:
  1. Elaboración de insumos.
     * Resp: DIPIR.
     * Act: Elaborar Anteproyecto Regional de Inversiones (ARI).
     * Act: Elaborar Programa Regional de Inversiones (PROPIR).
     * Src: Iniciativas de divisiones, municipios y servicios públicos.
     * Resp: DAF.
     * Act: Estimar ingresos y egresos corrientes.
  2. Consolidación y envío.
     * Act: Consolidar insumos en el Anteproyecto Regional.
     * Act: Enviar al Gobernador.
  3. Aprobación por Consejo Regional (CORE).
     * Act: Celebrar sesión del CORE para aprobar el proyecto.
     * Cond: Si existen observaciones.
       * Proc: Se incorpora una ronda de ajuste.

* Cpt: Modelo BPMN.
  * Mdl: Lanes para DIPIR y DAF.
  * Mdl: Gateway paralelo para juntar ARI y PROPIR.
  * Mdl: Gateway exclusivo para decisión del CORE.
    * Cond: No aprueba.
      * Proc: Retorna a DIPIR/DAF para ajustes.
    * Cond: Aprueba.
      * Proc: Pasa a fase de aprobación formal.

#### 1.2.2. Aprobación del Presupuesto

ID: PROC-GORE-BPMN-CICLO-PRESUP-APROBACION-01

* Proc:
  1. Remisión al CORE.
     * Cond: Una vez consolidado el proyecto.
     * Resp: Gobernador.
     * Dln: 10 días hábiles.
  2. Dictamen del CORE.
     * Dln: 10 días para dictaminar.
     * Cond: Si no responde.
       * Res: Se entiende aprobado.
  3. Envío a entidades externas.
     * Dest: Dirección de Presupuestos (DIPRES).
     * Dest: CGR.
     * Purp: Toma de razón y publicación.

* Cpt: Modelo BPMN.
  * Mdl: Evento temporizador de 10 días en el Gobernador.
  * Mdl: Evento temporizador de 10 días en el CORE.
  * Mdl: Gateway exclusivo para controlar resultado.
    * Cond: CORE aprueba.
      * Proc: Flujo continúa.
    * Cond: CORE no aprueba.
      * Proc: Se realizan correcciones.
    * Cond: CORE no se pronuncia.
      * Proc: Flujo avanza por default.

#### 1.2.3. Ejecución Presupuestaria

ID: PROC-GORE-BPMN-CICLO-PRESUP-EJECUCION-01
Cond: Tras la aprobación del presupuesto.

* Cpt: Actividades DAF.
  * Act: Registrar presupuesto en Sistema Integrado de Gestión Financiera (SIGFE).
  * Act: Realizar ajustes mensuales de caja.
  * Act: Ejecutar pagos según ley de compras.
* Cpt: Actividades DIPIR.
  * Act: Monitorear la ejecución física de los proyectos.
  * Act: Revisar avances en el Banco Integrado de Proyectos (BIP).
  * Act: Actualizar mensualmente la información a DIPRES.
* Cpt: Devengo de compromisos.
  * Cond: Convenios con municipalidades.
    * Mech: Se devenga al momento de la transferencia.
  * Cond: Convenios de ejecución.
    * Mech: Se devenga al devengar la transferencia.

* Cpt: Modelo BPMN.
  * Mdl: Subproceso de ciclo para procesos recurrentes mensuales.
  * Mdl: Tareas de DAF.
    * Act: "Registrar devengos".
    * Act: "Ejecutar pagos".
    * Act: "Actualizar SIGFE".
  * Mdl: Tareas de DIPIR.
    * Act: "Monitorear avances".
    * Act: "Validar rendiciones".
  * Mdl: Gateway exclusivo para decidir cumplimiento de programación.
    * Cond: Existen desviaciones.
      * Proc: Se genera un proceso de modificación.

#### 1.2.4. Modificación Presupuestaria

ID: PROC-GORE-BPMN-CICLO-PRESUP-MODIFICACION-01
Cpt: Tipos de modificaciones.

* Cpt: Suplementos.
* Cpt: Reasignaciones.
* Cpt: Traspasos entre subtítulos.
* Cpt: Fondos de emergencia.
Req: Cada tipo requiere actos distintos.
* Cond: Aprobación por decreto (firmado por gobernador, visado por DAF).
* Cond: Requiere acuerdo del CORE y toma de razón por CGR.
Proc:

1. Solicitud de la división.
2. Revisión de pertinencia en DAF/DIPIR.
3. Emisión del acto respectivo.
4. Obtención de aprobación del CORE (si corresponde).
5. Registro en SIGFE.

* Cpt: Modelo BPMN.
  * Mdl: Gateway exclusivo para determinar el tipo de modificación.
  * Mdl: Subproceso de aprobación para cada variante con firmas y visaciones necesarias.
  * Mdl: Eventos de mensaje para remisión al CORE y CGR.

#### 1.2.5. Control y Cierre

ID: PROC-GORE-BPMN-CICLO-PRESUP-CIERRE-01

* Cpt: Control Interno.
  * Resp: Unidad de Control.
  * Resp: DAF.
  * Resp: DIPIR.
  * Act: Verificar la legalidad de gastos y el cumplimiento de fines.
* Cpt: Control Externo.
  * Resp: DIPRES.
  * Resp: CGR.
* Proc: Cierre de ejercicio.
  * Resp: DAF.
    * Act: Consolidar la información.
    * Act: Cerrar las cuentas en SIGFE.
    * Act: Regularizar la deuda flotante.
    * Act: Elaborar un informe de cierre.
  * Resp: DIPIR.
    * Act: Evaluar los resultados físicos y financieros.
    * Act: Generar un informe de evaluación ex post.

* Cpt: Modelo BPMN.
  * Mdl: Evento de fin de tipo mensaje que envía informe de cierre a DIPRES y CGR.
  * Mdl: Subprocesos de auditoría y evaluación.

### 1.3. Gestión de Iniciativas de Inversión (IPR)

ID: PROC-GORE-BPMN-IPR-01
Purp: Gestionar el ciclo de vida de una iniciativa de inversión.
Cpt: Fases del ciclo.

* Cpt: Fase 1: Ingreso, pertinencia y admisibilidad.
* Cpt: Fase 2: Evaluación técnico-económica.
* Cpt: Fase 3: Obtención de financiamiento.
* Cpt: Fase 4: Formalización.
* Cpt: Fase 5: Ejecución y supervisión.
* Cpt: Fase 6: Modificaciones en ejecución.
* Cpt: Fase 7: Cierre técnico-financiero y evaluación ex post.

#### 1.3.1. Fase 1: Ingreso, Pertinencia y Admisibilidad

ID: PROC-GORE-BPMN-IPR-FASE1-01

* Proc:
  1. Ingreso de la iniciativa.
     * Resp: Proponente (municipio, servicio, otra división).
     * Mech: Vía SGDOC o mesa de partes.
  2. Asignación y derivación.
     * Act: Asignar un número.
     * Act: Derivar a DIPIR.
  3. Análisis de pertinencia.
     * Resp: DIPIR.
     * Req: Respecto a instrumentos de planificación.
     * Cond: Si corresponde.
       * Act: DIPIR declara la admisibilidad.
       * Act: Registrar proyecto en Banco Integrado de Proyectos (BIP).
     * Cond: Si no corresponde.
       * Act: Devolver al proponente con observaciones.

* Cpt: Modelo BPMN.
  * Mdl: Evento de inicio de mensaje.
  * Mdl: Gateway exclusivo para verificar pertinencia.
  * Mdl: Subproceso de registro en BIP se desencadena cuando se acepta.

#### 1.3.2. Fase 2: Evaluación Técnico-Económica

ID: PROC-GORE-BPMN-IPR-FASE2-01
Ctx: Dependiendo del tipo de inversión, existen distintos caminos.

* Cpt: Ruta Sistema Nacional de Inversiones (SNI).
  * Proc:
    1. Preparar perfil y evaluación social (RS) en MDSyF.
    2. DIPIR revisa antecedentes y solicita correcciones.
  * Res: Se obtiene recomendación satisfactoria (RS) o no satisfactoria (RNS).
* Cpt: Ruta Programas.
  * Ctx: Para iniciativas menores o transferencias.
  * Proc:
    1. Elaborar un proyecto simplificado.
    2. DIPIR revisa costos y cumplimiento de requisitos.
* Cpt: Ruta Simplificados.
  * Ctx: Para proyectos de bajo monto.
  * Proc: Se ejecuta una evaluación básica.
* Res: Cada ruta genera un resultado que habilita o no la búsqueda de financiamiento.

* Cpt: Modelo BPMN.
  * Mdl: Gateway inclusivo que dirige la iniciativa a la ruta SNI, programas o simplificada.
  * Mdl: Cada ruta es un subproceso con tareas.
    * Act: "Elaborar perfil".
    * Act: "Evaluar".
    * Act: "Obtener recomendación".

#### 1.3.3. Fase 3: Obtención de Financiamiento

ID: PROC-GORE-BPMN-IPR-FASE3-01
Cond: Con recomendación satisfactoria.

* Resp: DIPIR.
* Proc:
  1. Gestionar priorización y financiamiento.
  2. Ingresar iniciativa en el Programa de Inversión Regional (PROPIR).
  3. Coordinar con DIPIR y DAF para asignar recursos.
  4. Someter a aprobación del CORE.
* Cond: Si hay acuerdo del CORE.
  * Res: Se incorpora al presupuesto regional.
* Cond: Si no hay acuerdo del CORE.
  * Res: Se puede buscar financiamiento sectorial o retornar a etapa anterior.

* Cpt: Modelo BPMN.
  * Mdl: Gateway exclusivo para la decisión del CORE.
    * Cond: Aprueba.
      * Res: Se emite una resolución de asignación.
    * Cond: No aprueba.
      * Proc: Se considera búsqueda de fondos sectoriales o revaluación.

#### 1.3.4. Fase 4: Formalización

ID: PROC-GORE-BPMN-IPR-FASE4-01
Cond: Aprobado el financiamiento.

* Proc:
  1. Formalizar proyecto a través de un convenio GORE-ejecutor.
  2. UJ redacta el convenio.
  3. Autoridad lo firma.
  4. CGR toma razón.
  5. Publicación.
* Proc: Paralelamente.
  * Resp: DAF.
  * Act: Registrar compromiso en SIGFE.
  * Act: Transferir fondos según el convenio.

* Cpt: Modelo BPMN.
  * Mdl: Subproceso de tramitación de convenio. Ref: PROC-GORE-BPMN-TRAMITACION-CONVENIOS-01.
  * Mdl: Evento de mensaje para la transferencia de fondos.

#### 1.3.5. Fase 5: Ejecución y Supervisión

ID: PROC-GORE-BPMN-IPR-FASE5-01

* Proc:
  1. Ejecutor licita y ejecuta obras o adquisición.
  2. DIPIR y unidad sectorial hacen monitoreo técnico.
  3. DAF verifica rendiciones y pagos.
* Cpt: Hitos utilizados.
  * Cpt: "Inicio de obra".
  * Cpt: "Entrega de avance".
  * Cpt: "Recepción provisoria".
* Cond: Si surgen modificaciones.
  * Proc: Se inicia la Fase 6.

* Cpt: Modelo BPMN.
  * Mdl: Subproceso de ejecución con bucles de control de avance.
  * Mdl: Gateway exclusivo para determinar si el avance es conforme.
    * Cond: No es conforme.
      * Proc: Se genera una orden de cambio o se suspende el proyecto.

#### 1.3.6. Fase 6: Modificaciones en Ejecución

ID: PROC-GORE-BPMN-IPR-FASE6-01
Cond: Se requieren cambios durante la ejecución (aumento de plazo, incremento de monto).

* Proc:
  1. Ejecutor solicita una modificación.
  2. DIPIR y UJ analizan la pertinencia.
  3. CORE aprueba si corresponde.
  4. Se emite un acto modificatorio.
  5. Se actualizan los registros.

* Cpt: Modelo BPMN.
  * Mdl: Subproceso que replica el flujo de Fase 4. Ref: PROC-GORE-BPMN-IPR-FASE4-01.
  * Mdl: Gateway exclusivo que decide la aprobación del CORE.

#### 1.3.7. Fase 7: Cierre Técnico-Financiero y Evaluación Ex Post

ID: PROC-GORE-BPMN-IPR-FASE7-01
Cond: Finalizadas las obras.

* Proc:
  1. Se realiza la recepción definitiva.
  2. Entidad ejecutora rinde cuentas finales.
  3. DAF revisa y aprueba la rendición.
  4. DIPIR elabora una evaluación ex post.
     * Ctx: Sobre cumplimiento de objetivos y efectividad del gasto.
  5. Se archivan documentos.
  6. Se informan los resultados a DIPRES y CGR.

* Cpt: Modelo BPMN.
  * Mdl: Eventos de fin múltiple (cierre financiero, cierre técnico).
  * Mdl: Tarea manual para representar la recepción de obras.
  * Mdl: Tarea de usuario para representar la revisión de rendiciones.

### 1.4. Gestión de Rendiciones de Cuentas

ID: PROC-GORE-BPMN-RENDICION-01
Purp: Asegurar que los recursos de transferencias a terceros se utilicen según el convenio.
Cpt: Modalidades.

* Cpt: Tradicional (sin SISREC).
* Cpt: Actual (usando SISREC).

#### 1.4.1. Proceso Tradicional sin SISREC

ID: PROC-GORE-BPMN-RENDICION-TRADICIONAL-01

* Proc:
  1. Ejecución y recepción de rendición.
     * Resp: Beneficiario.
     * Act: Ejecutar la iniciativa y enviar la rendición a Oficina de Partes del GORE.
  2. Registro.
     * Resp: Oficina de Partes.
     * Act: Registrar el ingreso y derivar a la Unidad de Contabilidad y Rendiciones (UCR).
  3. Revisión UCR.
     * Resp: UCR.
     * Act: Revisar la documentación y solicitar correcciones si procede.
  4. Informe técnico-financiero (RTF).
     * Resp: DIPIR.
     * Act: Emitir un RTF considerando aspectos técnicos y cumplimiento de metas.
  5. Resolución de aprobación.
     * Resp: Autoridad.
     * Act: Emitir acto que aprueba o rechaza la rendición.
     * Act: Ordenar el archivo o devolución de fondos.

* Cpt: Modelo BPMN.
  * Mdl: Evento de inicio de mensaje para la entrega de la rendición.
  * Mdl: Tareas de "Registrar", "Revisar" y "Emitir RTF".
  * Mdl: Gateway exclusivo que evalúa si la rendición es aceptada.
    * Cond: Se rechaza.
      * Proc: Se solicita subsanación o devolución de fondos.

#### 1.4.2. Proceso SISREC (Plataforma Digital)

ID: PROC-GORE-BPMN-RENDICION-SISREC-01
Ctx: El proceso se divide entre la Entidad Ejecutora (EE) y el GORE.

* Cpt: Actividades Entidad Ejecutora.
  * Act: Aceptar el proyecto en SISREC.
  * Act: Ingresar la rendición con respaldo de gastos.
  * Act: Enviar la rendición al GORE.
  * Resp: Ministro de fe.
    * Act: Revisar internamente la rendición antes de su envío.
* Cpt: Actividades GORE.
  * Resp: Analista de Rendiciones.
    * Act: Crear el proyecto en SISREC.
    * Act: Revisar la rendición y generar observaciones.
  * Resp: Jefa de División (Autoridad).
    * Act: Aprobar o rechazar la rendición.
  * Resp: Contabilidad.
    * Act: Registrar los movimientos y archivar.

* Cpt: Modelo BPMN.
  * Mdl: Dos pools (Entidad Ejecutora y GORE).
  * Mdl: Tareas de EE.
    * Act: "Ingresar rendición".
    * Act: "Adjuntar respaldo".
    * Act: "Solicitar validación interna".
  * Mdl: Tareas GORE.
    * Act: "Crear proyecto en SISREC".
    * Act: "Revisar rendición".
    * Act: "Corregir observaciones".
    * Act: "Firmar".
    * Act: "Contabilizar".
  * Mdl: Eventos de mensaje para modelar intercambios.

### 1.5. Conclusión y Recomendaciones BPMN

ID: PROC-GORE-BPMN-CONCLUSION-01

* Cpt: Características de los procesos GORE Ñuble.
  * Nat: Secuencias claras.
  * Nat: Múltiples actores.
  * Nat: Controles normativos.
* Rec: Para modelarlos eficazmente en BPMN.
  * Rec: Definir pools para cada organismo (GORE Ñuble, Entidad Ejecutora, Contraloría, CORE).
  * Rec: Definir lanes para unidades internas (DIPIR, DAF, UJ, Oficina de Partes).
  * Rec: Utilizar subprocesos para etapas repetitivas (revisión de convenios, evaluaciones).
  * Rec: Utilizar gateways para decisiones (aprobado/no aprobado, requiere CORE, etc.).
  * Rec: Incorporar eventos temporizadores para respetar plazos legales.
  * Rec: Representar artefactos de datos (convenios, resoluciones, informes) para trazar la documentación.
* Res: Esta especificación sirve de base para diseñar diagramas BPMN que reflejen la complejidad administrativa y permitan identificar mejoras.

## 2. Aproximación al Modelamiento C4

ID: PROC-GORE-C4-01
Purp: Presentar la especificación textual C4 – Nivel 1 (Contexto del Sistema) para el GORE Ñuble.
Fnd: Artefactos adjuntos.
Obj: Fijar límites, actores, sistemas externos y relaciones clave que condicionan la arquitectura.

### 2.1. Sistema en Foco (Software System)

ID: PROC-GORE-C4-SISTEMA-01

* Cpt: Nombre (propuesto para modelado).
  * Def: Plataforma de Gestión del GORE Ñuble.
* Cpt: Descripción.
  * Def: Sistema institucional que soporta el ciclo presupuestario regional, la gestión de Intervenciones Públicas Regionales (IPR), la tramitación y firma de actos administrativos en expediente electrónico y la rendición de cuentas.
* Cpt: Integraciones.
  * Dep: Opera en integración con plataformas transversales del Estado (SIGFE, BIP/SNI, SISREC, DocDigital, Red de Interoperabilidad, ChileCompra).
* Cpt: Supervisión Externa.
  * Resp: Control externo de DIPRES y CGR.
  * Resp: Evaluación técnica de MDSF para proyectos SNI.
* Cpt: Límites Institucionales de Alto Nivel.
  * Def: El GORE es la administración superior de la región con misión de desarrollo regional.
  * Prohib: El gobierno interior (orden público/seguridad) no forma parte del alcance del sistema en foco.
  * Ctx: El rol de gobierno interior recae en el Delegado Presidencial; es una relación de coordinación.

### 2.2. Personas (Actores) y Objetivos

ID: PROC-GORE-C4-ACTORES-01

#### 2.2.1. Internos al GORE (Usuarios Primarios)

ID: PROC-GORE-C4-ACTORES-INTERNOS-01

* Cpt: Gobernador/a Regional.
  * Resp: Firma ejecutiva final de actos administrativos.
  * Resp: Propone presupuesto y planes al CORE.
* Cpt: Consejo Regional (CORE).
  * Resp: Aprueba presupuesto regional, distribución de fondos e inversiones (FNDR, 8%, FRIL).
  * Resp: Fiscaliza la gestión.
* Cpt: Administrador/a Regional.
  * Resp: Coordina gestión administrativa interna.
  * Resp: Ejerce VºBº previo a firmas del Gobernador.
* Cpt: DAF (División de Administración y Finanzas).
  * Resp: Ejecuta gestión financiera/contable.
  * Resp: Registra operaciones en SIGFE.
  * Resp: Gestiona pagos y rendiciones.
* Cpt: DIPIR (División de Presupuesto e Inversión Regional).
  * Resp: Lidera inversión.
  * Resp: Evalúa técnicamente IPR de tipo proyecto.
  * Resp: Gestiona BIP y cartera ARI/PROPIR.
* Cpt: DIPLADE (Planificación y Desarrollo).
  * Resp: Lidera ERD.
  * Resp: Secretaría ejecutiva de la coordinación del gasto (ARI/PROPIR).
* Cpt: Asesoría Jurídica y Unidad de Control.
  * Resp: Control preventivo de legalidad.
  * Resp: Auditoría selectiva de procesos.
* Cpt: Oficina de Partes.
  * Resp: Punto único de ingreso formal.
  * Resp: Registra y deriva documentación.
* Cpt: Comité Directivo Regional (CDR).
  * Resp: Filtro político–técnico de IPR antes de evaluación.
* Cpt: Referente Técnico-Financiero (RTF).
  * Resp: Primera línea de revisión y seguimiento técnico/financiero de convenios y rendiciones.

#### 2.2.2. Externos al GORE (Actores del Entorno)

ID: PROC-GORE-C4-ACTORES-EXTERNOS-01

* Cpt: CGR (Contraloría General de la República).
  * Resp: Control externo, toma de razón, fiscalización.
  * Ctx: Propietario de SISREC, obligatorio para rendiciones.
* Cpt: DIPRES (Hacienda).
  * Resp: Monitorea ejecución vía SIGFE.
  * Resp: Visa modificaciones.
  * Resp: Evalúa ex ante programas (Glosa 06).
* Cpt: MDSF / SEREMI.
  * Resp: Evaluación técnica SNI para proyectos (RATE/RS).
* Cpt: ChileCompra.
  * Ctx: Mercado Público para contratación pública.
* Cpt: Municipalidades, servicios públicos y entidades privadas.
  * Resp: Ejecutores de transferencias (p.ej. FRIL, 8% FNDR, FRPD).
  * Resp: Rendidores en SISREC.
* Cpt: SEREMI de Seguridad Pública / Consejos Regionales de Seguridad.
  * Ctx: Coordinación para iniciativas de prevención; no subordinación al GORE.

### 2.3. Sistemas Externos y Plataformas Transversales

ID: PROC-GORE-C4-SISTEMAS-EXTERNOS-01

* Cpt: SIGFE (Sistema de Información para la Gestión Financiera del Estado).
  * Purp: Sistema contable–presupuestario transaccional.
  * Mech: DAF registra preafectación, compromiso, devengo, pago y reporta a DIPRES.
* Cpt: BIP / SNI (Banco Integrado de Proyectos / Sistema Nacional de Inversiones).
  * Purp: Registro y seguimiento de proyectos de inversión.
  * Req: Requisito para evaluación MDSF y obtención de RS.
* Cpt: SISREC (CGR).
  * Purp: Plataforma obligatoria de rendición electrónica para transferencias subtítulos 24 y 33.
  * Mech: Flujo con firma electrónica avanzada y posterior contabilización en SIGFE.
* Cpt: DocDigital / Notificador.
  * Purp: Soporta comunicaciones y expediente electrónico.
  * Fnd: Conforme Ley 21.180 y sus normas técnicas.
* Cpt: Red de Interoperabilidad del Estado.
  * Req: Exigida por DS Nº12 (Interoperabilidad) para intercambio de datos entre OAE.
* Cpt: ClaveÚnica.
  * Purp: Autenticación unificada para personas.
  * Fnd: Alineamiento con DS Nº9 (Autenticación).
* Cpt: ChileCompra.
  * Purp: Mercado Público para compras y contrataciones.
* Warn: Nota de límite.
  * Ctx: SIGFE, BIP, SISREC, DocDigital, Red de Interoperabilidad y ChileCompra no son componentes internos del GORE; son sistemas externos con los que el sistema en foco se integra obligatoriamente.

### 2.4. Relaciones Clave

ID: PROC-GORE-C4-RELACIONES-01
Ctx: Texto estilo C4.

* Rel: DAF ⇄ SIGFE.
  * Purp: Registrar ejecución financiera; programar caja; emitir reportes a DIPRES; cerrar y devengar.
* Rel: DIPIR ⇄ BIP/SNI ⇄ SEREMI MDSF.
  * Purp: Carga y seguimiento de proyectos; obtención de RS/AD; conciliación con ejecución financiera en SIGFE.
* Rel: RTF/DAF ⇄ SISREC ⇄ Ejecutores.
  * Purp: Recepción, revisión, observación y aprobación de rendiciones; informe firmado con FEA; contabilización en SIGFE.
* Rel: Gobernador/Administrador/Asesoría ⇄ DocDigital/Expediente y FEA.
  * Purp: Tramitación y firma de resoluciones/decretos en expediente electrónico único.
* Rel: GORE ⇄ DIPRES/CGR.
  * Purp: Visación y toma de razón de actos presupuestarios; control y fiscalización externa continua.
* Rel: GORE ⇄ ChileCompra.
  * Purp: Contratación pública para adquisiciones y servicios.
* Rel: GORE ⇄ Red de Interoperabilidad / ClaveÚnica / Notificador.
  * Purp: Intercambio de datos, autenticación y notificaciones electrónicas conforme Normas Técnicas TDE.

### 2.5. Flujos de Negocio de Alto Nivel

ID: PROC-GORE-C4-FLUJOS-01
Ctx: Vista contextual.

* Cpt: Ciclo Presupuestario (anual).
  * Proc: Formulación (DIPIR/DAF) → Aprobación/Distribución (propuesta Gobernador, aprobación CORE; visación DIPRES; toma de razón CGR) → Ejecución (DAF en SIGFE; DIPIR en BIP) → Modificaciones (aprobación CORE, controles DIPRES/CGR) → Cierre.
* Cpt: Gestión de IPR (proyectos/programas).
  * Proc: Fase 1 Ingreso/pertinencia/admisibilidad (Of. Partes, CDR, DIPIR) → Fase 2 Evaluación técnica (SNI para proyectos; ex ante DIPRES para programas) → Aprobación CORE/actos administrativos → Ejecución y seguimiento → Cierre.
* Cpt: Rendición de cuentas (transferencias S.24/S.33).
  * Proc: Ejecutor carga en SISREC → RTF revisa → Jefatura DAF firma informe (FEA) → DAF contabiliza en SIGFE.
  * Warn: CGR es órgano rector y puede iniciar juicio de cuentas.
  * Prohib: No se entregan nuevos fondos si hay rendiciones exigibles pendientes.

### 2.6. Requisitos y Restricciones no Funcionales

ID: PROC-GORE-C4-REQUISITOS-NO-FUNCIONALES-01
Ctx: Marco de cumplimiento.

* Req: Escrituración y expediente electrónicos; FEA. (Ley 21.180; DS 4/2020; NT de documentos/expedientes).
* Req: Autenticación e interoperabilidad. (Uso de ClaveÚnica y Red de Interoperabilidad; DS 9 y DS 12).
* Req: Notificaciones electrónicas. (Reglas de cómputo y práctica; DS 8).
* Req: Probidad, transparencia, legalidad y control. (Principios y jerarquía normativa de la Administración).
* Req: Protección de datos personales. (Principios de licitud, finalidad, proporcionalidad y seguridad).

### 2.7. Alcances y Exclusiones

ID: PROC-GORE-C4-ALCANCE-01
Ctx: Frontera de contexto.

* Cpt: Incluye.
  * Cpt: Gestión presupuestaria regional.
  * Cpt: IPR (proyectos SNI y programas Glosa 06).
  * Cpt: Expedientes y firma electrónica.
  * Cpt: Rendiciones SISREC.
  * Cpt: Integración con SIGFE, BIP, DocDigital, Red de Interoperabilidad, ChileCompra.
* Cpt: Excluye.
  * Cpt: Gobierno interior/seguridad pública (rol del DPR y SEREMI de Seguridad).
  * Cpt: Operación orgánica de SIGFE/BIP/SISREC/ChileCompra (son sistemas de terceros).

### 2.8. Diccionario Mínimo

ID: PROC-GORE-C4-DICCIONARIO-01
Purp: Para coherencia C4.

* Def: IPR. Ctx: Intervención Pública Regional (proyecto, programa, estudio).
* Def: IDI/Proyecto SNI. Ctx: Iniciativa de inversión evaluada por MDSF, con resultado RATE/RS.
* Def: PPR/Programa (Glosa 06). Ctx: Oferta programática del GORE con evaluación ex ante DIPRES.
* Def: FNDR/FRIL/FRPD/8%. Ctx: Fondos/Instrumentos de inversión/subvención regulados por Ley de Presupuestos.
* Def: FEA. Ctx: Firma Electrónica Avanzada aplicable a actos y rendiciones.

### 2.9. Mapa Contextual

ID: PROC-GORE-C4-MAPA-01
Ctx: Resumen textual.

* Cpt: Personas (internas) → Plataforma de Gestión del GORE Ñuble.
  * Resp: Gobernador, CORE, Administrador, DAF, DIPIR, DIPLADE, Jurídica, Control, Oficina de Partes, CDR, RTF.
* Cpt: Sistemas externos ←→ Plataforma (integraciones obligatorias).
  * Cpt: SIGFE, BIP/SNI, SISREC, DocDigital/Notificador, Red de Interoperabilidad, ClaveÚnica, ChileCompra.

### 2.10. Observaciones para Capa Siguiente (C4-N2)

ID: PROC-GORE-C4-OBSERVACIONES-N2-01

* Rec: En N2 (Contenedores) convendrá separar.
  * Rec: Gestión Presupuestaria (interfaz SIGFE).
  * Rec: Portafolio IPR (interfaz BIP).
  * Rec: Rendiciones (interfaz SISREC).
  * Rec: Gestión de Actos y Expedientes (DocDigital/FEA).
  * Rec: Interoperabilidad/Notificaciones/Autenticación (DS 12/8/9).
  * Rec: Contratación (ChileCompra).
* Rec: Mantener los puntos de control de DIPRES y CGR como relaciones externas con *veto points*.
