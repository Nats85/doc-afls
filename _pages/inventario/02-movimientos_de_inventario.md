---
title: Movimientos de inventario
chapter: "inventario"
---

En este módulo puede gestionar el inventario ejecutando entradas, salidas y transferencias de productos ya configurados desde la administración de AFLS. De igual manera puede hacer una importación de entradas y salidas por medio de un archivo **.csv**.

![]({{ site.baseurl }}/assets/images/image257.png)

_Opción de ingreso a Movimientos_

### **Entrada de producto** {#entrada-de-producto}

Un usuario con el rol de gestor de inventarios podrá crear un movimiento de entrada en la pantalla de gestión de inventarios. Una entrada corresponde a la llegada de un nuevo elemento a una ubicación de inventario. Para crear una entrada, seleccione la opción **Nueva Entrada** de la categoría **Movimientos** y defina lo siguiente:

#### Información entrada {#informaci-n-entrada}

Esta sección tiene precargados los siguientes campos:

*   **Responsable:** nombre del usuario que inició sesión
*   **Fecha de registro**

Diligencie los siguientes campos:

*   **Número de factura o referencia**
*   **Fecha de compra:** fecha en la que la compañía adquirió los elementos
*   **ID de tercero:** identificador del proveedor: NIT, cédula u otro
*   **Descripción del movimiento**: información adicional relevante para la entrada de inventario


![]({{ site.baseurl }}/assets/images/image258.png)

_Pantalla para ingresar la información básica de la entrada_

#### Detalle del producto {#detalle-del-producto}

Si se trata de un producto tipo cantidad deberá ingresar la siguiente información:

*   **Cantidad (Unds):** cantidad de producto en su respectiva unidad de medida (m, cm, kg)
*   **Valor por unidad:** valor de compra del producto por unidad
*   **Ubicación:** lugar a donde se realiza la entrada del producto

![]({{ site.baseurl }}/assets/images/image259.png)

_Pantalla para ingresar la información de un producto tipo cantidad_

Si se trata de un producto tipo único deberá ingresar la siguiente información:

*   **Número de serie:** identificador único del producto
*   **Valor por unidad:** valor de compra del producto por unidad
*   **Ubicación:** lugar a donde se realiza la entrada del producto

![]({{ site.baseurl }}/assets/images/image260.png)

_Pantalla para ingresar la información de un producto tipo único_

### **Salida de producto** {#salida-de-producto}

En la pantalla de gestión de inventarios, un usuario con el rol de gestor de inventarios podrá crear un movimiento de salida (o baja) de un elemento de una ubicación de inventario. Para crear una salida, seleccione la opción **Nueva Salida** de la categoría **Movimientos** y defina lo siguiente:

#### Información salida {#informaci-n-salida}

Esta sección tiene precargados los siguientes campos:

*   **Responsable:** nombre del usuario que inicio sesión
*   **Fecha de registro**

Diligencie los siguientes campos:

*   **Número de factura o referencia**
*   **ID de tercero:** identificador del proveedor: NIT, cédula u otro
*   **Descripción del movimiento**: información adicional relevante para la salida de inventario
*   **Relacionar orden de trabajo:** campo para relacionar una orden de trabajo si es necesario. Las órdenes deben estar en estado **Ejecutado**.

![]({{ site.baseurl }}/assets/images/image261.png)

_Pantalla para ingresar la información básica de la salida_

#### Detalle del producto {#detalle-del-producto-0}

Si se trata de un producto tipo cantidad deberá ingresar la siguiente información:

*   **Cantidad (Unds):** cantidad de producto a sacar del inventario
*   **Ubicación:** lugar de donde se sacará el producto

Si se trata de un producto tipo único deberá ingresar la siguiente información:

*   **Número de serie:** identificador único del producto
*   **Ubicación:** lugar de donde se realiza la salida del producto

![]({{ site.baseurl }}/assets/images/image262.png)

_Pantalla para ingresar la información de un producto tipo cantidad_

### **Transferencia de producto** {#transferencia-de-producto}

Un usuario con el rol de gestor de inventario puede crear un movimiento de transferencia en la pantalla de gestión de inventarios. Una transferencia corresponde al traslado de un producto de una ubicación a otra. Para crear una transferencia, seleccione la opción **Nueva Transferencia** de la categoría **Movimientos** y defina lo siguiente:

#### Información de transferencia {#informaci-n-de-transferencia}

Esta sección tiene precargados los siguientes campos:

*   **Responsable:** nombre del usuario que inició sesión.
*   **Fecha de registro**

Diligencie los siguientes campos:

*   **Número de factura o referencia**
*   **Descripción del movimiento**

#### Transferir producto {#transferir-producto}

Si se trata de un producto tipo cantidad deberá ingresar la siguiente información:

*   **Cantidad (Unds):** cantidad de producto a transferir en su respectiva medida (m, cm, kg)
*   **Ubicación de origen:** lugar de donde saldrá el producto
*   **Ubicación de destino:** lugar a donde se hará la entrada del producto


![]({{ site.baseurl }}/assets/images/image263.png)

_Pantalla para ingresar la información de transferencia de un producto tipo cantidad_

Si se trata de un producto tipo único deberá ingresar la siguiente información:

*   **Número de serie:** identificador único del producto
*   **Ubicación de origen:** lugar de donde saldrá el producto
*   **Ubicación de destino:** lugar a donde se hará la entrada del producto

![]({{ site.baseurl }}/assets/images/image264.png)

_Pantalla para ingresar la información de transferencia de un producto tipo único_

### **Importación de movimientos** {#importaci-n-de-movimientos}

Un usuario con rol de gestor de inventario puede importar movimientos desde un archivo **.csv**, (valores separados por comas) con el cual puede crear entradas y salidas de inventario.

Para importar movimientos de inventario, seleccione la opción **Importación de movimientos**, aparecerá un buscador que le permitirá seleccionar el archivo de los movimientos a importar, y un enlace con el cual podrá descargar una plantilla modelo del archivo para realizar la importación.

![]({{ site.baseurl }}/assets/images/image265.png)

La siguiente es la estructura definida para la importación de movimientos.

*   **MovementType:** tipo de movimiento
    *   1: entrada
    *   2: salida
*   **PurchaseDate:** fecha de compra (formato DD/MM/AAAA)
*   **Reference:** referencia de producto
*   **SpecialistLocation:** nombre de usuario del especialista (debe ir vacío si la ubicación es una locación fija).
*   **Location:** ID de la ubicación. Debe ir vacío si el movimiento es sobre un especialista.
*   **Product:** ID del producto
*   **SerialNumber:** serial del producto (únicamente para producto de tipo único).
*   **ThirdId:** identificador único del proveedor: NIT, cédula u otro. Campo no obligatorio.
*   **WorkOrderId:** número de ticket de la orden de trabajo. La orden debe estar en estado Ejecutado. Campo no obligatorio.
*   **UniteValue:** valor por unidad del producto
*   **Quantity:** cantidad de producto. Solo aplica para productos de tipo cantidad

Una vez cargado el archivo correctamente configurado, haga clic en el botón **Importar**. El sistema procesará el archivo y al terminar, presentará un mensaje de confirmación, indicando los movimientos que se importaron.

![]({{ site.baseurl }}/assets/images/image266.png)
_Mensaje de importación exitosa de movimientos_

Si el archivo de movimientos a importar contiene uno o más registros configurados de manera errónea, en la ventana de finalización del proceso de carga, aparecerá la cantidad de registros no importados y un nuevo botón: **Ver archivo de errores** que le permitirá descargar un archivo **.csv** que contiene los registros que no se importaron.

![]({{ site.baseurl }}/assets/images/image267.png)

_Mensaje de importación de movimientos NO exitosa_

Al oprimir el botón, se mostrará una ventana del explorador de Windows para que el usuario seleccione la ubicación en la que desea guardar el archivo.

![]({{ site.baseurl }}/assets/images/image268.png)

_Archivo con los movimientos que no se importaron._

Al abrir el archivo, se observan los registros que se procesaron y al final de la línea de aquellos que fallaron, se mostrará la razón por la que fallaron.


![]({{ site.baseurl }}/assets/images/image269.png)
_Mensaje de validación dentro del archivo._

### **Filtro de búsqueda de inventario** {#filtro-de-b-squeda-de-inventario}

Este filtro permite a un usuario con rol de gestor de inventario visualizar los movimientos de inventario según su fecha inicial, fecha final y tipo de movimiento.
![]({{ site.baseurl }}/assets/images/image270.png)
