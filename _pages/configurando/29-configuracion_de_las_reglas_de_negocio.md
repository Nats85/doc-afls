---
title: Configuración de las reglas de negocio
chapter: "configurando"
---

### **Variables del Negocio** {#variables-del-negocio}

El motor de Field Service es personalizable y permite direccionar la asignación de las órdenes para poder cumplir con los objetivos de reducir costos, minimizar los desplazamientos, maximizar la calidad y garantizar el cumplimiento de los tiempos de atención pactados.

En el módulo **Reglas de asignación**, en la pestaña **Variables del negocio** es posible asignar determinada cantidad de estrellas (de un total de 40) a los objetivos que más se deseen optimizar. Los objetivos con mayor cantidad de estrellas tendrán más peso en la asignación de la orden y los que tengan menos estrellas influirán menos en la asignación.

![]({{ site.baseurl }}/assets/images/image137.png)

Los objetivos se clasifican así:

| **Costo de Operación** | **Satisfacción al cliente** | **Distribución** |
| --- | --- | --- |
| **Costo** | **Distancia** | **Habilidades** | **ANS** | **Distribución de carga** |

***** Por defecto, todas las variables vienen con la misma cantidad de estrellas lo que genera una asignación equilibrada y todos los objetivos se intentan cumplir de la mejor forma posible.

**Rendimiento del motor**

Aquí puede limitar la cantidad de procesos que el motor puede trabajar al tiempo dependiendo de las características de hardware del servidor.

![]({{ site.baseurl }}/assets/images/image138.png)


![Configuracion rendimiento del motor.jpg](C:\doc\manual\imagenes\configuracion_rendimiento_del_motor.jpeg)

También puede limitar el uso máximo de CPU, con el fin de evitar que los procesos que utilizan el motor consuman toda la capacidad cuando el servidor esté dedicado a varias tareas.

### **Proveedores** {#proveedores}

En esta pestaña se configuran las reglas que definen el orden para elegir un proveedor. Las opciones son:

*   **Asignar al proveedor con menos carga de trabajo por servicio:** se hace un conteo de órdenes abiertas por proveedor, y se le da prioridad al que tenga menos órdenes asignadas.
*   **Asignar por turnos:** se utiliza un algoritmo de _round trip_ para asignar las órdenes. O también, se asigna al proveedor que tenga la fecha más antigua de la última asignación.
*   **Asignar al proveedor con mejor puntaje en el último mes:** se le da prioridad al proveedor que tenga mayor calificación. Utilizando los tres discos controladores, el administrador puede decidir a cuáles criterios dar mayor o menor peso en el puntaje de los proveedores.

![]({{ site.baseurl }}/assets/images/image139.png)

El proveedor con mayor puntaje recibirá un beneficio que consiste en asignarle una cantidad adicional de órdenes. Dicha cantidad está configurada por defecto como 3, sin embargo, este valor es modificable desde la base de datos (tabla AFW_SETTING).
