## Canvas de Entidad de Valor: Gobernanza de Datos y Seguridad

ID: `EV-GORENUBLE-001` | Versión: `1.0` | Equipo Dueño: `Oficina Digital e IA (ODIA)` | Fecha: `2025-10-06`

---

#### Parte 1: La Anatomía del Valor

| 1. Propósito y Valor Público | 2. Actores y Experiencia | 3. Flujo de Valor Principal |
| :--- | :--- | :--- |
| **¿POR QUÉ existe esta EV?** | **¿PARA QUIÉN diseñamos?** | **¿CÓMO funciona de punta a punta?** |
| • **Propósito Esencial:** Establecer un marco de gobernanza para tratar los datos como un activo estratégico, asegurando su calidad, seguridad y uso ético para habilitar la toma de decisiones basada en evidencia. <br>• **Alineamiento Estratégico:** Capacidad Habilitante S.1 y S.2 del Mapa de Capacidades. <br>• **Problema/Oportunidad:** Resuelve la brecha crítica de una gestión de datos fragmentada ("silos"), reactiva y sin gobierno, mitigando riesgos de incumplimiento normativo y de ciberseguridad. | • **Clientes/Usuarios:** Jefaturas de División y equipos técnicos (consumen datos para análisis), Gobernador y Administradora (consumen dashboards para decisión estratégica). <br>• **Participantes Internos:** CISO, DPO, Asesoría Jurídica, equipos de TI, Dueños de Datos en cada división. <br>• **Experiencia (Journey):** Transitar de una experiencia de desconfianza y dificultad para acceder a datos, a una de autoservicio, confianza y facilidad de uso. | • **Evento de Inicio:** Aprobación de la Política de Gobierno de Datos por el CTD. <br>• **Etapas Macro:** 1. Definición de Políticas y Estándares → 2. Creación del Catálogo de Datos → 3. Implementación de Controles (Calidad y Seguridad) → 4. Monitoreo y Mejora Continua. <br>• **Resultado Final:** Un ecosistema de datos gobernado, seguro y confiable. |
| 4. Capacidades y Servicios Expuestos | 5. Datos Clave (Consumidos y Producidos) | 6. Componentes Tecnológicos |
| **¿Qué VALOR produce para otros?** | **¿Qué INFORMACIÓN necesita y genera?** | **¿Sobre qué CIMIENTOS se construye?** |
| • **Capacidades de Negocio:** Gobernanza de Datos, Gestión de Calidad de Datos (DQM), Gestión de Seguridad de la Información (ISM). <br>• **Servicios Expuestos (APIs):** API del Catálogo de Datos, API de Métricas de Calidad de Datos. <br>• **Consumidores:** Todas las demás EVs del GORE, especialmente `NEXO GORE - IPR` y el `Observatorio Ñuble 360`. | • **Datos Consumidos:** Metadatos de todos los sistemas y bases de datos del GORE. <br>• **Datos Producidos:** El **Catálogo de Datos Institucional**, el **Modelo Semántico Unificado**, Informes de Calidad de Datos, Registros de Auditoría de Acceso. <br>• **Fuente de Verdad:** Esta EV es la fuente de verdad sobre la gobernanza y metadatos. | • **Componentes Principales:** Herramienta de Catálogo de Datos (ej. DataHub), Plataforma de Calidad de Datos (ej. Great Expectations), Framework de Policy-as-Code para seguridad (ej. OPA). <br>• **Plataformas Transversales:** Se integra con la infraestructura de observabilidad y CI/CD. <br>• **Stack Tecnológico:** Python, SQL, Git. |

---

#### Parte 2: El Contexto Operacional

| 7. Dependencias y Riesgos | 8. Gobernanza y Cumplimiento | 9. Métricas de Éxito |
| :--- | :--- | :--- |
| **¿El éxito DEPENDE de alguien más?** | **¿Cuáles son las REGLAS DEL JUEGO?** | **¿Cómo sabremos que estamos GANANDO?** |
| • **Dependencias Internas:** Colaboración activa de **todas** las Jefaturas de División para nombrar "Dueños de Datos" y facilitar la catalogación. Dependencia del equipo de TI para la implementación de controles. <br>• **Dependencias Externas:** Ninguna crítica para el MVP. <br>• **Riesgos de Dependencia:** Resistencia cultural al cambio y a la transparencia en el manejo de datos. Baja priorización por parte de las divisiones. | • **Nodo de Gobernanza:** Comité de Transformación Digital (CTD). <br>• **Dueño de Producto/Servicio:** Jefe/a de la Oficina Digital e IA (ODIA). <br>• **Anclaje Regulatorio (Overlays):** Ley N° 21.719 (Protección de Datos), Ley N° 21.663 (Ciberseguridad), Marco de Gestión de Datos del Estado (SGD), Normas Técnicas de Ley 21.180. | • **Resultados Clave (KRs):** <br> - KR1: Lograr que el 50% de los datasets críticos del GORE estén catalogados y con un Dueño asignado en 6 meses. <br> - KR2: Reducir en un 90% los "activos de información sombra" (planillas Excel no gobernadas) en el proceso IPR en 9 meses. <br>• **Objetivos de Nivel de Servicio (SLOs):** <br> - Disponibilidad del Catálogo de Datos > 99.5%. <br>• **Métricas de Experiencia (UX):** <br> - Tiempo para encontrar un dataset crítico < 5 minutos. |
