# Segundo_RPD : Historial Clínico y Diagnósticos

## Sistema de locomoción
| **Target release** |  |
| --- | --- |
| **Epic** |  |
| **Document status** | **PROPOSAL** |
| **Document owner** | Miguel Angel Fortis Peréz |
| **Project Manager** | Jess |
| **Responsable de Viabilidad** |German |

## **Objective**
Proporcionar al personal médico una interfaz para registrar, consultar y actualizar de forma estructurada el historial clínico, diagnósticos y estudios de pacientes.

## **Success metrics**

| **Goal** | **Metric** |
| --- | --- |
| Reducción del tiempo de consulta de expedientes | Búsqueda y despliegue del historial de manera eficiente |
| Integridad de los datos médicos | ninguna pérdida de registros en la base de datos |
| Tasa de uso del módulo | muchas de las nuevas consultas registradas digitalmente |

## **Assumptions**
* Los usuarios tienen conocimientos básicos en navegación de software clínico.
* El servidor y la base de datos estan operativos.

## **Milestones**
3. Desarrollo de la interfaz de usuario para el registro médico.
4. Validación de usabilidad con la responsable de viabilidad 

## **Requirements**

| **Requirement** | **User Story** | **Importance** | **Issue** | **Notes** |
| --- | --- | --- | --- | --- |
| R-01: Creación de expediente base | Como veterinario, quiero registrar los datos médicos iniciales de un paciente para abrir su historial. | **Alta** | #10 | Incluye especie, raza, peso y antecedentes. |
| R-02: Registro de diagnósticos | Como veterinario, quiero agregar el diagnóstico y notas clínicas de la consulta actual. | **Alta** | #11 | Debe vincularse a la cita correspondiente. |
| R-03: Alertas médicas y alergias | Como usuario, quiero visualizar alertas destacadas de alergias al abrir el expediente para evitar mala praxis. | **media**|
| R-04: Adjuntar resultados de laboratorio | Como técnico, quiero subir archivos de resultados de laboratorio al expediente para centralizar la información. |**media**#13 | Soporte para formatos PDF y JPG. |

## **Design and usability requirements**
* Interfaz que priorice la lectura rápida de datos médicos sin distracciones.
* Formularios optimizados para navegación por teclado para agilizar la captura de información durante la consulta.

## **Open Questions**

| **Question** | **Answer** | **Date Answered** |
| --- | --- | --- |
| ¿Se implementará un catálogo estandarizado precargado para razas y especies? | | |
| ¿Cuál será el límite de almacenamiento permitido para los archivos adjuntos de laboratorio por paciente? | | |

## **Out of Scope**
* Gestión de citas, agenda y triaje 
* Hospitalización y registro de tratamientos 
* Módulo de cobros, facturación o control de inventario de medicamentos.

## **Reference materials**
