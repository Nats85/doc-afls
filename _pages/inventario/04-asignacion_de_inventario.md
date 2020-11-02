---
title: Asignación de inventario
chapter: "inventario"
---

Esta funcionalidad permite asignar material de una o varias ubicaciones hacia un especialista. Esto, en términos generales corresponde a un movimiento de transferencia entre dos ubicaciones (considerando el especialista como una ubicación).

Desde esta pantalla puede realizar una búsqueda para listar los elementos del inventario que un especialista necesita para atender todas las órdenes programadas dentro de un rango de fechas, y asignarlo al especialista.

[]({{ site.baseurl }}/assets/images/image272.png)

_Pantalla de asignación de inventario_

Los campos a diligenciar son:

*   Casilla de ordenes planeadas: marque esta casilla para incluir en la búsqueda los productos correspondientes a órdenes planeadas, entendiendo que las planeadas son aquellas que no tienen una fecha fija de atención, a diferencia de las órdenes programadas.
*   Especialista: Nombre del especialista al que se le quiere asignar inventario.
*   Fecha inicial: fecha desde la cual se asignará inventario (por omisión se muestra la fecha actual).
*   Fecha final: fecha hasta la cual se asignará inventario.

Luego haga clic en el botón **Buscar**.

[]({{ site.baseurl }}/assets/images/image273.png)

_Ejemplo de asignación de inventario_

El inventario puede estar reservado. Es decir, que ha sido apartado para unas órdenes y un especialista específicos, faltando solo confirmar la asignación. También puede asignarse de forma manual seleccionando la ubicación de donde se va a tomar como se muestra a continuación:

[]({{ site.baseurl }}/assets/images/image274.png)

Haga clic en el botón **Seleccionar todo** para hacer una preselección masiva de los productos que se van a asignar y luego haga clic en el botón **Asignar inventario**. Se realizarán los movimientos de transferencia entre las partes indicadas. Estos movimientos pueden confirmarse al consultar el módulo de movimientos.

[]({{ site.baseurl }}/assets/images/image275.png)

_Visualización de movimientos generados_

| **Nota:** las asignaciones de inventario corresponden a movimientos de transferencia entre una ubicación y un especialista. Los especialistas se tratan como una ubicación. De esta manera se observan transferencias de productos entre las ubicaciones. No es posible crear un movimiento de asignación. |
| --- |
