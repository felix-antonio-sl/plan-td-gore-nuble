# Gestión Financiera y Administrativa Interna

Estos artefactos norman los procesos internos del GORE, asegurando el correcto flujo de aprobaciones, la gestión presupuestaria y la rendición de cuentas.

## Guía de Gestión Financiera y Operativa del Presupuesto Regional

### Metadata

ID: GUIDE-STS-MASTER-01
Version: 1.0.0
Status: Published
Human-Creator: Félix Sanhueza
Human-Editor: FSA
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-05-26
Modification-Date: 2024-07-28
Primary-Source: knowledge/domains/gore_nuble/kb_018_gestion_prpto.md
Ref-STS-Guide: GUIDE-STS-MASTER-01

### Presentación

Asunto: Guía técnico-operativa para gestión completa de presupuesto en GORE.
Purp: Proveer marco de referencia para la gestión presupuestaria regional.
Dest: Jefaturas División Administración y Finanzas (DAF) y División Presupuesto e Inversión Regional (DIPIR).

### GORE-FIN-CTX-01: Contexto General y Marco Normativo

ID: GORE-FIN-CTX-INTRO-01
Purp: Establecer el propósito, alcance y marco normativo de la guía.
Req: Claridad operativa y precisión técnica para gestión diaria.
Cpt: Aborda ciclo presupuestario completo (formulación -> cierre).
Fnd:

- D.F.L. N°1-19.175 (LOC GORE)
- D.L. N°1.263/1975 (Adm. Financiera Estado)
- Ley de Presupuestos del Sector Público (anual, ej. Ley 21.722 para 2025)
- Normas DIPRES (ej. Of. Circulares, instructivos de ejecución)
- Normas Contraloría General de la República (CGR) (ej. Res. N°7/2019, instructivos)
- Cpt: Principio-Jerarquia: Ley > Decreto > Resolución > Oficio Circular > Instructivo.

ID: GORE-FIN-CTX-CAMBIOS-2025-01
Asunto: Cambios estructurales en presupuesto GORE desde 2025.
Src: Of. Circ. N°11 DIPRES 2025.
Cpt:

- Cambio-1: Creación de 16 programas presupuestarios (uno por región).
  - Cpt: Integran recursos de funcionamiento e inversión en un solo programa.
- Cambio-2: Creación de programa especial "Asociatividad y Planes Especiales".
  - Purp: Financiar iniciativas de asociatividad regional, planes de zonas extremas y territorios rezagados.
Cause: Proceso de descentralización fiscal.
Res: Requiere coordinación estrecha DAF-DIPIR.
Ctx:
- Crecimiento de oferta programática regional (ejecución directa o transferencias).
  - Cpt: Incluye 8% FNDR, programas Glosa 06.
  - Cpt: Complementa inversión tradicional en proyectos (SNI).
- Dualidad de Gestión: GORE debe manejar dos sistemas paralelos:
  - Sistema Nacional de Inversiones (SNI) para proyectos de inversión.
  - Evaluación ex-ante (DIPRES/MDSF) para programas públicos.

### GORE-FIN-CONCEPTOS-FUNDAMENTALES-01: Conceptos Presupuestarios Fundamentales

ID: GORE-FIN-CONCEPTOS-INTRO-01
Purp: Establecer conceptos básicos del sistema presupuestario chileno para contextualizar la gestión GORE.
Src: DL N° 1.263/1975, Decreto N° 854/2004 Hacienda.

#### GORE-FIN-CONCEPTOS-PUP-01: El Presupuesto del Sector Público

ID: GORE-FIN-CONCEPTOS-PUP-DEF-01
Def: Estimación financiera de ingresos y gastos del sector público para un año, compatibilizando recursos disponibles con metas y objetivos preestablecidos.
Fnd: Art. 11, DL N° 1.263/1975.
Nat: Instrumento de política fiscal que refleja prioridades de gobierno y gestión.
Cpt: Jurídica (Ley), técnica (clasificadores), contable (recursos financieros).

ID: GORE-FIN-CONCEPTOS-PUP-PRINCIPIOS-01
Asunto: Principios rectores del presupuesto público.
Cpt:

- Principio-Universalidad: Todos los ingresos y gastos del Estado deben reflejarse en el presupuesto.
  - Fnd: Art. 4°, DL N° 1.263/1975.
- Principio-Anualidad: El ejercicio presupuestario coincide con el año calendario.
  - Fnd: Art. 12, DL N° 1.263/1975.

#### GORE-FIN-CONCEPTOS-CLASIFICADORES-01: Clasificaciones Presupuestarias

ID: GORE-FIN-CONCEPTOS-CLAS-INTRO-01
Asunto: Sistema de ordenamiento de la información presupuestaria.
Fnd: Decreto N° 854, de 2004, del Ministerio de Hacienda.
Cpt: Funciones Clave

- Proporcionar información para la toma de decisiones.
- Vincular proceso presupuestario con planificación del sector público.
- Posibilitar control de eficiencia en el uso de recursos públicos.
Fnd: Art. 16, DL N° 1.263/1975.
Cpt: Tipos Principales: Institucional, Objeto o Naturaleza, Grado de Afectación.

ID: GORE-FIN-CONCEPTOS-CLAS-INST-01: Clasificación Institucional
Purp: Agrupar presupuestariamente los organismos incluidos en la Ley de Presupuestos.
Cpt: Estructura Jerárquica

- Partida: Nivel superior de agrupación.
  - Cpt: Asignación: Presidencia, Congreso Nacional, Poder Judicial, CGR, Ministerio Público, Ministerios y Partida 50 "Tesoro Público".
  - Ex: Partida 31 - Gobiernos Regionales.
- Capítulo: Subdivisión de la Partida.
  - Cpt: Asignación: Corresponde a cada organismo con presupuesto directo en la Ley.
  - Ex: Un capítulo por cada uno de los 16 Gobiernos Regionales.
- Programa: División presupuestaria de los Capítulos.
  - Cpt: Asignación: Relacionado con funciones u objetivos específicos.
  - Ex:
    - Programa 01: Funcionamiento.
    - Programa 02: Inversión Regional.
    - Programa 03: Asociatividad y Planes Especiales.

ID: GORE-FIN-CONCEPTOS-CLAS-OBJ-01: Clasificación por Objeto o Naturaleza
Purp: Ordenar las transacciones según su origen (ingresos) o destino (gastos).
Cpt: Estructura Jerárquica

- Subtítulo: Agrupación de operaciones de naturaleza homogénea.
  - Ex: Gasto: 21 (Gastos en Personal), 22 (Bienes y Servicios de Consumo), 33 (Transferencias de Capital).
  - Ex: Ingreso: 08 (Otros Ingresos Corrientes), 09 (Aporte Fiscal), 15 (Saldo Inicial de Caja).
- Ítem: Representa un "motivo significativo" de ingreso o gasto.
  - Ex: Dentro de Subtítulo 21, Ítem 01 "Personal de Planta", Ítem 02 "Personal a Contrata".
- Asignación: Corresponde a un "motivo específico" del ingreso o gasto.
  - Ex: Dentro de Ítem 22.04 "Materiales de Uso o Consumo", Asignación 001 "Materiales de Oficina".
- Sub-asignación: Subdivisión de la asignación en conceptos más particulares.
  - Ex: Dentro de Asignación 21.01.001 "Sueldos y Sobresueldos", Sub-asignación 001 "Sueldos Bases".

ID: GORE-FIN-CONCEPTOS-CLAS-AFECT-01: Clasificación por Grado de Afectación Presupuestaria
Purp: Registrar y controlar las instancias previas al devengo en la ejecución del presupuesto.
Obj: Conocer el avance en la aplicación de los recursos.
Cpt: Etapas

1. Preafectación: Intenciones de gasto sin obligación a terceros.
   - Ex: Llamados a licitación, solicitudes de cotización.
2. Afectación: Obligación sujeta a perfeccionamiento.
   - Ex: Adjudicación de contrato, selección de proveedor.
3. Compromiso Cierto: Obligación recíproca con un tercero.
   - Ex: Emisión de Orden de Compra, firma de contrato, resolución de nombramiento.
4. Compromiso Implícito: Gasto y devengo ocurren simultáneamente.
   - Ex: Servicios básicos (agua, luz), peajes.

### GORE-FIN-CICLO-PRESUP-01: Ciclo Presupuestario: Etapas y Responsabilidades

ID: GORE-FIN-CICLO-ETAPAS-01
Purp: Describir las etapas del ciclo presupuestario y los roles de DAF y DIPIR.
Cpt: Etapas

1. Formulación
2. Aprobación / Distribución Inicial
3. Ejecución
4. Modificaciones
5. Control y Seguimiento
6. Cierre
Resp:

- Rol General DAF: Financiero-administrativo.
- Rol General DIPIR: Estratégico-programático de inversión.
- Cpt: Roles complementarios.

#### GORE-FIN-CICLO-FORMULACION-01: Formulación Presupuestaria

ID: GORE-FIN-FORM-ROL-DIPIR-01
Resp: DIPIR lidera elaboración de proyecto de presupuesto GORE.
Ctx: Foco en inversión regional y oferta programática.
Cpt: Tareas de Inversión

- Elaborar proyecto presupuesto de inversiones.
- Asesorar a Gobernador en selección de proyectos.
- Coordinar Anteproyecto Regional de Inversiones (ARI) y Programa de Inversión Regional (PROPIR). Ref: GORE-FIN-FORM-ARI-PROPIR-01
- Recopilar iniciativas de servicios públicos (ej. plataforma Chileindica).
- Asegurar alineación con Estrategia Regional de Desarrollo (ERD).
- Req: Coordinación con División de Planificación y Desarrollo Regional (DIPLADE).

ID: GORE-FIN-FORM-ROL-DIPIR-PROGRAMAS-01
Cpt: Tareas de Oferta Programática

- Diseñar programas públicos a ejecutar por GORE.
- Req: Metodología de Marco Lógico.
- Preparar antecedentes para evaluación ex-ante.
- Resp: Entes Evaluadores: DIPRES y Ministerio de Desarrollo Social y Familia (MDSF).
- Fnd: Glosa 06 Ley Presupuestos, Of. Circ. N°22 DIPRES. Ref: GORE-FIN-INSTR-PROGDIR-EVAL-EXANTE-01.
- Req: Identificar programas "nuevos o sustancialmente reformulados" para evaluación obligatoria.
- Req: Coordinación con DIPLADE y otras divisiones técnicas.

ID: GORE-FIN-FORM-ROL-DAF-01
Resp: DAF aporta información financiera y administrativa.
Cpt: Tareas de Funcionamiento

- Proyectar gastos de funcionamiento (Subt. 21, 22).
- Cpt: Base de Cálculo: Dotación vigente, gastos recurrentes.
- Req: Cumplir restricciones legales (gasto personal, viáticos). Ref: Art. 4 Ley 21.722.
Cpt: Tareas de Clasificación
- Verificar correcta aplicación de clasificador presupuestario (Decreto N°854/2004 Hacienda).
- Ctx: Nivel de detalle: Subtítulo, ítem y asignación (especialmente en transferencias Subt. 24, 33).
- Cpt: Principio Rector: Legalidad del gasto.

ID: GORE-FIN-FORM-COORDINACION-01
Resp: Compartida entre DIPIR y DAF.
Cpt: Tareas de Glosas

- Identificar y explicitar glosas aplicables.
- Ex: Dotaciones máximas de personal, límites de gasto. Ref: Glosas Partida 31, Ley Presupuestos 2025.
Cpt: Tareas de Provisiones
- Prever creación de provisiones específicas.
- Ex: Provisión para Fondo Regional de Productividad y Desarrollo (FRPD) en ítem 33.03.
- Ref: GORE-FIN-GLOSAS-FRPD-01
Cpt: Tareas de Justificación de Inversiones
- Justificar técnica y socialmente inversiones propuestas.
- Resp: DIPIR coordina con MDSyF para obtención de Recomendación Satisfactoria (RS).
- Cond: RS es requisito para inclusión en presupuesto (salvo excepciones como FRIL). Ref: Art. 19 bis DL 1.263.
- Req: Todos los proyectos de inversión deben estar en el Sistema Nacional de Inversiones (SNI) con código BIP.
- Ctx: Código BIP es fundamental para formulación y seguimiento físico-financiero.
- Ref: GORE-FIN-HERRAM-BIP-01

ID: GORE-FIN-FORM-ARI-PROPIR-01
Asunto: Coordinación Regional del Gasto Público: ARI y PROPIR.
Src: Instructivo Coordinación Gasto Público ARI 2026 y PROPIR 2025.
Def:

- ARI: Anteproyecto Regional de Inversiones. Estimación de inversión de GORE, ministerios y servicios en la región para el año siguiente.
- PROPIR: Programa Público de Inversión en la Región. Planificación, coordinación y seguimiento del gasto público a realizar en la región en el año en curso.
Mech: Ambas se gestionan en <www.chileindica.cl>. Ref: GORE-FIN-HERRAM-CHILEINDICA-01
Resp: GORE
- Gobernador conduce el proceso. Puede delegar en Jefe DIPLADE.
- DIPLADE conforma y lidera Secretaría Ejecutiva de la Coordinación Regional del Gasto Público.
  - Cpt: Integrantes: SEREMIs y Jefes de Servicios Regionales.
  - Act: Admite iniciativas en la plataforma Chileindica.
  - Act: Fija plazo para postulación ARI (no exceder primeros 4 meses del año).
- GORE presenta informe trimestral de ejecución PROPIR al CORE.
- GORE envía ARI aprobado por CORE a ministerios para su consideración en formulación presupuestaria.
Resp: Servicios Públicos
- Ingresar y gestionar iniciativas en Chileindica para PROPIR y ARI.
  - Req: Desglose comunal, montos, fuente, beneficiarios, alineación con ERD.
- Informar ejecución financiera mensual de PROPIR.
- Informar si no tienen inversión para ARI/PROPIR vía oficio en primeros 60 días.
Proc: Proceso de Discrepancias

1. Instancia Regional: Resolución a nivel regional.
2. Nivel Central: Si persisten, se tratan en Comisiones Técnicas de formulación presupuestaria con autoridades nacionales.

#### GORE-FIN-CICLO-APROBACION-01: Aprobación y Distribución Inicial

ID: GORE-FIN-APROB-PROCEDIMIENTO-01
Asunto: Procedimiento legal para aprobación de presupuesto inicial GORE.
Src: Glosa 01 Partida 31 Ley 21.722; Instructivo CGR Aprobación Presupuesto Inicial 2025.
Proc: Fases y Plazos

1. Propuesta Gobernador: Gobernador elabora y somete a CORE la distribución inicial de presupuestos.
   - Dln: 10 días corridos desde publicación Ley de Presupuestos.
2. Aprobación CORE: CORE se pronuncia sobre la propuesta.
   - Dln: 10 días corridos desde recepción.
3. Envío DIPRES: Gobernador remite distribución aprobada por CORE a DIPRES.
   - Dln: 5 días corridos post-aprobación CORE.
4. Elaboración Resoluciones DIPRES: DIPRES elabora resoluciones de presupuesto de funcionamiento e inversión.
   - Dln: 10 días desde recepción.
5. Toma de Razón CGR: Resoluciones deben ser tomadas de razón por CGR para entrar en vigencia.
   - Dln: 15 días desde recepción (prorrogable por 15 más).

ID: GORE-FIN-APROB-CONTENIDO-01
Asunto: Contenido y requisitos de la propuesta de presupuesto inicial.
Src: Instructivo CGR Aprobación Presupuesto Inicial 2025.
Req: Generales

- Desagregación conforme a clasificador presupuestario, a nivel de subtítulo e ítem.
- Desagregación de transferencias a nivel de asignación (Subt. 24, 33).
- Clasificaciones deben corresponder a naturaleza del gasto y receptor (Legalidad del Gasto).
- Cuadratura de ingresos y gastos con montos de Ley de Presupuestos.
- Presupuesto debe estar equilibrado.
- Propuesta de Gobernador, acuerdo CORE y resolución DIPRES deben ser coincidentes.
Req: Presupuesto de Funcionamiento
- Incluir glosas obligatorias (dotación, vehículos, viáticos, gasto COREs en extranjero).
- Monto del Subt. 21 debe coincidir con el autorizado en la glosa específica.
Req: Presupuesto de Inversión
- Incluir arrastres de años anteriores, conservando N° de asignación y código BIP.
- Se pueden incorporar nuevas iniciativas, cumpliendo requisitos de glosas.
- Para nuevas transferencias a privados: Acreditar selección vía concurso (o excepción fundada), personalidad jurídica vigente.
- Crear asignación "Provisión sin distribuir para el Fondo Regional para la Productividad y el Desarrollo" en ítem 33.03.
- Incluir otras provisiones (FRIL, Concurso 8% FNDR).
Req: Acuerdo del CORE
- Voluntad del CORE debe ser clara sobre conceptos y montos.
- Acuerdo debe ser certificado por Secretario Ejecutivo del CORE.

ID: GORE-FIN-APROB-ROL-CORE-01
Act: Propuesta de distribución se somete a aprobación del Consejo Regional (CORE).
Dln: 10 días corridos para pronunciarse.
Cpt: Facultades del CORE (Art. 25 LOCGAR): Aprobar, modificar o sustituir proyecto de presupuesto y distribución.
Fnd: Dictamen E548580/2024 CGR: Resolver de manera informada, razonada y ajustada a intereses regionales.
Proc: Exposición

- DIPIR expone presupuesto de inversiones.
- DAF expone presupuesto de funcionamiento.
- Ambas divisiones responden consultas y ajustan propuesta si es necesario.

ID: GORE-FIN-APROB-TRAM-DIPRES-01
Act: Gobernador remite distribución aprobada por CORE a DIPRES.
Dln: 5 días corridos post-aprobación CORE.
Resp: DAF prepara oficio conductor y antecedentes para DIPRES.
Req:

- Oficio firmado por Gobernador(a) titular o subrogante (adjuntar acto).
- Incluir contacto formal.
- Adjuntar acuerdo del CORE certificado.
Act: DIPRES revisa y elabora resoluciones de presupuesto inicial.
Dln: 10 días para elaboración.
Cpt: Facultades de DIPRES (Instructivo CGR)
- Subsanar errores materiales (copia, cálculo).
- Reclasificar ingresos y gastos, informando al GORE y CGR.
Res: Si hay errores, DIPRES devuelve para corrección.

ID: GORE-FIN-APROB-TRAM-CGR-01
Act: DIPRES remite Resoluciones a Contraloría General de la República (CGR) para Toma de Razón (TDR).
Nat: Control previo de legalidad, obligatorio.
Dln: 15 días desde recepción (prorrogable por 15 más).
Ctx: Foco del Control CGR

- Correcta clasificación presupuestaria.
- Cumplimiento de glosas legales.
- Conformidad con normativa general.
- Coincidencia entre solicitud GORE, acuerdo CORE y resolución DIPRES.
Res:
- Toma Razón: Acto entra en vigencia.
- Representa: Rechaza por ilegalidad o formula alcances.
Act: DAF carga presupuesto inicial en sistemas financieros (SIGFE).
Ref: GORE-FIN-HERRAM-SIGFE-01

#### GORE-FIN-CICLO-EJECUCION-01: Ejecución Presupuestaria

ID: GORE-FIN-EJEC-PROGRAMACION-01
Asunto: Programación de Ejecución y de Caja.
Src: Instructivo DIPRES Ejecución Presupuestaria 2025.
Cpt: Programa de Ejecución Inicial

- Act: DIPRES elabora programa de ejecución inicial mensualizado.
- Req: GOREs deben enviar propuesta de programa de ejecución mensualizado a DIPRES.
Cpt: Actualización Mensual
- Act: GORE remite actualizaciones al programa de ejecución a DIPRES.
- Dln: A más tardar el día 15 de cada mes.
- Req: Detallar aporte fiscal percibido (Remuneraciones, Resto, Pago Centralizado).
Cpt: Programa de Caja Mensual
- Fnd: Programa de Ejecución actualizado.
- Obj: Determinar necesidades de aporte fiscal para mes siguiente.
- Mech: Gasto programado MENOS saldos disponibles en cuentas corrientes.
- Purp: Evitar recursos ociosos ("empozados") y no presionar caja fiscal.

ID: GORE-FIN-EJEC-ROL-DAF-01
Resp: DAF en la administración financiera diaria.
Cpt: Tareas de Gestión Financiera

- Garantizar gasto dentro de montos y clasificación autorizada.
- Registrar transacciones en SIGFE (preafectación, compromiso, devengo, pago).
- Supervisar programación de caja mensual con DIPRES.
Cpt: Tareas de Pagos y Contabilidad
- Tramitar órdenes de compra, afectar gastos, realizar pagos.
- Req: Pago obligatorio vía transferencia electrónica de fondos (Art. 8 Ley 21.722).
- Cumplir normativa de compras públicas y rendición de cuentas.
- Elaborar informes financieros periódicos para DIPRES.
- Req: Identificación mensual de iniciativas de inversión (Subt. 31) por código BIP.
Cpt: Tareas de Control Interno
- Velar por respaldo legal de cada desembolso.
- Asegurar respeto al destino de fondos (glosas).
- Certificar disponibilidad y no exceder límites legales.
- Req: Coordinación con Unidad de Control del GORE.

ID: GORE-FIN-EJEC-ROL-DIPIR-01
Resp: DIPIR en el seguimiento físico y presupuestario de la inversión.
Cpt: Tareas de Monitoreo de Proyectos

- Revisar avance físico de obras e iniciativas (Subt. 31, 33).
- Detectar atrasos/desviaciones y proponer acciones correctivas.
- Evaluar cumplimiento de hitos de convenios (trimestral).
- Preparar informes para instancias externas (web regional, Congreso).
- Cpt: Contenido de Informe: Cartera de proyectos, avances, beneficiarios.
Cpt: Tareas de Coordinación Externa
- Articular con SEREMIs y servicios públicos sectoriales.
- Mantener comunicación con municipios beneficiarios de transferencias.
Cpt: Tareas de Uso de Herramientas
- Actualizar estados en Banco Integrado de Proyectos (BIP).
- Req: Ingresar información de ejecución físico-financiera mensual en BIP en primeros 8 días del mes siguiente.
- Verificar vigencia técnica de proyectos (RS).
- Usar SIGFE para trackear ejecución financiera por iniciativa.
- Ref: GORE-FIN-HERRAM-BIP-01, GORE-FIN-HERRAM-SIGFE-01

ID: GORE-FIN-EJEC-DEVENGO-01
Asunto: Reglas de Devengo Diferenciadas según tipo de transferencia.
Src: Minuta CGR-AGORECHI-DIPRES (Marzo 2025); Dictamen CGR N°E583841/2024.
Fnd: Momento del devengo varía crucialmente según receptor y modalidad.
Cpt: Casos

- Caso 1: Transferencias Extrapresupuestarias (no consolidables).
  - Def: A Instituciones contenidas en la Ley de Presupuestos.
  - Ex: SERCOTEC, INDAP.
  - Ctx: Imputación: Subt. 24-03, 33-03.
  - Cpt: Regla de Devengo: Al momento de aprobarse la respectiva rendición de cuentas.
  - Warn: No se devenga al transferir. Impacta metas de ejecución.
- Caso 2: Transferencias Presupuestarias (Consolidables o a Municipios).
  - Def: Consolidable: A entidades del Gobierno Central. Municipal: A instituciones públicas no contenidas en ley de presupuestos.
  - Ex: Consolidable: A Ministerio de Salud. Municipal: A Municipalidad para proyecto FRIL.
  - Ctx: Imputación Consolidable: Subt. 24-02, 33-02. Municipal: Subt. 24-03, 33-03.
  - Cpt: Regla de Devengo: Regla general. Cuando obligación es exigible (acto/convenio tramitado).
- Caso 3: Transferencias a Entidades Privadas.
  - Ex: Corporación Regional, Bomberos.
  - Ctx: Imputación: Subt. 24-01, 33-01.
  - Cpt: Regla de Devengo: Regla general. Cuando obligación es exigible (acto/convenio tramitado).

ID: GORE-FIN-EJEC-COORDINACION-01
Fnd: Comunicación constante DAF-DIPIR es esencial.
Ex:

- DIPIR a DAF: Informar de proyectos retrasados para evaluar modificación presupuestaria.
- DAF a DIPIR: Alertar sobre partidas agotándose o riesgo de sobregiro.

#### GORE-FIN-CICLO-MODIFICACION-01: Modificaciones Presupuestarias

ID: GORE-FIN-MOD-INICIATIVA-01
Cause: Reubicar recursos, incorporar nuevos ingresos, ajustar costos, financiar imprevistos.
Dln: Solicitud a DIPRES hasta 31 de octubre de 2025 (Instructivo DIPRES Ejecución).
Resp:

- Iniciativa DIPIR (Inversión): Reasignar fondos de proyectos retrasados, incorporar ingresos adicionales.
- Iniciativa DAF (Funcionamiento): Suplementar partidas con ahorros, incorporar Saldo Inicial de Caja.
Warn: Evitar peticiones para regularizar situaciones ya ocurridas (excepto excedibilidades legales).

ID: GORE-FIN-MOD-TIPOS-ACTOS-01
Asunto: Tipología de modificaciones y actos administrativos requeridos.
Src: Of. Circ. N°11 DIPRES 2025.
Fnd: Naturaleza del acto depende si modifica presupuesto de la Partida 31 o solo presupuesto interno GORE.
Cpt: Tipos de Modificación

- Suplemento Presupuestario:
  - Def: Aumento de presupuesto por mayor aporte fiscal.
  - Ctx: Afecta Ppto. Partida 31 y Ppto. GORE.
  - Proc: Requiere Decreto Supremo (DIPRES) y Resolución GORE.
- Incorporación/Reducción de Ingresos Ley:
  - Def: Distribución de fondos concursables o de contingencia.
  - Ctx: Afecta Ppto. Partida 31 y Ppto. GORE.
  - Proc: Requiere Decreto Supremo (DIPRES) y Resolución GORE.
- Reasignación Presupuestaria Interna:
  - Def: Movimiento de fondos entre subtítulos dentro del presupuesto del GORE.
  - Ctx: Afecta solo Ppto. GORE.
  - Proc: Requiere solo Resolución GORE.
- Transferencia a Otros Organismos (Consolidable):
  - Def: Reasignación desde FNDR para transferir a un ministerio.
  - Ctx: Afecta Ppto. Partida 31 y Ppto. GORE.
  - Proc: Requiere Decreto Supremo (DIPRES) y Resolución GORE.
- Financiamiento Emergencias (3%):
  - Def: Uso del fondo de emergencia para transferir a otra entidad.
  - Ctx: Afecta Ppto. Partida 31 y Ppto. GORE.
  - Proc: Requiere Decreto Supremo (DIPRES) y Resolución GORE.
- Creación Iniciativas FRPD:
  - Def: Asignación de fondos desde la provisión del FRPD a proyectos específicos.
  - Ctx: Afecta solo Ppto. GORE.
  - Proc: Requiere solo Resolución GORE.
- Incorporación Deuda Flotante:
  - Ctx: Financiada con Saldo Inicial de Caja (SIC) del GORE.
    - Afecta solo Ppto. GORE.
    - Proc: Requiere solo Resolución GORE.
  - Ctx: Financiada con Aporte Fiscal (si SIC es insuficiente).
    - Afecta Ppto. Partida 31 y Ppto. GORE.
    - Proc: Requiere Decreto Supremo (DIPRES) y Resolución GORE.

ID: GORE-FIN-MOD-APROB-INTERNA-01
Req: Modificaciones que alteran presupuesto de inversión requieren aprobación del CORE.
Cpt: Excepciones explícitas en Glosa 01. Ref: GORE-FIN-MOD-EXCEPCIONES-01.
Resp:

- DIPIR: Preparar propuesta de modificación con justificaciones para el CORE.
- DAF: Proveer información de respaldo financiero.

ID: GORE-FIN-MOD-TRAM-EXTERNA-01
Act: GORE emite resolución de modificación, firmada por Gobernador.
Resp: DAF redacta resolución, detallando cambios y fundamentación.
Proc:

1. Visación por DIPRES (paso previo a CGR).
   - Ctx: DIPRES verifica cumplimiento normativo. Si hay errores, devuelve.
2. Toma de Razón por CGR (paso final).
   - Ctx: CGR revisa fundamento legal.
3. Post-TDR: DAF ajusta presupuesto en SIGFE, DIPIR notifica a unidades ejecutoras.

ID: GORE-FIN-MOD-DOCS-REQUERIDOS-01
Src: Of. Circ. N°11 DIPRES 2025.
Cpt: Lista de Antecedentes para DIPRES

1. Certificado de acuerdo del CORE (cuando aplica).
2. Minuta explicativa (justificación, origen/destino de fondos, cita glosa habilitante).
3. Informe favorable MDSyF/DIPRES (si financia programas directos nuevos).
4. Otros documentos (certificados de disponibilidad, convenios, etc.).

ID: GORE-FIN-MOD-EXCEPCIONES-01
Asunto: Modificaciones de inversión sin acuerdo CORE.
Src: Glosa 01, Ley 2025; Of. Circ. N°11 DIPRES.
Cpt: Casos Permitidos

- Aplicación de leyes generales (reajustes, sentencias, deuda flotante).
- Regularización de ingresos que no inciden en gastos.
- Variaciones de tipo de cambio en compras de activos no financieros.
- Aplicación del 3% para emergencias. Ref: Glosa 14.
- Aumento de costo de proyectos en ejecución (hasta 10% del monto RS, tope 7.000 UTM).
- Adjudicación de licitaciones (hasta 10% sobre monto RS, tope 7.000 UTM).
Warn: Aunque no requieren CORE, sí necesitan visación DIPRES y TDR de CGR. GORE debe informar mensualmente al CORE.

ID: GORE-FIN-MOD-ROLES-SINTESIS-01
Resp:

- DIPIR: Lidera modificaciones de inversión (racionalidad técnico-programática).
- DAF: Lidera modificaciones de funcionamiento (racionalidad financiero-legal).
- Cpt: Trabajo conjunto: DIPIR provee detalle de proyectos, DAF estructura la modificación formal.
Warn: Antes de enviar, verificar que no vulnere normas (ej. prohibición de traspasar a Subt. 22 desde inversión).

##### GORE-FIN-MOD-LIMITES-01: Límites y Flexibilidades de Traspasos (Funcionamiento vs. Inversión)

ID: GORE-FIN-MOD-LIMITES-PRINCIPIO-01
Fnd: Fondos de inversión no deben usarse para financiar gastos corrientes de funcionamiento.
Cond: Excepción requiere autorización legal expresa (glosa).
Src: D.L. N°1.263, Art. 4 Ley 21.722.

ID: GORE-FIN-MOD-LIMITES-GLOSAS-01
Cpt: Reglas Clave (Ley 21.722)

- Glosa 03 (Prohibición): Recursos de inversión no pueden financiar préstamos, gastos en personal, o gastos en bienes y servicios de consumo de entidades receptoras.
- Glosa 04 (Flexibilidad Inversión): Permite traspasar recursos *entre* subtítulos de inversión.
- Glosa 04 (Restricción): Excluye explícitamente al Subtítulo 22 de recibir fondos desde inversión.
- Glosa 01 (Excepción Ley Reajuste): Habilita usar fondos de inversión para cubrir gasto de personal si una ley específica lo mandata.
- Glosa 06 (Excepción Programas Directos): Permite destinar hasta 5% del monto total de un programa a gastos de administración del propio GORE (Subt. 21, 22, 29). También permite a receptor público usar hasta 5% para contratar honorarios. Ref: GORE-FIN-INSTR-PROGDIR-GASTOS-ADM-01.
- Artículo 7 Ley 21.722: Refuerza necesidad de habilitación legal expresa para financiar gastos operativos con fondos de transferencia.

##### GORE-FIN-MOD-CONSOL-01: Transferencias Consolidables

ID: GORE-FIN-MOD-CONSOL-DEF-01
Def: Transferencias desde un GORE a otras instituciones del Presupuesto del Sector Público.
Obj: Evitar doble contabilización del gasto público.
Fnd: Oficio Circular N°11 DIPRES 2025, Glosa 01 Partida 31, Art. 26 Ley 21.722.

ID: GORE-FIN-MOD-CONSOL-PROC-01
Proc:

1. GORE solicita formalmente a DIPRES la creación de la transferencia.
2. GORE emite resolución interna con la rebaja presupuestaria.
3. GORE adjunta documentación de respaldo (acuerdo CORE, resolución, justificación, aceptación del receptor).
4. DIPRES elabora Decreto Supremo que modifica presupuesto GORE.
5. Decreto sigue curso legal (Toma de Razón CGR, publicación).
Ctx: Transferencias consolidables pueden efectuarse sin convenio formal, cumpliendo procedimiento presupuestario (Art. 26 Ley 21.722).

ID: GORE-FIN-MOD-CONSOL-EJEMPLO-01
Asunto: Ejemplo de flujo para transferencia consolidable.
Ctx: GORE "X" transfiere M$10 de su presupuesto de inversión (Subt. 33.03) al Ministerio de Salud.
Proc:

1. Aprobación del CORE.
2. GORE envía oficio a DIPRES.
3. GORE emite resolución que rebaja su presupuesto.
4. DIPRES emite Decreto que crea la asignación y reasigna fondos.
5. Ajustes Presupuestarios (Decreto):
    - Ppto. GORE X: Rebaja (-) Subt. 33.03.150; Aumento (+) Subt. 33.02.100.
    - Ppto. Min. Salud: Aumento (+) Ingreso 13.02; Aumento (+) Gasto 33.03.10.
6. Ajustes Presupuestarios (Resolución GORE):
    - Ppto. GORE X: Rebaja (-) Ingreso 13.03; Rebaja (-) Gasto 31.02.

#### GORE-FIN-CICLO-CONTROL-01: Control y Seguimiento Presupuestario

ID: GORE-FIN-CONTROL-INTERNO-01
Resp: Unidad de Control (o auditoría interna) del GORE.
Act: Revisa actos administrativos de contenido financiero (control ex-ante).
Ex: Visa resoluciones, verifica respaldos, revisa rendiciones.
Req: DAF colabora para subsanar observaciones.

ID: GORE-FIN-CONTROL-LEGALIDAD-CGR-01
Resp: Contraloría General de la República (CGR).
Cpt:

- Control Previo: Toma de Razón de resoluciones presupuestarias.
- Control Posterior: Auditorías e investigaciones especiales.
Req: DIPIR y DAF deben mantener antecedentes ordenados para responder a fiscalizaciones.

ID: GORE-FIN-CONTROL-SEGUIMIENTO-DIPRES-01
Resp: Dirección de Presupuestos (DIPRES).
Act: Monitorea ejecución presupuestaria mensual de los GORE.
Mech:

- Informes formales.
- Reuniones de seguimiento.
- Alertas sobre baja ejecución y solicitud de planes de aceleración.
Req: GORE debe manejar calendario de hitos para asegurar cumplimiento.

ID: GORE-FIN-CONTROL-TRANSPARENCIA-01
Nat: Control social.
Fnd: Glosa 16, Ley 21.722; Art. 14 Ley 21.722.
Req: Publicar en sitio web del GORE información de ejecución de inversión.
Cpt: Contenido a Publicar Mensual:

- Cartera de proyectos financiada con inversión regional.
Cpt: Contenido a Publicar Trimestral:
- Uso de recursos de inversión (beneficiarios, comuna, receptor, monto, productos).
- Destino de FNDR por sector económico.
- Proyectos adjudicados con votación del CORE.
- Información sobre corporaciones en las que participa. Ref: Glosa 08.
Cpt: Contenido a Publicar Otros:
- Acuerdos del CORE (≤5 días hábiles).
Resp: DIPIR compila información, DAF valida cifras.

#### GORE-FIN-CICLO-CIERRE-01: Cierre del Ejercicio Presupuestario

ID: GORE-FIN-CIERRE-COMPROMISOS-01
Act: Establecer fechas de corte para contraer nuevos compromisos (usualmente en diciembre).
Resp: DAF comunica fechas límite; DIPIR verifica registro de compromisos.

ID: GORE-FIN-CIERRE-DEUDA-FLOTANTE-01
Def: Obligaciones devengadas en el año pero pendientes de pago al 31 de diciembre.
Resp: DAF calcula, registra y tramita su incorporación en presupuesto del año siguiente.
Mech: Modificación presupuestaria que crea el Ítem 34.07 "Deuda Flotante".
Fnd: Art. 34 Ley 21.722 habilita exceder sumas fijadas para este ítem.
Cpt: Lógica de Financiamiento

- Fuente de financiamiento y acto administrativo dependen de relación Saldo Inicial de Caja (SIC) vs. Deuda Flotante (DF).
- Src: Of. Circ. N°11 DIPRES 2025.
- Caso 1: SIC > DF.
  - Cond: SIC es suficiente.
  - Ctx: Financiamiento 100% con SIC.
  - Proc: Requiere solo Resolución del GORE.
- Caso 2: SIC <= DF.
  - Cond: SIC es insuficiente.
  - Ctx: Financiamiento con todo el SIC y la diferencia con Mayor Aporte Fiscal.
  - Proc: Requiere Resolución del GORE y Decreto de DIPRES.
Warn: Priorizar pago de deuda flotante al inicio del nuevo ejercicio.

ID: GORE-FIN-CIERRE-EVALUACION-01
Act: Cierre contable y evaluación de la gestión.
Resp:

- DAF: Realiza ajustes contables, prepara Informe de Ejecución Anual. Saldo no gastado pasa a Saldo Inicial de Caja.
- DIPIR: Elabora evaluación de ejecución física de proyectos. Identifica logros, retrasos, cuellos de botella.
Res: Resultados alimentan la siguiente formulación presupuestaria.

ID: GORE-FIN-CIERRE-SISTEMAS-01
Act: Cierre formal en plataformas.
Resp: DAF realiza cierre en SIGFE; DIPIR actualiza estado final en BIP.

### GORE-FIN-SUBTITULOS-01: Gestión de Subtítulos Presupuestarios

ID: GORE-FIN-SUB-INTRO-01
Purp: Describir los subtítulos más relevantes, su contenido y consideraciones operativas.
Src: Chileindica.md; Ley de Presupuestos 2025.
Ctx: Subtítulos Clave: 21, 22, 23, 24, 26, 29, 31, 33, 34.

#### GORE-FIN-SUB-21-PERS-01: Subtítulo 21 - Gastos en Personal

ID: GORE-FIN-SUB-21-CONTENIDO-01
Cpt: Remuneraciones y obligaciones del empleador para personal del GORE.
Resp: DAF.
Act: Asegurar que pagos se ajusten a dotaciones y topes de glosas.
Ctx: Flexibilidad 2025

- Glosa 01 Partida 31: Sin límite de antigüedad para contratas, contratas pueden ejercer funciones directivas (hasta 20%), honorarios pueden actuar como Agente Público.
- Art. 5 Ley 21.722: Suspende compatibilidad de cargo de planta con contrata.

ID: GORE-FIN-SUB-21-ITEMS-RELEVANTES-01
Asunto: Ítems y asignaciones del Subtítulo 21 relevantes para la inversión regional.
Src: doc/curados/presupuesto/chileindica.md
Ctx: Ciertos programas de inversión pueden imputar gastos de personal.

- Ítem 03: Otras Remuneraciones
  - Asignación 001: Honorarios a Suma Alzada - Personas Naturales.
    - Purp: Contratar profesionales/expertos para asesoría o ejecución en programas de inversión.
    - Ctx: Fundamental para programas directos (Glosa 06) que permiten % para gastos de adm., incluyendo personal.

#### GORE-FIN-SUB-22-BS-01: Subtítulo 22 - Bienes y Servicios de Consumo

ID: GORE-FIN-SUB-22-CONTENIDO-01
Cpt: Gastos operativos del GORE (insumos, servicios básicos, arriendos, pasajes).
Resp: DAF.
Act: Asegurar adquisiciones vía Ley de Compras Públicas y buscar eficiencia.
Prohib: No se permite reasignar recursos de inversión hacia Subtítulo 22 (Glosa 04 Partida 31).
Fnd: Incremento de Subt. 22 solo con ingresos propios o saldo inicial de caja.
Ctx: DIPIR interviene solo si un programa directo (Glosa 06) destina parte de su 5% de adm. a este subtítulo.

ID: GORE-FIN-SUB-22-ITEMS-RELEVANTES-01
Asunto: Ítems y asignaciones del Subtítulo 22 relevantes para la inversión regional.
Src: doc/curados/presupuesto/chileindica.md
Ctx: Ciertos gastos de consumo son informados como Inversión Pública Regional en Chileindica.

- Ítem 08: Servicios Generales
  - Asignación 007: Pasajes, Fletes y Bodegajes.
- Ítem 11: Servicios Técnicos y Profesionales
  - Asignación 001: Estudios e Investigaciones.

#### GORE-FIN-SUB-23-PRESTSEC-01: Subtítulo 23 - Prestaciones de Seguridad Social

ID: GORE-FIN-SUB-23-CONTENIDO-01
Cpt: Gastos por prestaciones previsionales y de asistencia social.
Ctx: Uso en GORE generalmente bajo o nulo.
Resp: DAF.

#### GORE-FIN-SUB-24-TRANSFCORR-01: Subtítulo 24 - Transferencias Corrientes

ID: GORE-FIN-SUB-24-CONTENIDO-01
Cpt: Recursos transferidos sin contraprestación directa para gastos corrientes de otras instituciones.
Nat: Doble componente (funcionamiento e inversión).
Fnd: Asignación a privados debe ser por concurso público, con convenio (Art. 23-27 Ley 21.722).

ID: GORE-FIN-SUB-24-ITEMS-01
Asunto: Ítems del Subtítulo 24.
Cpt:

- Ítem 01: Al Sector Privado.
- Ítem 03: A Otras Entidades Públicas.
- Ítem 04: A Empresas Públicas no Financieras.
- Ítem 05: A Empresas Públicas Financieras.
- Ítem 08: A Instituciones Privadas Ejecutoras de Políticas Públicas.
- Ítem 09: A Unidades o Programas del Servicio.

ID: GORE-FIN-SUB-24-CONCURSO-8FNDR-01
Asunto: Concurso de Vinculación con la Comunidad 8% FNDR.
Src: Glosa 07 Partida 31 Ley 21.722.
Cond: Límite hasta 8% del total del presupuesto de inversión regional.
Ctx: Áreas financiables: Deporte, seguridad, cultura, social, etc.
Req: Mínimo 1% del presupuesto de inversión para cultura y patrimonio.
Proc: DIPIR elabora bases (aprueba CORE) -> Comisiones evalúan -> CORE aprueba adjudicados -> DAF formaliza y fiscaliza.
Fnd: Artículos 23-27 Ley 21.722.
Cond: Excepción de concurso: hasta 10% del 8% puede asignarse directamente a casos emblemáticos.
Cond: Concursos del 8% están exentos de evaluación ex-ante de Glosa 06.

ID: GORE-FIN-SUB-24-PROGRAMAS-01
Asunto: Transferencias corrientes a entidades públicas y ejecución directa de programas.
Fnd: Glosa 06 Partida 31 Ley 21.722.
Cond: Programas nuevos de ejecución directa requieren evaluación ex-ante DIPRES/MDSF. Ref: GORE-FIN-INSTR-PROGDIR-EVAL-EXANTE-01.
Prohib: No usar fondos de inversión para financiar gastos permanentes de otros servicios (Glosa 03).
Cond: Excepción Glosa 06: Receptor público puede usar hasta 5% de lo transferido para contratar honorarios.
Cond: Habilitaciones específicas (Glosa 06) para financiar áreas fuera de competencias LOC GORE.

#### GORE-FIN-SUB-26-OTROSCORR-01: Subtítulo 26 - Otros Gastos Corrientes

ID: GORE-FIN-SUB-26-CONTENIDO-01
Cpt: Devoluciones y compensaciones por daños a terceros.

- Ítem 01: Devoluciones.
- Ítem 02: Compensaciones por Daños.
Ctx: Uso en GORE bajo, pero posible.
Resp: DAF.

#### GORE-FIN-SUB-29-ACTIVOS-01: Subtítulo 29 - Adquisición de Activos no Financieros

ID: GORE-FIN-SUB-29-CONTENIDO-01
Cpt: Adquisición de bienes de capital por el GORE (equipos, vehículos, terrenos).
Purp: Financiar adquisición de activos de reposición para otras instituciones públicas (Glosa 09 Partida 31).
Cond: Activos nuevos requieren certificado de la institución receptora garantizando presupuesto para gastos operativos futuros.
Req: Certificados especiales para compras a policías, bomberos y coordinación con SERVIU para terrenos.
Resp: DIPIR identifica necesidades, DAF conduce adquisición.

ID: GORE-FIN-SUB-29-ITEMS-01
Asunto: Ítems del Subtítulo 29.
Cpt:

- Ítem 01: Terrenos
- Ítem 02: Edificios
- Ítem 03: Vehículos
- Ítem 04: Mobiliario y Otros
- Ítem 05: Máquinas y Equipos
- Ítem 06: Equipos Informáticos
- Ítem 07: Programas Informáticos
- Ítem 99: Otros Activos no Financieros

#### GORE-FIN-SUB-31-INVDIR-01: Subtítulo 31 - Iniciativas de Inversión (Ejecución Directa)

ID: GORE-FIN-SUB-31-CONTENIDO-01
Cpt: Inversión real ejecutada directamente por el GORE.
Fnd: Glosa 10 Partida 31.
Req: Respetar competencias y someterse al SNI.
Proc: GORE actúa como Unidad Mandante, DAF gestiona licitación y contratación.
Cond: Licitación pública obligatoria si proyecto > 1.000 UTM (Art. 6 Ley 21.722).
Cond: Aumento de costos hasta 10% del monto RS (tope 7.000 UTM) no requiere acuerdo CORE.

ID: GORE-FIN-SUB-31-ITEMS-01
Asunto: Ítems del Subtítulo 31.
Cpt:

- Ítem 01: Estudios Básicos.
- Ítem 02: Proyectos (estudios preinversionales y ejecución).
- Ítem 03: Programas de Inversión.

#### GORE-FIN-SUB-33-TRANSFCAP-01: Subtítulo 33 - Transferencias de Capital

ID: GORE-FIN-SUB-33-CONTENIDO-01
Cpt: Transferencia de recursos a terceros para que ejecuten proyectos de inversión. Subtítulo de mayor peso.
Resp: Municipalidades, servicios públicos, corporaciones, etc.
Fnd: Glosa 11 enumera iniciativas adicionales.
Req: Cada transferencia debe formalizarse en un convenio.
Cond: Convenio debe incluir partes, objeto, monto, plazos, obligaciones, seguimiento, garantías, etc.

ID: GORE-FIN-SUB-33-ITEMS-01
Asunto: Ítems del Subtítulo 33.
Cpt:

- Ítem 01: Al Sector Privado.
- Ítem 03: A Otras Entidades Públicas (ítem principal de inversión GORE).
- Ítem 04: A Empresas Públicas no Financieras.
- Ítem 05: A Empresas Públicas Financieras.
- Ítem 06: A Gobiernos Extranjeros.
- Ítem 07: A Organismos Internacionales.

ID: GORE-FIN-SUB-33-CASOS-ESPECIALES-01
Cpt: Casos Especiales

- FRIL (Fondo Regional de Iniciativa Local):
  - Src: Glosa 12 Partida 31.
  - Ctx: Proyectos de menor escala de municipios.
  - Cond: Requieren RS, salvo si costo < 5.000 UTM.
  - Req: Seguir Guía Operativa FRIL de SUBDERE.
- Emergencia Hídrica:
  - Src: Glosa 11.
  - Ctx: Permite transferir a municipios y sanitarias para reparaciones de redes de agua.
  - Req: Visación de órgano técnico competente.

ID: GORE-FIN-SUB-33-ROLES-01
Resp:

- DIPIR: Articula cartera de proyectos, coordina para RS, prioriza, coordina convenios y seguimiento técnico.
- DAF: Elabora aspectos financieros de convenios, ejecuta transferencias, revisa rendiciones.

#### GORE-FIN-SUB-34-DEUDA-01: Subtítulo 34 - Servicio de la Deuda y Otros

ID: GORE-FIN-SUB-34-CONTENIDO-01
Cpt: Pagos asociados a endeudamiento.
Prohib: GOREs no están autorizados a endeudarse sin ley especial.
Purp: Principalmente para registrar pago de la Deuda Flotante del año anterior.
Mech: Se utiliza Ítem 34.07 "Deuda Flotante". Ref: GORE-FIN-CIERRE-DEUDA-FLOTANTE-01.
Warn: Alto nivel de deuda flotante recurrente es indicador de gestión deficiente.

### GORE-FIN-GLOSAS-01: Aplicación Operativa de Glosas Relevantes

ID: GORE-FIN-GLOSAS-FNDR-01
Asunto: Fondo Nacional de Desarrollo Regional (FNDR)
Def: Principal fuente de financiamiento de inversión regional.
Ctx: Distribución 2025: 90% distribuido por ley, 10% manejado por Subdere/DIPRES.
Proc: DIPIR programa cartera para ejecutar el 90%. DAF vigila que giros sean para fines autorizados.
Req: Glosa 16 Partida 31 exige reportar trimestralmente destino de fondos y publicar proyectos.

ID: GORE-FIN-GLOSAS-FRPD-01
Asunto: Fondo Regional para la Productividad y el Desarrollo (FRPD)
Def: Reemplaza al antiguo FIC. Para iniciativas de innovación, competitividad, ciencia y tecnología.
Fnd: Glosa 13 Partida 31 Ley 21.722; Art. 13 Ley 21.591; Reglamento específico.
Proc:

- GORE debe crear provisión para el FRPD en Ítem 33.03 en presupuesto inicial.
- Durante el año, se reasigna a iniciativas específicas vía modificación presupuestaria.
Cpt: Reglas Clave
- Se evita doble concursabilidad.
- Tipología "Innovación y Competitividad" (Res. Ex. N°33 Subdere 2024) no requiere evaluación ex-ante de Glosa 06.
- Otras tipologías se rigen por normativa general.
Resp: DIPIR gestiona el fondo; DAF maneja provisión y control financiero.

ID: GORE-FIN-GLOSAS-EQUIDAD-01
Asunto: Fondos para corregir desigualdades territoriales.
Cpt:

- Fondo de Equidad Interregional: Se maneja como parte del programa de inversión.
- Planes de Zonas Extremas y Territorios Rezagados: Se financian con programa especial "Asociatividad y Planes Especiales".

ID: GORE-FIN-GLOSAS-SUBV8-01
Asunto: Subvenciones Concursables (Concurso 8% FNDR)
Fnd: Glosa 07 Partida 31 Ley 21.722. Ref: GORE-FIN-SUB-24-CONCURSO-8FNDR-01.
Req: Proceso transparente, rendición vía SISREC de CGR (Art. 24 Ley 21.722).

ID: GORE-FIN-GLOSAS-ASOC-01
Asunto: Asociatividad Regional
Mech: Participación de GOREs en personas jurídicas (Corporaciones, Fundaciones).
Fnd: Art. 101 LOC GORE; Programa especial de asociatividad; Glosa 08 Partida 31 Ley 21.722.
Cond:

- Aporte máximo GORE: 5% de su presupuesto de inversión.
- Aporte para funcionamiento es anual, no proceden convenios plurianuales.
- Cofinanciamiento de programas/proyectos hasta 50% con recursos GORE.
- Aportes privados pueden ser no pecuniarios, valorizados en convenio.
Req: GORE debe informar y publicar anualmente/trimestralmente sobre corporaciones que financia.

ID: GORE-FIN-GLOSAS-UNIV-01
Asunto: Transferencias a Universidades Regionales
Fnd: Glosa 05 Partida 31 Ley 21.722.
Cpt: Habilita transferir recursos a universidades del DFL N°4 de 1981 con casa central en la región.
Cond: Fines dentro de competencia universitaria, ejecución íntegra por la universidad, sujeto a concursabilidad si aplica.

### GORE-FIN-CONTROL-EXT-01: Control Externo y Documentación

ID: GORE-FIN-CTRL-TDR-01
Asunto: Toma de Razón (TDR) y Control de Legalidad por Contraloría (CGR).
Cpt: Hitos Clave de TDR

- Resolución de Presupuesto Inicial.
- Resoluciones de Modificación Presupuestaria (previa visación DIPRES).
- Decretos Supremos.
- Convenios Relevantes.
Rec: Planificar con tiempo, asegurar calidad de documentación, archivar actos tramitados.

ID: GORE-FIN-CTRL-DOC-DIPRES-01
Asunto: Preparación de antecedentes para DIPRES.
Cpt: Reportes Regulares

- Programa de Ejecución y Caja (mensual).
- Ejecución mensual.
- Reporte trimestral transferencias.
- Ejecución de Inversión Subt. 31 (por código BIP).
- Informe Dotación Personal (mensual).
Rec: Ante dudas, solicitar dictamen a DIPRES o CGR antes de ejecutar.

ID: GORE-FIN-CTRL-DOC-DIPRES-FORMATOS-01
Asunto: Formatos y anexos requeridos por DIPRES.
Src: Of. Circ. N°11 DIPRES 2025.
Purp: Estandarizar la información remitida.
Cpt: Anexos

- Anexo 1: Certificado de Acuerdo CORE.
- Anexo 2: Reporte Mensual de Ejecución.
- Anexo 3: Reporte Trimestral de Transferencias.

### GORE-FIN-INSTRUMENTOS-01: Instrumentos de Ejecución

#### GORE-FIN-INSTR-CONVENIOS-01: Convenios y Transferencias de Fondos

ID: GORE-FIN-INSTR-CONV-CONTENIDO-01
Cpt: Herramienta Jurídica: Convenio de transferencia.
Purp: Materializar transferencias Subt. 24 y 33.
Fnd: Art. 23-27 Ley 21.722 para transferencias a privados.
Req: Contenido Mínimo

- Partes, objeto, monto, plazos, obligaciones, seguimiento, garantías, etc.

ID: GORE-FIN-INSTR-CONV-PROCESO-01
Proc:

1. Elaboración borrador.
2. Suscripción.
3. Entrega de garantías.
4. Toma de Razón (si aplica).
5. Ejecución (pago y monitoreo).
6. Rendición (vía SISREC).
7. Cierre (aprobación de rendición, reintegro de saldos).

#### GORE-FIN-INSTR-PROGDIR-01: Programas Ejecutados Directamente por el GORE

ID: GORE-FIN-INSTR-PROGDIR-MARCO-01
Asunto: Oferta programática adicional ejecutada por el GORE.
Fnd: Art. 20 letra k) LOC GORE; Glosa 06 Partida 31 Ley 21.722.
Mech: GORE desarrolla programas con cargo a su presupuesto de inversión.
Mdl: Ejecución directa o a través de privados (vía concurso público).

ID: GORE-FIN-INSTR-PROGDIR-EVAL-EXANTE-01
Req: Programas nuevos ejecutados directamente por GORE deben someterse a evaluación ex-ante de diseño por MDSyF/DIPRES (Glosa 06).
Src: Of. Circ. N°22 DIPRES.
Proc: GORE nomina contraparte -> presenta perfil -> completa Formulario de Diseño Ex Ante -> SES/DIPRES revisan -> emiten certificado.
Res: Calificación "Recomendado Favorablemente" (RF) es requisito para financiar.
Cond: Excepciones a evaluación: continuidad, 8% FNDR, transferencias a públicos, emergencias, programas con RF previo, programas FRPD.

ID: GORE-FIN-INSTR-PROGDIR-GASTOS-ADM-01
Cpt: Regla Clave (Glosa 06)

- Gasto Adm. GORE: Hasta 5% del monto del programa puede destinarse a gastos de adm. del GORE.
- Gasto Adm. Receptor Público: Si se transfiere, receptor puede usar hasta 5% para contratar honorarios para gestión.

### GORE-FIN-CUMPLIMIENTO-01: Cumplimiento de Hitos Físicos y Financieros

ID: GORE-FIN-CUMPL-PLAN-01
Purp: Instaurar sistema interno de seguimiento de hitos de ejecución.
Proc:

1. Planificación Anual: DIPIR y DAF definen hitos y cronograma maestro.
2. Monitoreo Periódico: Reuniones técnicas mensuales y directivas trimestrales.
3. Coordinación Interinstitucional: DIPIR lidera coordinación con Unidades Técnicas.
4. Alertas Tempranas: Detectar problemas y reaccionar.

ID: GORE-FIN-CUMPL-KPIS-01
Asunto: Indicadores de desempeño clave (KPIs) para monitoreo.
Src: Indicadores de desempeño GORE Ñuble, Ley Presupuestos 2025.
Ctx: La Ley de Presupuestos fija indicadores de desempeño para cada GORE.
Cpt: Tipos de Indicador: Eficacia, Eficiencia, Calidad, Economía.
Ex: GORE Ñuble 2025

- Eficacia/Producto 1: % de proyectos Subt. 31 y 33 (FRIL) con visita en terreno.
- Eficacia/Producto 2: % de iniciativas FNDR del PROPIR georreferenciadas y pertinentes.
- Eficacia/Producto 3: % de iniciativas de fomento productivo que benefician a mujeres.
Obj: Lograr gestión por resultados, evitando ejecución apresurada ("dicembreo").

### GORE-FIN-HERRAMIENTAS-01: Herramientas de Soporte

#### GORE-FIN-HERRAM-SIGFE-01: Sistema SIGFE

ID: GORE-FIN-HERRAM-SIGFE-DEF-01
Def: Sistema de Información para la Gestión Financiera del Estado.
Nat: Sistema contable-presupuestario oficial y transaccional.
Resp: DAF.
Purp: Control presupuestario en línea, fuente de info para DIPRES, gestión de pagos, generación de reportes.
Rec: DIPIR debería tener usuarios de consulta.

#### GORE-FIN-HERRAM-BIP-01: Banco Integrado de Proyectos (BIP)

ID: GORE-FIN-HERRAM-BIP-DEF-01
Def: Plataforma del Sistema Nacional de Inversiones (SNI).
Nat: Registro único de todos los proyectos de inversión pública (código BIP).
Resp: DIPIR.
Purp: Evaluación ex-ante (obtener RS), seguimiento físico, reporte a nivel central, planificación multianual (ARI).
Warn: Interoperabilidad limitada con SIGFE. Requiere conciliación manual.

#### GORE-FIN-HERRAM-CHILEINDICA-01

ID: GORE-FIN-HERRAM-CHILEINDICA-DEF-01
Asunto: Plataforma Chileindica.
Src: Chileindica.md; Instructivo Coordinación Gasto Público ARI-PROPIR.
Def: Plataforma para la coordinación y seguimiento de la Inversión Pública Regional.
Ctx: URL: <www.chileindica.cl>
Purp: Formulación y aprobación de ARI y PROPIR; seguimiento de ejecución del PROPIR.
Resp: Secretarías Regionales Ministeriales y Servicios Públicos Regionales.

### GORE-FIN-CONCLUSION-01: Conclusión

ID: GORE-FIN-CONCLUSION-SINTESIS-01
Cpt: Gestión presupuestaria GORE es un proceso complejo que requiere trabajo colaborativo DAF-DIPIR.
Cpt: Sinergia de Roles

- DAF: Rigor financiero, cumplimiento normativo, control de fondos.
- DIPIR: Visión de desarrollo, priorización de inversiones, seguimiento de resultados.
Obj:
- Cuantitativo: Ejecutar 100% del presupuesto.
- Cualitativo: Ejecutar con eficiencia, legalidad y pertinencia.
Cpt: Claves del Éxito
- Dominar ciclo presupuestario.
- Aplicar correctamente clasificador y glosas.
- Documentar y someter a controles.
- Usar esta guía como referencia.
Res: Gestión presupuestaria sólida y confiable que respalda los objetivos de desarrollo regional.

## Catálogo de Flujos de Aprobación de Documentos para el GORE Ñuble

ID: kb_gn_102_flujos-aprobacion_sts.md
Version: 1.1.0
Status: Published
Human-Creator: FS
Human-Editor: FS
Model-Collaborator: IA-GEMINI
Creation-Date: 2025-07-10
Modification-Date: 2025-07-10
Ref-STS-Guide: GUIDE-STS-MASTER-01

### 2. Principios y Actores del Proceso de Aprobación

ID: KB-GN-102-PRINCIPIOS-ACTORES-01
Purp: Establecer el marco conceptual, jurídico y organizacional que sustenta todos los flujos de aprobación, definiendo los principios rectores y los roles de cada participante.

#### 2.1. Fundamentos Jurídico-Procedimentales

ID: KB-GN-102-FUNDAMENTOS-01
Fnd: La totalidad de los flujos de aprobación del Gobierno Regional (GORE) de Ñuble se enmarcan en un estricto conjunto de principios jurídicos que garantizan su legalidad, probidad y eficiencia. La inobservancia de estos fundamentos puede acarrear la nulidad de los actos administrativos.

- Cpt: Principio de Legalidad
- Def: Los órganos de la Administración del Estado, incluyendo el GORE, deben someter su acción a la Constitución y a las leyes, actuando exclusivamente dentro del ámbito de su competencia. Todo acto que exceda estas atribuciones es nulo y puede ser impugnado.
- Cpt: Principio de Escrituración Electrónica
- Def: La Ley N° 21.180 de Transformación Digital del Estado mandata que todos los procedimientos administrativos se realicen por medios electrónicos. El papel es la excepción. Esto implica que todo flujo de aprobación debe quedar registrado en un expediente electrónico único y accesible.
- Cpt: Principio de Impugnabilidad
- Def: Todo acto administrativo emanado del GORE es susceptible de ser impugnado a través de los recursos que establece la ley, como el recurso de reposición ante la misma autoridad o el recurso jerárquico, si procede.
- Cpt: Principio de Probidad y Transparencia
- Def: La función pública debe ejercerse con una conducta funcionaria intachable, anteponiendo siempre el interés general sobre el particular. Asimismo, los procedimientos, contenidos y fundamentos de las decisiones deben ser públicos y accesibles, promoviendo el control ciudadano.
- Cpt: Control Externo de Legalidad
- Def: La autonomía del GORE para administrar sus asuntos no lo exime del control superior de la Contraloría General de la República (CGR). La CGR fiscaliza la legalidad de los actos, el correcto uso de los fondos y ejerce un control preventivo a través de la Toma de Razón.

#### 2.2. Matriz de Actores y Responsabilidades Clave

ID: KB-GN-102-ACTORES-MATRIZ-01
Purp: Definir los roles y responsabilidades de las unidades y autoridades que intervienen en los flujos de aprobación, estableciendo una referencia única para la correcta derivación de documentos y tareas.
Fnd: La estructura de gobernanza del GORE se caracteriza por un sistema de control dual y múltiples puntos de veto, donde se separan las funciones ejecutivas (Gobernador), de fiscalización y financiamiento (CORE), y las de gestión técnica (DIPIR/DIPLADE) de las de gestión financiera (DAF). A esto se suman los controles externos obligatorios de CGR, DIPRES y MDSF, que actúan como compuertas indispensables en el proceso.

| Actor/Unidad | Rol Principal en Aprobaciones | Fuente Normativa/Contextual |
|-|-|-|
| Gobernador/a Regional | Act: Firma ejecutiva final de actos adm. \| Act: Propone presupuesto y planes al CORE. \| Cpt: Representación judicial y extrajudicial del GORE. | GORE-GUIA-ESTRUCTURA-GOBERNADOR-01 |
| Consejo Regional (CORE) | Act: Aprueba presupuesto regional, planes de desarrollo (ERD), distribución de fondos (FNDR, 8%, FRIL) y mods. presupuestarias. \| Act: Ejerce fiscalización sobre gestión del Gobernador. | GORE-GUIA-ESTRUCTURA-CORE-01 |
| Administrador/a Regional | Act: Coordina gestión adm. interna. \| Act: Ejerce V°B° final antes de firma del Gobernador. \| Cpt: Subrogancia legal del Gobernador. | GORE-GUIA-ESTRUCTURA-ADM-REGIONAL-01 |
| DAF (Div. de Adm. y Finanzas) | Act: Ejecuta gestión financiera y contable. \| Act: Elabora convenios y resoluciones de pago. \| Act: Controla rendiciones de cuentas. \| Act: Registra operaciones en SIGFE. | KB-GN-CTX-AUTH-01-03, STS-KB-GN-RENDICION-ACTOR-DAF-01 |
| DIPIR (Div. de Presupuesto e Inv. Reg.) | Resp: Lidera formulación y mod. de presupuesto de inversión. \| Act: Evalúa técnicamente las Iniciativas de Inversión (IDI). \| Act: Monitorea avance físico-financiero en BIP. | KB-GN-CTX-AUTH-01-03, GORE-IPR-PHASE1-ENTRY-01 |
| DIPLADE (Div. de Planificación y Desarrollo) | Resp: Lidera elaboración y seguimiento de ERD. \| Resp: Actúa como secretaría ejecutiva en coordinación del gasto (ARI/PROPIR). | KB-GN-CTX-AUTH-01-03, GORE-FIN-FORM-ROL-DIPIR-01 |
| Asesoría Jurídica | Act: Realiza control de legalidad interno de actos y convenios. \| Act: Redacta y revisa borradores de resoluciones y decretos. | |
| Unidad de Control | Act: Ejerce control preventivo y posterior de legalidad de actos y procedimientos. \| Dep: Dependencia técnica de CGR. \| Act: Audita selectivamente procesos. | STS-KB-GN-RENDICION-ACTOR-CONTROLINTERNO-01 |
| Oficina de Partes | Cpt: Punto único de ingreso formal de documentación externa. \| Act: Asigna número de registro (SGDOC). \| Act: Deriva a unidad competente. | GORE-IPR-PHASE1-RECEPTION-01 |
| Comité Directivo Regional (CDR) | Act: Realiza filtro estratégico y político-técnico de IPR pre-evaluación. \| Cpt: Compuesto por Jefaturas de División y Administrador/a Regional. | GORE-IPR-PHASE1-PERTINENCE-01 |
| Referente Técnico-Financiero (RTF) | Resp: Funcionario de división técnica. \| Act: Actúa como primera línea de revisión y seguimiento de proyecto/programa (técnico y financiero). | STS-KB-GN-RENDICION-ACTOR-RTF-01 |
| SEREMI de Desarrollo Social y Familia | Act: Evalúa técnicamente IDI para otorgar la Recomendación Satisfactoria (RS) o Admisibilidad (AD). \| Req: Indispensable para financiamiento de mayoría de proyectos de inversión. | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |
| Dirección de Presupuestos (DIPRES) | Act: Evalúa ex-ante Programas Públicos Regionales (Glosa 06). \| Act: Elabora resoluciones de presupuesto inicial. \| Act: Visa mods. presupuestarias que afectan Partida 31. | GORE-FIN-CTX-CAMBIOS-2025-01, GORE-IPR-PHASE2-TRACK-GLOSS06-01 |
| Contraloría General de la República (CGR) | Act: Ejerce control preventivo de legalidad (Toma de Razón) sobre actos que comprometen fondos públicos. \| Act: Fiscaliza a posteriori la legalidad de todos los actos adm. del GORE. | LAW-CGR-TOMA-RAZON-01, GORE-FIN-APROB-TRAM-CGR-01 |

#### 2.3. El Expediente Electrónico y la Firma Electrónica Avanzada (FEA)

ID: KB-GN-102-EXPEDIENTE-FEA-01
Purp: Detallar los instrumentos tecnológicos que son pilares del procedimiento administrativo moderno y que garantizan la validez, integridad y trazabilidad de los flujos de aprobación.

- Cpt: Expediente Electrónico
- Def: Conforme a la Ley N° 21.180, todo procedimiento debe constar en un expediente electrónico único que contenga el registro de todas las actuaciones, documentos, dictámenes e informes. Este expediente debe ser accesible para los interesados y garantiza la trazabilidad del flujo de aprobación.
- Cpt: Firma Electrónica Avanzada (FEA)
- Def: Mecanismo que sustituye la firma manuscrita, otorgando plena validez legal a los documentos electrónicos. Las resoluciones y decretos del Gobernador/a Regional, así como otros actos que la normativa especifique, deben ser firmados con FEA para ser válidos y ejecutorios.

### 3. Flujos de Aprobación para Actos Administrativos de Tramitación General

ID: KB-GN-102-FLUJOS-GENERALES-01
Purp: Modelar el flujo de trabajo estándar para la creación y aprobación de actos administrativos que no conllevan una imputación presupuestaria directa, como el nombramiento de comisiones, la aprobación de reglamentos internos o la respuesta a solicitudes ciudadanas. Este flujo sirve como base para procesos más complejos.

#### 3.1. Flujo para Resoluciones Exentas y Decretos (Sin Imputación Presupuestaria Directa)

ID: KB-GN-102-FLUJO-RES-EXENTA-01
Fnd: Este procedimiento se deduce de la aplicación de los principios de la Ley N° 19.880 y la estructura organizacional del GORE. La cadena de aprobación es tanto jerárquica como funcional, asegurando que un acto sea validado por la unidad con competencia técnica, la unidad con supervisión legal y la unidad con control procedimental antes de la firma ejecutiva.

- Cpt: Paso 1: Iniciación y Borrador
- Resp: Unidad GORE competente (ej. DAF, DIDESOH, etc.). Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: La unidad identifica la necesidad y elabora el borrador del acto administrativo (ej. Resolución Exenta), fundamentando debidamente las razones de hecho y de derecho que lo motivan.
- Cpt: Paso 2: Revisión Jurídica
- Resp: Asesoría Jurídica. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El borrador se remite a la Asesoría Jurídica para un control de legalidad, verificando que el acto se ajuste a la normativa vigente y a las competencias del GORE.
- Cpt: Paso 3: Visto Bueno (V°B°) de Control Interno
- Resp: Unidad de Control. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: La Unidad de Control revisa el borrador para asegurar su conformidad con los procedimientos internos y los principios de buena administración.
- Cpt: Paso 4: V°B° de Jefaturas y Administrador/a Regional
- Resp: Jefatura de División iniciadora; Administrador/a Regional. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El acto es visado por la jefatura de la división que lo origina. Posteriormente, es revisado y visado por el/la Administrador/a Regional, quien actúa como el último filtro de coordinación administrativa.
- Cpt: Paso 5: Firma del Gobernador/a
- Resp: Gobernador/a Regional. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: Una vez completados todos los V°B° internos, el acto es presentado al Gobernador/a para su firma mediante FEA. Ref: KB-GN-102-EXPEDIENTE-FEA-01
- Cpt: Paso 6: Notificación y Archivo
- Resp: Unidad GORE competente; Oficina de Partes. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El acto firmado se notifica a los interesados, si los hubiere, y se archiva en el expediente electrónico correspondiente. Ref: KB-GN-102-EXPEDIENTE-FEA-01
- Cpt: Control Externo
- Resp: Contraloría General de la República (CGR). Ref: KB-GN-102-ACTORES-MATRIZ-01
- Ctx: Por regla general, los actos que no comprometen recursos presupuestarios están exentos del trámite de Toma de Razón previo. Sin embargo, la CGR siempre conserva la facultad de ejercer un control de legalidad posterior sobre ellos.

### 4. Flujos de Aprobación para Iniciativas de Inversión (IDI) y Programas

ID: KB-GN-102-FLUJOS-INVERSION-01
Purp: Detallar los flujos de trabajo específicos para la aprobación de iniciativas que implican gasto, los cuales están altamente segmentados según el tipo, monto y naturaleza de la intervención.
Fnd: El primer paso crítico en este dominio es la correcta clasificación de la iniciativa para determinar la ruta de aprobación correspondiente, aplicando un principio de proporcionalidad en el control.

#### 4.1. Flujo Estándar del Sistema Nacional de Inversiones (SNI)

ID: KB-GN-102-FLUJO-SNI-ESTANDAR-01
Fnd: Corresponde al proceso de evaluación para Iniciativas de Inversión (IDI) de mayor complejidad o envergadura que requieren una evaluación técnica y económica completa por parte del Ministerio de Desarrollo Social y Familia (MDSF) para obtener la Recomendación Satisfactoria (RS).

| Paso | Responsable | Actividades Clave | Requisitos/Instrucciones | Resultado/Entregable | Ref. Normativa |
|-|-|-|-|-|-|
| 1 | Analista GORE (DIPIR) | Revisión Previa y Preparación | Act: Realizar revisión de fondo. \| Act: Verificar cumplimiento metodologías SNI. \| Act: Elaborar "Acta de Admisibilidad" interna. | IDI ADMISIBLE PARA ENVÍO A MDSF | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |
| 2 | Jefatura DIPIR / Gobernador/a | Envío Formal a MDSF | Act: Elaborar y visar oficio conductor solicitando evaluación ex-ante. \| Cpt: Cadena de V°B° interna culmina con firma del Gobernador/a. | Oficio despachado a SEREMI MDSF. | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |
| 3 | Analista MDSF | Análisis Técnico-Económico (ATE) | Act: MDSF realiza análisis de mérito técnico, económico y social. \| Dln: 5 días para admisibilidad, 10 días para ATE. | RATE: RS (Recomendado Satisfactorio), FI (Observado) u OT (Otro). | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |
| 4 | Unidad Formuladora / Analista GORE | Gestión del Resultado | Cond: Si es RS, avanza a financiamiento. \| Cond: Si es FI u OT, subsanar observaciones. \| Dln: Plazo máx. 60 días hábiles. | IDI con APROBADO TÉCNICAMENTE (RS) | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |
| 5 | Jefatura DIPIR | Priorización para Financiamiento | Act: Monitorear BIP. \| Act: Comunicar cartera de proyectos con RS al Gobernador/a para su priorización y eventual envío al CORE. | Cartera RS disponible para priorización. | GORE-IPR-PHASE2-TRACK-SNI-STANDARD-01 |

#### 4.2. Flujos Simplificados del SNI

ID: KB-GN-102-FLUJO-SNI-SIMPLIFICADO-01
Fnd: Para iniciativas de menor riesgo y costo, el sistema contempla vías de aprobación agilizadas que radican la responsabilidad de la aprobación técnica principalmente en el propio GORE.

##### 4.2.1. Proyectos de Inversión Menores a 5.000 UTM (Exentos de RS)

- Def: Proceso expedito donde la aprobación técnica no la otorga el MDSF, sino el propio GORE, tras verificar el cumplimiento de requisitos mínimos y enviar una "Carta de Responsabilidad" al MDSF informando que el proyecto no presenta impedimentos ni constituye un fraccionamiento.

##### 4.2.2. Proyectos de Conservación

- Def: Proceso específico para proyectos cuyo costo no supera el 30% del valor de reposición del activo. La evaluación del MDSF se limita a verificar la admisibilidad de la iniciativa como "Conservación", otorgando un resultado "AD" (Admisible para financiamiento), que es distinto y menos exigente que un RS completo.

#### 4.3. Flujo para Programas Públicos Regionales (Evaluación DIPRES/SES)

ID: KB-GN-102-FLUJO-PPR-GLOSA06-01
Fnd: Los programas de gasto corriente o mixto, financiados a través de la Glosa 06 de la Ley de Presupuestos, siguen un carril de evaluación completamente distinto al SNI. La aprobación técnica es otorgada por el nivel central (DIPRES y Subsecretaría de Evaluación Social) en un proceso de dos etapas.

- Cpt: Filtro 1: Evaluación de Pertinencia del Perfil
- Act: El GORE presenta un "Formulario de Perfil" conciso. DIPRES/SES evalúan si la iniciativa es pertinente y corresponde a un programa. Si es aprobado, se solicita al GORE elaborar el diseño detallado.
- Cpt: Filtro 2: Evaluación de Fondo del Diseño
- Act: El GORE elabora un "Formulario de Diseño" con Metodología de Marco Lógico (MML). DIPRES/SES realizan una revisión iterativa, enviando observaciones hasta que el diseño es subsanado y calificado como "RF (Recomendado Favorablemente)", lo que habilita su financiamiento.

### 5. Flujo de Aprobación para Modificaciones Presupuestarias

ID: KB-GN-102-FLUJOS-MOD-PPTO-01
Purp: Describir el proceso para ajustar el presupuesto regional aprobado. El flujo y el instrumento legal requerido dependen críticamente del alcance de la modificación: si afecta solo al presupuesto interno del GORE o si impacta la estructura presupuestaria nacional (Partida 31).

#### 5.1. Tipología de Modificaciones y Acto Administrativo Requerido

ID: KB-GN-102-MODPPTO-TIPOLOGIA-01
Fnd: La siguiente tabla clasifica los tipos de modificación presupuestaria y el acto administrativo que se requiere para su formalización, constituyendo una matriz de decisión clave para la gestión financiera.

| Tipo de Modificación | Descripción Breve | Afecta Presupuesto Partida 31 | Acto Administrativo Requerido | Ref. Normativa |
|-|-|-|-|-|
| Reasignación Presupuestaria Interna | Cpt: Movimiento de fondos entre subtítulos dentro del presupuesto GORE. | No | Solo Resolución GORE | GORE-FIN-MOD-TIPOS-ACTOS-01 |
| Creación Iniciativas FRPD | Cpt: Asignación de fondos desde provisión FRPD a proyectos específicos. | No | Solo Resolución GORE | GORE-FIN-MOD-TIPOS-ACTOS-01 |
| Suplemento Presupuestario | Cpt: Aumento de presupuesto por mayor aporte fiscal. | Sí | Decreto Supremo (DIPRES) y Resolución GORE | GORE-FIN-MOD-TIPOS-ACTOS-01 |
| Transferencia a Otros Organismos | Cpt: Reasignación desde FNDR para transferir a ministerio (consolidable). | Sí | Decreto Supremo (DIPRES) y Resolución GORE | GORE-FIN-MOD-TIPOS-ACTOS-01 |
| Financiamiento Emergencias (3%) | Cpt: Uso de fondo de emergencia para transferir a otra entidad. | Sí | Decreto Supremo (DIPRES) y Resolución GORE | GORE-FIN-MOD-TIPOS-ACTOS-01 |

#### 5.2. Proceso de Aprobación Interna: Rol del Consejo Regional (CORE) y sus Excepciones

ID: KB-GN-102-MODPPTO-CORE-01
Fnd: Por regla general, toda modificación que altere el presupuesto de inversión debe ser aprobada por el CORE. Sin embargo, la Ley de Presupuestos contempla excepciones para agilizar la gestión.

- Cpt: Aprobación CORE (Regla General)
- Proc: La propuesta de modificación es preparada por DIPIR (inversión) y DAF (funcionamiento), presentada por el Gobernador y sometida a votación del CORE. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Cpt: Excepciones a la Aprobación CORE
- Def: La Glosa 01 de la Ley de Presupuestos permite al Gobernador realizar ciertas modificaciones sin acuerdo previo del CORE, como aumentos de costo de proyectos en ejecución (hasta un 10% con tope de 7.000 UTM) o la aplicación del 3% para emergencias.
- Req: Aunque no requieren aprobación previa, el GORE debe informar mensualmente al CORE sobre estas modificaciones.

#### 5.3. Proceso de Aprobación Externa: Visación DIPRES y Toma de Razón CGR

ID: KB-GN-102-MODPPTO-EXTERNO-01
Fnd: Las modificaciones presupuestarias, incluso las exentas de aprobación del CORE, deben pasar por un riguroso control externo antes de su vigencia.

- Cpt: Paso 1: Visación por DIPRES
- Act: La resolución de modificación del GORE se envía a DIPRES para una revisión de cumplimiento normativo. DIPRES puede devolverla con observaciones para su corrección. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Cpt: Paso 2: Toma de Razón por CGR
- Act: Una vez visada por DIPRES, la resolución se remite a la CGR para el control preventivo de legalidad. Solo después de la Toma de Razón, el acto entra en vigencia y la DAF puede ajustar el presupuesto en SIGFE. Ref: KB-GN-102-ACTORES-MATRIZ-01

### 6. Flujo de Aprobación para Convenios y Transferencias de Recursos

ID: KB-GN-102-FLUJOS-CONVENIOS-01
Purp: Detallar el flujo para la formalización de la entrega de recursos a terceros, un proceso altamente regulado para gestionar el riesgo fiscal y asegurar la probidad y la correcta rendición de cuentas.
Fnd: La aprobación del convenio es un hito de control crítico que precede a cualquier desembolso.

#### 6.1. Flujo para Convenios de Transferencia a Terceros (Públicos y Privados)

ID: KB-GN-102-FLUJO-CONVENIO-01
Fnd: Este flujo transforma una decisión de financiamiento (ej. un acuerdo del CORE) en una obligación legal ejecutable, estableciendo el marco que regirá el uso y la rendición de los fondos públicos.

- Cpt: Paso 1: Elaboración del Borrador del Convenio
- Resp: División técnica proponente (ej. DIDESOH, DIPIR). Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: Se redacta el borrador del convenio, especificando claramente el objeto, monto, plazos, productos esperados, obligaciones de las partes y los mecanismos de rendición de cuentas.
- Cpt: Paso 2: Revisión Jurídica y Financiera
- Resp: Asesoría Jurídica; DAF. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El borrador es revisado por la Asesoría Jurídica para garantizar su legalidad (esp. transferencias a privados según Ley de Presupuestos: concurso, garantías, etc.). La DAF revisa las cláusulas financieras y de rendición.
- Cpt: Paso 3: Firma del Convenio
- Resp: Gobernador/a Regional; Representante Legal de la entidad receptora. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El convenio es firmado por ambas partes, formalizando el acuerdo de voluntades.
- Cpt: Paso 4: Emisión de Resolución Aprobatoria y Toma de Razón
- Resp: GORE; CGR. Ref: KB-GN-102-ACTORES-MATRIZ-01
- Act: El GORE emite una resolución que aprueba el convenio suscrito y autoriza la transferencia de fondos. Este acto, al comprometer gasto público, debe ser remitido obligatoriamente a CGR para su Toma de Razón.
- Warn: La transferencia de fondos no puede realizarse hasta que la CGR tome razón de la resolución.

### 7. Conclusiones

ID: KB-GN-102-CONCLUSIONES-01
Purp: Sintetizar las características estructurales del sistema de aprobación del GORE Ñuble.
Fnd: El análisis de los flujos de aprobación del GORE Ñuble revela un sistema de gobernanza complejo y multifacético, diseñado para equilibrar la autonomía regional con un estricto control de legalidad y probidad. Se identifican tres características estructurales clave:

- Cpt: Segmentación de Flujos por Proporcionalidad
- Def: El sistema no es monolítico; segmenta los flujos de trabajo basándose en la naturaleza, costo y riesgo de cada iniciativa. Actos de trámite general siguen una ruta ágil, mientras que las iniciativas de inversión y modificaciones presupuestarias se canalizan por vías diferenciadas y más rigurosas.
- Just: Este diseño aplica un principio de proporcionalidad, reservando los controles más exhaustivos y externos para las decisiones de mayor impacto fiscal y estratégico.
- Cpt: Gobernanza de Control Dual y Vetos Múltiples
- Def: La estructura de aprobación se fundamenta en una separación de poderes interna (Gobernador, CORE, Divisiones técnicas) y externa (CGR, DIPRES, MDSF).
- Just: Los organismos externos no son meros supervisores, sino "compuertas" obligatorias con poder de veto. Un flujo exitoso es la navegación a través de filtros políticos, técnicos, financieros y legales.
- Cpt: Centralidad del Control Externo y Preventivo
- Def: La Toma de Razón de la CGR constituye el hito de control preventivo más importante para todos los actos que comprometen el erario público.
- Just: Esta instancia asegura que ninguna obligación financiera se materialice sin un examen previo de su legalidad, actuando como el principal garante del buen uso de los recursos públicos antes del desembolso.

## Guía Integrada de Rendición de Cuentas: GORE Ñuble

ID: STS-KB-GN-RENDICION-MASTER-01
Version: 1.0.0
Status: Draft
Human-Creator: FSA
Human-Editor: Gemini-2.5-Pro
Model-Collaborator: IA-GEMINI
Creation-Date: 2024-07-28
Modification-Date: 2024-07-28
Primary-Source: kb_020_gestion_rendiciones.md (Original Version)
Ref-STS-Guide: GUIDE-STS-MASTER-01
Purp: Consolidar en un artefacto de conocimiento único, según estándar STS, el marco normativo, conceptual y operativo para la gestión de rendiciones de cuentas en el Gobierno Regional de Ñuble.

### SECCIÓN 1: Marco Conceptual y Normativox

ID: STS-KB-GN-RENDICION-MARCO-01
Purp: Establecer los fundamentos conceptuales y el marco legal que rigen la rendición de cuentas en el sector público chileno, con aplicabilidad directa al GORE Ñuble.

#### 1.1. Fundamentos y Principios

ID: STS-KB-GN-RENDICION-MARCO-CONCEPTOS-01

##### 1.1.1. Definición de Rendición de Cuentas

ID: STS-KB-GN-RENDICION-DEF-01
Src: @guia_rendiciones_gores.md, @generalidades_sistema_rendicion_electronica_cuentas_sisrec.md

- Def: Procedimiento administrativo y de control.
- Resp: Toda persona o entidad (pública/privada) que custodia, administra, recauda, recibe, invierte o paga fondos públicos.
- Obj: Demostrar y justificar la correcta utilización de dichos recursos.
- Req: Conforme a los fines para los cuales fueron otorgados.
- Req: En cumplimiento de la normativa vigente.
- Mssn: Comprobar cómo se realizó el ingreso, egreso o traspaso de los recursos públicos.
- Cpt: Deber de informar, explicar y responder por la gestión y resultados.

##### 1.1.2. Principios Rectores

ID: STS-KB-GN-RENDICION-PRINCIPIOS-01
Src: @guia_rendiciones_gores.md (Res. 30/2015 CGR)

- Cpt: Legalidad. Def: Gastos amparados por ley y disposiciones reglamentarias.
- Cpt: Veracidad-Fidelidad. Def: Información y documentación deben ser auténticas, íntegras y reflejar fielmente las operaciones.
- Cpt: Acreditación. Def: Todo ingreso, egreso o traspaso debe estar debidamente documentado con comprobantes auténticos.
- Cpt: Exactitud. Def: Cálculos y montos deben ser precisos.
- Cpt: Oportunidad. Def: Rendiciones deben presentarse en los plazos establecidos.
- Cpt: Transparencia. Def: Proceso y resultados deben ser accesibles al control ciudadano y fiscalizador.
- Cpt: Eficiencia-Eficacia. Def: Uso de fondos debe orientarse al logro de objetivos institucionales de manera óptima.
- Cpt: Probidad. Def: Actuación recta y leal, con preeminencia del interés general sobre el particular. Ref: STS-KB-GN-RENDICION-NORMA-LOCBGAE-01.

#### 1.2. Jerarquía Normativa Aplicable

ID: STS-KB-GN-RENDICION-MARCO-NORMATIVA-01
Purp: Detallar el conjunto de normas, desde la Constitución hasta las resoluciones específicas, que regulan la rendición de cuentas para el GORE Ñuble.
Ref: @kb_022_compendios_legales.md

##### 1.2.1. Constitución Política de la República

ID: STS-KB-GN-RENDICION-NORMA-CPR-01
Src: @guia_rendiciones_gores.md

- Fnd: Art-3. Cpt: Principios de responsabilidad, eficiencia, control, probidad, transparencia como base para la rendición.
- Fnd: Art-8. Cpt: Principio de probidad como obligación; publicidad de actos como base de transparencia.
- Fnd: Art-98-99. Cpt: Establece a Contraloría General de la República (CGR) como órgano autónomo de control, con facultad para examinar y juzgar cuentas.
- Fnd: Art-111-ss. Cpt: Regulación de GORE, cuya autonomía se ejerce dentro del marco legal, implicando la obligación de rendir cuentas.

##### 1.2.2. Resolución N° 30 de 2015, CGR

ID: STS-KB-GN-RENDICION-NORMA-RES30-01
Src: @resolucion_30_2015_cgr_rendicion_cuentas.txt

- Def: Norma de procedimiento sobre rendición de cuentas, de aplicación obligatoria para GORE Ñuble.
- Fnd: Art-1. Ctx: Ámbito de aplicación incluye a GORE y cualquier entidad (pública/privada) que reciba fondos de éste.
- Fnd: Art-2. Def: Define la constitución del expediente de rendición. Ref: STS-KB-GN-RENDICION-PROCESO-EXPEDIENTE-COMPONENTES-01.
- Fnd: Art-4. Def: Define "documentación auténtica" en papel (original).
- Fnd: Art-5-9. Cpt: Regula documentación electrónica/digital, requiere autorización CGR para su uso, define autenticidad y validez de firma electrónica.
- Fnd: Art-10. Def: Define "expediente de rendición de cuentas".
- Fnd: Art-13. Cpt: Regla general de gastos posteriores a total tramitación del acto que autoriza la transferencia.
- Fnd: Art-18. Prohib: Entregar nuevos fondos si hay rendiciones exigibles pendientes.
- Fnd: Art-26. Cpt: Regula rendición de transferencias a otros servicios públicos.
- Fnd: Art-27. Cpt: Regula rendición de transferencias a entidades privadas.
- Fnd: Art-31. Req: Obligación de restituir fondos no rendidos, observados o no ejecutados.

##### 1.2.3. Ley N° 18.575 (LOCBGAE)

ID: STS-KB-GN-RENDICION-NORMA-LOCBGAE-01
Src: @guia_rendiciones_gores.md

- Cpt: Ley Orgánica Constitucional de Bases Generales de la Administración del Estado.
- Fnd: Art-3. Req: Reitera principios de responsabilidad, eficiencia, probidad y transparencia.
- Fnd: Art-52-53. Def: Probidad administrativa como conducta funcionaria intachable y desempeño honesto y leal, con preeminencia del interés general. Ctx: La rendición es un mecanismo de verificación de este principio.

##### 1.2.4. Ley N° 19.880 (LBPA)

ID: STS-KB-GN-RENDICION-NORMA-LBPA-01
Src: @guia_rendiciones_gores.md

- Cpt: Ley de Bases de los Procedimientos Administrativos.
- Fnd: Art-5, 16bis, 18, 19. Cpt: Consagra el principio de escrituración electrónica, el expediente electrónico y el uso de plataformas electrónicas. Ctx: Sienta las bases para la digitalización de la rendición.

##### 1.2.5. Ley de Presupuestos del Sector Público (Anual)

ID: STS-KB-GN-RENDICION-NORMA-LEYPPTOS-01
Src: @guia_rendiciones_gores.md, @kb_021_extractos_legales.md

- Nat: Fuente normativa primordial de aplicación directa y anual.
- Fnd: Art-23-26 (ej. Ley 2025). Cpt: Marco estricto para transferencias a privados (concurso, convenio, rendición vía SISREC, garantías, prohibiciones). Req: Obligatorio para GORE.
- Cpt: Glosas-Partida-31-(GORE). Ctx: Contienen instrucciones operativas cruciales.
  - Cpt: Glosa-06. Req: Regula oferta programática GORE (S.24 inversión), evaluación ex ante DIPRES/SES, tope 5% gastos adm.
  - Cpt: Glosa-07. Req: Regula 8% FNDR para subvenciones (cultura, deporte, etc.).
  - Cpt: Glosa-12. Req: Regula Fondo Regional de Iniciativa Local (FRIL).
  - Cpt: Glosa-13. Req: Regula Fondo Regional para la Productividad y el Desarrollo (FRPD).

##### 1.2.6. Ley N° 21.180 (Transformación Digital del Estado)

ID: STS-KB-GN-RENDICION-NORMA-LEY21180-01
Src: @guia_rendiciones_gores.md

- Purp: Mandata la digitalización de procedimientos administrativos.
- Res: Consolida la obligación de tramitar rendiciones por medios electrónicos, usar expedientes electrónicos y firma electrónica.

##### 1.2.7. Ley N° 21.719 (Protección de Datos Personales)

ID: STS-KB-GN-RENDICION-NORMA-LEY21719-01
Src: @guia_rendiciones_gores.md, @kb_021_extractos_legales.md

- Purp: Marco robusto para el tratamiento de datos personales.
- Req: GORE debe tratar datos personales en expedientes de rendición y en publicaciones de transparencia respetando principios de licitud, finalidad, proporcionalidad y seguridad. Ctx: Especial cuidado con datos sensibles de beneficiarios.

##### 1.2.8. Resolución Exenta N° 1.858 de 2023, CGR

ID: STS-KB-GN-RENDICION-NORMA-RES1858-01
Src: @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md

- Purp: Establece el uso obligatorio del Sistema de Rendición Electrónica de Cuentas (SISREC).
- Ctx: Para todos los servicios públicos, municipalidades y otros organismos que transfieren recursos de Subtítulos 24 (Transferencias Corrientes) y 33 (Transferencias de Capital).
- Req: Obliga al GORE Ñuble y a sus entidades ejecutoras a utilizar SISREC según el cronograma de implementación de CGR.

### SECCIÓN 2: Actores y Responsabilidades

ID: STS-KB-GN-RENDICION-ACTORES-01
Purp: Definir los roles y responsabilidades de cada actor involucrado en el ciclo de rendición de cuentas del GORE Ñuble.
Src: @guia_rendiciones_gores.md, @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md

#### 2.1. Actores Internos GORE Ñuble

ID: STS-KB-GN-RENDICION-ACTORES-INTERNOS-01

##### 2.1.1. Gobernador/a Regional

ID: STS-KB-GN-RENDICION-ACTOR-GOBERNADOR-01

- Cpt: Rol. Def: Máxima autoridad ejecutiva. Responsable final de la correcta inversión de todos los fondos.
- Cpt: Funciones.
  - Req: Aprobar mediante resolución los convenios de transferencia.
  - Req: Velar por el funcionamiento de un sistema de control interno adecuado para rendiciones.
  - Req: Representar al GORE ante organismos de control externo.

##### 2.1.2. Consejo Regional (CORE)

ID: STS-KB-GN-RENDICION-ACTOR-CORE-01

- Cpt: Rol. Def: Órgano fiscalizador.
- Cpt: Funciones.
  - Req: Fiscalizar actos del GORE, incluyendo ejecución presupuestaria y uso de fondos.
  - Req: Requerir informes sobre estado de rendiciones.
  - Req: Considerar historial de rendiciones de ejecutores al aprobar nuevos fondos.

##### 2.1.3. Administrador/a Regional

ID: STS-KB-GN-RENDICION-ACTOR-ADMREG-01

- Cpt: Rol. Def: Coordinador de la gestión administrativa interna.
- Cpt: Funciones.
  - Req: Supervisar la eficiencia de los procesos de rendición.
  - Req: Coordinar acción de divisiones involucradas (DAF, DIPIR, Unidades Técnicas).

##### 2.1.4. División de Administración y Finanzas (DAF)

ID: STS-KB-GN-RENDICION-ACTOR-DAF-01

- Cpt: Rol. Def: Unidad central en la gestión financiera y administrativa de las rendiciones.
- Cpt: Funciones.
  - Req: Elaborar convenios y resoluciones de pago.
  - Req: Recepcionar, registrar y custodiar expedientes de rendición.
  - Req: Realizar revisión financiera y de legalidad de gastos rendidos.
  - Req: Contabilizar en SIGFE.
  - Req: Gestionar SISREC como entidad otorgante (roles Administrador y Encargado Otorgante usualmente radican aquí).

##### 2.1.5. Unidad de Control de Rendiciones (U.C.R.)

ID: STS-KB-GN-RENDICION-ACTOR-UCR-01
Ctx: Unidad especializada dentro de la DAF, según modelo de @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md. Rec: Buena práctica.

- Cpt: Rol. Def: Centraliza y especializa el proceso de control de rendiciones.
- Cpt: Funciones.
  - Req: Registrar rendiciones en base de datos de programas.
  - Req: Derivar a Referentes Técnicos para revisión.
  - Req: Controlar antecedentes para contabilización.
  - Req: Contabilizar en SIGFE.
  - Req: Archivar expedientes.
  - Req: Supervisar tiempos de revisión de los referentes.

##### 2.1.6. Divisiones Técnicas (DIPIR, DIDESOH, DIFOI, DIT)

ID: STS-KB-GN-RENDICION-ACTOR-DIVISIONES-01

- Cpt: Rol. Def: Albergan a los Referentes Técnicos y Financieros (RTF) de proyectos/programas.
- Cpt: Funciones.
  - Req: Definir aspectos técnicos en convenios.
  - Req: Realizar seguimiento técnico de la ejecución.
  - Req: Revisar coherencia de gastos rendidos con avance físico.
  - Req: Emitir informes técnicos de aprobación/observación de rendiciones.

##### 2.1.7. Referente Técnico-Financiero (RTF)

ID: STS-KB-GN-RENDICION-ACTOR-RTF-01

- Cpt: Rol. Def: Primera línea de revisión y seguimiento de un proyecto/programa.
- Cpt: Funciones.
  - Req: Supervisar cumplimiento del convenio.
  - Req: Vigilar que la entidad ejecutora rinda mensualmente (o según plazo).
  - Req: Revisar detalladamente rendiciones (técnica y financiera).
  - Req: Solicitar subsanación de observaciones.
  - Req: Aprobar técnicamente la rendición y derivar a DAF/U.C.R.
- Cpt: Rol-SISREC. Def: Corresponde al "Analista Otorgante". Src: @generalidades_sistema_rendicion_electronica_cuentas_sisrec.md

##### 2.1.8. Unidad de Control Interno del GORE

ID: STS-KB-GN-RENDICION-ACTOR-CONTROLINTERNO-01

- Cpt: Rol. Def: Control preventivo y posterior de la legalidad.
- Cpt: Funciones.
  - Req: Auditar selectivamente procesos de transferencia y rendición.
  - Req: Asesorar a divisiones en procedimientos de control.
  - Req: Informar al Gobernador y al CORE sobre hallazgos y recomendaciones.

#### 2.2. Entidades Ejecutoras

ID: STS-KB-GN-RENDICION-ACTORES-EJECUTORES-01

- Cpt: Rol. Def: Receptoras de fondos GORE. Principales responsables de la correcta ejecución y rendición.
- Cpt: Deberes.
  - Req: Usar fondos exclusivamente para fines convenidos.
  - Req: Administrar con probidad, eficiencia y transparencia.
  - Req: Llevar registros y documentación de respaldo completa y fidedigna.
  - Req: Presentar rendiciones en forma y plazos establecidos (vía SISREC).
  - Req: Subsanar observaciones oportunamente.
  - Req: Reintegrar fondos no utilizados o mal rendidos.

##### 2.2.1. Municipalidades

ID: STS-KB-GN-RENDICION-EJECUTOR-MUNI-01

- Ctx: Receptoras de FNDR, FRIL, 8% FNDR.
- Req: Obligadas a usar SISREC para rendir al GORE (Res. Ex. 1858/2023 CGR).

##### 2.2.2. Otros Servicios Públicos Sectoriales

ID: STS-KB-GN-RENDICION-EJECUTOR-SSPP-01

- Ctx: SERVIU, Vialidad, etc.
- Req: Rinden al GORE según convenio.
- Req: CGR examina inversión en sede del servicio ejecutor (Res. 30 CGR, Art. 26).

##### 2.2.3. Entidades Privadas (Corporaciones, Fundaciones, ONGs)

ID: STS-KB-GN-RENDICION-EJECUTOR-PRIVADO-01

- Ctx: Receptoras de 8% FNDR, FRPD, etc.
- Req: Sujetas a marco regulatorio estricto (Ley Presupuestos Art. 23-26).
- Req: Inscripción en Registro de Colaboradores del Estado (Ley 19.862).
- Req: Obligadas a usar SISREC para rendir al GORE.

#### 2.3. Organismos de Control Externo

ID: STS-KB-GN-RENDICION-ACTORES-EXTERNOS-01

##### 2.3.1. Contraloría General de la República (CGR)

ID: STS-KB-GN-RENDICION-EXTERNO-CGR-01

- Cpt: Rol. Def: Principal órgano de control externo.
- Cpt: Funciones.
  - Req: Ejercer control de legalidad de actos GORE (Toma de Razón).
  - Req: Fiscalizar ingreso e inversión de fondos GORE.
  - Req: Examinar y juzgar cuentas rendidas.
  - Req: Realizar auditorías financieras y de cumplimiento.
  - Req: Formular reparos e iniciar Juicios de Cuentas.
  - Req: Administrar y establecer uso obligatorio de SISREC.

##### 2.3.2. Dirección de Presupuestos (DIPRES)

ID: STS-KB-GN-RENDICION-EXTERNO-DIPRES-01

- Cpt: Rol. Def: Control y seguimiento de ejecución presupuestaria y programática.
- Cpt: Funciones.
  - Req: Monitorear ejecución presupuestaria GORE vía SIGFE.
  - Req: Evaluar programas públicos regionales (ex ante, durante, ex post).
  - Req: Velar por cumplimiento de glosas presupuestarias.

### SECCIÓN 3: El Proceso Operativo de Rendición de Cuentas

ID: STS-KB-GN-RENDICION-PROCESO-01
Purp: Describir la documentación requerida y los flujos de trabajo para la gestión de rendiciones en el GORE Ñuble, distinguiendo la modalidad legado de la modalidad estándar vía SISREC.

#### 3.1. Documentación y Expediente de Rendición

ID: STS-KB-GN-RENDICION-PROCESO-EXPEDIENTE-01

##### 3.1.1. Componentes Esenciales

ID: STS-KB-GN-RENDICION-PROCESO-EXPEDIENTE-COMPONENTES-01
Src: @resolucion_30_2015_cgr_rendicion_cuentas.txt (Art. 2)

- Cpt: Informe de Rendición de Cuentas. Def: Documento formal de la entidad ejecutora que resume la gestión. Ctx: En SISREC, es el informe electrónico firmado con FEA.
- Cpt: Comprobantes de Ingresos. Def: Documentación que acredita recepción de fondos.
- Cpt: Comprobantes de Egresos. Def: Documentación auténtica que respalda cada desembolso. Ref: STS-KB-GN-RENDICION-PROCESO-EXPEDIENTE-DOCS-01.
- Cpt: Comprobantes de Traspasos. Def: Documentos de operaciones contables sin movimiento de efectivo.
- Cpt: Registro Ley N° 19.862. Ctx: Cuando corresponda (transferencias a privados).
- Cpt: Medios de Verificación. Def: Evidencia de cumplimiento de objetivos (informes técnicos, fotos, listas, etc.).

##### 3.1.2. Documentación Auténtica y de Respaldo

ID: STS-KB-GN-RENDICION-PROCESO-EXPEDIENTE-DOCS-01
Src: @resolucion_30_2015_cgr_rendicion_cuentas.txt (Art. 4, 5)

- Cpt: Soporte Papel. Def: Documento original. Copias solo si son autentificadas por ministro de fe o funcionario autorizado.
- Cpt: Soporte Electrónico. Def: Documento electrónico según Ley 19.799 (con firma electrónica).
- Cpt: Documento Digitalizado. Def: Se considera copia simple, salvo que sea autentificado con firma electrónica. Ctx: En SISREC, el Ministro de Fe del ejecutor cumple esta función.
- Cpt: Tipos Comunes. Def: Facturas y boletas electrónicas (verificables en SII), contratos, liquidaciones de sueldo, comprobantes de pago de cotizaciones, comprobantes de transferencia bancaria, actas de recepción.

#### 3.2. Flujo de Proceso Sin SISREC (Modalidad Legado)

ID: STS-KB-GN-RENDICION-PROCESO-SIN-SISREC-01
Ctx: Para convenios antiguos no migrados a SISREC.
Src: @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md (Sec. 7.1)

1. Resp: EE. Act: Prepara y presenta rendición en papel/digital a Oficina de Partes (OP) GORE. Dln: 15 días hábiles del mes siguiente.
2. Resp: OP. Act: Recepciona, registra y deriva a U.C.R./DAF. Dln: 2 días hábiles (GORE).
3. Resp: U.C.R./DAF. Act: Registra en B.D. interna y deriva a RTF. Dln: 2 días hábiles (GORE).
4. Resp: RTF. Act: Revisa técnica y financieramente. Dln: 7 días hábiles (GORE).
    - Cond: Si OK. Res: Emite certificado de aprobación y devuelve a U.C.R./DAF.
    - Cond: Si Observa. Res: Comunica a EE para subsanación. Dln: 2 días hábiles (GORE) para comunicar. EE reingresa correcciones.
5. Resp: U.C.R./DAF. Act: Recibe rendición aprobada por RTF, realiza control final (checklist). Dln: 4 días hábiles (GORE).
6. Resp: U.C.R./DAF. Act: Contabiliza en SIGFE. Dln: 2 días hábiles (GORE).
7. Resp: U.C.R./DAF. Act: Archiva expediente. Dln: 1 día hábil (GORE).

#### 3.3. Flujo de Proceso Con SISREC (Modalidad Estándar)

ID: STS-KB-GN-RENDICION-PROCESO-CON-SISREC-01
Ctx: Procedimiento obligatorio para nuevas transferencias S.24 y S.33.
Src: @generalidades_sistema_rendicion_electronica_cuentas_sisrec.md, @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md (Sec. 7.2)

##### 3.3.1. Flujo Entidad Otorgante (GORE)

ID: STS-KB-GN-RENDICION-SISREC-GORE-01

1. Resp: Analista-Otorgante (RTF).
    - Act: Crea Programa/Proyecto en SISREC.
    - Act: Registra y envía transferencia a Ejecutor.
    - Act: Recibe y revisa rendición del Ejecutor. Dln: 7 días hábiles (GORE).
    - Act: Aprueba/Observa cada transacción.
    - Act: Envía a Encargado Otorgante para firma.
2. Resp: Encargado-Otorgante (Jefe DAF).
    - Act: Recibe rendición del Analista.
    - Act: Revisa propuesta.
    - Cond: Si Observa. Res: Devuelve rendición al Ejecutor con FEA. Dln: 1 día hábil (GORE) para devolver.
    - Cond: Si Aprueba. Res: Firma Informe de Aprobación (total/parcial) con FEA.
3. Resp: Analista-Otorgante (RTF).
    - Act: Descarga Informe de Aprobación firmado.
    - Act: Deriva a U.C.R./DAF para contabilización.
4. Resp: U.C.R./DAF.
    - Act: Recibe informe.
    - Act: Contabiliza en SIGFE. Dln: 2 días hábiles (GORE).
    - Act: Archiva registro. Dln: 2 días hábiles (GORE).

##### 3.3.2. Flujo Entidad Ejecutora

ID: STS-KB-GN-RENDICION-SISREC-EJECUTOR-01

1. Resp: Analista-Ejecutor.
    - Act: Recibe y acepta transferencia del GORE en SISREC.
    - Act: Crea informe de rendición (mensual, regularización, sin movimiento). Dln: 15 días hábiles mes siguiente.
    - Act: Ingresa transacciones y adjunta documentos de respaldo digitalizados.
    - Act: Envía a Ministro de Fe.
2. Resp: Ministro-de-Fe-Ejecutor.
    - Act: Revisa autenticidad de documentos.
    - Cond: Si OK. Res: Aprueba/certifica y pasa a Encargado Ejecutor.
    - Cond: Si Observa. Res: Devuelve a Analista Ejecutor.
3. Resp: Encargado-Ejecutor.
    - Act: Revisa rendición.
    - Cond: Si OK. Res: Firma Informe de Rendición con FEA y envía al GORE.
    - Cond: Si Observa. Res: Devuelve a Analista Ejecutor.
4. Resp: Analista-Ejecutor (si hay devolución del GORE).
    - Act: Recibe rendición observada.
    - Act: Crea informe de "Regularización".
    - Act: Corrige transacciones observadas y reenvía por el mismo flujo.

### SECCIÓN 4: Rendición por Tipología de Fondos

ID: STS-KB-GN-RENDICION-FONDOS-01
Purp: Detallar las particularidades de la rendición de cuentas para los principales fondos y programas gestionados por el GORE Ñuble.
Src: @guia_rendiciones_gores.md, @extractos_normativos_clave_gore_2025.md (Ley Presupuestos y Glosas)

#### 4.1. Fondo Nacional de Desarrollo Regional (FNDR)

ID: STS-KB-GN-RENDICION-FONDOS-FNDR-01

##### 4.1.1. Iniciativas de Inversión (Subtítulo 31 - Ejecución Directa GORE)

ID: STS-KB-GN-RENDICION-FNDR-S31-01

- Ctx: Obras, adquisición de activos, estudios de preinversión ejecutados directamente por el GORE.
- Ref: @kb_024_guia_idi_sni.md
- Cpt: Rendición. Def: Rendición interna de gastos y cumplimiento de etapas.
- Cpt: Respaldo Clave. Ex: Contratos (Ley 19.886), estados de pago visados por ITO, facturas de contratistas, resoluciones de adjudicación, boletas de garantía.
- Cpt: Sistema. Req: Los gastos se imputan al código BIP del proyecto en SIGFE. Se actualiza avance físico-financiero en plataforma BIP.
- Cpt: Contabilización. Proc: La DAF verifica disponibilidad y correcta imputación en S.31 del presupuesto GORE.
- Cpt: Cierre. Req: Se debe completar Carpeta Digital Ex Post en BIP al finalizar el proyecto.

##### 4.1.2. Transferencias de Capital (Subtítulo 33 - Ejecución por Terceros)

ID: STS-KB-GN-RENDICION-FNDR-S33-01

- Ctx: Modalidad más común. GORE transfiere a Municipalidades, Servicios Públicos o (excepcionalmente) privados para ejecutar proyectos con RS.
- Ref: @kb_024_guia_idi_sni.md
- Fnd: Convenio de Transferencia que detalla proyecto (código BIP), monto, plazos y obligaciones.
- Cpt: Rendición Ejecutor. Req: Obligatoria vía SISREC, presentando informe, comprobantes de gasto, informes de avance físico-financiero y actas de recepción de obras.
- Cpt: Revisión GORE. Proc: El RTF revisa coherencia técnica-financiera, y DAF/U.C.R. la legalidad y documentación.

##### 4.1.3. Fondo Regional de Iniciativa Local (FRIL)

ID: STS-KB-GN-RENDICION-FONDOS-FRIL-01

- Ctx: Asignación FNDR para proyectos de inversión de pequeña escala de municipalidades.
- Fnd: Guía Operativa FRIL SUBDERE e instructivo regional del GORE.
- Ref: @kb_026_guia_fril.md
- Cpt: Exención RS. Req: Proyectos < 5.000 UTM exentos de RS, pero deben registrarse en BIP.
- Prohib: Financiar proyectos por etapas o fraccionados.
- Cpt: Rendición. Proc: Las municipalidades rinden al GORE vía SISREC, acreditando gastos y avance de obras.
- Cpt: Supervisión GORE. Proc: Se verifica cumplimiento de la guía operativa y el correcto uso de la exención de RS.

##### 4.1.4. Fondo Regional para la Productividad y el Desarrollo (FRPD)

ID: STS-KB-GN-RENDICION-FONDOS-FRPD-01

- Ctx: Fondos de Royalty Minero para iniciativas de innovación, competitividad y CTI.
- Fnd: Resolución Exenta N°33/2024 Subsecretaría CTCI y glosas presupuestarias.
- Ref: @kb_027_guia_frpd.md
- Resp: Universidades, centros de investigación, corporaciones, empresas.
- Cpt: Rendición. Req: Vía SISREC. Debe acreditar no solo el gasto financiero, sino también el logro de hitos, productos y resultados de I+D+i comprometidos.
- Cpt: Supervisión GORE. Proc: La DIFOI y DIPIR realizan seguimiento técnico verificando cumplimiento de metas.

##### 4.1.5. Subvenciones de Vinculación con la Comunidad (8% FNDR)

ID: STS-KB-GN-RENDICION-FONDOS-SUBV8-01

- Ctx: Fondos concursables para cultura, deporte, seguridad, medio ambiente, destinados a municipalidades y entidades privadas sin fines de lucro.
- Fnd: Glosa 07 Ley de Presupuestos, bases del concurso del GORE, instructivo regional.
- Ref: @kb_028_guia_subv8.md
- Cpt: Rendición. Req: Vía SISREC. Énfasis en la coherencia del gasto con el proyecto adjudicado.
- Cpt: Respaldo Clave. Ex: Boletas de honorarios (con pago de cotizaciones), facturas por bienes/servicios específicos de la actividad.
- Cpt: Medios de Verificación. Req: Listas de asistencia, fotos, material de difusión son cruciales.
- Cpt: Restricciones. Req: Las bases establecen gastos prohibidos (operativos, premios en dinero, alcohol, etc.) que deben ser fiscalizados.

##### 4.1.6. Programas FNDR (Subtítulo 24 Inversión - Ejecución Directa GORE)

ID: STS-KB-GN-RENDICION-FONDOS-PROG-GLOSA06-01

- Ctx: Programas ejecutados directamente por el GORE.
- Fnd: Glosa 06 Ley de Presupuestos, evaluación ex ante DIPRES/SES.
- Ref: @kb_025_guia_programas.md
- Cpt: Gasto Adm. Req: Hasta 5% del programa puede destinarse a gastos de administración del GORE (honorarios S.21, consumo S.22), imputados con cargo al presupuesto del programa.
- Cpt: Rendición Interna. Proc: La DAF debe controlar el tope del 5% y la correcta imputación.
- Cpt: Rendición Externa. Proc: Se rinde el cumplimiento de los componentes y metas del programa, en coherencia con el diseño aprobado en la evaluación ex ante.

##### 4.1.7. Conservación de Infraestructura (Circular 33)

ID: STS-KB-GN-RENDICION-FONDOS-C33-01

- Ctx: Iniciativas de mantención/reparación de infraestructura pública que no afectan capacidad original.
- Fnd: Oficio Circular N°33/2009 MINHAC, NIP 2025.
- Ref: @kb_029_guia_circ33.md
- Proc: BIP. Req: Obtener RATE "AD (Admisible para Financiamiento)" del MDSF.
- Prohib: Costo de reparación > 30% del costo de reposición del activo. Cond: Si supera, debe ir a SNI estándar.
- Cpt: Rendición. Proc: Sigue flujo estándar de proyecto de inversión, acreditando ejecución de partidas de conservación.

### SECCIÓN 5: Control, Fiscalización y Transparencia

ID: STS-KB-GN-RENDICION-CONTROL-01
Purp: Describir los mecanismos de control, el rol de la fiscalización externa y las obligaciones de transparencia asociadas a las rendiciones.
Src: @guia_rendiciones_gores.md

#### 5.1. Control Interno GORE

ID: STS-KB-GN-RENDICION-CONTROL-INTERNO-01

- Purp: Asegurar la correcta administración y rendición desde dentro de la institución.
- Mech: Unidad de Control Interno. Proc: Realiza revisión preventiva y auditorías selectivas sobre el proceso de rendición. Informa al Gobernador y al CORE.
- Mech: Listas de Chequeo. Proc: Aplicación de checklists estandarizadas para la revisión formal, documental, financiera y técnica de cada rendición. Ref: Anexo 10.3 @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md
- Mech: Seguimiento Físico-Financiero. Proc: Verificación de que el gasto se traduce en avances concretos. Req: Implica análisis integrado de informes de rendición y de avance técnico, y visitas a terreno por parte de los RTF.

#### 5.2. Fiscalización Externa

ID: STS-KB-GN-RENDICION-CONTROL-EXTERNO-01

- Purp: Control ejercido por organismos externos al GORE.
- Resp: Contraloría General de la República (CGR).
  - Act: Examen y Juzgamiento de Cuentas. Verifican legalidad, fidelidad y exactitud de rendiciones.
  - Act: Auditorías. Realizan auditorías financieras y de cumplimiento al GORE.
  - Act: Observaciones y Reparos. Formulan objeciones que el GORE debe subsanar.
  - Act: Juicio de Cuentas. Inician procedimiento para determinar responsabilidades pecuniarias ante perjuicio fiscal.
- Resp: Dirección de Presupuestos (DIPRES).
  - Act: Monitoreo. Siguen la ejecución presupuestaria y programática del GORE.
  - Act: Evaluación. Realizan evaluación de programas regionales para medir su eficacia.

#### 5.3. Transparencia y Acceso a la Información

ID: STS-KB-GN-RENDICION-CONTROL-TRANSPARENCIA-01

- Purp: Deber del GORE de transparentar el uso de los fondos públicos.
- Fnd: Ley N° 20.285. Ref: @kb_021_extractos_legales.md#RLAIP-01
- Req: Transparencia Activa. Cpt: Publicación proactiva y mensual en el sitio web del GORE de:
  - Convenios de transferencia.
  - Detalle de transferencias (beneficiario, monto, objeto).
  - Nóminas de beneficiarios de programas.
  - Presupuesto y su ejecución.
  - Resultados de auditorías.
- Req: Transparencia Pasiva. Cpt: Responder a solicitudes de acceso a la información de la ciudadanía sobre rendiciones de cuentas, dentro de los plazos legales, resguardando datos personales sensibles.

### SECCIÓN 6: Responsabilidades y Sanciones

ID: STS-KB-GN-RENDICION-RESPONSABILIDAD-01
Purp: Detallar el régimen de responsabilidades y las posibles sanciones derivadas de irregularidades en el proceso de rendición.
Src: @guia_rendiciones_gores.md, @kb_021_extractos_legales.md

- Cpt: Responsabilidad Administrativa.
  - Cause: Infracción a deberes de cuidado, supervisión o probidad por parte de funcionarios GORE.
  - Proc: Sumario administrativo. Ref: @kb_021_extractos_legales.md#ESTATUTO-ADMIN-ART119-01
  - Res: Sanción de censura, multa, suspensión o destitución (Ley 18.834).
- Cpt: Responsabilidad Civil.
  - Cause: Perjuicio patrimonial al Fisco por acción negligente o dolosa.
  - Proc: Juicio de Cuentas (ante CGR) o demanda civil (ante tribunales).
  - Res: Orden de restituir los fondos.
- Cpt: Responsabilidad Penal.
  - Cause: Hechos constitutivos de delito (malversación, fraude al fisco, cohecho).
  - Proc: Investigación por Ministerio Público, juicio en tribunales penales.
  - Res: Sanción de multas, inhabilitación, penas privativas de libertad.
- Cpt: Consecuencia Directa - Obligación de Restituir Fondos.
  - Cause: Rendición no presentada, no aprobada u observada por CGR.
  - Res: Genera obligación de reintegro (Res. 30 CGR, Art. 31).
- Cpt: Consecuencia Directa - Suspensión de Nuevas Transferencias.
  - Cause: Existencia de rendiciones exigibles pendientes.
  - Res: GORE no debe entregar nuevos fondos (Res. 30 CGR, Art. 18).

### SECCIÓN 7: Gestión Estratégica y Contingencias

ID: STS-KB-GN-RENDICION-GESTION-01
Purp: Ofrecer recomendaciones para una gestión de excelencia y planes para contingencias operativas.
Src: @guia_rendiciones_gores.md, @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md

#### 7.1. Buenas Prácticas

ID: STS-KB-GN-RENDICION-GESTION-BPR-01

- Rec: Planificación Anual. Calendarizar rendiciones y programar revisiones internas.
- Rec: Coordinación Interdivisional. Fortalecer comunicación entre DAF, DIPIR y unidades técnicas con roles claros.
- Rec: Capacitación Continua. A funcionarios GORE y a entidades ejecutoras, especialmente en uso de SISREC.
- Rec: Uso Óptimo de Tecnología. Integrar y aprovechar plenamente SIGFE, BIP y SISREC.
- Rec: Manuales Internos. Desarrollar y mantener actualizados manuales de procedimientos y protocolos claros.
- Rec: Gestión de Riesgos. Identificar riesgos (ej. fraude, errores, demoras) y establecer medidas preventivas y de control.
- Rec: Fomento de Cultura de Probidad. Liderazgo comprometido con la transparencia y la rendición de cuentas.
- Rec: Enfoque en Resultados. Articular la rendición financiera con la medición de resultados e impacto de los proyectos/programas.

#### 7.2. Contingencias y Planes de Acción

ID: STS-KB-GN-RENDICION-GESTION-CONTINGENCIAS-01
Src: @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md (Sec 7.3)

- Cpt: Contingencia - Pérdida de Rendición al Interior del GORE.
  - Proc: Mantener libro de correspondencia/registro digital en cada unidad (OP, U.C.R., RTF) para asegurar trazabilidad. Como último recurso, solicitar copia a entidad ejecutora. Warn: SISREC minimiza este riesgo.
- Cpt: Contingencia - Entidad Privada solicita cuota siguiente sin haber rendido la anterior.
  - Proc: Aplicar Art. 18, Res. 30 CGR. Si el convenio lo permite, GORE puede autorizar el adelanto si la entidad ejecutora constituye una garantía (vale vista, póliza) por el monto no rendido, fijando un plazo perentorio para la rendición o para ejecutar la garantía.
- Cpt: Contingencia - Demoras en revisión interna por alta carga de trabajo.
  - Proc: Utilizar planificación anual para anticipar peaks y reasignar temporalmente revisores o priorizar rendiciones que habilitan transferencias críticas. Ref: STS-KB-GN-RENDICION-GESTION-BPR-01.

### SECCIÓN 8: Procedimientos Contables Clave (DAF)

ID: STS-KB-GN-RENDICION-CONTABILIDAD-01
Purp: Detallar los procedimientos contables en SIGFE para registrar transferencias y rendiciones.
Src: @manual_procedimientos_rendicion_cuentas_st24_st33_gore_ñuble.md (Sec 8)
Warn: Los números de cuenta corresponden al Plan de Cuentas del Sector Público.

#### 8.1. Transferencias Condicionadas a Sector Privado (F-07)

ID: STS-KB-GN-RENDICION-CONTABILIDAD-F07-01
Ctx: Aplicación en Subvenciones 8% FNDR, programas con ONGs.

- Cpt: Fase 1 - Entrega de Fondos.
  - Proc: Devengo Obligación.
    - Debe: 12106 Deudores por Transferencias Reintegrables
    - Haber: 21524 Cuentas por Pagar - Transf. Corrientes / 21533 Cuentas por Pagar - Transf. de Capital
  - Proc: Pago.
    - Debe: 21524 / 21533
    - Haber: 11102/11103 Banco
- Cpt: Fase 2 - Aprobación Rendición.
  - Proc: Reconocimiento Gasto.
    - Debe: 54101 Transf. Corr. Sector Privado / 54201 Transf. Cap. Sector Privado
    - Haber: 12106 Deudores por Transferencias Reintegrables
- Cpt: Fase 3 - Reintegro.
  - Proc: Devengo Cobro.
    - Debe: 11508 Cuentas por Cobrar
    - Haber: 12106 Deudores por Transferencias Reintegrables
  - Proc: Recepción Pago.
    - Debe: 11102/11103 Banco
    - Haber: 11508 Cuentas por Cobrar

#### 8.2. Transferencias Condicionadas a Sector Público (F-08)

ID: STS-KB-GN-RENDICION-CONTABILIDAD-F08-01
Ctx: Aplicación en FNDR a Municipalidades (FRIL, Proyectos), transferencias a otros Servicios Públicos.
Warn: Para transferencias a otros Servicios Públicos (no Municipalidades), el devengo del gasto se realiza al aprobar la rendición. Para Municipalidades, al momento de la transferencia. Ref: @kb_gn_018_gestion_prpto.md#GORE-FIN-EJEC-DEVENGO-01

- Cpt: Fase 1 - Entrega de Fondos.
  - Proc: Devengo Obligación.
    - Debe: 12106 Deudores por Transferencias Reintegrables
    - Haber: 21524 / 21533
  - Proc: Pago.
    - Debe: 21524 / 21533
    - Haber: 11102/11103 Banco
- Cpt: Fase 2 - Aprobación Rendición.
  - Proc: Reconocimiento Gasto.
    - Debe: 54103 Transf. Corr. Otras Ent. Públicas / 54203 Transf. Cap. Otras Ent. Públicas
    - Haber: 12106 Deudores por Transferencias Reintegrables
- Cpt: Fase 3 - Reintegro.
  - Proc: Idéntico a Fase 3 de F-07.

#### 8.3. Anticipos a Servicios Públicos (sin incorporación a presupuesto receptor) (C-01)

ID: STS-KB-GN-RENDICION-CONTABILIDAD-C01-01
Ctx: Aplicación en casos donde GORE encarga a otro ente público una gestión específica sin que éste integre los fondos a su presupuesto.

- Cpt: Fase 1 - Entrega Anticipo.
  - Proc: Salida Fondos.
    - Debe: 11403 Anticipos a Rendir Cuenta
    - Haber: 11102/11103 Banco
- Cpt: Fase 2 - Aprobación Rendición.
  - Proc: Reconocimiento Gasto del GORE.
    - Debe: Cuenta de Gasto respectiva (ej. 52208 Servicios Generales)
    - Haber: Cuenta por Pagar respectiva (ej. 21522 Cuentas por Pagar - B&S de Consumo)
  - Proc: Cancelación vía Compensación.
    - Debe: Cuenta por Pagar respectiva (ej. 21522)
    - Haber: 11403 Anticipos a Rendir Cuenta
- Cpt: Fase 3 - Reintegro Saldos.
  - Proc: Recepción Fondos.
    - Debe: 11102/11103 Banco
    - Haber: 11403 Anticipos a Rendir Cuenta
