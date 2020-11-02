---
title: Configuración de cronómetros
chapter: "configurando"
---

En el rol de administrador se pueden definir los conceptos de tiempo que la organización desee medir por medio de la configuración de cronómetros. Estos cronómetros correrán para cada orden de servicio independientemente de los acuerdos con los clientes. Son útiles para detectar casos en los que, por ejemplo, el tiempo utilizado por los especialistas en alguno de los pasos de ejecución de la orden sea crítico, ya sea porque no se ha podido medir o porque es excesivo.

Es posible definir un cronómetro que mida cuánto tiempo se demoró el especialista en la actividad y configurar el flujo de trabajo para que tenga en cuenta este cronómetro de acuerdo a los estados de las órdenes. Los cronómetros solo pueden contar tiempo en unidades de una actividad, por lo tanto, el flujo de trabajo debe estar configurado según la información del proceso de la organización.

Para facilitar el uso de los cronómetros Aranda FIELD SERVICE provee tres cronómetros por defecto: **Tiempo de atención**, **tiempo de ejecución** y **tiempo de solución**.

![]({{ site.baseurl }}/assets/images/image37.png)


Para definir un cronómetro basta ingresar el nombre y la descripción con el fin de crear el concepto. En una próxima sección se explicará cómo se integran estos cronómetros dentro del flujo de trabajo.

**Cronómetro Tiempo de Atención**

La herramienta crea el cronómetro Tiempo de Atención por defecto. Mide el tiempo total desde que se registra una orden hasta que un especialista llega a trabajar a la ubicación del cliente.

**Cronómetro Tiempo de Ejecución**

El cronómetro Tiempo de Ejecución se crea por defecto en la herramienta. Este cronómetro empieza a contar una vez el especialista en campo tiene contacto con el cliente e inicia su labor. Este cronómetro es especialmente importante porque cuando inicia, significa que el especialista ya está con el cliente, es decir, indica si se ha cumplido o no la cita establecida.

**Cronómetro Tiempo de Solución**

El cronómetro Tiempo de Solución se crea por defecto en la herramienta. Mide el tiempo total desde que se registra una orden hasta que se termina de ejecutar.
