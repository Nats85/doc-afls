---
title: Configuración de un cliente
chapter: "configurando"
---

Para adicionar un cliente, haga clic en el botón **Nuevo** de la categoría Clientes y, a la derecha en la pestaña **Cliente**,defina los siguientes campos: Nombre del cliente, código del cliente, número de teléfono, correo electrónico, compañía a la que pertenece, dirección y detalle de la dirección (para especificar otros datos de la dirección como oficina, piso etc.).

![]({{ site.baseurl }}/assets/images/image63.png)

**Servicios asociados a un cliente**

En la pestaña **Servicios** puede asociar y activar cualquiera de los servicios ya configurados anteriormente o el cliente puede tener dichos servicios heredados por la compañía.

![]({{ site.baseurl }}/assets/images/image64.png)

### **Firma del cliente**

En esta pestaña podrá cargar el archivo que contiene la firma del cliente que se utilizará para ser validada con la orden de trabajo cerrada.


![]({{ site.baseurl }}/assets/images/image65.png)


### **Campos Adicionales del cliente**

Corresponden a los campos adicionales que se hayan configurado en el módulo de configuración para clientes y están habilitados para poder ser utilizados al momento de crear el cliente.


![]({{ site.baseurl }}/assets/images/image66.png)


### **Canales del cliente** {#canales-del-cliente}

Se refiere a los canales de comunicación disponibles para el cliente. Por ahora solo se encuentra disponible el canal AssistMe. Para que el cliente pueda acceder al canal, es necesario enviar una invitación con la información de acceso a través de correo electrónico, adicionalmente es necesario que el canal esté activo.

![]({{ site.baseurl }}/assets/images/image67.png)

### **Inventario** {#inventario}

En esta pestaña se visualiza el inventario tipo único con el que cuenta el cliente, este tuvo que ser entregado por algún especialista al momento de tramitar una orden de trabajo del cliente.

![]({{ site.baseurl }}/assets/images/image68.png)

### **Importación masiva de clientes** {#importaci-n-masiva-de-clientes}

La opción de importación de clientes desde archivo está en el menú desplegable al lado del botón **Nuevo**. Esta funcionalidad le permitirá importar clientes masivamente a AFLS, por medio de un archivo **.csv** de excel, con un formato específico con el fin de gestionar y crear sus órdenes de trabajo con la información de sus clientes de manera mucho más rápida.

![]({{ site.baseurl }}/assets/images/image69.png)

El archivo de Excel debe ser **.csv** (valores separados por comas) y guardado con codificación UTF-8.

El enlace permite descargar la plantilla del modelo para importación que contiene los siguientes campos y un ejemplo.

![]({{ site.baseurl }}/assets/images/image70.png)

**Estructura del archivo de clientes a importar**:

Campos Client_Template.csv

*   Name: Nombre del cliente
*   Email: Correo del cliente
*   Telephone: Teléfono asociado al cliente
*   CompanyId: Compañía a la que se asocia el cliente
*   Latitude-Longitude: latitud y longitud del cliente, debe estar separada por **“,”** Ejemplo 40.741895,-73.989308
*   Address: Dirección del cliente
*   AddressDetail: Detalle de la dirección, como Apartamento, casa, etc
*   State: Estado, (Activo 1 /Inactivo 0)
*   UniqueReference: Código único del cliente (Cédula o NIT)

| **Nota**: Al momento de realizar la importación de clientes por archivo .csv es necesario que en la dirección se especifique la Ciudad seguido de “,” y el país. Ejemplo Cra. 71a #75b-24, Bogotá, Colombia. Tener en cuenta que con los nuevos proveedores de mapas hay que ser más específicos en las direcciones, incluir barrio y/o localidad. |
| --- |

Al oprimir el botón de importación de clientes, se despliega el formulario para cargar el archivo de clientes a importar. Oprima el botón **Buscar** para que se despliegue la ventana del explorador de Windows y seleccione el archivo **.csv**.


![]({{ site.baseurl }}/assets/images/image71.png)


Una vez cargado el archivo correctamente configurado haga clic en el botón **Importar**, así el sistema procesará el archivo.


![]({{ site.baseurl }}/assets/images/image72.png)


Al terminar, se presentará una ventana de confirmación indicando el número de clientes que se importaron.

| **Nota**: Al momento de realizar la importación, si se ingresa la dirección del cliente, se visualizará en el mapa el pin de dicha dirección. |
| --- |


![]({{ site.baseurl }}/assets/images/image73.png)


Si el archivo de clientes a importar contiene uno o más registros configurados de manera errónea, en la ventana de finalización del proceso de carga se presentará la cantidad de registros no importados al sistema y un nuevo botón de descarga.

![]({{ site.baseurl }}/assets/images/image74.png)


El sistema generará un archivo CSV con un nombre propio y con los registros que no se importaron a la aplicación. Al oprimir el botón de descarga, una ventana del explorador de Windows se mostrará para que el usuario seleccione la ubicación en la que desea guardar el archivo.

![]({{ site.baseurl }}/assets/images/image75.png)


Al abrir el archivo, se observarán los registros que se procesaron y al final de la línea de aquellos que fallaron, se mostrará la razón por la que falló.


![]({{ site.baseurl }}/assets/images/image76.png)


**Tenga en cuenta:**

*   Al no lograr una importación exitosa de clientes, la aplicación le permitirá descargar el archivo para visualizar la razón de la no importación.
