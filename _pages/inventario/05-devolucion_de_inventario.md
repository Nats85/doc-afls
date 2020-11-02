---
title: Devolución de inventario
chapter: "inventario"
---

Esta funcionalidad permite realizar una devolución de material de un especialista hacia una o varias ubicaciones. Esto, en términos generales, corresponde a un movimiento de transferencia entre dos ubicaciones (considerando el especialista como una ubicación).

Esto puede suceder por varias razones:

*   El especialista presentó cancelación de una orden y ya tenía el material asignado.
*   El especialista usó menos cantidad de material en una orden.
*   El especialista ya no va a trabajar más con la compañía.

Al realizar los movimientos de transferencias, los materiales quedarán disponibles en la nueva ubicación para que sean utilizados por otras órdenes. Puede realizar dichas transferencias de forma masiva para agilizar el proceso.

En esta pantalla, una vez seleccionado el especialista, el gestor de inventario podrá emplear los siguientes criterios para buscar elementos dentro del inventario asignado de dicho especialista:

*   Todo el inventario libre: realiza una búsqueda por todo el inventario que se encuentre libre (Inventario libre = inventario de órdenes canceladas o inventario de órdenes ejecutadas que no fue utilizado).
*   Por producto
*   Por número de serie

[]({{ site.baseurl }}/assets/images/image276.png)

_Visualización de criterios de búsqueda y productos a devolver_

Haga clic en el botón **Seleccionar todo** para hacer una preselección de todos los productos disponibles para devolución y luego haga clic en el botón **Devolver Inventario**. Se transferirán los elementos del especialista a la ubicación definida por el gestor de inventario.

Estos movimientos de transferencia pueden confirmarse al consultar el módulo de movimientos.

[]({{ site.baseurl }}/assets/images/image277.png)

_Visualización de movimientos generados_

| **Nota:** las devoluciones de inventario corresponden a movimientos de transferencia entre un especialista y una ubicación. Los especialistas se tratan como una ubicación. De esta manera se observan transferencias de productos entre las ubicaciones. No es posible crear un movimiento de devolución. |
| --- |
