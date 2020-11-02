---
title: Configuración de acuerdos de contratos de apoyo (UC)
chapter: "configurando"
---

A través del módulo de niveles de contratos de apoyo es posible definir los acuerdos con los proveedores externos de un servicio.

La configuración de los UC en Aranda FIELD SERVICE se realiza a través de cronómetros y acuerdos de tiempo. Las configuraciones de los tiempos relacionados con un UC son globales (se definen una vez), sin embargo, algunas de sus características pueden ser específicas a un modelo en particular.

Los UC pueden asociarse a servicios o a proveedores. Aranda FIELD SERVICE se encarga de seleccionar el UC más apropiado siempre y cuando se encuentre vigente.

Para crear nuevos UC haga clic en el botón **Nuevo** e ingrese la siguiente información:

![]({{ site.baseurl }}/assets/images/image28.png)

### **Detalle del UC** {#detalle-del-uc}

*   **Nombre del UC:** Nombre que se le dará al acuerdo.
*   **Descripción:** Texto claro y explicativo del acuerdo UC.

### **Duración del UC** {#duraci-n-del-uc}

*   **Fecha de inicio:** permite establecer la fecha de inicio del UC.
*   **Fecha de finalización:** permite establecer la fecha de finalización del UC, al ingresar una fecha en este campo se habilita el campo Alarma para la fecha de finalización.
*   **Fecha de revisión:** permite establecer la fecha de revisión del UC, al ingresar una fecha en este campo se habilita el campo de alarma para la fecha de revisión.
*   **Costo relacionado al UC:** permite establecer el costo relacionado a la ejecución del UC.
*   **Penalización por incumplimiento de UC:** permite establecer el valor del incumplimiento cuando se vence el UC.

| **Nota**: El usuario puede habilitar el envío enviar alarma cuando se acerque la fecha de revisión o la fecha de finalización del UC, esto hará que se le envíe a los administradores una notificación con la información correspondiente. |
| --- |

### **Acuerdos de tiempos** {#acuerdos-de-tiempos}

En esta pestaña se muestra un buscador que funciona con la característica de autocompletar y lista los cronómetros que existan en AFLS, al seleccionar alguno de los cronómetros este se muestra con los respectivos campos para ingresar las horas, los minutos y el porcentaje de cumplimiento que debe tener dicho cronómetro para el UC. Todos los UC deben tener solo un cronómetro marcado como principal y es el que se va a visualizar en la orden de trabajo.

![]({{ site.baseurl }}/assets/images/image29.png)

| **Nota**: si el usuario cambia el cronómetro de básico a avanzado, se copian los valores a las 3 prioridades **Emergencia**, **Normal** y **Prioridad**, si el usuario cambia de avanzando a básico, se limpian todos los campos dejándolos vacíos en básico (siguen siendo obligatorios) |
| --- |


![]({{ site.baseurl }}/assets/images/image30.png)


### **Archivos adjuntos** {#archivos-adjuntos}

En esta pestaña puede adjuntar archivos del UC, siempre que no excedan el peso de 10 MB.

![]({{ site.baseurl }}/assets/images/image31.png)
