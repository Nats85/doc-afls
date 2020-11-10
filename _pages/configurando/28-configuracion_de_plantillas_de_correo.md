---
title: Configuración de plantillas de correo
chapter: "configurando"
---

Bajo el módulo **Plantillas de correo** encontrará 6 submódulos para configuración y personalización de los mensajes que se enviarán al cliente para informarlo sobre las órdenes de trabajo.

![]({{ site.baseurl }}/assets/images/image128.png)

En cada uno de los submódulos encontrará opciones de personalización que son comunes para todos. Podrá escoger la opción de enviar correo o no, además de personalizar el mensaje e insertar tokens que se reemplazan con la información de la orden. También puede restaurar la plantilla y dejar la que está por defecto haciendo clic en **Restaurar plantilla**.

![]({{ site.baseurl }}/assets/images/image129.png)

Los tokens son textos rápidos que se rellenan con la información que está en las órdenes de trabajo, ej. Un saludo al cliente por su nombre podría redactarse como: Hola, Señor(a) Plantilla:ClientName.

![]({{ site.baseurl }}/assets/images/image130.png)

_Lista de Tokens_

Una vez finalice la plantilla haga clic en **Guardar**, o **Cancelar** si no desea guardar los cambios.

Con el fin de complementar el uso de las plantillas de correo dentro de AFLS, se propone habilitar el uso de las macros para incluir información relacionada con el caso. En algunos casos los tokens harán referencia a valores que pueden aún no existir, por ejemplo, la fecha de atención si aún no ha sido asignada. Estas excepciones se detallan en la tabla adjunta.

Para el uso de los tokens se propone utilizar doble corchete, ej. {{Id}}. Estos tokens no manejarán multilenguaje, siempre serán las mismas cadenas para todos los lenguajes soportados en AFLS. Los tokens no tendrán en cuenta el uso de mayúsculas o minúsculas.

| **Token** | **Definición** | **Excepciones** |
| --- | --- | --- |
| {{WorkOrder}} | Número de orden |  |
| {{AgentName}} | Nombre del agente que atiende la orden | Si no ha sido asignada aparecerá: Sin definir aún. (en multilenguaje) |
| {{AttentionDate}} | Fecha de atención | Si no ha sido asignada, aparecerá: Sin definir aún. |
| {{AgentPhone}} | Teléfono del agente que atiende la orden | Si no ha sido asignada, aparecerá. No disponible. |
| {{Subject}} | Asunto de la orden | Subject completo |
| {{ClientName}} | Nombre del cliente | Ninguna, siempre debe existir. |
| {{ClientPhone}} | Teléfono del cliente | Ninguna, siempre debe existir. |
| {{Direccion}} | Dirección de la orden | Ninguna, siempre debe tener una dirección |

### **General**

En la parte superior de este submódulo se encuentran las plantillas para los mensajes que informan a los clientes sobre el estado de sus órdenes de trabajo, a saber:

![]({{ site.baseurl }}/assets/images/image131.png)

*   **Registro:** Se envía al cliente como confirmación de la recepción de una nueva orden de trabajo.
*   **Asignación:** Informa a un cliente la fecha y el responsable de atender el caso.
*   **Retraso:** Se envía al cliente cuando el especialista no puede cumplir la cita.
*   **Cambio de especialista:** Se envía cuando se ha modificado una cita para informar al cliente la nueva persona que la atenderá.
*   **Cancelación:** Se envía al cliente cuando se cancela una orden de trabajo.
*   **Ejecutada:** Se envía al cliente cuando una orden se ha finalizado con éxito.
*   **Vinculación:** Se envía a los especialistas para que puedan vincular sus dispositivos fácilmente.
*   **Proveedores:** Se envía cada vez que se crea una orden, o se reasigne a un proveedor.

### **Encuestas**

En la parte superior de este submódulo se encuentran las plantillas para los mensajes relacionados con encuestas, a saber:

![]({{ site.baseurl }}/assets/images/image132.png)

*   **Encuesta de Satisfacción:** Se envía a los clientes una vez se ha finalizado la ejecución de un servicio. Contiene un enlace a la página donde está la encuesta.
*   **Alerta de Nivel de Satisfacción:** Se envía a los monitores encargados de satisfacción del cliente cuando una encuesta está por debajo del mínimo permitido.
*   **Notificación de medición de encuesta:** Este es un correo de informe periódico que se envía a los monitores para que conozcan el nivel de satisfacción general.
*   **Notificación de resumen de encuesta:** Este es un correo de informe que se envía al cliente como resumen una vez ha calificado la encuesta.

### **SLA**

Las plantillas del submódulo SLA se utilizan para notificar a los administradores cuando se acerca una fecha relevante relacionada con los SLA configurados.


![]({{ site.baseurl }}/assets/images/image133.png)


*   **Revisión**: plantilla para el correo que notificará cuando se cumpla la fecha de revisión configurada en los SLA.
*   **Finalización**: plantilla para el correo que notificará cuando un SLA está a punto de finalizar.

### **UC**

![]({{ site.baseurl }}/assets/images/image134.png)

Las plantillas del submódulo UC se utilizan para notificar a los administradores cuando se acerca una fecha relevante relacionada con la medición del nivel de cumplimiento de los proveedores externos.

*   **Revisión**: plantilla para el correo que notificará cuando se cumpla la fecha de revisión configurada en los UC.
*   **Finalización**: plantilla para el correo que notificará cuando un UC está a punto de finalizar.

### **OLA**

Las plantillas del submódulo OLA se utilizan para notificar a los administradores cuando se acerca una fecha relevante relacionada con la medición del nivel de cumplimiento de los proveedores internos.

![]({{ site.baseurl }}/assets/images/image135.png)

*   **Revisión**: plantilla para el correo que notificará cuando se cumpla la fecha de revisión configurada en los OLA.
*   **Finalización**: plantilla para el correo que notificará cuando un OLA está a punto de finalizar.

### **Assist Me** 

Las plantillas de este submódulo están relacionadas con los mensajes que reciben los clientes que hacen parte del canal de asistencia Assist Me.

*   **Notificación de cuenta de usuarios AssistMe:** Informa al usuario final los datos de acceso y URL para ingreso a AssistMe.
*   **Notificación de orden registrada desde AssistMe:** Notifica a los usuarios la creación de una nueva solicitud registrada desde el canal.
*   **Verificación datos de usuario:** Notifica que el usuario realizó registro en el canal.
*   **Restablecer contraseña:** Envía al usuario el link para poder restablecer la contraseña.


![]({{ site.baseurl }}/assets/images/image136.png)
