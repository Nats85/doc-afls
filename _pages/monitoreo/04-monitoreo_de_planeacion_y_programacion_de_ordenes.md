---
title: Monitoreo de planeación y programación de órdenes
chapter: "monitoreo"
---

En la opción **Planeación** del módulo de **Monitoreo**, el monitor puede emplear el buscador para seleccionar varios especialistas en campo y observar, a través de un diagrama de Gantt, como se distribuyen las órdenes en un día, una semana o un mes. Esta información es particularmente útil para encontrar tiempos ociosos por parte de los especialistas.

![]({{ site.baseurl }}/assets/images/image319.png)

### **Filtrando y ordenando la consulta de planeación**

Puede filtrar la información de la consulta bajo los siguientes criterios:

*   **Proveedor**: el monitor solo podrá visualizar los proveedores que tiene asignados, por lo tanto, podrá filtrar los especialistas sólo según dichos proveedores desde el selector.
*   **Disponibilidad especialista**: filtra los especialistas según una de estas condiciones:
    *   Que se encuentren prestando alguno de los servicios configurados, que tienen órdenes de trabajo asignadas.
    *   Que estén capacitados y tengan las habilidades para atender alguno de los servicios configurados, que estén disponibles y tengan la capacidad de atender el servicio.
*   **Servicios**: filtra los especialistas según el servicio que estén prestando o para el que estén capacitados y que tengan ese o varios servicios configurados como criterio de consulta. El filtro de servicios depende de la configuración definida en el combo anterior de disponibilidad del especialista.
*   **Grupos**. filtra los especialistas según el grupo al que estén asociados.

Al seleccionar uno de los especialistas arrojados por la consulta, en el panel de la derecha visualizará la información de las órdenes, presentada en dos pestañas: **Agenda de órdenes** y **Plan de rutas**.

### **Agenda de órdenes**

En esta pestaña podrá observar la carga que se le ha asignado a cada uno de los especialistas seleccionados. Cada orden contiene información sobre el momento en que el especialista inicia el desplazamiento y el tiempo programado de ejecución y finalización del trabajo. Los espacios en la gráfica donde no existen órdenes programadas se consideran tiempos muertos.


![]({{ site.baseurl }}/assets/images/image320.png)

*   Los espacios en blanco representan los tiempos en los que el especialista puede atender órdenes de trabajo.
*   El patrón de rayas representa los tiempos programados donde el especialista debe desplazarse hasta el lugar de la siguiente orden.
*   El color en cada una de las órdenes representa el estado en el que se encuentra.

A través de los controles ubicados en la parte superior derecha, el monitor puede modificar las fechas sobre las que se despliega la información. Estos datos se pueden mostrar de manera diaria, semanal o mensual.

Al mover el puntero sobre cualquier orden se puede observar un resumen de la misma y se despliega las horas de desplazamiento y la hora programada de inicio. Así mismo el botón de “ver orden” abrirá el detalle.

### **Plan de rutas**

En esta pestaña el usuario podrá visualizar el mapa con la ruta planeada para uno o varios especialistas y las posiciones en las que se encontrarán de acuerdo al rango de fecha seleccionado.

| **Nota**: las posiciones en las que se encontrará el especialista, son las posiciones de las órdenes de trabajo que tiene asignadas a él. |
| --- |

Este mapa ofrece las opciones para expandir y para mostrar la ubicación de la compañía.

![]({{ site.baseurl }}/assets/images/image321.png)

**Ruta de distintos especialistas seleccionados**

En el mapa aparecerán las rutas de todos los especialistas que se hayan seleccionado, cada uno con un color diferente.

![]({{ site.baseurl }}/assets/images/image322.png)

_Ruta de distintos especialistas seleccionados_

Los controles ubicados en la parte superior derecha permiten modificar las fechas sobre las que se despliega la información. Estos datos se pueden mostrar de manera diaria, semanal o mensual.

Si los especialistas seleccionados coinciden en una o varias ubicaciones, el usuario puede hacer clic en el punto en común para separarlos y observar qué usuarios tienen posiciones en ese punto.

| **Nota**: los puntos de ubicación del especialista se verán únicamente si este tiene órdenes asignadas para el rango de fecha seleccionado. |
| --- |

Al hacer clic sobre la posición del especialista, el sistema presentará una descripción emergente con algunos datos básicos como el nombre del especialista, la distancia al próximo punto y las órdenes restantes. La distancia al próximo punto se muestra de manera lineal, este valor puede variar si el usuario selecciona la opción de presentar la ruta con la opción de Google.

![]({{ site.baseurl }}/assets/images/image323.png)

_Ruta presentada de manera lineal_
