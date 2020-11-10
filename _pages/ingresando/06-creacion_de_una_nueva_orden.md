---
title: Creación de una nueva orden
chapter: "ingresando"
---

Aquí los especialistas en campo podrán crear nuevas órdenes ingresando la información solicitada:

![]({{ site.baseurl }}/assets/images/image339.png)

_Creación de nueva orden desde la consola móvil_

| **Nota**: el especialista sólo podrá visualizar esta funcionalidad si se habilita previamente desde la consola web en la pantalla de **Ajustes Globales**. Si ya hay especialistas con sesión iniciada, es necesario cerrar sesión e iniciar nuevamente para visualizar la funcionalidad en el dispositivo. |
| --- |

| **Nota**: los servicios que se visualizan para la creación de una nueva orden deben haber sido habilitados por el administrador en la opción de **Servicios**. |
| --- |

**Funcionamiento a mi nombre**

Esta funcionalidad hace un llamado manual al motor de asignación para saber en qué fecha y hora el especialista en sesión puede atender la orden de trabajo que se va a crear.

![]({{ site.baseurl }}/assets/images/image340.png)

_Asignación de nueva orden al especialista en sesión_

**Funcionamiento a otro especialista**

Hace un llamado al motor de asignación para saber la fecha y hora en que los otros especialistas que pertenecen al proveedor del usuario en sesión pueden atender la orden de trabajo.

![]({{ site.baseurl }}/assets/images/image341.png)

_Asignación de nueva orden a otro especialista_

Al crear una nueva orden, el sistema verifica si se presenta alguna de las siguientes situaciones:

| Sin cobertura, es decir, que la dirección ingresada no está dentro de la zona de cobertura para su atención: | Sin proveedor disponible, es decir que la zona y servicios seleccionados no pueden ser atendidos por ningún proveedor: |
| --- | --- |

![]({{ site.baseurl }}/assets/images/image342.png)
![]({{ site.baseurl }}/assets/images/image343.png)

| **Nota**: Esta funcionalidad solo está disponible en línea. |
| --- |
