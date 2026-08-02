# Hospitalización y registro de tratamientos

## Equipo de datos
| **Target release** | Lunes 10 Agosto |
| --- | --- |
| **Epic** |  |
| **Document status** | **PROPOSAL** |
| **Document owner** | Abigail |
| **Project Manager** | Jess |
| **Responsable de Viabilidad** | Germán |


## **Objective**

Diseñar e implementar un sistema de control de pacientes hospitalizados que permita el registor en tiempo real, la programación de administración de medicamentos con alertas, el monitoreo vital y el control de insumos consumidos

## **Success metrics**

Garantizar un correcto tratamiento de los pacientes internados y minimizar errores humanos en el cambio de turno

| **Goal** | **Metric** |
| --- | --- |
| **Puntualidad de medicamentos** | >95% de los medicamentos administrados se marcan dentro de un rango de 154 minutos respecto a la hora programada |
| **Cero omisiones en cambio de turno** | 100% de los pacientes hospitalizados con notas registradas al cambio de turno |
| **Trazabilidad de ocupación** | Visualizar en tiempo real el estado de disponibilidad de jaulas/camas en la clínica |

## **Assumptions**
El área de hospitalización cuenta con un dispositivo (tables/laptop) para el uso de médicos y enfermeros
La dosis de medicamentos se calculan de acuerdo al peso actual del paciente
Cada espacio de hospitalización (jaula/cama) está identificado en la clínica

## **Milestones**
Definir el esquema de base de datos para el ingreso/alta de pacientes
Lógica de motor de alertas e indicaciones médicas programadas por horarios
Tener un diseño de interfaz gráfica "Pizarra de hospitalización" para tener una vista general de los pacientes internados

## **Requirements**

| **Requirement** | **User Story** | **Importance** | **Issue** | **Notes** |
| --- | --- | --- | --- | --- |
| RF-1 El sistema debe permitir al veterinario dar de alta a un paciente a un paciente | --- | **Alta** | RF-1 | El alta a hospitalización permite una asignación a jaula/cama, motivo de ingreso y pronóstico inicial |
| RF-2 El sistema debe permitir al veterinario prescribir medicamentos ppara el paciente | --- | **Alta** | RF-2 | La prescripción de medicamentos solicita fármaco, dosis, vía de administración y frecuencia por horas|
| RF-3 El sistema debe permitir al enfermero marcar el estado de un medicamento como "Aplicado"| --- | **Alta** | RF-3 | Marcar el estado de un medicamento requiere la hora y firma del aplicador|
| RF-4 El sistema debe permitir al personal médico monitorear las constantes vitales de los pacientes| --- | **Alta** | RF-4 | Se registra peso, temperatura, frecuencia cardiaca/respiratoria, apetito y micción/defecación|
| RnF-1 El formulario de registro de constantes vitales no debe perder la información si la conexión se llega a perder| --- | **Alta** | RnF-1 | Implementar un guardado de local borrador|


## **Design and usability requirements**

---

## **Open Questions**

| **Question** | **Answer** | **Date Answered** |
| --- | --- | --- |
| ¿Que ocurre si un paciente cambia de jaula durante su estancia? |  |  |

## **Out of Scope**
Integración de bombas de infusión inteligentes mediante IoT

## **Reference materials**
Sistemas de Kardex médico electrónico