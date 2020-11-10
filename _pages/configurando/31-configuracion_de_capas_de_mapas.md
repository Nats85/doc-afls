---
title: Configuración de capas de mapas
chapter: "configurando"
---

Una capa de mapa es un conjunto de puntos georeferenciados que representan lugares de interés para el negocio, como sucursales, gasolineras, bodegas, etc.

Desde este módulo es posible consultar, agregar, editar y eliminar todas las capas de mapas según lo requiera la operación.

![]({{ site.baseurl }}/assets/images/image141.png)


Para crear una nueva capa haga clic en el botón **Nuevo** e ingrese la información solicitada en la pestaña **Configuración de capa**.

Tenga en cuenta que:

*   Los campos correspondientes al nombre y descripción de la capa son obligatorios.
*   La capa se crea por defecto en estado inactivo, esto quiere decir que debe activarse para que sea visible desde la interfaz web o móvil.
*   Antes de adicionar localizaciones es necesario crear la capa.

Una vez ingrese la información necesaria, haga clic en el botón **Guardar** para conservar los cambios realizados. Aparecerá un mensaje confirmando que se ha guardado correctamente.

![]({{ site.baseurl }}/assets/images/image142.png)


Para personalizar el icono con el que se representarán los puntos creados dentro de la capa, haga clic en el botón **Cambiar**.


![]({{ site.baseurl }}/assets/images/image143.png)


Seleccione alguno de los iconos predefinidos o agregue una URL remota que conduzca a la imagen deseada. Se recomienda que el icono tenga dimensiones de 40x40 para una visualización adecuada.


![]({{ site.baseurl }}/assets/images/image144.png)


### **Adicionar Localización**

En la pestaña **Adicionar Localización** puede visualizar los puntos o localizaciones agregados a la capa. Al situar el cursor sobre cada punto de localización marcado en el mapa, se despliega un mensaje mostrando el nombre, la descripción, las coordenadas (longitud, latitud) y el estado actual.


![]({{ site.baseurl }}/assets/images/image145.png)


Puede agregar, modificar o eliminar localizaciones de forma manual (una a una) o masivamente, importando archivos en formato GeoJSON, bajo el sistema internacional de coordenadas geográficas World Geodetic System 1984, con unidades de grados decimales.

![]({{ site.baseurl }}/assets/images/image145.png)

Al hacer clic en el botón **Editar**, se desplegará una ventana emergente con el listado de los puntos agregados a la capa. Puede editar o borrar cada punto según requiera.

![]({{ site.baseurl }}/assets/images/image146.png)

Puede agregar una localización haciendo clic sobre el punto requerido en el mapa, o usando la barra de búsqueda en la parte superior izquierda para ingresar una dirección o nombre de lugar para referenciarlo como una nueva localización de la capa.

### **Agregar localización manualmente a través del mapa**

Haga clic sobre el punto del mapa que requiere georeferenciar como nueva localización de la capa. Se desplegará un recuadro solicitando la información necesaria.

Tenga en cuenta que:

*   El campo **Nombre de Localización** es obligatorio.
*   El campo **Descripción** es opcional.
*   El punto debe estar en estado activo para que se pueda visualizar en la interfaz web o móvil


![]({{ site.baseurl }}/assets/images/image147.png)


Haga clic en el botón **Guardar** para conservar los cambios. Si la localización fue adicionada correctamente se visualizará como un punto en el mapa y como un item dentro del listado de localizaciones en la parte derecha de la pantalla.


![]({{ site.baseurl }}/assets/images/image148.png)


### **Agregar localización a través del buscador de direcciones**

Ingrese la dirección o nombre de la localización en el buscador y haga clic en la lupa. Es sistema realizará un geocodificación a través del proveedor de mapas configurado y mostrará el punto en la longitud y latitud obtenida.

![]({{ site.baseurl }}/assets/images/image149.png)

Tenga en cuenta que:

*   Si la instancia de Aranda FIELD SERVICE cuenta con configuración multi-país, se mostrará el país sobre el cual se realizará la búsqueda.
*   De no encontrarse la dirección ingresada se mostrará un recuadro rojo sobre el buscador.

El resultado de la búsqueda se mostrará sobre el mapa de acuerdo a las coordenadas entregadas por el proveedor de mapas y se desplegará el recuadro para diligenciar la información necesaria para dar de alta la nueva localización.

![]({{ site.baseurl }}/assets/images/image150.png)

Tenga en cuenta que:

*   El campo **Nombre de Localización** es obligatorio.
*   El campo **Descripción** es opcional.
*   El punto debe estar en estado activo para que se pueda visualizar en la interfaz web o móvil

### **Agregar localización por medio de importación GeoJSON**

Una vez configurados los atributos de importación GeoJSON en los ajustes globales, Aranda FIELD SERVICE podrá importar localizaciones masivamente a una capa bajo el sistema de referencias de coordenadas geográficas World Geodetic Sistem 1984 y unidades de grados decimales.

Para esto, en la ventana de gestión de localizaciones haga clic sobre el texto **Seleccione Archivo**:

![]({{ site.baseurl }}/assets/images/image151.png)


Seleccione el archivo GeoJSON a importar y haga clic en **Abrir**

![]({{ site.baseurl }}/assets/images/image152.png)


Luego haga clic en el botón **Importar**

![]({{ site.baseurl }}/assets/images/image153.png)

El sistema verificará cada uno de los puntos y, a través de una ventana emergente, informará cuáles pueden agregarse como localizaciones de la capa y cuáles no.

![]({{ site.baseurl }}/assets/images/image154.png)


A partir de este resultado verifique los atributos del archivo GeoJSON a importar y elimine todas las localizaciones que no cumplen con los parámetros mínimos para ser agregadas a la capa (nombre, lontigud, latitud). La importación no podrá terminarse hasta que estos puntos sean eliminados o corregidos desde el archivo GeoJSON.

Una vez depurados los puntos, haga clic en el botón **Importar** para completar el proceso.

### **Visualización de capas y localizaciones** 

Para visualizar las capas creadas y activas dentro de Aranda FIELD SERVICE en los mapas de las interfaces web y móvil, diríjase al recuadro en la esquina superior izquierda del mapa y seleccione la capa requerida

![]({{ site.baseurl }}/assets/images/image155.png)

Los puntos de la capa seleccionada se desplegarán de forma automática en el mapa:

![]({{ site.baseurl }}/assets/images/image156.png)
