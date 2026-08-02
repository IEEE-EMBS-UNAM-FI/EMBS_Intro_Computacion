# Primer_PRD: Calculadora de Dosis y Generador de Recetas medicas

## Sistema de locomoción
| **Target release** |  |
| --- | --- |
| **Epic** |  |
| **Document status** | **PROPOSAL** |
| **Document owner** | Fortis |
| **Project Manager** | Jess |
| **Responsable de Viabilidad** | German |


## **Objective**
Proporcionar una herramienta que calcule automáticamente las dosis de medicamentos basadas en el peso y la especie del paciente, y que genere una receta médica en formato PDF 


## **Success metrics**



| **Goal** | **Metric** |
| Prevención de errores de medicación|  ninguna discrepancia en cálculos matemáticos de dosificación |
| Uso de la herramienta | la mayoria de las consultas utilizan el generador en lugar de recetas manuales |
| --- | --- |
| --- | --- |

## **Assumptions**
- El expediente clínico base del paciente ya contiene información actualizada sobre su peso y especie.
- El veterinario conoce la dosis recomendada por kilogramo (mg/kg) del medicamento a recetar.

## **Milestones**
Desarrollo de la matemática de cálculo (peso vs. dosis) en el lado del cliente y la creación del diseño y plantilla base de la receta médica (logo de la clínica, datos del médico, firma).

## **Requirements**

| **Requirement** | **User Story** | **Importance** | **Issue** | **Notes** |
|R-01: Calculadora de dosis|quiero ingresar el peso del animal y la concentración del fármaco para obtener los mililitros y dias de trtamiento| **Alta** | --- | --- |
| R-02: Generación de PDF | presionar un botón para transformar las indicaciones médicas en una receta con formato en PDF. | **media** | --- | --- |
| --- | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |


## **Design and usability requirements**

- Campos numéricos con validación para evitar el ingreso de letras o valores negativos.
- Diseño limpio del PDF, con tipografía clara y tamaño de letra legible 

## **Open Questions**

| **Question** | **Answer** | **Date Answered** |
| ¿Cómo se gestionará la firma digital o el sello del médico veterinario en el documento? | --- | --- |
|  |  |  |

## **Out of Scope**
Facturación o cobro de la consulta médica.

## **Reference materials**
