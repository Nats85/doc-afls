---
title: Alta Disponibilidad
chapter: "configurando"
---

Con el fin de soportar una operación continua (24/7), AFLS permite emplear un mayor número de servidores con el mismo ambiente instalado (Aplicación y servicios Windows), y así, en caso de que un servidor presente cierres en funcionamiento (de forma voluntaria o forzada), los demás podrán soportar la aplicación y mantenerla en funcionamiento.

Esto se logra de la siguiente forma:

[]({{ site.baseurl }}/assets/images/image199.png)

1.  Mediante comunicaciones que llegan desde un ordenador o un móvil, se reciben peticiones hacia los servidores donde está instalado AFLS.
2.  El balanceador de carga direcciona la petición hacia una instancia de la aplicación que esté en funcionamiento.
3.  Las instancias web comparten un sitio de almacenamiento (en caso cloud se recomienda Azure Storage) para respaldo de adjuntos.
4.  Desde la instancia de la aplicación web se realiza la comunicación con los servidores de servicios Windows.
5.  En caso de que la información se reciba en un servidor que esté caído, el otro servidor se pone en funcionamiento automáticamente para recibir la información.
6.  Se realiza la comunicación con una única base de datos.

Esta estrategia de alta disponibilidad busca reducir los tiempos de posibles caídas de AFLS por motivos de infraestructura.

| **Nota**: La infraestructura actual de alta disponibilidad para AFLS se centra en arquitectura de Azure, y debe configurarse sobre zona horaria GTM-5. |
| --- |
