# PRD: Sistema de Telemetría Web para Collar de Monitoreo Térmico


## Sistema de locomoción
| **Target release** | Diciembre 2026 |
| --- | --- |
| **Epic** | Plataforma IoT para Monitoreo Biométrico |
| **Document status** | **PROPOSAL** |
| **Document owner** | Rodrigo Aguilar |
| **Project Manager** | Jessica Espejel |
| **Responsable de Viabilidad** | Germán |


## **Objective**
* Desarrollar y desplegar una aplicación web capaz de recibir, almacenar y visualizar en tiempo real los datos de temperatura capturados por el hardware de un collar. 

* El sistema deberá permitir el análisis histórico de los datos y la configuración de umbrales de alerta para prevenir problemas de salud.


## **Success metrics**
| **Goal** | **Metric** |
| --- | --- |
|**Baja Latencia de Transmisión**| < 5 segundos de retraso entre la lectura del sensor en el collar y la actualización en la plataforma web. |
|**Precisión de Visualización**| La interfaz web refleja el valor exacto de temperatura procesado, con una resolución de al menos 0.1 °C. |



## **Assumptions**
* El hardware del collar ya cuenta con un microcontrolador funcional, un sensor de temperatura calibrado y un módulo de transmisión (Wi-Fi, Bluetooth o LoRa) operativo.
* Existe una conexión a internet estable en el entorno donde operará el dispositivo emisor.

## **Milestones**
1. **Investigación**: Definición de los protocolos de comunicación y selección de las herramientas más pertinentes para el servidor.
1. **Diseño y Modelado**: Creación de la arquitectura de la base de datos para almacenar las series de tiempo y diseño inicial de la interfaz de usuario.

## **Requirements**

| **Requirement** | **User Story** | **Importance** | **Issue** | **Notes** |
| --- | --- | --- | --- | --- |
| **API de Recepción** | Como microcontrolador, necesito un endpoint seguro para enviar los datos de temperatura y el timestamp. | Alta | Backend | --- |
| **Dashboard en Tiempo Real** | Como usuario de la plataforma, quiero ver un indicador con la temperatura actual para conocer el estado inmediato. | Alta | Frontend | --- |
| **Gráficos Históricos** | Como analista, quiero poder visualizar el historial de la temperatura en una curva para identificar tendencias anómalas. | Media | Frontend | --- |


## **Design and usability requirements**
* **Accesibilidad**: Diseño de alto contraste con indicadores de color.
* **Responsividad**: La página web debe ser completamente funcional tanto en monitores de escritorio como en dispositivos móviles.


---

## **Open Questions**

| **Question** | **Answer** | **Date Answered** |
| --- | --- | --- |
| ¿Qué protocolo de capa de aplicación (MQTT vs HTTP) consumirá menos recursos energéticos en la batería del collar? |  |  |

## **Out of Scope**
* Diseño electrónico de la placa de circuito impreso (PCB) del collar.
* Modelado mecánico, manufactura y ergonomía de la carcasa del dispositivo físico.
* Selección de los componentes pasivos, microcontroladores y baterías del hardware.

## **Reference materials**
* Normativas: Estándares IEEE 802.11 (si es transmisión Wi-Fi) o IEEE 802.15.4 (para redes de área personal de baja tasa). Adicionalmente, revisar la normativa IEC 60601-1 si el collar se enfoca en uso clínico/médico humano.
* Documentación: Manuales técnicos de protocolos MQTT y plataformas de bases de datos para series de tiempo.