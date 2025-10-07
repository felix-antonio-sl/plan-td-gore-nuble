# Plan de Transformación Digital del GORE Ñuble 2026-2028

**Versión:** 1.0.0  
**Fecha de Aprobación:** [Pendiente]  
**Vigencia:** 2026-2028  
**Próxima Revisión:** Diciembre 2026 (Retrospectiva Estratégica Anual)

---

## Navegación Rápida del Plan

### Para la Alta Dirección (Gobernador, Jefe de Gabinete, Jefes de División)

**Lectura Obligatoria:**

1. [**Documento Principal**](plan_td_gore_nuble_2026-2028_sts.md)
   - **Parte 0:** Mesa de Análisis Técnico (fundamentos de las decisiones)
   - **Parte I:** Resumen Ejecutivo (10 páginas, visión estratégica y decisión solicitada)

**Lectura Recomendada (según rol):**

- **Gobernador:** Sección 2 (Visión), Sección 3 (Objetivos Estratégicos), Sección 8 (KPIs y Transparencia)
- **Jefe de Gabinete:** Anexo G (Gestión de Conflictos), Sección 5 (Gobernanza)
- **Administradora Regional:** Anexo A (Marco de Gobernanza), Anexo D (Implementación)
- **Jefe DIPIR:** Anexo B - Canvas EV-1 NEXO GORE, Anexo D (Cronograma y Presupuesto)
- **Jefe DAF:** Anexo B - Canvas EV-1 (Módulo Rendiciones), Anexo E (Datos)
- **Jefe DIPLADE:** Anexo B - Canvas EV-3 IDE Ñuble
- **Jefa Comunicaciones:** Anexo F (Comunicación y Adopción)

---

### Para el Comité de Transformación Digital

**Documentos de Trabajo Mensual:**

- [Anexo A](./anexos_plan_td/anexo_a_gobernanza.md): Resolución constitutiva, RACI, protocolo de decisiones.
- [Anexo D](./anexos_plan_td/anexo_d_implementacion.md): Plan de acción y cronograma.

**Documentos de Referencia para Decisiones:**

- [Anexo A.3](./anexos_plan_td/anexo_a_gobernanza.md#a3-matriz-de-gates-de-cumplimiento-detallada): Matriz de Gates (para aprobar iniciativas).
- [Anexo A.7](./anexos_plan_td/anexo_a_gobernanza.md#a7-protocolo-de-toma-de-decisiones-en-el-ctd): Protocolo de toma de decisiones.
- Sección 5.2 del Resumen Ejecutivo: Ritual CVC (cómo se evalúan las EVs trimestralmente).

---

### Para el Subcomité de IA

**Documentos de Trabajo Quincenal:**

- [Anexo C](./anexos_plan_td/anexo_c_ia_responsable.md): Política de IA, evaluación de riesgos, Fichas SDA.

**Herramientas Operativas:**

- [C.2 - Plantilla Ficha SDA](./anexos_plan_td/anexo_c_ia_responsable.md#c2-plantilla-de-ficha-sda): Para documentar cada sistema de IA.
- [C.3 - Protocolo de Evaluación de Riesgos](./anexos_plan_td/anexo_c_ia_responsable.md#c3-protocolo-de-evaluacion-de-riesgos-de-ia): Cuestionario de clasificación.
- [C.5 - Protocolo de Incidentes](./anexos_plan_td/anexo_c_ia_responsable.md#c5-protocolo-de-gestion-de-incidentes-de-ia): Gestión de reportes ciudadanos.

---

### Para Equipos de Desarrollo (Oficina ODIA, Equipo Campeón)

**Arquitectura y Diseño:**

- [Anexo B](./anexos_plan_td/anexo_b_arquitectura_evs.md): Canvas de las 5 EVs, contratos conversacionales, mapa de dependencias.

**Estándares Técnicos:**

- [Anexo E](./anexos_plan_td/anexo_e_datos.md): Políticas de datos, catálogo, metadatos, modelo semántico.
- Anexo C: Requisitos de IA responsable.

**Metodología:**

- [Anexo D.5](./anexos_plan_td/anexo_d_implementacion.md#d5-metodologia-de-gestion-de-proyectos-td): Metodología híbrida (ágil + predictiva).

---

### Para Responsables de Comunicación

**Estrategia y Mensajes:**

- [Anexo F](./anexos_plan_td/anexo_f_comunicacion_adopcion.md): Estrategia de comunicación interna y externa completa.

**Herramientas:**

- [F.8 - Kit de Mensajes](./anexos_plan_td/anexo_f_comunicacion_adopcion.md#f8-kit-de-mensajes-oficial-para-vocerias): Q&A oficial para vocerías.
- [F.4 - Protocolo de Crisis](./anexos_plan_td/anexo_f_comunicacion_adopcion.md#f4-gestion-de-expectativas-y-comunicacion-de-riesgos): Comunicación de incidentes.

---

## Estructura del Plan Completo

```
/00_gobernanza/
│
├── plan_td_gore_nuble_2026-2028.md          [DOCUMENTO PRINCIPAL]
│   ├── Parte 0: Mesa de Análisis Técnico (Diálogo Digitrans-Kore-Goreólogo)
│   │   ├── 0.1 - Presentación de especialistas
│   │   ├── 0.2 - Análisis de contexto y diagnóstico
│   │   ├── 0.3 - Evaluación de propuesta previa
│   │   ├── 0.4 - Integración con Ñuble 250
│   │   ├── 0.5 - Estructura temporal
│   │   ├── 0.6 - Arquitectura bajo ASTA-Kore
│   │   └── 0.7 - Síntesis de decisiones fundamentales
│   │
│   └── Parte I: Resumen Ejecutivo (10 páginas)
│       ├── 1. Contexto y Mandato
│       ├── 2. Visión y Principios Rectores
│       ├── 3. Objetivos Estratégicos y Alcance
│       ├── 4. Arquitectura de Capacidades (5 EVs)
│       ├── 5. Gobernanza y Modelo de Decisión
│       ├── 6. Hoja de Ruta (H1/H2/H3)
│       ├── 7. Sostenibilidad y Financiamiento
│       └── 8. Medición de Impacto y Transparencia
│
├── anexos_plan_td/                           [ANEXOS TÉCNICOS]
│   ├── anexo_a_gobernanza.md                 [514 líneas]
│   │   ├── A.1 - Resolución constitutiva del CTD
│   │   ├── A.2 - Matriz RACI completa
│   │   ├── A.3 - Matriz de Gates de cumplimiento
│   │   ├── A.4 - Vademécum jurídico-administrativo
│   │   ├── A.5 - Calendario operativo 2026
│   │   └── A.6-A.9 - Roles, protocolos, integración con CORE
│   │
│   ├── anexo_b_arquitectura_evs.md           [1.054 líneas]
│   │   ├── B.1 - Canvas de EV-1: NEXO GORE
│   │   ├── B.2 - Canvas de EV-2: Mi Ñuble
│   │   ├── B.3 - Canvas de EV-3: IDE Ñuble
│   │   ├── B.4 - Canvas de EV-4: CIES Regional
│   │   ├── B.5 - Canvas de EV-5: Gobernanza Regional TD
│   │   ├── B.6 - Mapa de dependencias entre EVs
│   │   ├── B.7 - Integración con plataformas nacionales
│   │   ├── B.8 - Contratos conversacionales (APIs)
│   │   ├── B.9 - Estrategia de integración de Gesdoc
│   │   └── B.10 - Plan de transferencia de capacidades
│   │
│   ├── anexo_c_ia_responsable.md             [711 líneas]
│   │   ├── C.1 - Política de uso de IA
│   │   ├── C.2 - Plantilla Ficha SDA
│   │   ├── C.3 - Protocolo de evaluación de riesgos
│   │   ├── C.4 - Catálogo de asistentes existentes
│   │   ├── C.5 - Protocolo de gestión de incidentes de IA
│   │   ├── C.6 - Checklist de pre-despliegue
│   │   ├── C.7 - Directrices de comunicación ciudadana
│   │   └── C.8 - Protocolo de auditoría externa
│   │
│   ├── anexo_d_implementacion.md             [373 líneas]
│   │   ├── D.1 - Plan de acción por horizonte (H1/H2/H3)
│   │   ├── D.2 - Cronograma visual (Gantt)
│   │   ├── D.3 - Presupuesto trianual detallado
│   │   ├── D.4 - Plantillas de formulación (Glosa 06, SNI)
│   │   └── D.5 - Metodología de gestión de proyectos TD
│   │
│   ├── anexo_e_datos.md                      [474 líneas]
│   │   ├── E.1 - Política de gobierno de datos
│   │   ├── E.2 - Catálogo de datasets críticos
│   │   ├── E.3 - Estándares de metadatos (DCAT, ISO 19115)
│   │   ├── E.4 - Guía de anonimización
│   │   ├── E.5 - Política de datos abiertos
│   │   ├── E.6 - Arquitectura del RUC
│   │   ├── E.7 - Modelo semántico unificado (glosario)
│   │   └── E.8 - Protocolo de calidad de datos
│   │
│   ├── anexo_f_comunicacion_adopcion.md      [518 líneas]
│   │   ├── F.1 - Estrategia de comunicación interna
│   │   ├── F.2 - Programa de desarrollo de competencias
│   │   ├── F.3 - Estrategia de comunicación externa
│   │   ├── F.4 - Gestión de expectativas y riesgos
│   │   ├── F.5 - Estrategia de adopción de Mi Ñuble
│   │   ├── F.6 - Alianzas estratégicas
│   │   ├── F.7 - Protocolo de comunicación de crisis
│   │   └── F.8 - Kit de mensajes oficial
│   │
│   └── anexo_g_gestion_conflictos.md         [404 líneas]
│       ├── G.1 - Análisis del ecosistema de poder
│       ├── G.2 - Estrategia de integración de Gesdoc
│       ├── G.3 - Mitigación de riesgos políticos
│       ├── G.4 - Gestión del "Factor Prometeo"
│       ├── G.5 - Resolución de conflictos entre divisiones
│       ├── G.6 - Cambio de liderazgo político
│       ├── G.7 - Relacionamiento con actores externos
│       └── G.8 - Escenarios de contingencia
│
└── README_plan_td.md                         [ESTE ARCHIVO]
```

---

## Cómo Usar Este Plan Según Tu Rol

### Si eres el Gobernador Regional

1. **Lee:** Resumen Ejecutivo completo (Parte I del documento principal).
2. **Enfócate en:** Secciones 2 (Visión), 3 (Objetivos), 6 (Hoja de Ruta), Decisión Solicitada.
3. **Tu decisión clave:** Aprobar el plan y autorizar constitución del CTD.
4. **Tiempo estimado de lectura:** 30 minutos.

### Si eres Miembro del Comité de Transformación Digital

1. **Lee:** Resumen Ejecutivo + Anexo A (Gobernanza) + Anexo D (Implementación).
2. **Enfócate en:**
   - Anexo A.2: Tu rol en la Matriz RACI.
   - Anexo A.3: Los Gates de cumplimiento que deberás verificar.
   - Sección 5.2 del Resumen: El ritual CVC que ejecutarás trimestralmente.
3. **Tiempo estimado:** 2 horas.

### Si eres Responsable de una Entidad de Valor

1. **Lee:** El Canvas de tu EV en Anexo B.
2. **Estudia:** Los Contratos Conversacionales (APIs) que deberás exponer o consumir.
3. **Usa:** Anexo D para entender el cronograma de tu EV.
4. **Ejemplo:** Si lideras Mi Ñuble, lee B.2 (Canvas completo de EV-2).

### Si eres del Equipo Técnico (ODIA, Desarrolladores)

1. **Lee:** Anexo B (Arquitectura completa de EVs).
2. **Estudia:** Anexo E (estándares de datos), Anexo C (requisitos de IA).
3. **Usa:** Anexo D.5 para metodología de trabajo (sprints, artefactos).

### Si eres Responsable de Comunicaciones

1. **Lee:** Anexo F completo.
2. **Usa:** F.8 (Kit de Mensajes) para vocerías.
3. **Implementa:** F.5 (Estrategia de adopción de Mi Ñuble).

### Si eres Asesor Jurídico o de Control

1. **Lee:** Anexo A.4 (Vademécum jurídico-administrativo).
2. **Verifica:** Anexo D.4 (Plantillas de formulación cumplen requisitos legales).
3. **Colabora:** Anexo A.3 (Eres verificador de Gates de cumplimiento).

---

## Documentos de Gobernanza Clave

| Documento | Propósito | Frecuencia de Actualización |
|:---|:---|:---|
| **OKRs Anuales** | Objetivos estratégicos del año | Anual (diciembre) |
| **OKRs Trimestrales (por EV)** | Hipótesis de valor del trimestre | Trimestral (en cada CVC) |
| **Actas del CTD** | Registro de decisiones del Comité | Mensual |
| **Informes CVC** | Rendición de evidencia de cada EV | Trimestral |
| **Fichas SDA** | Transparencia sobre sistemas de IA | Al desplegar sistema, revisión anual |
| **Catálogo de Datos** | Inventario de datasets institucionales | Mensual (actualización continua) |
| **Registro de Incidentes de IA** | Reporte de problemas y su resolución | Continuo |

---

## Ciclo Anual de Gobernanza (Calendario 2026)

| Mes | Evento de Gobernanza | Decisión/Entregable |
|:---|:---|:---|
| **Enero** | Sesión Constitutiva del CTD | Aprobación Plan Maestro y OKRs Anuales 2026 |
| **Marzo** | Primer CVC (Q1) | Decisiones de inversión para Q2 en cada EV |
| **Junio** | Segundo CVC (Q2) | Decisiones Q3 + Informe Semestral a Gobernador/CORE |
| **Septiembre** | Tercer CVC (Q3) | Decisiones Q4 + Aprobación presupuesto TD 2027 |
| **Diciembre** | Cuarto CVC (Q4) + Retrospectiva Estratégica | Evaluación de OKRs Anuales 2026 + Definición OKRs 2027 + Actualización Plan Maestro v2.0 |

---

## Glosario de Acrónimos del Plan

| Acrónimo | Significado | Definición Resumida |
|:---|:---|:---|
| **TD** | Transformación Digital | Proceso de modernización digital del Estado (Ley 21.180) |
| **TDE** | Transformación Digital del Estado | Ídem TD |
| **EV** | Entidad de Valor | Sistema sociotécnico con propósito, fronteras, equipo y métricas (concepto ASTA-Kore) |
| **CTD** | Comité de Transformación Digital | Instancia de gobernanza máxima del Plan TD |
| **CVC** | Ciclo de Valor y Capacidad | Ritual trimestral de rendición de cuentas y decisión de inversión |
| **ODIA** | Oficina Digital e IA | Unidad técnica ejecutora del Plan TD (a crear formalmente en H3) |
| **IPR** | Intervención Pública Regional | Proyectos y programas financiados por el GORE |
| **IDI** | Iniciativa de Inversión | Proyecto de inversión (SNI) |
| **PPR** | Programa Público Regional | Programa de gasto corriente (Glosa 06) |
| **RUC** | Repositorio Único de Conocimiento | Base de conocimiento institucional para asistentes de IA |
| **SDA** | Sistema de Decisión Automatizada | Sistema de IA que apoya/toma decisiones (terminología CPLT) |
| **EIPD** | Evaluación de Impacto en Protección de Datos | Análisis de riesgos de privacidad (Ley 21.719) |
| **DPO** | Delegado de Protección de Datos | Responsable de cumplimiento de Ley 21.719 |
| **CISO** | Oficial de Seguridad de la Información | Responsable de ciberseguridad (Norma Técnica DS N°7) |
| **IDE** | Infraestructura de Datos Espaciales | Sistema de datos geoespaciales (DS N°28) |
| **CIES** | Centro Integrado de Emergencia y Seguridad | Sistema regional de videovigilancia y emergencias |
| **SITIA** | Sistema de Información Territorial Integrado de Apoyo | Plataforma nacional de seguridad ciudadana (Subsec. Prev. Delito) |

---

## Métricas de Éxito del Plan (Resumen)

### 7 KPIs Estratégicos (Visión Ejecutiva)

| KPI | Línea Base | Meta 2027 | Medición |
|:---|:---|:---|:---|
| **KPI-1:** Madurez Digital CPAT | 21% Nivel 3+ | >=50% Nivel 3+ | Trimestral (actualización CPAT) |
| **KPI-2:** Cumplimiento Normas Técnicas | 0% (6 normas) | 100% (6/6) | Anual (auditoría interna) |
| **KPI-3:** Tiempo de Ciclo IPR | >180 días | <90 días | Trimestral (datos de NEXO GORE) |
| **KPI-4:** Tasa Observaciones CGR | A establecer | -40% | Trimestral (datos de DAF) |
| **KPI-5:** Adopción Mi Ñuble | 0% | >=20% | Mensual (analítica de app) |
| **KPI-6:** CSAT Ciudadana | A establecer | >=4.0/5.0 | Trimestral (encuesta in-app) |
| **KPI-7:** Adopción Municipal Estándares | ~10% | >=71% | Semestral (CPAT municipal) |

Publicación: Todos los KPIs se publican mensualmente en el Observatorio Ñuble 360 (módulo del Observatorio Ñuble 250).

---

## Próximos Pasos Inmediatos (Post-Aprobación)

Sujeto a la aprobación de la Alta Dirección, la secuencia de activación es:

**Semana 1:**

1. Coordinador TD redacta borrador de Resolución Exenta constitutiva del CTD.
2. Asesoría Jurídica revisa y visa.
3. Gobernador firma y tramita Resolución.

**Semana 2:**
4. Administradora Regional convoca primera sesión constitutiva del CTD.
5. CTD sesiona: Aprobación formal del Plan Maestro TD y OKRs Anuales.

**Semana 3:**
6. CTD aprueba constitución del Subcomité de IA.
7. Coordinador TD inicia ejecución del Plan de Quick Wins (H1).

**Semana 4:**
8. Primera Ficha SDA publicada en sitio de Transparencia Activa.
9. Inicio de despliegue de IDE Ñuble v0.1.

---

## Contacto y Consultas

**Coordinador de Transformación Digital:**  
[Nombre a designar]  
Email: <coordinador.td@gorenuble.cl>  
Teléfono: [A definir]

**Comité de Transformación Digital:**  
Email: <ctd@gorenuble.cl>

**Sitio Web del Plan TD:**  
<https://www.gorenuble.cl/transformacion-digital>

**Observatorio Ñuble 360 (Módulo TD):**  
<https://nuble250.cl/observatorio/td>

---

## Control de Versiones del Plan

| Versión | Fecha | Cambios Principales | Aprobado Por |
|:---|:---|:---|:---|
| **1.0.0** | 06/10/2025 | Versión inicial completa | [Pendiente: CTD] |
| **1.1.0** | [Futura] | Actualización post-Primer CVC (ajustes basados en evidencia Q1) | [Futuro] |
| **2.0.0** | Dic-2026 | Actualización Anual (Retrospectiva Estratégica 2026, nuevos OKRs 2027) | [Futuro] |

Req: El Plan es un documento vivo. Se actualiza anualmente (versión mayor) y puede ajustarse trimestralmente (versión menor) basado en aprendizaje del CVC.

---

**Última Actualización:** 06 de Octubre de 2025  
**Estado:** Presentado a la Alta Dirección para Aprobación  

_Gobierno Regional de Ñuble - Transformación Digital e Inteligencia Artificial_
