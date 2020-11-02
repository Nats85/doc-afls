---
title: Configuración de Acuerdos de Nivel de Servicio (SLA)
chapter: "configurando"
---

Tan importante como brindar un buen servicio es brindarlo a tiempo. A través del módulo de niveles de servicio es posible definir los tiempos que un especialista puede necesitar para la atención de una orden y los umbrales para su ejecución.

La configuración de los SLA en Aranda FIELD SERVICE se realiza a través de cronómetros y acuerdos de tiempo. Las configuraciones de los tiempos relacionados con un SLA son globales (se definen una vez), sin embargo, algunas de sus características pueden ser específicas a un modelo de negocio en particular.

Los ANS pueden asociarse a servicios, a compañías o a clientes. Aranda FIELD SERVICE se encarga de seleccionar el SLA más apropiado siempre y cuando se encuentre vigente.

Para crear nuevos SLA haga clic en el botón **Nuevo** e ingrese la siguiente información:

![]({{ site.baseurl }}/assets/images/image20.png)


### **Detalle del SLA** {#detalle-del-sla}

*   **Nombre del SLA:** Nombre que se le dará al acuerdo.
*   **Descripción:** Texto claro y explicativo del acuerdo ANS.

### **Duración del SLA** {#duraci-n-del-sla}

*   **Fecha de inicio:** permite establecer la fecha de inicio del SLA.
*   **Fecha de finalización:** permite establecer la fecha de finalización del SLA, al ingresar una fecha en este campo se habilita el campo de alarma para la fecha de finalización.
*   **Fecha de revisión:** permite establecer la fecha de revisión del SLA, al ingresar una fecha en este campo se habilita el campo de alarma para la fecha de revisión.
*   **Costo relacionado al SLA:** permite establecer el costo relacionado a la ejecución del SLA.
*   **Penalización por incumplimiento de SLA:** permite establecer el valor por incumplimiento cuando se vence el SLA.

| **Nota**: el usuario puede habilitar el envío de una alarma cuando se acerque la fecha de revisión o la fecha de finalización del ANS, esto hará que se le envíe a los administradores una notificación con la información correspondiente. |
| --- |

### **Acuerdos de tiempos** {#acuerdos-de-tiempos}

En esta pestaña se muestra un buscador que funciona con la característica de autocompletar y lista los cronómetros que existen en AFLS, al seleccionar uno de los cronómetros este se muestra con los respectivos campos para ingresar las horas, los minutos y el porcentaje de cumplimiento que debe tener dicho cronómetro para el SLA. Todos los SLA deben tener solo un cronómetro marcado como principal y es el que se va a visualizar en la orden de trabajo.

![]({{ site.baseurl }}/assets/images/image21.png)

| **Nota**: si el usuario cambia el cronómetro de básico a avanzado, se copian los valores a las 3 prioridades de **Emergencia**, **Normal** y **Prioridad**; si el usuario cambia de avanzando a básico, se limpian todos los campos dejándolos vacíos y en básico (se mantienen obligatorios). |
| --- |

![]({{ site.baseurl }}/assets/images/image22.png)

### **Archivos adjuntos** {#archivos-adjuntos}

En esta pestaña puede adjuntar archivos del SLA siempre que no excedan de 10 MB.

![]({{ site.baseurl }}/assets/images/image23.png)
