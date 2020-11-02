---
title: Configuración de inventarios por parte del administrador
chapter: "configurando"
---

En el módulo **Inventarios** puede configurar y definir los productos, las bodegas y las unidades de medida que utiliza el negocio. Un usuario con rol de administrador podrá crear, eliminar o editar los submódulos **Medidas**, **Productos** y **Ubicaciones**.

**Medidas**

Aquí puede crear las medidas que se van a usar en la creación de productos, los siguientes son los campos necesarios para crear una medida.

*   **Nombre de la medida:** ejemplo metros (mt), centímetros (cm) ...
*   **Descripción:** Resumen del uso que se dará a este tipo de medida
*   **Estado:** La medida puede estar activa o inactiva y esto determinará si puede usarse para la creación o edición de productos.

![]({{ site.baseurl }}/assets/images/image101.png)

**Productos**

Aquí puede crear, editar y eliminar los productos que se usarán en la operación del negocio, los siguientes son los campos necesarios para la creación de un producto:

*   **Tipo de producto:** Puede ser de dos tipos:
*   **Cantidad:** Producto que se puede medir por cantidades y no tiene un identificador único. Ej. Cable coaxial, medida metros.
*   **Código único:** Producto que se puede identificar con un serial. Ej. Decodificador.
*   **Número de referencia(SKU)**
*   **Nombre del producto**
*   **Descripción:** Máximo 250 caracteres.
*   **Cantidad mínima:** Cantidad mínima que debe haber en inventario. Activa una alerta cuando se llega a esta cantidad.
*   **Unidad de medida**
*   **Precio de compra (calculado):** Este valor se calcula de manera automática una vez se van haciendo entradas del producto en el inventario.
*   **Precio de venta:** Precio al cual se vende el producto.
*   **Estado:** Puede ser activo o inactivo y esto determinará si se puede usar el producto o no.

| **Nota:** Todos los campos son requeridos para la creación del producto |
| --- |


![]({{ site.baseurl }}/assets/images/image102.png)

**Ubicaciones**

Aquí se configuran las zonas, sedes y transporte para distribuir el inventario. Se mostrará un árbol con las diferentes ubicaciones como principales e hijas.

**Creación de una sede principal:** haga clic en **Nueva Sede** o en el **icono** y llene los siguientes campos:

*   **Tipo de sede:** puede ser:
*   Edificio.
*   Almacén.
*   Bodega.
*   **Nombre de la sede**
*   **Descripción:** máximo 250 caracteres.
*   **Dirección**
*   **Detalle de la dirección:** información que ayuda a identificar mejor la ubicación de la sede.
*   **Estado:** puede ser activa o inactiva.
*   **Marcar como ubicación por defecto:** es la ubicación que por defecto se asigna a un especialista móvil cuando al crearlo no se selecciona una sede de inventario.

![]({{ site.baseurl }}/assets/images/image104.png)

**Creación de un transporte principal:** haga clic en **Nuevo transporte** o en el iconoy llene los siguientes campos:

*   **Tipo de transporte:** puede ser:
*   Camión
*   Vehículo
*   **Nombre del transporte:** Puede ser la placa o algún otro identificador del transporte.
*   **Descripción**
*   **Estado:** Puede ser activo o inactivo.
*   **Información de contacto:** Esta información es opcional y no es requerida para la creación de la sede.


![]({{ site.baseurl }}/assets/images/image105.png)


**Zonas:** Al hacer clic en el icono de una sede o transporte creado, se podrá crear una nueva zona, la cual puede ser de los siguientes tipos:

*   Estante
*   Piso
*   Caja

Estas zonas pueden contener zonas dentro de ellas, ej. un piso puede tener caja 1 y caja 2 y a su vez las cajas pueden contener caja 001.

Diligencie los campos restantes para completar la creación de la zona.

![]({{ site.baseurl }}/assets/images/image107.png)

| **Nota:** Puede editar una sede, transporte o zona haciendo clic sobre su nombre y seleccionando el icono de la acción deseada. Solo puede eliminar los nodos que no tengan hijos. |
| --- |
