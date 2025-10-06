# Mapeo de Historias (Story Map) - EV NEXO GORE - Ciclo de Vida de IPR

ID: `NEXO-IPR-SM-001`
Versión: 1.0
Fecha: 2025-10-06

### Propósito

Este artefacto traduce el `Canvas de EV` de `NEXO GORE - IPR` en un backlog de desarrollo visual y priorizado. Su objetivo es definir los incrementos de valor sucesivos, comenzando por el "Esqueleto Andante" (MVP), para asegurar una entrega iterativa y alineada con la estrategia.

---

### La Espina Dorsal (Actividades del Usuario)

La espina dorsal representa el flujo de valor de punta a punta para la gestión de una Intervención Pública Regional (IPR).

| Formulación Asistida | Evaluación y Aprobación | Ejecución y Seguimiento | Cierre y Aprendizaje |
| :--- | :--- | :--- | :--- |

---

### El Cuerpo (Historias de Usuario por Actividad)

*Las historias se ordenan verticalmente por prioridad. Las que están por encima de la primera línea (`--- MVP: Esqueleto Andante ---`) constituyen el Mínimo Producto Viable.*

| Formulación Asistida | Evaluación y Aprobación | Ejecución y Seguimiento | Cierre y Aprendizaje |
| :--- | :--- | :--- | :--- |
| **Como Formulador,** quiero crear una nueva Ficha de Idea de IPR con sus datos básicos (nombre, objetivo, división) para registrarla en el sistema. | **Como Analista DIPIR,** quiero ver una lista de IPRs "Ingresadas" para asignarme una y comenzar la evaluación de admisibilidad. | **Como Jefe de División,** quiero registrar manualmente el porcentaje de avance físico y financiero de una IPR "En Ejecución" para mantener la información actualizada. | **Como Analista DIPIR,** quiero marcar una IPR como "Finalizada" para iniciar el proceso de cierre. |
| **Como Formulador,** quiero adjuntar documentos de respaldo a mi Ficha de Idea. | **Como Analista DIPIR,** quiero cambiar el estado de una IPR a "Admisible" o "No Admisible" y registrar mis observaciones. | **Como Jefe de División,** quiero adjuntar informes de avance o fotografías como evidencia del progreso. | **Como Jefe de División,** quiero adjuntar el informe de cierre final y los documentos de rendición de cuentas. |
| **Como Formulador,** quiero ver el estado de mi IPR ("Ingresada", "En Evaluación", "Aprobada", etc.) en un panel simple. | **Como Jefe de División (DIPIR),** quiero recibir una notificación para revisar las IPRs marcadas como "Admisibles". | | **Como Administrador/a Regional,** quiero ver un listado de todas las IPRs "Finalizadas" para dar el visto bueno de cierre administrativo. |
| **Como Formulador,** quiero editar mi Ficha de Idea mientras está en estado "Borrador". | **Como Jefe de División (DIPIR),** quiero aprobar o rechazar la admisibilidad, cambiando el estado a "Priorización" o "Rechazada" y notificando al formulador. | | |
| --- | --- | --- | --- |
| **< Rebanada 1: Esqueleto Andante (MVP) >** | **< Rebanada 1: Esqueleto Andante (MVP) >** | **< Rebanada 1: Esqueleto Andante (MVP) >** | **< Rebanada 1: Esqueleto Andante (MVP) >** |
| --- | --- | --- | --- |
| **Como Formulador,** quiero que el sistema me asista con plantillas y ejemplos para cada sección de la Ficha (IA Copiloto). | **Como CTD,** quiero que el sistema orqueste el flujo de aprobación, asignando tareas automáticamente según reglas de negocio (Motor BPMN). | **Como Jefe de División,** quiero ver un dashboard con alertas predictivas que me indiquen qué IPRs tienen riesgo de desviarse del plan. | **Como Analista DIPLADE,** quiero que el sistema capture automáticamente las lecciones aprendidas y las vincule al Mapa de Capacidades. |
| **Como Formulador,** quiero que el sistema valide automáticamente mi RUT contra el Registro Civil y pre-rellene mis datos. | **Como Asesor Jurídico,** quiero que el sistema genere automáticamente el borrador del Convenio de Transferencia cuando una IPR es aprobada (IA Copiloto). | **Como Gobernador,** quiero consultar en lenguaje natural el estado de la cartera de inversión regional ("¿cuál es el avance del Trazo Rojo de Ñuble 250?"). | **Como IA,** quiero analizar los resultados de las IPRs cerradas para identificar patrones que mejoren la evaluación de futuras iniciativas. |
| **Como Formulador,** quiero adjuntar información geoespacial a mi IPR, visualizándola en un mapa (Integración IDE Ñuble). | **Como Analista DAF,** quiero que el sistema pre-audite los documentos de una IPR para verificar el cumplimiento con la normativa CGR (IA Copiloto). | **Como Ciudadano,** quiero ver el avance de las IPRs de mi comuna en un portal de transparencia (`Mi Ñuble` App). | |
| --- | --- | --- | --- |
| **< Rebanada 2: Orquestación e IA >** | **< Rebanada 2: Orquestación e IA >** | **< Rebanada 2: Orquestación e IA >** | **< Rebanada 2: Orquestación e IA >** |
| --- | --- | --- | --- |

### Hoja de Ruta del MVP (Esqueleto Andante)

El objetivo del MVP es validar el flujo de valor de punta a punta con la mínima funcionalidad posible, pero que sea completa y entregue valor real.

1.  **Sprint 1: Fundación y Formulación.**
    *   **Historias:** Crear Ficha de IPR, adjuntar documentos, ver panel de estado simple.
    *   **Técnico:** Montar arquitectura base, modelo de datos inicial, sistema de autenticación (ClaveÚnica).
2.  **Sprint 2: Evaluación y Aprobación.**
    *   **Historias:** Flujo de admisibilidad (Analista -> Jefe de División), notificaciones básicas por email.
    *   **Técnico:** Implementar máquina de estados para el ciclo de vida de la IPR.
3.  **Sprint 3: Ejecución y Cierre.**
    *   **Historias:** Funcionalidad para registrar avance manual y marcar como finalizada.
    *   **Técnico:** Desarrollar vistas de seguimiento y roles de usuario.
4.  **Sprint 4: Despliegue y Puesta en Marcha.**
    *   **Acción:** Desplegar el MVP en un ambiente controlado y realizar un piloto con una División (ej. DIPLADE).
    *   **Objetivo:** Recopilar feedback real para informar la siguiente rebanada de valor.
