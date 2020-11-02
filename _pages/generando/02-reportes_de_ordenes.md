---
title: Reportes de órdenes
chapter: "generando"
---

Estos reportes tienen una orden asociada y por ende un proveedor asociado. Los monitores solo podrán ver los reportes de los proveedores que tengan asociados.

[]({{ site.baseurl }}/assets/images/image278.png)

| **Nota:** si el perfil con el que se inició la sesión es monitor + despachador, se presentará la opción de visualizar todos los proveedores. |
| --- |

### **Reporte de órdenes creadas** {#reporte-de-rdenes-creadas}

Este reporte presenta al usuario una estadística de las órdenes de trabajo creadas en AFLS. El sistema permite consultar las órdenes de trabajo creadas para un servicio en específico o para todos los servicios dentro de un rango de fechas.

[]({{ site.baseurl }}/assets/images/image279.png)

_Selección de servicio (Lista de servicios)_

| **Nota**: Si no hay órdenes creadas con el servicio o en el rango de fechas seleccionado, el sistema presentará un mensaje indicando que no hay datos para el filtro configurado. |
| --- |

Una vez haya seleccionado el servicio y el rango de fechas, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image280.png)

_Reporte generado para órdenes creadas_

El reporte incluye también una grilla con los datos más relevantes de las órdenes creadas que coincidan con los servicios y fechas seleccionados.

[]({{ site.baseurl }}/assets/images/image281.png)
_Grilla del reporte generado para órdenes creadas_

### **Reporte de costos** {#reporte-de-costos}

Este reporte presenta al usuario una estadística del costo de las órdenes de trabajo ejecutadas dentro de un rango de tiempo y permite filtrarlas por servicio y por compañía.

[]({{ site.baseurl }}/assets/images/image282.png)

_Selección de compañía (Lista de compañías)_

| **Nota:** Si el servicio no tiene órdenes ejecutadas dentro del rango de fecha que seleccionó el usuario, el sistema presentará un mensaje indicando que no hay datos para el filtro configurado. |
| --- |

Una vez haya seleccionado el rango de fechas, el servicio y la compañía, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image283.png)

_Reporte generado para costos de órdenes creadas_

El reporte muestra tres secciones: costo ejecutado, costo promedio ejecutado y grilla de datos.

En **costo ejecutado**, hay una gráfica indicando el costo de cada uno de los siguientes cuatro parámetros:

*   Costo base total de servicios.
*   Costo total de inventario.
*   Costo total de transporte.
*   Costo total de especialistas

En **costo promedio ejecutado**, hay una gráfica indicando el costo promedio de los mismos cuatro parámetros.

| **Nota**: el valor de los costos dependerá de la configuración de costos que se le haya dado a los servicios y a los especialistas; si el servicio o especialista no tienen valores configurados, el resultado no será visible en la gráfica, es decir, será 0. |
| --- |

La grilla de datos muestra información más detallada de los costos:

[]({{ site.baseurl }}/assets/images/image284.png)

_Grilla del reporte generado para costos_

### **Reporte de tendencia de servicio** {#reporte-de-tendencia-de-servicio}

Este reporte presenta al usuario un resumen del comportamiento de un servicio dentro de AFLS y le permitirá al administrador de la mesa validar si se están cumpliendo las metas propuestas para ese servicio. Aquí el usuario podrá consultar específicamente la tendencia de un servicio en el último año, el último mes o la última semana.

[]({{ site.baseurl }}/assets/images/image285.png)

_Selección del periodo de tiempo_

Una vez haya seleccionado el periodo y el servicio, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image286.png)

_Reporte generado para tendencia del servicio_

El reporte muestra tres partes: grado de cumplimiento, promedio de cronómetro de solución y tendencia de servicio.

En **grado de cumplimiento**, se muestra una gráfica indicando la cantidad de órdenes cerradas que están dentro o fuera del SLA de solución por servicio.

En **promedio de cronómetro de solución**, se muestra una gráfica indicando el tiempo promedio de solución de todas las órdenes correspondientes al servicio y periodo seleccionados.

En **tendencia de servicio**, se muestra una gráfica indicando la tendencia en la creación y cierre de los casos u órdenes correspondientes al servicio y periodo seleccionados. Esta gráfica permite comparar el número de órdenes creadas con el número de órdenes ejecutadas.

### **Reporte de promedio de tiempo de solución de órdenes por servicio** {#reporte-de-promedio-de-tiempo-de-soluci-n-de-rdenes-por-servicio}

Este reporte indica la velocidad a la que se solucionan las órdenes de trabajo. Ayudará al monitor a saber cuáles servicios tardan más tiempo, y posiblemente requieran mayor atención o más personal para dar solución. Aquí el usuario podrá consultar los servicios según el rango de fecha seleccionado.

[]({{ site.baseurl }}/assets/images/image287.png)

_Selección de rango de fecha_

| **Nota**: si el servicio no tiene órdenes dentro del rango de fecha seleccionado, el sistema presentará un mensaje indicando que no hay datos para el filtro configurado. |
| --- |

Una vez seleccionado el rango de fechas, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image288.png)

_Reporte generado para promedio de tiempo de solución de órdenes_

El reporte muestra una gráfica que indica el total de horas que se han empleado en la solución de un servicio dentro del periodo de tiempo indicado. Debajo de la gráfica se presenta el tiempo promedio de solución de todas las órdenes presentadas.

La grilla de datos generada muestra información más detallada sobre las horas empleadas en atención y ejecución de cada orden de trabajo.

### **Reporte de órdenes ejecutadas por especialista** {#reporte-de-rdenes-ejecutadas-por-especialista}

Este reporte indica el desempeño de los especialistas en un rango de tiempo con respecto a un servicio en particular. Aquí es posible ver cuáles especialistas han ejecutado la mayor cantidad de órdenes y el tiempo que han tardado en ejecutarlas.

Una vez seleccionado el rango de fechas y el servicio, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image289.png)

_Gráfica del reporte de órdenes cerradas_

El reporte muestra dos partes: promedio de tiempos acumulados y mayor cantidad de casos ejecutados.

En **promedio de tiempos acumulados**, se muestra una gráfica indicando el promedio de las horas ejecutadas por cada especialista para el servicio seleccionado.

En **mayor cantidad de casos ejecutados**, se muestra una gráfica indicando la cantidad de casos cerrados por cada especialista.

La grilla de datos generada con el reporte muestra el total de órdenes ejecutadas y los datos de los tiempos de ejecución por cada especialista.

| **Nota**: si el servicio no tiene órdenes dentro del rango de fecha seleccionado, el sistema presentará un mensaje indicando que no hay datos para el filtro configurado. |
| --- |

### **Reporte de cumplimiento de SLA** {#reporte-de-cumplimiento-de-sla}

Este reporte indica la cantidad de casos por servicio que fueron solucionados en un rango de tiempo en AFLS. Aquí el usuario podrá consultar la cantidad de órdenes creadas y que se encuentren dentro o fuera del SLA de solución.

Una vez seleccionado el rango de fechas y el servicio, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image290.png)
_Reporte generado para cumplimiento del SLA_

El reporte muestra dos partes: total de órdenes dentro del SLA y servicios dentro del SLA.

En **total de órdenes dentro del SLA**, se muestra una gráfica indicando la cantidad total de órdenes ejecutadas que están dentro o fuera del SLA de solución.

En **servicios dentro del SLA**, se muestra una gráfica indicando la cantidad de casos ejecutados que estén dentro o fuera del SLA de solución por servicio.

| **Nota**: la información presentada depende de la configuración de filtro realizada. Si son más de 5 servicios, en la gráfica se presentarán los 5 primeros servicios con más casos ejecutados. |
| --- |

La grilla de datos generada con el reporte muestra la información detallada de cada una de las órdenes ejecutadas.

### **Reporte de cumplimiento del nivel de satisfacción.** {#reporte-de-cumplimiento-del-nivel-de-satisfacci-n}

Este reporte detalla el nivel de satisfacción de los clientes según una encuesta específica en determinado periodo de tiempo.

[]({{ site.baseurl }}/assets/images/image291.png)

_Selección de rango de tiempo y encuesta_

| **Nota**: si no se han generado encuestas dentro del rango de fecha seleccionado, el sistema indicará que no hay datos. |
| --- |

Una vez seleccionado el rango de fechas y la encuesta, haga clic en **Enviar** y se generará un reporte como el siguiente:

[]({{ site.baseurl }}/assets/images/image292.png)

_Reporte generado para cumplimiento del nivel de satisfacción_

El reporte muestra dos partes: nivel de satisfacción y calificación por pregunta.

En **nivel de satisfacción**, se muestra una gráfica indicando el nivel de satisfacción obtenido de la encuesta dentro del rango de fechas seleccionadas.

En **calificación por pregunta**, se muestra una gráfica mostrando las preguntas que son de tipo calificación con su respectivo promedio.

| **Nota**: algunas de las preguntas pueden ser de tipo calificación pero si no están marcadas para contar dentro de las estadísticas, estas no se tendrán en cuenta en el nivel de satisfacción obtenido. |
| --- |

La grilla de datos generada con el reporte muestra la información detallada de cada una de las encuestas contestadas por los clientes.

[]({{ site.baseurl }}/assets/images/image293.png) 
_Grilla del reporte generado para cumplimiento de nivel de satisfacción_
