---
title: Configuración de acuerdos de niveles operacionales (OLA)
chapter: "configurando"
---

A través del módulo de niveles operacionales es posible definir los acuerdos con los proveedores internos de un servicio.

La configuración de los OLA en Aranda FIELD SERVICE se realiza a través de cronómetros y acuerdos de tiempo. Las configuraciones de los tiempos relacionados con un OLA son globales (se definen una vez), sin embargo, algunas de sus características pueden ser específicas a un modelo en particular.

Los OLA pueden asociarse a servicios o a proveedores. Aranda FIELD SERVICE se encarga de seleccionar el OLA más apropiado siempre y cuando se encuentre vigente.

Para crear nuevos OLA se debe hacer clic en el botón **Nuevo** e ingresar la siguiente información:

![]({{ site.baseurl }}/assets/images/image24.png)

### **Detalle del OLA**

*   **Nombre del OLA:** Nombre que se le dará al acuerdo.
*   **Descripción:** Texto claro y explicativo del acuerdo OLA.

### **Duración del OLA**

*   **Fecha de inicio:** Permite establecer la fecha de inicio del OLA.
*   **Fecha de finalización:** Permite establecer la fecha de finalización del OLA, al ingresar una fecha en este campo se habilita el campo Alarma para la fecha de finalización.
*   **Fecha de revisión:** Permite establecer la fecha de revisión del OLA, al ingresar una fecha en este campo se habilita el campo Alarma para la fecha de revisión.
*   **Costo relacionado al OLA:** Permite establecer el costo relacionado a la ejecución del OLA.
*   **Penalización por incumplimiento de OLA:** Permite establecer el valor del incumplimiento cuando se vence el OLA.

| **Nota**: El usuario puede habilitar el envío de una alarma cuando se acerque la fecha de revisión o la fecha de finalización del OLA, esto hará que se le envíe a los administradores una notificación con la información correspondiente. |
| --- |

### **Acuerdos de tiempos**

En esta pestaña se muestra un buscador que funciona con la característica de autocompletar y lista los cronómetros que existan en AFLS, al seleccionar uno de los cronómetros este se muestra con los respectivos campos para ingresar las horas, los minutos y el porcentaje de cumplimiento que debe tener dicho cronómetro para el OLA. Todos los OLA deben tener solo un cronómetro marcado como principal y es el que se va a visualizar en la orden de trabajo.

![]({{ site.baseurl }}/assets/images/image25.png)

| **Nota**: Si el usuario cambia el cronómetro de básico a avanzado, se copian los valores a las 3 prioridades **Emergencia**, **Normal** y **Prioridad**; si el usuario cambia de avanzando a básico, se limpian todos los campos dejándolos vacíos en básico (siguen siendo obligatorios) |
| --- |

![]({{ site.baseurl }}/assets/images/image26.png)

### **Archivos adjuntos**

En esta pestaña puede adjuntar archivos del OLA, siempre que no excedan el peso de 10 MB.


![]({{ site.baseurl }}/assets/images/image27.png)
