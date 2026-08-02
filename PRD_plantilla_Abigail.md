# Gestión de Citas, agenda y triaje de pacientes

## Equipo de datos
| **Target release** | Lunes 10 Agosto |
| --- | --- |
| **Epic** |  |
| **Document status** | **PROPOSAL** |
| **Document owner** | Abigail |
| **Project Manager** | Jess |
| **Responsable de Viabilidad** | Germán |


## **Objective**

Diseñar e implementar un sistema de programación de citas y recepción de pacientes que mejore los tiempos de atención y gestione la disponibilidad de los médicos veterinarios 

## **Success metrics**

Tener un módulo de agenda y recepción que clasifique correctamente las citas y reduzca tiempos de espera

| **Goal** | **Metric** |
| --- | --- |
| **Priorizar urgencias** | 100% de las citas etiquetadas como "urgente" pasan a la cola inmediata |
| **Cero sobreagendamiento** | 0% de solapamiento de horarios no autorizados para un mismo veterinario |

## **Assumptions**
La clínica cuenta con un equipo de recepción (PC o laptop) para operar la agenda en tiempo real
Los veterinarios tienen horarios de atención predefinidos en el sistema
El cliente puede solicitar una cita vía telefónica, presencial o a través de la web

## **Milestones**
Definir el catálogo de servicios (Nombre, duración, costo)
Tener una lógica de asginación de triaje
Diseño de interfaz de agenda/calendario para recepción y veterinarios

## **Requirements**

| **Requirement** | **User Story** | **Importance** | **Issue** | **Notes** |
| --- | --- | --- | --- | --- |
| RF-1 El sistema debe permitir al cliente agendar citas | --- | **Alta** | RF-1 | Las citas se pueden realizar a través del número telefónico, presencial o por la página web |
| RF-2 El sistema debe permitir registrar una clasificación de llegada del paciente con nivel de gravedad | --- | **Alta** | RF-2 | El triaje se manejará con los colores: Verde, amarillo y rojo para priorizar su atencion|
| RF-3 El sistema debe permitir al personal clínico cambiar el estado de la cita| --- | **Alta** | RF-3 | El estado se manejara con: Agendada, confirmada, en sala de espera, en consulta, cancelada, no asistió para monitorear el flujo|
| RF-4 El sistema debe validar la disponibilidad del veterinario y consultorio antes de guardar una cita para evitar empalmes| --- | **Alta** | RF-4 | |
| RnF-1 El sistema debe tener un tiempo de respuesta de 1.5 segundos al cargar las citas en el calendario/agenda| --- | **Alta** | RnF-1 | Requiere optimización de consultas SQL|


## **Design and usability requirements**

---

## **Open Questions**

| **Question** | **Answer** | **Date Answered** |
| --- | --- | --- |
| ¿Qué pasa si llega una urgencia médica (rojo) y no hay veterinarios disponibles? |  |  |

## **Out of Scope**
Recordatorios automáticos por SMS o WhatsApp

## **Reference materials**
Guía clinicas para clasificación de urgencias
Ejemplos de UI estilo Google Calendars para recepción