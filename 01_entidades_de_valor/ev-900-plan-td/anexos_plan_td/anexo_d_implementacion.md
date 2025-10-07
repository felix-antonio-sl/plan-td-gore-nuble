# Anexo D: Implementación Detallada

ID: PTD-ANEXO-D-IMPLEMENTACION-01
Version: 1.0.0
Status: Published
Parent-Document: plan_td_gore_nuble_2026-2028.md
Creation-Date: 2025-10-06

---

## D.1. Plan de Acción Detallado por Horizonte

### D.1.1. Horizonte 1 (H1): Gobernar y Ganar Rápido (Meses 1-6)

**Mes 1: Instalación de Gobernanza**

| Semana | Tarea | Responsable | Entregable | Gate |
|:---|:---|:---|:---|:---|
| S1 | Borrador Resolución CTD/Subcomité IA | Coord. TD + Asesoría Jurídica | Borrador visado | - |
| S2 | Aprobación y firma de Resolución | Gobernador | Resolución tramitada | - |
| S3 | Convocatoria y sesión constitutiva del CTD | Admin. Regional | Acta constitutiva | - |
| S4 | Primera sesión ordinaria CTD: Aprobación Plan Maestro y OKRs Anuales | CTD | OKRs Anuales aprobados | G1 |

**Mes 2: Quick Wins Técnicos**

| Semana | Tarea | Responsable | Entregable |
|:---|:---|:---|:---|
| S1-2 | Despliegue IDE Ñuble v0.1 (Geonodo + 3 datasets base) | DIPLADE + ODIA | Geonodo operativo, URL pública |
| S2-3 | Elaboración primera Ficha SDA (Asistente 8% FNDR) | Coord. TD + Resp. Sistema | Ficha SDA publicada |
| S3-4 | Desarrollo Copiloto Jurídico v0.1 (convenios) | ODIA + Asesoría Jurídica | Prototipo funcional en piloto |
| S4 | Inicio de gestión de Convenio GORE-SITIA | ODIA + DIT | Borrador de convenio |

**Mes 3: Primer CVC y Consolidación**

| Semana | Tarea | Responsable | Entregable |
|:---|:---|:---|:---|
| S1-2 | Preparación de informes CVC para 5 EVs | Responsables de cada EV | 5 Informes CVC |
| S3 | **Primer CVC:** Rendición de EVs, decisiones Q2 | CTD | Acta con decisiones de inversión |
| S4 | Borrador Política de Gobierno de Datos | Coord. TD + DPO | Política para aprobación CTD |

**Meses 4-6: Escalado de H1**

- Expansión IDE Ñuble a 5 datasets, integración con 2 municipios.
- Chat GORE Ciudadano en beta pública (versión web).
- Firma de Convenio GORE-SITIA.
- PoC técnica de integración CIES-SITIA exitosa.
- Segundo CVC (mes 6): Evaluación de avance H1, aprobación de prioridades H2.

### D.1.2. Horizonte 2 (H2): Pilotos y Escalado (Meses 6-18)

**Sprints de Desarrollo (Metodología Ágil, sprints de 2 semanas)**

Req: Cada EV opera con su propio backlog priorizado, pero todos reportan avance en los CVCs trimestrales.

**Meses 6-9: Inicio de Pilotos Mayores**

- NEXO GORE: Desarrollo de módulo IPR (gestión de ciclo de vida de proyectos).
  - Hito Mes 9: Piloto con DIPIR gestionando 10 proyectos FRIL.
- Mi Ñuble: Desarrollo de app móvil (backend + frontend React Native).
  - Hito Mes 9: Beta en TestFlight (iOS) y Google Play Beta.

**Meses 9-12: Consolidación de Pilotos**

- NEXO GORE: Módulo de rendiciones con Pre-Auditor de IA.
  - Hito Mes 12: Piloto con DAF procesando 20 rendiciones reales.
- Mi Ñuble: Lanzamiento público en tiendas (iOS + Android).
  - Hito Mes 12: App disponible para descarga, módulos Mi GORE y Mi Seguridad activos.
- CIES-SITIA: Integración en producción.
  - Hito Mes 12: 50 cámaras integradas, SOPs aplicados.
- IDE Ñuble: Certificación como nodo regional de IDE Chile.

**Meses 12-18: Escalado**

- NEXO GORE: Gestiona 50% de cartera de inversión nueva (proyectos del año en curso).
- Mi Ñuble: Campaña de adopción, meta 5% de población.
- Gobernanza Regional TD: Primera capacitación masiva a municipios, 10 municipios usando servicios compartidos.

### D.1.3. Horizonte 3 (H3): Industrialización (Meses 18-36)

**Meses 18-24: Consolidación Operativa**

- NEXO GORE: Gestiona 80% de cartera de inversión, integración completa con SIGFE/BIP.
- Mi Ñuble: 15% de adopción, módulo de Participación activo.
- Transferencia de Capacidades: Equipo Campeón asume operación de asistentes.

**Meses 24-30: Madurez**

- Modelo AaaS operativo para municipios.
- Auditorías externas de IA y Ciberseguridad superadas.

**Meses 30-36: Sostenibilidad**

- NEXO GORE: 100% de IPR nuevas gestionadas.
- Mi Ñuble: 20% de adopción, integración con Carpeta Ciudadana nacional.
- Propuesta de creación formal de Oficina ODIA.

---

## D.2. Cronograma Visual (Gantt Simplificado)

```
Año 2026                Q1          Q2          Q3          Q4
────────────────────────┼───────────┼───────────┼───────────┼───────────
Gobernanza (H1)         ████████████
├─ Constitución CTD     ██
├─ Políticas (Datos/IA) ░░░░████
└─ CVCs                     ▲           ▲           ▲           ▲

IDE Ñuble (H1-H2)       ████████████████████████████
├─ v0.1 (3 datasets)    ██
├─ v1.0 (5 datasets)        ░░░░██
└─ Certificación IDE            ░░░░░░░░████

CIES-SITIA (H1-H2)      ████████████████████████
├─ Convenio             ░░██
├─ PoC                      ░░░░██
└─ Producción                   ░░░░░░░░████

Mi Ñuble (H2)                   ████████████████████████████
├─ Beta web                     ░░██
├─ App tiendas                      ░░░░░░░░██
└─ Adopción 5%                              ░░░░░░░░░░░░░░██

NEXO GORE (H2)                  ████████████████████████████████
├─ Módulo IPR piloto                ░░░░░░██
├─ Módulo Rendiciones                   ░░░░░░░░██
└─ 50% cartera                                      ░░░░░░██


Año 2027-2028          Q1-Q4 2027                  Q1-Q4 2028
────────────────────────┼───────────────────────────┼──────────
Todos los sistemas      ████████████████████████████████████████
en Horizonte H3         (Escalado a 80-100% de capacidad)

Transferencia           ░░░░░░░░░░░░████████████████████
Equipo Campeón                      (Asumen operación)

Leyenda:
██ Ejecución activa
░░ Preparación/diseño
▲  CVC (Ciclo de Valor y Capacidad trimestral)
```

---

## D.3. Presupuesto Trianual Detallado

### D.3.1. Desagregación por Categoría de Gasto

**Año 2026 (H1-H2)**

| Categoría | Concepto | Monto (M$) | Subtítulo | Observaciones |
|:---|:---|---:|:---|:---|
| **Equipo Habilitante** | Coord. TD + 2 ingenieros (honorarios) | 60.000 | 21.03.001 | Programa Habilitante, Glosa 06 (5%) |
| **Infraestructura** | Servidores cloud, licencias, almacenamiento | 50.000 | 29.06 o 22.08 | Según política Cloud |
| **Desarrollo EV-1** | NEXO GORE (módulos IPR, Rendiciones) | 80.000 | 31.02 (IDI-SNI) | Requiere RS |
| **Desarrollo EV-2** | Mi Ñuble (backend, app móvil) | 40.000 | 31.02 (IDI-SNI) | Requiere RS |
| **Operación EV-3** | IDE Ñuble (Geonodo, datasets) | 15.000 | 24.03 (Glosa 06 PPR) | Ejecución directa |
| **Integración EV-4** | CIES-SITIA (PoC, SOPs) | 10.000 | 24.03 (Glosa 06) | Convenio sectorial |
| **Capacitación** | Talleres, formación Equipo Campeón | 15.000 | 24.03 (Glosa 06) | PPR Gobernanza |
| **TOTAL 2026** | | **270.000** | | ~0.4% del FNDR anual |

**Año 2027 (H2-H3)**

| Categoría | Monto (M$) | Observaciones |
|:---|---:|:---|
| Equipo (4 ingenieros + Coord.) | 90.000 | Equipo Campeón en formación |
| Infraestructura (escalado) | 40.000 | Aumento por mayor tráfico |
| Desarrollo/Evolución EVs | 180.000 | NEXO módulo financiero, Mi Ñuble escalado, nuevos asistentes |
| Capacitación (interna + municipal) | 30.000 | Programa regional |
| Auditorías externas | 10.000 | Primera auditoría IA y Ciberseguridad |
| **TOTAL 2027** | **350.000** | |

**Año 2028 (H3)**

| Categoría | Monto (M$) | Observaciones |
|:---|---:|:---|
| Equipo ODIA (6 funcionarios) | 110.000 | Oficina formal, equipo consolidado |
| Infraestructura (estable) | 40.000 | |
| Evolución EVs + AaaS municipal | 150.000 | Enfoque en sostenibilidad y escalado territorial |
| Capacitación continua | 35.000 | |
| Auditorías | 10.000 | Segunda auditoría |
| **TOTAL 2028** | **345.000** | |

**TOTAL TRIANUAL: M$ 965.000** (~1.5% del presupuesto FNDR anual promedio)

### D.3.2. Distribución por Fuente de Financiamiento

| Fuente | Año 2026 | Año 2027 | Año 2028 | Total | % |
|:---|---:|---:|---:|---:|---:|
| **FNDR - Subt. 24 (Programas PPR)** | 90.000 | 130.000 | 195.000 | 415.000 | 43% |
| **FNDR - Subt. 31 (Proyectos IDI)** | 120.000 | 180.000 | 100.000 | 400.000 | 41% |
| **Convenios Sectoriales (SITIA)** | 10.000 | 20.000 | 20.000 | 50.000 | 5% |
| **FRPD (Productividad)** | 50.000 | 20.000 | 30.000 | 100.000 | 10% |
| **TOTAL** | 270.000 | 350.000 | 345.000 | 965.000 | 100% |

---

## D.4. Plantillas de Formulación

### D.4.1. Plantilla de Formulación para Programa Habilitante (Glosa 06)

**Título del Programa:** Programa de Gobernanza y Habilitación para la Transformación Digital e IA del GORE Ñuble

**Tipo:** Programa Público Regional (PPR) de Ejecución Directa del GORE

**Fuente de Financiamiento:** FNDR - Subtítulo 24 (Transferencias Corrientes, Ítem 24.03.109 - A Unidades o Programas del Servicio)

**Evaluación Ex-Ante:** Requiere Recomendación Favorable (RF) de DIPRES/SES según Glosa 06.

**División Responsable:** División de Planificación y Desarrollo Regional (DIPLADE) en coordinación con Oficina Digital e IA (ODIA, una vez constituida).

**Período de Ejecución:** Anual (renovable), 01/01/2026 - 31/12/2026.

**Descripción del Problema (Metodología de Marco Lógico):**

Causa: El GORE Ñuble carece de una estructura formal de gobernanza, capacidades técnicas consolidadas y procesos estandarizados para liderar su proceso de Transformación Digital del Estado (TDE), en cumplimiento del mandato de la Ley N° 21.180 con plazo 31/12/2027.

Efecto: Riesgo de incumplimiento normativo, inversiones tecnológicas descoordinadas (silos de información), vulnerabilidad en ciberseguridad, ineficiencia operativa y pérdida de la oportunidad de posicionar al GORE como líder regional en modernización.

**Objetivo del Programa:**

Instalar la capacidad institucional permanente de gobernanza, ingeniería y operación de la Transformación Digital e Inteligencia Artificial en el GORE Ñuble, mediante la constitución del Comité de Transformación Digital, la conformación de un equipo técnico especializado y la provisión de infraestructura tecnológica compartida, para habilitar el cumplimiento del mandato legal y la ejecución del Plan TD 2026-2028.

**Población Objetivo:**

- Directa: Funcionarios del GORE Ñuble (~150 funcionarios).
- Indirecta: Ciudadanía de Ñuble (512.000 hab.), 21 municipios, servicios públicos regionales.

**Componentes del Programa:**

1. **Gobernanza y Coordinación:**
   - Operación del CTD y Subcomité de IA (sesiones, actas, reportes).
   - Coordinación de la Mesa Regional de TD.
   - Gestión de cumplimiento normativo (Gates, reportes a SGD/DIPRES/CGR).

2. **Equipo Técnico Especializado:**
   - Coord. de TD (1 funcionario, tiempo completo).
   - Ingenieros de desarrollo y operación (2-3 contratados vía honorarios S.21).
   - Curadores de conocimiento (1-2 funcionarios, tiempo parcial).

3. **Infraestructura Tecnológica Compartida:**
   - Servidores cloud (IaaS), bases de datos, almacenamiento.
   - Licencias de software (Geonodo, herramientas de desarrollo).
   - Servicios de ciberseguridad (monitoreo, respaldos).

4. **Desarrollo de Capacidades Internas:**
   - Programa de capacitación en TDE, IA, gestión de datos para funcionarios.
   - Formación del Equipo Campeón (mentoría).

**Presupuesto Año 1:** M$ 90.000 (financiado vía Glosa 06, uso permitido de hasta 5% para gastos de administración del programa).

**Indicadores de Desempeño:**

- Eficacia: % de Normas Técnicas TDE implementadas (Meta: 50% hacia dic-2026).
- Eficiencia: Número de iniciativas TD ejecutadas dentro de plazo (Meta: 80%).
- Calidad: Satisfacción de usuarios internos con servicios de ODIA (Meta: >=4.0/5.0).

---

### D.4.2. Plantilla de Formulación para Proyecto SNI (EV Mi Ñuble, Fase Desarrollo)

**Nombre de la Iniciativa:** Desarrollo de Aplicación Móvil y Portal Web "Mi Ñuble" - Ecosistema Ciudadano Digital del GORE

**Código BIP:** [A asignar por MDSF]

**Tipo:** Proyecto de Inversión (IDI)

**Proceso:** Desarrollo de Activo Intangible (Software)

**Fuente:** FNDR - Subtítulo 31.02 (Proyectos, Iniciativas de Inversión)

**Etapa:** Diseño → Ejecución

**Unidad Responsable:** Gobierno Regional de Ñuble (ejecución directa o mediante contrato con desarrollador externo vía Ley 19.886).

**Objetivo del Proyecto:**

Desarrollar y desplegar una aplicación móvil (iOS + Android) y portal web que actúe como el canal digital unificado del GORE Ñuble, permitiendo a los ciudadanos acceder 24/7 a información de servicios, inversión pública, oportunidades de fomento, mecanismos de participación y reportes de emergencia, mejorando la experiencia ciudadana y la eficiencia operativa del GORE.

**Beneficiarios:**

- Directos: 307.000 adultos con smartphone (60% de población).
- Indirectos: Totalidad de población de Ñuble (acceso vía web).

**Problema a Resolver:**

Los ciudadanos de Ñuble enfrentan barreras para acceder a información y servicios del GORE:

- Deben llamar por teléfono en horario hábil (consultas repetitivas saturan líneas).
- No existe visibilidad en tiempo real de inversión pública en su comuna.
- Postulación a fondos concursables es compleja (formularios poco intuitivos, falta de orientación).
- No hay canal directo para reportar emergencias geollocalizadas.

Causa: Ausencia de un canal digital moderno, accesible y unificado.

**Solución Propuesta:**

Desarrollo de aplicación móvil nativa con 5 módulos principales (Mi GORE, Trámites y Oportunidades, Mi Seguridad, Observatorio, Participación), integrada con sistemas internos (NEXO GORE, IDE Ñuble, CIES) y plataformas nacionales (ClaveÚnica), diseñada con enfoque UX/UI centrado en el usuario y cumpliendo estándares de accesibilidad (WCAG 2.1 AA).

**Alternativas Evaluadas:**

1. Portal web responsive: Descartada. Menor usabilidad en móvil, no permite notificaciones push ni uso offline.
2. App híbrida (WebView): Descartada. Rendimiento inferior, experiencia de usuario degradada.
3. **App nativa con React Native (SELECCIONADA):** Mejor balance rendimiento/costo, una base de código para iOS y Android.

**Monto Total:** M$ 180.000

- Diseño UX/UI: M$ 15.000.
- Desarrollo backend (APIs, base de datos): M$ 50.000.
- Desarrollo frontend (app móvil + web): M$ 80.000.
- Testing y QA: M$ 15.000.
- Despliegue, capacitación, documentación: M$ 20.000.

**Plazo de Ejecución:** 12 meses (Mes 6 a Mes 18 del Plan TD).

**Indicadores de Resultado:**

- Tasa de adopción: >=5% de población objetivo hacia mes 18 (15.350 descargas).
- CSAT: >=4.0/5.0.
- Reducción de consultas telefónicas: 30%.

**Riesgos y Mitigación:**

- Riesgo: Baja adopción ciudadana → Mitigación: Campaña de difusión masiva, alianza con municipios, incentivos (ej. sorteos).
- Riesgo: Complejidad técnica de integraciones → Mitigación: Arquitectura modular, priorización de MVP, integraciones por fases.

---

## D.5. Metodología de Gestión de Proyectos TD

Fnd: Guía Metodológica Unificada para Gestión de Proyectos TIC (kb_tde_070_guia_txdig_sts.md).

Req: Toda iniciativa del Plan TD se gestionará aplicando una metodología híbrida:

- **Planificación predictiva** para cumplimiento de hitos normativos y presupuestarios (compatibilidad con ciclo presupuestario del GORE).
- **Ejecución ágil** para desarrollo de software y aprendizaje rápido (sprints de 2 semanas, demos continuas).

### Artefactos Obligatorios por Fase

**Fase de Inicio:**

- Acta de Constitución del Proyecto (1 página): Problema, objetivo, alcance, equipo, presupuesto preliminar, sponsor.
- Registro de Stakeholders.

**Fase de Planificación:**

- Canvas de EV (Σ-T): Modelo de la anatomía del servicio/producto.
- OKRs Trimestrales (Δ-T): Hipótesis de valor a validar.
- Backlog Priorizado: Historias de usuario ordenadas por valor.
- Registro de Riesgos.

**Fase de Ejecución:**

- Tablero de Flujo (Xanpan): Gestión visual del trabajo en progreso.
- Informes de Avance para CVC (trimestral).
- Demos de software funcionando (quincenal).
- Bitácoras de Decisión (ADRs): Para decisiones arquitectónicas significativas.

**Fase de Cierre (si aplica):**

- Informe Final de Proyecto.
- Lecciones Aprendidas.
- Transferencia a operación (si es producto continuo, no cierra; evoluciona).

---

**Fin del Anexo D**

Este anexo provee el plan de acción operativo detallado por horizonte, el cronograma visual, el presupuesto desagregado por categoría y fuente, y las plantillas de formulación para los principales vehículos de financiamiento (Programa Habilitante vía Glosa 06, Proyecto SNI para desarrollo de software).

Ref: Las políticas de gestión de datos que rigen el desarrollo de las EVs se encuentran en el Anexo E.
