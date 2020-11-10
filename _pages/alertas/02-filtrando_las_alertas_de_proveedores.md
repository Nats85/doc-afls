---
title: Filtrando las alertas de proveedores
chapter: "alertas"
---

Los filtros para facilitar la búsqueda de alertas de proveedores generadas son los siguientes:

**Proveedor**: el monitor solo podrá visualizar los proveedores que tiene asignados, por lo tanto, podrá filtrar las alertas solo por dichos proveedores desde el selector. Cuando se ingresa con un perfil de usuario Despachador + Monitor el selector contará con la opción de Todos los proveedores.

### **Tipos de Alerta:** {#tipos-de-alerta}

*   **Asignación:** son las alertas creadas por el motor de asignación cuando no es posible encontrar las personas idóneas para ejecutar una orden de trabajo. Dentro de esta categoría se encuentra la alerta de orden no asignada.
*   **Cumplimiento:** son todas aquellas alertas generadas por la operación cuando se incumplen las citas o los acuerdos de nivel de servicio de las órdenes de trabajo. Dentro de esta categoría se encuentran:
*   **Orden sin zona:** se genera cuando se crea una orden sin zona de cobertura.
*   **Asignación de proveedor:** cuando no es posible asignar un proveedor a la orden de trabajo.
*   **Orden no ejecutada:** cuando una orden que estaba programada no fue ejecutada.
*   **Solicitud de tiempo:** cuando un especialista desde la consola móvil solicita más tiempo para completar su orden de trabajo.
*   **Cita incumplida:** cuando un especialista incumple la cita pactada con el cliente para la ejecución de un servicio
*   **Acuerdo incumplido:** cuando alguno de los acuerdos, SLA, OLA o UC no alcanzó el 100%.
*   **Reasignación de órdenes:** cuando una orden cambia de un proveedor a otro.
*   **No se ha iniciado la gestión en campo de la orden de trabajo:** cuando una orden de trabajo ABIERTA/PROGRAMADA supera el tiempo de espera definido para que el especialista inicie el desplazamiento hacia la misma.
*   **No se identifica movimiento del especialista:** cuando el GPS del dispositivo del especialista no ha detectado movimiento durante un tiempo definido.
*   **No se ha iniciado tarea:** cuando no se registra inicio en una tarea programada.
*   **Satisfacción:** son las alertas generadas por una baja puntuación de las encuestas por parte de los usuarios. Dentro de esta categoría se encuentran:
*   **Nivel de satisfacción de una orden de trabajo:** cuando una orden recibe una baja calificación del cliente.
*   **Encuesta no calificada:** cuando transcurre un tiempo determinado y la encuesta aún no ha sido calificada.
*   **Resultados por debajo del nivel esperado:** cuando los resultados de un informe de nivel de satisfacción están por debajo de los límites definidos.
*   **Inventario:** son las alertas que se generan cuando la cantidad de un producto está por debajo de los niveles permitidos en el inventario. Dentro de esta categoría se encuentran:
*   **Nivel mínimo de inventario:** cuando un producto alcanza la cantidad mínima de inventario.
*   **Existencias no encontradas:** cuando un especialista solicita inventario adicional por inexistencia en el inventario actual.

**Recálculo de órdenes de trabajo (por alerta de cumplimiento)**

Cuando un especialista en campo solicita más tiempo para atender la orden, el monitor es responsable de aceptar o rechazar la petición.

![]({{ site.baseurl }}/assets/images/image327.png)

_Alerta de solicitud de tiempo_

Al seleccionar la notificación y presionar el botón **Aprobar**, la herramienta desplegará una pantalla donde el monitor podrá tomar la decisión adecuada teniendo en cuenta tres factores:

*   Citas incumplidas hasta el momento.
*   Número de órdenes por reasignar.
*   Ordenes de trabajo próximas a vencer.

![]({{ site.baseurl }}/assets/images/image328.png)

_Pantalla al seleccionar Aprobar_

El motor recalculará las órdenes pendientes teniendo en cuenta tres opciones posibles:

*   Aceptar el tiempo y cumplir la mayor cantidad de citas posibles.
*   Aceptar el tiempo y reorganizar la agenda para optimizar la operación.
*   No aceptar el tiempo.

| **Nota:** por defecto se realiza la primera simulación automáticamente. Cada simulación muestra la cantidad de órdenes afectadas para cada caso y sus respectivas ID para ser consultadas. Esta pantalla solo se visualizará si se afecta alguna orden al aprobar el tiempo solicitado por el especialista, de lo contrario se visualizará un mensaje confirmando la aprobación de tiempo. |
| --- |

Si la solicitud de tiempo no corresponde al día actual, las opciones de aprobar y rechazar serán deshabilitadas.

Una vez aceptada alguna de las simulaciones, la agenda del especialista se actualizará con la información simulada.

El ciclo de vida de las alertas se mueve a través de tres estados diferentes:

*   **Nueva**: alertas creadas por el sistema que no se han validado.
*   **Revisada**: alertas que requieren algún tipo de acción por parte de los usuarios o los monitores.
*   **Cerrada**: alertas validadas que no importan o que ya fueron revisadas en la operación.

#### Visualización de alertas de proveedores {#visualizaci-n-de-alertas-de-proveedores}

![]({{ site.baseurl }}/assets/images/image329.png)

Cada alerta incluye información relevante de la operación. En el detalle de la alerta es posible cambiar el estado adicionando un mensaje.

| **Nota:** si se cambia el estado de una orden a EJECUTADA o CANCELADA, la alerta ya no se visualizará en este módulo, sino directamente en el de órdenes de trabajo, en el estado que se le haya asignado. |
| --- |
