---
title: Creación de órdenes de trabajo
chapter: "gestionando"
---

Para generar una orden de trabajo, haga clic en el botón **Nueva orden** en la parte superior de la consola de despacho y complete los siguientes campos:

*   Nombre o código único del cliente. A partir de esto, se habilitan los datos básicos de la orden.
*   Los **datos básicos** corresponden al nombre de solicitante de la cita, teléfono, correo, dirección y detalle dirección. Si el cliente cuenta con estos datos, se cargarán de forma automática. En este punto se puede editar la dirección y su detalle, si se requiere.
*   La **dirección** definida se presentará de forma gráfica en el mapa.

| **Nota**: en caso de tener algún proveedor de mapas diferente a Google, es necesario especificar las direcciones con mayor detalle, incluyendo el barrio, la localidad y el municipio para que la calibración sea más exacta. |
| --- |

Luego seleccione el servicio que requiere el cliente. Si el servicio es tipo **Estándar** se mantienen en el formulario los datos básicos como los diligenció el despachador.

![]({{ site.baseurl }}/assets/images/image201.png)

_Pantalla de creación de orden con servicio tipo estándar_

Si el servicio es tipo **Desplazamiento** se mostrarán dos nuevos campos: **Dirección de destino** y **Detalle de dirección de destino**, para ingresar la información del punto al cual se dirige el cliente.

![]({{ site.baseurl }}/assets/images/image202.png)

_Pantalla de creación de orden con servicio tipo desplazamiento_****

*   La **dirección de destino** permite al despachador definir un desplazamiento de un punto A a un punto B y visualizarlo en el mapa.
*   En el campo de **servicio** se visualiza una etiqueta que muestra la cantidad de inventario configurado por defecto en el servicio.
*   Se muestra el ANS configurado para el servicio seleccionado, el cual dependerá de la configuración del servicio para el cliente, la compañía del cliente o por defecto en el servicio.

| **Nota**: si un ANS se encuentra vencido no se permitirá la creación de órdenes para el servicio, es necesario cambiar las fechas para poder visualizarlo. |
| --- |

*   En **Tipo de orden** podrá seleccionar si la orden es **Normal**, de **Emergencia** o de **Prioridad**. El tipo de orden solo se podrá cambiar si en el servicio se configuró esta opción.
*   El **Asunto** será el que se haya ingresado en el servicio, pero puede cambiarse si se requiere.
*   En **Descripción** puede detallar las tareas a ejecutar en la orden de trabajo o ampliar las características del servicio.
*   Puede adjuntar archivos a la orden de trabajo para agregar información necesaria para la evolución del servicio.

| **Nota**: Los tipos de archivos que se pueden agregar a la orden de trabajo pueden ser de formatos .doc, .xls, .ppt, .PDF y que no superen los 10 MB de tamaño. |
| --- |

El despachador podrá adicionar en cualquier momento, notas y avisos que ayuden al especialista en campo al desarrollo de la orden de trabajo. Estas notas serán visibles en la categoría comentarios de la orden de trabajo en la aplicación móvil del especialista en campo.

Una vez ingresada toda la información necesaria para despachar una orden de trabajo, AFLS se encargará de asociar el proveedor y el especialista indicados.

La nueva orden quedará con fecha de creación del momento en el que se generó y luego de asignarle el proveedor y el especialista, se le fijará una fecha de solución según el ANS del servicio.

Una vez creada la orden de trabajo y asignados los responsables y los recursos, el especialista tendrá la información pertinente para atender la orden en la fecha programada, el monitor podrá realizar el seguimiento y control, y el despachador podrá consultar, editar, reasignar y cerrar la orden.

### **Creación de una orden de emergencia o prioritaria** {#creaci-n-de-una-orden-de-emergencia-o-prioritaria}

![]({{ site.baseurl }}/assets/images/image203.png)

Las órdenes de emergencia o prioritarias son aquellas que no pueden esperar a ser asignadas automáticamente:

**Emergencia:** el especialista debe dejar el trabajo que esté realizando y dirigirse inmediatamente a solucionar la emergencia. La orden de trabajo que deja se reasignará a otro especialista.

**Prioritaria:** la orden debe atenderse lo antes posible; se asigna al especialista más cercano, quien debe finalizar el trabajo actual y luego dirigirse a la orden prioritaria.

Cuando el usuario despachador selecciona el tipo de orden como de **Emergencia** o de **Prioridad**, el motor de asignación tomará en consideración la distancia y las habilidades de los especialistas y avisará al más apropiado para que ejecute la orden rápidamente.

Con el fin de tener visibilidad sobre este tipo de órdenes, AFLS les asigna marcas que permiten a los despachadores y monitores ver cuáles son de **Emergencia** y cuáles de **Prioridad**.

![]({{ site.baseurl }}/assets/images/image204.png)

_Orden marcada como Emergencia_

![]({{ site.baseurl }}/assets/images/image205.png)

_Orden marcada como Prioridad_

### **Asignación de un especialista a la orden de trabajo** {#asignaci-n-de-un-especialista-a-la-orden-de-trabajo}

Una vez creada la orden, al abrirla, en la pestaña **Asignación** encontrará tres tipos posibles de asignación de especialistas:

*   **Asignación Automática:** la realiza el motor de asignación teniendo en cuenta la configuración de la orden creada y la de los especialistas en campo que pueden atender la orden.

![]({{ site.baseurl }}/assets/images/image206.png)

*   **Asignación por Restricción:** permite restringir la asignación seleccionando al menos uno de los siguientes criterios de restricción: **Proveedor**, **Especialista**, **Fecha Inicial** y **Jornada**.

El campo **Jornada** dependerá de la configuración de las variables del negocio.

![]({{ site.baseurl }}/assets/images/image207.png)

*   **Asignación Manual:** la realiza directamente el despachador teniendo en cuenta la disponibilidad del especialista por los filtros de proveedor y fecha de atención.

![]({{ site.baseurl }}/assets/images/image208.png)

### **Tareas** {#tareas}

Las tareas permiten hacer una gestión más minuciosa de una orden de trabajo, y un seguimiento más preciso de cada procedimiento. Las tareas están pensadas para que los especialistas las gestionen desde sus dispositivos de manera simple y clara.

**¿Cómo funcionan las tareas dentro de una orden de trabajo?**

Al crear una orden, las tareas se cargan cuando se selecciona un servicio que las requiera; estas tareas se listan de forma consecutiva según el orden que se haya configurado desde el servicio.

![]({{ site.baseurl }}/assets/images/image209.png)

_Visualización de nueva tarea_

La pestaña **Tareas** cuenta con las siguientes características:

*   Puede agregar nuevas tareas dentro de una orden haciendo clic en el botón **Nueva Tarea**.
*   A las tareas nuevas se les puede parametrizar los siguientes campos:
    *   **Nombre de la tarea:** ingrese un nombre que indique de qué se trata la tarea. Ej: Instalación de dispositivo.
    *   **Responsable:** seleccione el especialista en campo que se encargará de ejecutar la tarea. El especialista depende del proveedor.
    *   **Fecha y hora estimada de atención:** ingrese una fecha y hora aproximada pero no obligatoria para el especialista en campo.
*   Las tareas pueden pasar por 3 estados: **SIN INICIAR**, **EN MARCHA** y **TERMINADA**. Un control tipo switch permitirá hacer el cambio de estado desde la consola web.
*   Cuando una orden de trabajo **no tiene proveedor**, pero sí tiene un servicio con tareas, estas se pueden reorganizar, desasociar o cambiar de nombre, sin embargo, no es posible asignar responsables o establecer fechas y horas.

Las tareas que ya vienen del servicio, y las recién creadas, pueden editarse dependiendo del estado en el que se encuentren, así:

Cuando está **SIN INICIAR**

*   Permite asignar un responsable y la fecha y hora estimada de atención.
*   Permite cambiar el estado, si es la tarea actual.
*   Permite moverla para cambiar el orden, solo si la anterior esta **SIN INICIAR.**
*   Permite desasociarla de la orden de trabajo, si está en estado **SIN INICIAR.**


![]({{ site.baseurl }}/assets/images/image210.png)


_Visualización de tarea SIN INICIAR._

Cuando está **EN MARCHA**

*   Solo permite cambiar el estado a **TERMINADA**.


![]({{ site.baseurl }}/assets/images/image211.png)

_Visualización de tarea EN MARCHA_

Cuando está **TERMINADA**

*   No permite hacer ajustes.


![]({{ site.baseurl }}/assets/images/image212.png)

_Visualización de tarea TERMINADA_

| **NOTA**: Los ajustes realizados sobre esta lista de tareas (Agregar, reorganizar o desasociar), no afectan las tareas configuradas originalmente en el servicio. |
| --- |

### **Asignación de productos a la orden de trabajo (Inventario)** {#asignaci-n-de-productos-a-la-orden-de-trabajo-inventario}

El inventario o los productos necesarios para la ejecución del servicio, se cargarán de forma automática con los recursos básicos configurados por el administrador para ese servicio. El despachador puede modificar la cantidad de repuestos asociados a la orden según las necesidades del servicio.

![]({{ site.baseurl }}/assets/images/image213.png)
_Pantalla de asociación de repuestos para la orden_

### **Costos de la orden de trabajo** {#costos-de-la-orden-de-trabajo}

El sistema calculaautomáticamente el costo total de operación de un servicio sumando los siguientes costos:

*   **Costo base del servicio:** es el costoconfigurado por el administrador al momento de la creación del servicio.
*   **Costo del inventario:** es el costo de los repuestos o productos configurados por el administrador para el servicio.
*   **Costo del transporte:** no tendrá un valor registrado hasta que el especialista en campo termine las actividades y cierre la orden de trabajo. El costo del transporte corresponde al valor configurado por kilómetro según el medio de transporte, multiplicado por la cantidad de kilómetros recorridos.
*   **Costo del especialista:** se actualizará cuando el responsable atienda la orden de trabajo. El costo del especialista por hora lo configura el administrador y este valor se multiplica por el número de horas registradas por el especialista en la atención de la orden asignada.

![]({{ site.baseurl }}/assets/images/image214.png)

_Costos generados por la orden de trabajo._

### **Notas y comentarios en la orden de trabajo** {#notas-y-comentarios-en-la-orden-de-trabajo}

En la pestaña **Comentarios** quedan registradas las notas, los comentarios y los cambios que realizan el despachador, el monitor o el especialista durante la creación o edición de una orden de trabajo, así como los mensajes que el usuario final ingresa como notas públicas desde la aplicación AssistMe, las cuales también serán visibles para el especialista en campo asignado.

Tanto el despachador, como el especialista podrán agregar información relevante para la atención de la orden, como cambios a la solicitud de registro, confirmación de inventario, seguimiento al especialista en campo, recomendaciones y sugerencias.


![]({{ site.baseurl }}/assets/images/image215.png)

_Pantalla de visualización de comentarios, cambios y notas_

### **Notas Públicas y Privadas** {#notas-p-blicas-y-privadas}

Las notas públicas o privadas se ingresan en el campo para notas que aparece en el listado de órdenes de trabajo o en las pantallas de Edición/Creación desde la consola web (despachador o monitor) o desde la aplicación móvil (especialista en campo).

Por defecto, el campo de notas tiene activa la opción **PRIVADA** (icono de candado), es decir que solo será visible para los especialistas.

![]({{ site.baseurl }}/assets/images/image216.png)

_Campo de nota PRIVADA_

Si desea enviar una nota pública, (visible para todos los usuarios incluidos los de la consola AssistMe), haga clic en el botón tipo switch para cambiarla a **PÚBLICA** (icono de globo terráqueo).

![]({{ site.baseurl }}/assets/images/image216.png)

_Campo de nota PÚBLICA_

| **Nota:** cuando un despachador, monitor o especialista crea una nota pública, esta se envía por correo electrónico al usuario final y también queda visible en la consola AssistMe. |
| --- |

**Cambios**

Los cambios a la orden de trabajo los puede realizar el despachador, el monitor o el especialista y se registran de la siguiente manera:

![]({{ site.baseurl }}/assets/images/image217.png)
_Pantalla de visualización de cambios_

### **Cronómetros en la orden de trabajo** {#cron-metros-en-la-orden-de-trabajo}

Los cronómetros de los acuerdos asociados a una orden de trabajo permiten visualizar el avance y cumplimiento de cada etapa del servicio, ya sean acuerdos con los clientes o con el proveedor:

![]({{ site.baseurl }}/assets/images/image218.png)

_Pantalla de acuerdos con el cliente_


![]({{ site.baseurl }}/assets/images/image219.png)
_Pantalla de acuerdos con el proveedor_

### **Alertas generadas para la orden de trabajo** {#alertas-generadas-para-la-orden-de-trabajo}

Si el sistema encuentra alguna incompatibilidad en la asignación automática de una orden de trabajo, se generarán las alertas o notificaciones correspondientes en la consola de despacho. Las posibles razones que activan estas alertas, son:

*   Incumplimiento en los tiempos o acuerdos de servicio establecidos ANS, OLA y UC.
*   Problemas con el inventario de la orden.
*   Falta de coincidencias entre las fechas de atención, las fechas de solución programadas en la orden y los tiempos disponibles de los especialistas en campo.

El despachador, debe analizar y valorar las alertas registradas y determinar si continúa con el proceso de generación de la orden o no.

![]({{ site.baseurl }}/assets/images/image220.png)

_Pantalla de visualización de Alertas generadas para la orden_

Esta pantalla también reporta el estado de la encuesta de satisfacción del cliente. Cuando aparezca en estado **RESPONDIDA**, podrá visualizar los resultados haciendo clic en el botón **Ver Resultados**.
![]({{ site.baseurl }}/assets/images/image221.png)

_Botón de consulta de resultados de la encuesta_

![]({{ site.baseurl }}/assets/images/image222.png)
_Pantalla de resultados de la encuesta_

### **Campos adicionales de la orden de trabajo** {#campos-adicionales-de-la-orden-de-trabajo}

En esta pestaña puede visualizar los campos adicionales generales para todas las órdenes y los configurados para un servicio específico. Esta información se presenta así:

![]({{ site.baseurl }}/assets/images/image223.png)

_Visualización de los campos adicionales generales y por servicio._

### **Campos adicionales generales de orden de trabajo:** {#campos-adicionales-generales-de-orden-de-trabajo}

Estos campos adicionales generales aplican a todas las órdenes de trabajo que se creen en AFLS y se configuran en la pantalla **Configuración &gt; Campos adicionales &gt; Órdenes de trabajo**.

### **Campos adicionales de orden de trabajo dado el servicio** {#campos-adicionales-de-orden-de-trabajo-dado-el-servicio}

Pueden ser diligenciados o visualizados por el monitor o especialista dependiendo de los permisos configurados en los campos adicionales del modelo y del estado en el que esté la orden de trabajo.

### **Firma de la orden de trabajo** {#firma-de-la-orden-de-trabajo}

Esta pestaña permite comparar la firma registrada del cliente (desde la configuración) con la firma que haga el cliente al momento de tomar el servicio (desde la móvil):


![]({{ site.baseurl }}/assets/images/image224.png)

_Pantalla de visualización de firmas para la orden_

### **Información del cliente** {#informaci-n-del-cliente}

Puede crear o editar la información de un cliente desde la pantalla de creación de la orden de trabajo:

![]({{ site.baseurl }}/assets/images/image225.png)

_Opciones para creación de nuevo cliente desde la orden_

Se solicitan los mismos datos básicos que desde la configuración de clientes:

![]({{ site.baseurl }}/assets/images/image226.png)

_Pantalla de nuevo cliente desde la orden_

También puede editar la información del cliente desde el módulo de creación de la orden de trabajo:

![]({{ site.baseurl }}/assets/images/image227.png)

_Pantalla editar cliente desde la orden_

Si se consulta una orden ya creada, la información del cliente se visualizará de la siguiente manera:

![]({{ site.baseurl }}/assets/images/image228.png)

_Pantalla de información de cliente_

### **Relaciones de órdenes de trabajo** {#relaciones-de-rdenes-de-trabajo}

En la pestaña **Relaciones** podrá vincular 2 o más órdenes de trabajo. Para crear una relación, haga clic en el botón **Nueva relación**:

![]({{ site.baseurl }}/assets/images/image229.png)

Aparecerá la siguiente pantalla donde deberá seleccionar si la relación será de sucesión o de vínculo:


![]({{ site.baseurl }}/assets/images/image230.png)


*   **Sucesión:** significa que es necesario atender otra orden de trabajo antes de atender la orden sobre la cual se está realizando la relación.
*   **Vínculo:** significa que las órdenes están relacionadas, sin importar el orden en el que se atiendan.

Luego busque la orden sobre la cual va a generar la relación:

![]({{ site.baseurl }}/assets/images/image231.png)

Una vez creada, la relación se visualiza de la siguiente manera:

[]({{ site.baseurl }}/assets/images/image232.png)
