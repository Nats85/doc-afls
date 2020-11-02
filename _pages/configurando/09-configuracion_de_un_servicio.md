---
title: Configuración de un servicio
chapter: "configurando"
---

El eje central del negocio debe ser el servicio principal que se ofrece a los clientes. Para crear cada uno de los servicios haga clic en el botón **Nuevo** de la categoría Servicios

![]({{ site.baseurl }}/assets/images/image49.png)

**Información del Servicio**

Para crear un servicio es necesario ingresar la siguiente información:

*   El nombre del servicio configurado en Aranda FIELD SERVICE y la descripción
*   El servicio debe tener un modelo asociado
*   El servicio debe tener un Asunto.
*   El servicio debe tener un Calendario, ANS, OLA y UC asociados.
*   El servicio debe tener un costo base que debe definirse como **Costo Base.**
*   Costo inventario: Este valor se define de acuerdo al inventario asociado al servicio.
*   El tipo de servicio que puede ser **Estándar** o **Desplazamiento**
*   El servicio puede otorgarse por **Asignación Directa** o por **Distribución Pública** en la opción de **Publicación de órdenes a proveedores.**
*   Tiempo de duración del servicio: Es el tiempo en horas y minutos que va a tomar la ejecución de este.

El servicio puede ser configurable para:

*   **Brindar este servicio a todos los clientes:** Permite que el servicio esté habilitado para todos los clientes.
*   **Habilitar órdenes de emergencia para el servicio:** Permite crear órdenes de trabajo con el servicio en modo **emergencia** y **prioridad** (no disponible para configuración de Distribución Pública).

Los **tipos de servicio** corresponden a:

*   **Estándar:** Indica que se va a prestar el servicio a los clientes en un punto específico que corresponde a la ubicación del cliente.
*   **Desplazamiento:** Indica la atención en campo a los clientes de un punto (A) a un punto (B), por ejemplo: conductor elegido.

La **Publicación de órdenes a proveedores** determina lo siguiente:

*   **Asignación Directa:** Se realiza asignación de órdenes a un proveedor específico, de acuerdo a las reglas de asignación a proveedores que se hayan configurado.
*   **Distribución Pública:** Se refiere a las órdenes que tienen un servicio con la distribución pública habilitada, y que quedarán en un listado de **“Disponibles”** hasta que cualquier proveedor decida tomarlas.

| **Nota**: El costo de inventario configurado para el servicio se calcula automáticamente de acuerdo a los repuestos incluidos en el servicio (Pestaña Inventario). |
| --- |

*** Nuevo versión AFLS 9.9***

Cuando desde la configuración de Ajustes Globales se habilite la opción de Creación de orden al especialista, se mostrará un botón para Activar o Inactivar la visualización del servicio para los especialistas.

![]({{ site.baseurl }}/assets/images/image50.png)

| **Nota**: Para que el especialista pueda visualizar el servicio en la creación de la orden es necesario que el servicio se habilite. |
| --- |

### **Inventario** {#inventario}

La cantidad de repuestos asociados al servicio serán los repuestos básicos necesarios para atenderlo, sin embargo, esta información puede variar y ser personalizada de acuerdo a los requerimientos definidos por el cliente en cada una de las órdenes de trabajo.

![]({{ site.baseurl }}/assets/images/image51.png)

### **Habilidades** {#habilidades}

Las habilidades requeridas para la ejecución de una orden deben crearse en la pestaña **Habilidades** para luego asociarlas al respectivo servicio.

![]({{ site.baseurl }}/assets/images/image52.png)

Cuando una habilidad es requerida quiere decir que la persona que va a atender el servicio debe poseer dicha habilidad.

### **Tareas** {#tareas}

Una orden de trabajo se relaciona con un servicio, y el servicio puede requerir la ejecución de una serie de tareas. Esta sección permite de manera opcional, crear una lista de plantillas de tareas consecutivas para la orden de trabajo que esté relacionada con ese servicio.

**¿Cómo crear una plantilla de tareas?**

Para crear una plantilla de tareas diríjase a **Configuración &gt; Catálogo de Servicios &gt; Servicios**, y en la pestaña **Tareas** ingrese el nombre de la tarea en el campo de texto disponible y luego haga clic en **Agregar**.

![]({{ site.baseurl }}/assets/images/image53.png)

Una vez tenga el listado completo, usted puede cambiar el orden, arrastrando con el mouse la tarea que desee cambiar hasta la nueva posición; también puede **eliminar** las tareas que desee excluir.

| **Nota:** esta plantilla de tareas se verá reflejada en la creación de una orden de trabajo que tenga el servicio. Al momento de guardar la orden de trabajo con la plantilla de tareas, esas tareas se convierten en tareas para realizar. |
| --- |

### **Proveedores** {#proveedores}

En la pestaña **Proveedores** podrá configurar los proveedores que van a prestar el servicio con el respectivo acuerdo dependiendo del tipo de proveedor que se asocie al servicio.

![]({{ site.baseurl }}/assets/images/image54.png)

### **Campos adicionales** {#campos-adicionales}

En esta pestaña podrá diligenciar los campos adicionales que se hayan configurado en el módulo de configuración de campos adicionales para servicios.


![]({{ site.baseurl }}/assets/images/image55.png)


### **Configuración de Órdenes de Emergencia** {#configuraci-n-de-rdenes-de-emergencia}

El administrador de la herramienta puede activar la opción de “Habilitar el servicio para órdenes de emergencia o prioritarias”.

![]({{ site.baseurl }}/assets/images/image56.png)

De esta manera, una orden puede tener tres tipos de prioridad:

*   **Normal:** corresponde a las órdenes de trabajo que deben atenderse según la prioridad que define el motor de asignación. El motor de asignación optimiza la planeación de los especialistas evitando así que se incumplan los acuerdos con los clientes y minimizando el costo operativo y de desplazamiento de los agentes. Esta es la prioridad seleccionada por defecto.
*   **Prioritaria:** es cuando la orden se debe atender lo antes posible. En este tipo de prioridad, la orden será asignada al especialista más cercano, dándole el tiempo necesario para terminar el trabajo que esté realizando en el momento. El especialista debe finalizar el trabajo actual y luego dirigirse a la orden prioritaria.
*   **Emergencia:** es el mayor nivel de prioridad. El especialista debe dejar el trabajo que esté realizando y dirigirse inmediatamente a solucionar la emergencia. La orden de trabajo que deja se reasignará a otro especialista.

Estas prioridades solo están disponibles cuando el servicio se encuentra habilitado para trabajo prioritario. De lo contrario, una orden sólo podrá estar en prioridad “Normal”.
