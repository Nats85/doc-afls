---
title: Importación masiva de órdenes de trabajo
chapter: "gestionando"
---

El despachador puede cargar masivamente órdenes de trabajo desde un archivo **.csv** (valores separados por comas) con codificación UTF-8 que cumpla con la estructura requerida por el sistema (se describe más adelante), para generar órdenes de trabajo en AFLS a partir de aplicaciones de terceros o propias.

Para importar órdenes masivamente, ingrese por **Órdenes**, y haga clic en el ícono **Importar** que seencuentra al lado del botón **Nueva**:

[]({{ site.baseurl }}/assets/images/image247.png)

_Opción de importación masiva de órdenes_

Aparecerá un buscador que le permitirá seleccionar el archivo de las órdenes a importar, y un enlace con el cual podrá descargar una plantilla modelo del archivo para realizar satisfactoriamente la importación de órdenes.

[]({{ site.baseurl }}/assets/images/image248.png)

_Archivo de órdenes a importar seleccionado_

**Estructura requerida para el archivo de órdenes de trabajo a importar:**

Campos Workorder_Template.csv

*   ContactName: nombre de usuario que el cliente de la orden tenga configurado.
*   ServiceID: ID del servicio a asociar a la orden de trabajo.
*   Subject: asunto que tendrá la orden de trabajo.
*   Description: descripción de la orden de trabajo.
*   SpareParts: ID del repuesto que se le asociará a la orden, seguido de la cantidad (separadas por espacio).
*   ContactEmail: correo electrónico del contacto de la orden de trabajo.
*   ContactPhone: teléfono del contacto de la orden de trabajo.
*   Latitude-Longitude: latitud y longitud de la dirección (separadas por coma).
*   Address: dirección de la orden de trabajo.
*   AddAddress: detalle de la dirección.
*   Specialist: nombre del especialista asignado a la orden.
*   UniqueReference: código único del cliente al que se le va crear la orden de trabajo.
*   Los campos obligatorios que se requieren para realizar el proceso son: ContactName, ServiceID, Subject, Description, Address y UniqueReference.
*   Los campos opcionales de este archivo son SpareParts, ContactEmail, ContactPhone, Latitude-Longitude, AddAddress y Specialist.
*   Si el usuario no asocia ningún ID de repuesto (SpareParts), el sistema tomará los repuestos por defecto que tiene el servicio (si los tiene asociados).
*   Si el usuario asocia un ID de repuesto, es necesario indicar la cantidad de repuestos a asociar; se pone primero el ID del repuesto y luego la cantidad. Ejemplo: 1 1 (ID 1 y cantidad 1).
*   Si el usuario configura latitud y longitud, no es necesario configurar el campo Address. Si el usuario configura el campo Address, no es necesario configurar latitud y longitud.

| **Nota**: se deben dejar en blanco los campos no usados. |
| --- |

Una vez seleccionado el archivo correctamente configurado, haga clic en **Importar** y el sistema procesará el archivo. Al terminar el proceso, se presentará un mensaje de confirmación, indicando el número las órdenes de trabajo que se importaron.

[]({{ site.baseurl }}/assets/images/image249.png)

_Mensaje importación de órdenes exitosa_

Cuando una orden se importa correctamente, en la información detallada de esa orden aparecerá un comentario en la pestaña **Comentarios** indicando que es una orden importada.

[]({{ site.baseurl }}/assets/images/image250.png)

_Comentario generado en la orden cuando es importada._

Si el archivo de órdenes a importar contiene uno o más registros configurados de manera errónea, aparecerá un mensaje con la cantidad de registros no importados y la opción de descargar un archivo **.csv** que contiene los registros que no se importaron.

[]({{ site.baseurl }}/assets/images/image251.png)

_Mensaje de importación de órdenes NO exitosa_

Al oprimir el botón **Descargar**, se mostrará una ventana del explorador de Windows para que el usuario seleccione la ubicación en la que desea guardar el archivo.

[]({{ site.baseurl }}/assets/images/image252.png)

_Archivo con las órdenes fallidas_

Al abrir el archivo, se observarán los registros que se procesaron y al final de la línea de aquellos que fallaron, se mostrará la razón por la que fallaron.

[]({{ site.baseurl }}/assets/images/image253.png)

_Mensaje de validación dentro del archivo_

**Tenga en cuenta que:**

*   Por defecto las órdenes se importan en estado Abierta.
*   En el listado de órdenes de trabajo se podrá identificar cuáles han sido importadas.
*   Las órdenes importadas seguirán el consecutivo del listado de órdenes existentes en la aplicación, es decir, si se tiene 98 órdenes creadas hasta la fecha y se importan 10, el consecutivo que tomará la importación será desde el 99 al 109.

| **Nota:** luego de la importación, para que las órdenes sean asignadas automáticamente por el motor de asignación deben contar con un proveedor. La asignación del proveedor la realiza la tarea UNASSIGNER_ORDERS_PROVIDER que por defecto se ejecuta cada hora (este tiempo se puede cambiar, dependiendo como lo requiera cada cliente). |
| --- |

**Importación de órdenes de trabajo con campos adicionales**

Para la importación de ordenes se deben tener en cuenta las siguientes recomendaciones (algunas están en la pantalla de importación):

1.  Verifique que los títulos de las columnas en el encabezado no estén vacíos.
2.  Los campos adicionales deben tener en el título de columna el nombre del campo adicional. (Tabla AFW_ADDITIONAL_FIELD campo name)
3.  Los campos adicionales configurados en la aplicación como solo lectura no deben ser añadidos en el encabezado del archivo.
4.  Verifique que todos los campos adicionales configurados como obligatorios en la aplicación estén diligenciados en el archivo (tener en cuenta campos adicionales generales y de modelo).
5.  Solo agregar ordenes con servicios asociados a un mismo modelo.
6.  Para campos adicionales tipo fecha, diligenciar formato DD/MM/AAAA
7.  Verifique que no existan registros vacíos.
8.  Dentro de la información de los campos de la importación no se debe usar punto y coma (;), porque este es el separador que se utiliza entre columnas para el proceso.
9.  Los campos adicionales que se incluyan en el encabezado deben diligenciarse, en caso contrario se debe dejar el registro vacío, respetando el separador punto y coma (;)
10.  El usuario que realice la importación con campos adicionales de modelo debe tener permisos para el estado SIN PROGRAMAR en el flujo de trabajo para el rol.

Este es un ejemplo:

[]({{ site.baseurl }}/assets/images/image254.png)

| **Nota:** el tiempo de procesamiento del archivo depende de los recursos de memoria y procesador del equipo. Además la complejidad del negocio en cuanto a configuraciones de flujo de estado, campos adicionales y permisos, puede hacer que la verificación de campos tome más tiempo; por este motivo se recomienda que las importaciones contemplen el mismo servicio para que el modelo al que este pertenece y sus campos adicionales sean consistentes y permitan un procesamiento más óptimo. |
| --- |
