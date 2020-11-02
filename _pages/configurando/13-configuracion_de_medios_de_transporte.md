---
title: Configuración de medios de transporte
chapter: "configurando"
---

Como parte del modelamiento de un negocio, un administrador puede crear diferentes tipos de vehículo dentro de Aranda FIELD SERVICE. Una compañía podrá incluir dentro de sus activos diferentes tipos de vehículo, y cada uno tener asociado un costo relacionado. Este costo se utilizará para calcular el costo total de la orden ejecutada.

Cada tipo de vehículo se configura teniendo en cuenta la siguiente información:

*   **Nombre del tipo de vehículo**. Identifica el tipo de vehículo que posteriormente será asociado a un especialista.
*   **Descripción**. Permite ingresar información adicional sobre el tipo de vehículo.
*   **Costo**. La sección de costos se divide en dos. Por un lado, el costo inicial permite agregar un costo fijo al cálculo de la orden, por otro lado, el costo por kilómetro permite deducir el costo total de ejecución de la orden teniendo en cuenta la distancia que el especialista necesita recorrer para llegar a la ubicación seleccionada.
*   **Tipo de Transporte**. El tipo de transporte se utiliza para trazar la ruta óptima que debe recorrer el especialista por las calles de la ciudad. Se podrían definir por ejemplo varios vehículos que utilizan las carreteras principales con diferente costo (vehículo particular y taxi), o a la vez tener varios medios de transporte público.

**Tipos de transporte.** Los tipos de transporte definidos para crear un vehículo son los siguientes:

*   **Carro**. Utiliza la información proporcionada por Google para encontrar la ruta óptima de desplazamiento de vehículos particulares.
*   **Caminando**. Utiliza la información proporcionada por Google para calcular el desplazamiento del especialista a pie.
*   **Bicicleta**. Utiliza la información de la ciudad de creación de la orden sobre rutas optimizadas para transporte en bicicleta.
*   **Transporte público**. A partir de la información registrada en Google se pueden encontrar las rutas de diferentes medios de transporte público que puede utilizar un especialista para llegar al lugar donde está registrada una orden.


![]({{ site.baseurl }}/assets/images/image77.png)


**Tipo de transporte público**

Google almacena información sobre transporte público de algunas de las principales ciudades del mundo. Esta información es consultada por Aranda FIELD SERVICE para optimizar el desplazamiento de los especialistas que utilizan este medio de transporte.

De acuerdo a la información almacenada en Google, se pueden seleccionar algunas configuraciones (que aplican solo a algunas ciudades), para luego seleccionar las siguientes subcategorías:

• Bus • Metro • Tren • Tranvía • Trenes de cercanía

Si el medio de transporte no está disponible para una ciudad, se utilizará el tipo de transporte de vehículo privado en su lugar.

Las ciudades donde se tiene cobertura para transporte público se pueden consultar en el siguiente enlace:

[https://maps.google.com/landing/transit/cities/](https://maps.google.com/landing/transit/cities/)
