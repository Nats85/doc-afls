---
title: Ajustes Globales
chapter: "utilizando"
---

En este módulo se pueden realizar modificaciones fundamentales del negocio, como cambiar el proveedor de mapas, importar datos GeoJSON o habilitar o deshabilitar funciones a los especialistas en campo.

Para poder realizar cambios en esta sección haga clic en el botón **Habilitar Edición**.

![]({{ site.baseurl }}/assets/images/image6.png)

Una vez habilitada la edición, el sistema presentará un mensaje de confirmación advirtiendo que los cambios afectan considerablemente la herramienta.

![]({{ site.baseurl }}/assets/images/image7.png)

Luego de confirmar que desea continuar, en el módulo de **Ajustes Globales** podrá acceder a las siguientes dos pestañas disponibles:

### **Pestaña Ajustes Globales**

En esta pestaña el usuario administrador puede personalizar cuatro parámetros de operación; la configuración de estos parámetros afecta directamente la operación y el desempeño de la herramienta.

![]({{ site.baseurl }}/assets/images/image8.png)

*   Aplicación

Parámetros de configuración sobre el sistema en general:

![]({{ site.baseurl }}/assets/images/image9.png)

**Nota**: Luego de habilitar o deshabilitar el registro de consumo de mapas de la aplicación, es necesario cerrar sesión e iniciar nuevamente para que visualizar el cambio.

*   Consola especialista

Parámetros de configuración para habilitar o inhabilitar capacidades funcionales a los especialistas en campo.

![]({{ site.baseurl }}/assets/images/image10.png)

**Nota**: Luego de habilitar o deshabilitar cualquiera de las opciones de la consola de especialista, es necesario que los especialistas cierren sesión e inicien nuevamente para que puedan visualizar los cambios.

*   Asignación

Dependiendo del tipo de negocio, puede decidir bajo qué circunstancias se reasignan las órdenes de trabajo en el sistema. Puede habilitar o deshabilitar las siguientes opciones:

*   *   Reasignar órdenes por cambio de disponibilidad, inactividad o revocación de licencia.
    *   Mantener la asignación de las órdenes manuales, aunque estas hayan expirado (de lo contrario, pasan a ser automáticas)
    *   Tomar la última ubicación reportada para la asignación de órdenes de trabajo (de lo contrario se tomará la ubicación asociada al perfil del especialista o la ubicación del establecimiento).

![]({{ site.baseurl }}/assets/images/image11.png)

*   Integración

Este parámetro complementa la integración con la herramienta de ASDK, ya que permite configurar la notificación de ejecución de órdenes de trabajo de AFLS a tareas en campo de ASDK.

Para las versiones más recientes de AFLS y ASDK se recomienda seleccionar el tipo de integración directa (Direct), que permite que AFLS y ASDK interactúen directamente. Para integrar por medio del bus de integración de WSO2, seleccionar la opción ESB.

Si escogió la integración directa, es necesario diligenciar los siguientes campos:

*   Usuario de integración y su contraseña
*   Si va a tener regla de alimentación de campo solución de un caso en ASDK a partir de una orden de trabajo de AFLS, puede colocar el nombre de sistema de un campo adicional de AFLS para este fin.
*   Homologación de estados ASDK: esta opción permite hacer pares de ID de estados de ASDK y AFLS cuando se van a notificar cambios de estado desde AFLS hacia ASDK.
*   Homologación de estados de AFLS desde ASDK: esta opción permite hacer pares de ID de estados de AFLS y ASDK cuando se van notificar cambios de estado desde ASDK hacia AFLS.


![]({{ site.baseurl }}/assets/images/image12.png)


### **Pestaña Configuración de Mapas**

En esta pestaña el administrador puede cambiar el proveedor de servicio para los mapas en la aplicación web, AssistMe y la aplicación móvil. Las opciones que se ofrecen dentro de la aplicación son:

| **Paquete** | **Por defecto en instalación** | **Tipo** | **Costo** | **Consideraciones** |
| --- | --- | --- | --- | --- |
| OpenStreet Maps + Nominatim | Si | Mapas open source y geocoding con open source | Ninguno | El geocoding (servicio de Nominatim) a comparación de los otros dos paquetes, tiene menor efectividad en los resultados. |
| OpenStreet Maps + ArcGIS | No | Mapas open source y geocoding que consume de servicio en nube de ArcGIS | Consumo de servicio de geocoding y geocoding inverso. Cada petición genera costo. | Para registrar el servicio, debe acceder a la página de Arcgis, registrar una aplicación y obtener el _Client Id_ y _Secret Id - API Key_ para consignarlo en AFLS. |
| Google Maps | No | Mapas y geocoding por Google Maps | Tanto el pintar mapas como el geocoding y geocoding inverso genera costo por cada petición | Para registrar el servicio, debe acceder a la página de Google Maps y obtener el _Secret Id - API Key_ (para paquetes BASIC) y si el paquete es PREMIUM también el C_lient Id._ |

![]({{ site.baseurl }}/assets/images/image13.png)


Al hacer un cambio de proveedor se pueden habilitar nuevos campos que varían dependiendo del proveedor elegido. Ejemplo: para Google se habilitan los campos de _Api Key_, _Client ID_, y Tipo de plan.

![]({{ site.baseurl }}/assets/images/image14.png)

| **Nota**: Luego de hacer el cambio de proveedor de mapas y guardar, es necesario que los usuarios inicien sesión nuevamente para visualizar el cambio en las aplicaciones web, móvil y AssistMe. |
| --- |

### **Importación GeoJSON**

En esta sección se configuran los atributos que se usarán del archivo GeoJson, cuando se importan localizaciones de la funcionalidad Capa Mapas.

![]({{ site.baseurl }}/assets/images/image15.png)

*   El campo **Nombre** puede tener múltiples atributos.
*   El campo **Descripción** puede tener múltiples atributos.
*   Los campos **Longitud** y **Latitud** solo permiten un atributo en su configuración.

De acuerdo al estándar si el archivo GeoJson cuenta con localizaciones que tengan el atributo “Geometry” este prevalecerá sobre los campos **Longitud** y **Latitud** aquí configurados.
