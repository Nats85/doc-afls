---
title: Configuración de los proveedores
chapter: "configurando"
---

Los proveedores son las entidades que suministran especialistas en campo para que atiendan las órdenes de trabajo según las zonas y servicios específicos a los que se dediquen. Es posible personalizar su funcionamiento de acuerdo con las opciones de configuración.

**Información básica del proveedor**

En el módulo de **Proveedores**, encontrará la lista de tarjetas de los proveedores existentes. Cada tarjeta muestra la siguiente información básica:

*   Nombre del proveedor
*   Descripción
*   Tipo de proveedor (interno o externo)
*   Número de especialistas asociados al proveedor
*   Estado actual del proveedor (Activo, Inactivo)


![]({{ site.baseurl }}/assets/images/image79.png)


Al seleccionar un proveedor del listado, la información asociada a este se presentará al lado derecho de la pantalla en 5 pestañas:

![]({{ site.baseurl }}/assets/images/image80.png)

### **Asignación de especialistas por proveedor** {#asignaci-n-de-especialistas-por-proveedor}

Para asignar especialistas de un proveedor se pueden escoger dos opciones:

*   **Asignar especialistas manualmente:** significa que, cuando hay una orden asignada al proveedor, la asignación específica del especialista no la realiza el motor de asignación automáticamente, sino que un usuario con privilegios de edición de órdenes (despachador o monitor) escoge manualmente el especialista que va a atender la orden.
*   **Asignar al mejor especialista:** la asignación de especialistas se realiza de manera automática, escogiendo al especialista que, según su disponibilidad y habilidades, sea la mejor opción. Esta opción es la seleccionada por defecto cuando se crean proveedores nuevos.

**Selección del tipo de proveedor**

La selección del tipo de proveedor define los tipos de acuerdo que se aplican a la prestación de servicios, estos son:

*   **OLA** (Operational Level Agreement) para proveedores internos. Son acuerdos negociados internamente dentro de la compañía, que identifican los niveles de servicio que se esperan (p.e.: tiempos de respuesta y solución.)
*   **UC** (Underpinning Contract) para proveedores externos. Son las obligaciones de los proveedores externos que prestan servicios a la compañía y están documentados a través de contratos.

### **Importancia del proveedor** {#importancia-del-proveedor}

El nivel de importancia de un proveedor se refiere a la preferencia o prioridad que se le da sobre otros proveedores para que pueda tomar las órdenes de servicio que se asignan por **Distribución Pública.** De esta manera, un proveedor con importancia **Alta** puede ver una orden en la sección “**Órdenes Disponibles**” antes que los proveedores de importancia **Media** o **Baja**.

| **NOTA:** Por defecto, un proveedor de importancia **Alta** puede ver la orden 10 minutosantes que los de importancia **Media** y 20 minutos antes que los demás. Ese tiempo se puede ajustar en la configuración de base de datos: **DeltaMinByProviderPriority** |
| --- |

### **Servicios asociados a un proveedor** {#servicios-asociados-a-un-proveedor}

Un proveedor podrá asociarse con servicios ya configurados dentro de AFLS. De esta manera ese proveedor aparecerá disponible para atender el o los servicios que se le hayan asociado.

![]({{ site.baseurl }}/assets/images/image81.png)

#### Barra de búsqueda de servicios {#barra-de-b-squeda-de-servicios}

En esta barra podrá buscar y seleccionar los servicios existentes que se hayan configurado anteriormente con algún OLA o UC en la pantalla de configuración de “Catálogo de servicios/Servicios/Pestaña General de servicio” (la selección de estos acuerdos no es obligatoria).

![]({{ site.baseurl }}/assets/images/image82.png)

### **Zonas asociadas al proveedor** {#zonas-asociadas-al-proveedor}

Las zonas asociadas serán las zonas en las cuales el proveedor estará en capacidad de atender órdenes.

![]({{ site.baseurl }}/assets/images/image83.png)

#### Barra de búsqueda de zonas {#barra-de-b-squeda-de-zonas}

En esta barra podrá buscar y seleccionar las zonas ya existentes en la configuración de AFLS, una vez seleccionado un ítem, este será agregado a la sección del listado, si no ha sido agregada previamente.

### **Especialistas asociados al proveedor** {#especialistas-asociados-al-proveedor}

Esta opción es solo de consulta, es decir, solo se podrán visualizar los especialistas que han sido asociados al proveedor en edición desde la pantalla de creación de Usuarios Móviles (Especialistas).

Se mostrará también, información sobre el estado del especialista, informando entre paréntesis cuando esté inactivo y/o cuando se encuentre sin licencia.

![]({{ site.baseurl }}/assets/images/image84.png)

### **Monitores asociados al proveedor** {#monitores-asociados-al-proveedor}

Puede asociar usuarios web con el rol “Monitor” a un proveedor específico para que tengan acceso a los reportes, órdenes, configuración de especialistas y grupos móvil, así como al monitoreo de Especialistas, Clientes y Planeación, que se relacionen con dicho proveedor.

Los monitores, a su vez, tendrán la opción de realizar filtros por proveedor en las pantallas mencionadas anteriormente.

![]({{ site.baseurl }}/assets/images/image85.png)

#### Barra de búsqueda de monitores {#barra-de-b-squeda-de-monitores}

En esta barra podrá buscar y seleccionar usuarios web que tengan el rol “Monitor”.
