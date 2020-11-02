---
title: Clientes
chapter: "ingresando"
---

En la sección de clientes los especialistas en campo podrán actualizar la información básica de los clientes (correo electrónico, teléfono, dirección)

[]({{ site.baseurl }}/assets/images/image344.png)
_Actualización de cliente_

| **Nota**: El nombre y código único del cliente solo se pueden actualizar desde la Consola Web. |
| --- |

Al hacer clic en el botón **VER INVENTARIO**, **e**l especialista podrá visualizar qué inventario tipo único tiene el cliente:

![]({{ site.baseurl }}/assets/images/image345.png)
_Inventario tipo único del cliente_

Al seleccionar un producto de la lista, aparecerá el botón **RECOGER**; el especialista usará este botón cuando haya recogido ese producto y así indicar que ahora queda a su cargo.

![]({{ site.baseurl }}/assets/images/image346.png)

| **Nota**: Esta funcionalidad solo está disponible en línea. |
| --- |

### **Filtrando y ordenando las órdenes asignadas** {#filtrando-y-ordenando-las-rdenes-asignadas}

En la esquina superior derecha de la consola móvil se encuentra el menú para desplegar los filtros por estado y los criterios para ordenar las órdenes de trabajo asignadas al especialista en campo:

![]({{ site.baseurl }}/assets/images/image347.png)

_Filtros y criterios para ordenar_

### **Detalles de la orden de trabajo** {#detalles-de-la-orden-de-trabajo}

Al tocar cualquiera de las órdenes de la lista, podrá visualizar los detalles de esa orden de trabajo.

![]({{ site.baseurl }}/assets/images/image348.png)

| _Detalle de orden con servicio tipo Estándar_

![]({{ site.baseurl }}/assets/images/image349.png)

| _Detalle de orden con servicio tipo Desplazamiento_ |
| --- | --- |

En la pantalla de detalles el especialista en campo podrá actualizar el estado de la orden a medida que vaya adelantando las etapas previamente configuradas del servicio.

En el caso de una orden con servicio tipo Desplazamiento, el especialista podrá además utilizar la opción **VER RUTA** para visualizar el recorrido propuesto a través de la aplicación de mapas que el dispositivo tenga configurada por defecto.

### **Cambio de estados** {#cambio-de-estados}

El cambio de estados permite reportar los tiempos de atención, las pausas en el servicio y el cierre de la orden.

En el menú de la parte superior derecha de la pantalla de detalles aparecerán todas las transiciones de estado disponibles (de las configuradas previamente en el modelo de flujo de trabajo) y la transición principal estará identificada con una estrella.

![]({{ site.baseurl }}/assets/images/image350.png)
![]({{ site.baseurl }}/assets/images/image351.png)

_Menú de transiciones de estado_

En el modelo principal que viene en AFLS están configuradas las siguientes transiciones de estado:

*   **Iniciar desplazamiento:** reporta el momento en el que el especialista inicia el recorrido hacia la ubicación de la orden de trabajo.
*   **Iniciar trabajo:** reporta el momento en el que el especialista inicia las actividades específicas del servicio.
*   **Escalar:** informa cuando el especialista en campo no puede atender la orden de trabajo por alguna razón (problema de inventario, problemas con el cliente, etc..). Se escala al despachador de AFLS.
*   **Pausar:** reporta cuando el especialista hace una pausa en las actividades. La información del tiempo de ejecución de la orden no se registra hasta que se reinicie la actividad (esto depende de las configuraciones del modelo, cronómetros, etc.)
*   **Finalizar:** reporta cuando el especialista finaliza el servicio.

Al seleccionar la transición con la que se cambiará el estado de la orden, se solicitará elegir una razón (de las configuradas previamente en el flujo de trabajo del modelo):

![]({{ site.baseurl }}/assets/images/image352.png)

_Visualización de razones_

| **Nota**: todos los cambios serán visibles por el monitor para que pueda hacer el seguimiento y las modificaciones que sean necesarias. |
| --- |

### **Acciones** {#acciones}

Dependiendo de la etapa en la que se encuentre el servicio, en la consola móvil se habilitarán las siguientes acciones para que el especialista las ejecute según el caso:

*   **Contactar al cliente**

Permite al especialista ponerse en contacto con el cliente para reportar alguna novedad o confirmar un dato. El contacto se hace a través de las instancias de teléfono de contacto y correo electrónico que aparecen en el detalle de la orden en la sección **INFORMACIÓN DEL SOLICITANTE**:

![]({{ site.baseurl }}/assets/images/image353.png)

*   **Tareas**

Una orden de trabajo puede tener una o varias tareas asociadas y estas pueden tener diferentes especialistas a cargo. Es decir, que en una orden de trabajo puede haber un especialista principal y otros especialistas colaboradores. Solo el especialista principal puede avanzar en el flujo de trabajo una vez las tareas de la orden estén terminadas. Un especialista principal puede ser responsable de una o varias tareas de su propia orden, y también ser colaborador de tareas de otras órdenes.

Para gestionar las tareas de una orden de trabajo, ingrese al detalle de una orden y toque la sección de **Tareas**:

![]({{ site.baseurl }}/assets/images/image354.png)

Allí visualizará la lista de tareas y sus estados representados con iconos, así:

*   *   : la tarea ha sido terminada
    *   : la tarea está “bloqueada” sin iniciar
    *   : la tarea estáen marcha
    *   : identifica las tareas a cargo del especialista actual.
    *   Cuando la tarea está en negrilla y sin icono, indica que la tarea actual está “desbloqueada” y sin iniciar


![]({{ site.baseurl }}/assets/images/image359.png)

_Visualización de tareas_

Puede acceder a cada una de las tareas y las visualizará según el estado de la siguiente manera:

Cuando está **SIN INICIAR** y no le corresponde al especialista actual, entonces no requiere acciones:

![]({{ site.baseurl }}/assets/images/image360.png)

Cuando está **SIN INICIAR**, le corresponde al especialista actual, pero está bloqueada, entonces n**o** permite acciones:

![]({{ site.baseurl }}/assets/images/image361.png)

Cuando está **SIN INICIAR**, le corresponde al especialista actual y no está bloqueada, entonces permite iniciar tarea:

![]({{ site.baseurl }}/assets/images/image362.png)

Cuando está **EN MARCHA** y no le corresponde al especialista actual, entonces no requiere acciones:

![]({{ site.baseurl }}/assets/images/image363.png)

Cuando está **EN MARCHA** y le corresponde al especialista actual, entonces permite terminar la tarea:

![]({{ site.baseurl }}/assets/images/image364.png)

Cuando está **TERMINADA**, sin importar a quien le corresponda, no requiere acciones:

![]({{ site.baseurl }}/assets/images/image365.png)

*   **Agregar tiempo**

Durante la atención de la orden, el especialista asignado puede solicitar tiempo adicional para terminar una tarea pendiente en caso de eventualidades tales como actividades no programadas, inconvenientes en el proceso, o defectos en alguno de los repuestos.

Para solicitar tiempo adicional el especialista debe tocar el icono flotante y seleccionar la opción **Agregar Tiempo**.Se habilitarán cuatro opciones: Adicionar 15 minutos, 30 minutos, 45 minutos o 60 minutos.

![]({{ site.baseurl }}/assets/images/image366.png)
![]({{ site.baseurl }}/assets/images/image367.png)
![]({{ site.baseurl }}/assets/images/image368.png)

| **Nota**: las solicitudes de tiempo adicional generan una notificación que será visible por el monitor, quien será el encargado de aprobar o rechazar el tiempo solicitado por el especialista. |
| --- |

*   **Inventario**

El especialista asignado a una orden puede consultar el inventario de repuestos configurados para la atención del servicio y confirmar si está disponible o no.

![]({{ site.baseurl }}/assets/images/image369.png)

_Visualización del inventario requerido_

![]({{ site.baseurl }}/assets/images/image370.png)

_Disponibilidad del inventario requerido_

*   **Actualización de CI**

Cuando AFLS se integra con la herramienta ASDK (Aranda Service Desk), las órdenes de trabajo se asocian a un activo o CI (elemento de configuración). Para consultar y actualizar el CI de una orden de trabajo, se establece una conexión directa con la CMDB (base de datos de la gestión de configuración). AFLS provee una opción en la consola móvil que permite realizar dicha gestión, aunque no interactúa directamente con todos los datos del CI, ya que AFLS solo guarda las ID de los CI.

Para esto se deben configurar las rutas de ASDK y API de CMDB en el archivo Web.config que se encuentra en la carpeta de archivos de aplicación de AFLS. Una vez hecha la configuración, el ítem de actualización de CI se habilita en la consola móvil. Los parámetros de configuración son:

*   ASDKUpdateCIStateURL: este parámetro es la URL de visualización del CI, esta URL es de la herramienta CMDB de Aranda.
*   CMDBAPI: este parámetro es la URL del API de CMDB para iniciar sesión y así obtener permiso de visualización y edición.
*   USERCMDBAPI: este parámetro es el nombre de usuario de la CMDB para iniciar sesión.
*   PASSWORDCMDBAPI: este parámetro es la contraseña de usuario de la CMDB para iniciar sesión.

| **Nota:** el usuario que se use en esta configuración debe tener permisos de lectura y edición del CI (permisos otorgados en la CMDB). |
| --- |

![]({{ site.baseurl }}/assets/images/image371.png)
![]({{ site.baseurl }}/assets/images/image372.png)

_Visualización la opción de consulta del CI (inactivo y activo)_

![]({{ site.baseurl }}/assets/images/image373.png)

_Página de información del CI_

*   **Notas**

Esta acción permite ingresar comentarios relacionados con la asignación o atención de la orden de trabajo, y también consultar comentarios anteriores realizados por el despachador, el monitor o el usuario final.

*   Las notas de un especialista en campo están identificadas con el icono .
*   Las notas de un despachador o monitor están identificadas con el icono .
*   Las notas de un usuario final están identificadas con el icono .


![]({{ site.baseurl }}/assets/images/image377.png)

_Visualización de listado de notas_

Las notas son útiles para agregar información relevante para la atención de la orden, como cambios a la solicitud de registro, confirmación de repuestos, seguimiento al especialista en campo, recomendaciones y sugerencias, entre otros mensajes.

Las notas escritas por el especialista en campo quedarán registradas en la instancia de comentarios de la consola móvil y serán visibles en la consola de despachador_._

Para agregar una nueva nota, ingrese a la opción **Notas** ytoque el icono flotante . En la siguiente pantalla encontrará el espacio necesario para escribir la nota, y la opción para marcar la nota como pública (si no se activa la opción de nota pública, se entenderá que la nota es privada).

![]({{ site.baseurl }}/assets/images/image378.png)

_Creación de una nueva nota_

| **Nota:** si se crea una nota pública, ya sea de un despachador, monitor o especialista, se envía un correo electrónico al usuario final, y este podrá visualizarla desde la consola de AssistMe. |
| --- |

*   **Adjuntar**

Esta acción permite adjuntar los archivos requeridos durante la atención de la orden de trabajo como fotografías, videos o audios de evidencia de la evolución del servicio.

Para adjuntar un archivo, ingrese a la opción **Adjuntos** y toque el icono flotante .

![]({{ site.baseurl }}/assets/images/image379.png)
![]({{ site.baseurl }}/assets/images/image380.png)

Los tipos de archivos que puede agregar a la orden pueden ser de formatos con contenido de texto, imágenes, fotografía, videos o audio como: .png, .jpeg, .mp4, .mp3,.doc, .xls, .ppt, .PDF, archivos que tengan un tamaño máximo de 10MB (a excepción de los .exe)

*   **Campos adicionales**

Esta acción permite visualizar y diligenciar los campos adicionales que se encuentren activos para el modelo y para las órdenes de trabajo. Allí podrá recoger la información adicional que se requiera para el proceso.

![]({{ site.baseurl }}/assets/images/image381.png)
![]({{ site.baseurl }}/assets/images/image382.png)

Según la configuración en el modelo, los campos adicionales pueden ser de los siguientes tipos:

![]({{ site.baseurl }}/assets/images/image383.png)
| **Campo tipo texto**
![]({{ site.baseurl }}/assets/images/image384.png)
| **Campo tipo párrafo**
![]({{ site.baseurl }}/assets/images/image385.png)
| **Campo tipo numérico**
![]({{ site.baseurl }}/assets/images/image386.png)
| **Campo tipo fecha** |
![]({{ site.baseurl }}/assets/images/image387.png)
| **Campo tipo listado**

*   **Relaciones**

Esta acción permite visualizar las órdenes con las que se estableció una relación ya sea de sucesión o de vínculo.

*   **Sucesión**: significa que es necesario ejecutar una orden de trabajo antes de ejecutar otra. Por ejemplo, se puede definir una orden de ejecución y una orden de monitoreo. La orden de monitoreo (una persona visitando en campo el trabajo del especialista) solo se podrá hacer después de que se ejecute la primera.
*   **Vínculo:** significa que las órdenes están relacionadas, sin importar el orden en el que se atiendan. Se establece la relación principalmente para tener trazabilidad. Por ejemplo, un especialista realiza una visita de control y reporta que se debe hacer un mantenimiento. La orden de mantenimiento se relaciona por vínculo a la de control.

![]({{ site.baseurl }}/assets/images/image388.png)

_Relación por vínculo_

*   **Firmas**

Esta acción permite que el cliente firme la orden luego de que esta haya sido atendida.

![]({{ site.baseurl }}/assets/images/image389.png)

Dicha firma se compara con la que se ha configurado previamente para ese cliente en AFLS, y de esta manera es posible corroborar la satisfacción del cliente y también auditar y controlar la atención de los servicios. La firma no es obligatoria.

*   **Encuesta**

Esta acción permite que, al final del trámite de la orden, el cliente conteste la encuesta de satisfacción, en caso de que el modelo la tenga configurada.

![]({{ site.baseurl }}/assets/images/image390.png)
![]({{ site.baseurl }}/assets/images/image391.png)

| **Nota**: luego de contestar la encuesta, se enviará un correo al cliente con las respuestas que este haya suministrado. |
| --- |
