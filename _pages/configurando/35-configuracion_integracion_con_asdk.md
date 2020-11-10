---
title: Configuración integración con ASDK
chapter: "configurando"
---

Esta funcionalidad tiene por objetivo integrar la mesa de servicio Aranda Service Desk (ASDK) y el sistema de organización de trabajo en campo (AFLS), para los clientes que posean ambas soluciones.

![]({{ site.baseurl }}/assets/images/image160.png)

_Ejemplo de configuración de integración con ASDK_

En este módulo se deben configurar los siguientes parámetros teniendo en cuenta el esquema de integración:

*   **Información de la conexión:** URL donde se encuentran alojados los servicios de integración expuestos por ASDK.
*   **Proyecto:** proyectos creados en ASDK, y disponibles para migrar.
*   **Fuente de Información:** permite definir la fuente para importar los clientes a Field Service.
*   **Fecha y hora de inicio:** fecha y hora en la cual se empieza el proceso de sincronización con los datos de ASDK (Compañías, clientes y despachadores o especialistas).
*   **Periodicidad:** De este campo depende cada cuanto tiempo se realiza la sincronización, si se elige una periodicidad diaria el sistema sincronizará todos los días a la hora programada en el campo fecha y hora de inicio.
*   **Estado:** indica si el proceso de sincronización se debe ejecutar o no.
*   **Actualizar ahora:** Es un botón de una sola ejecución, si este se presiona el proceso se iniciará al siguiente minuto.

### **Importando Compañías de ASDK a AFLS**

AFLS ejecuta una sincronización de las compañías que se encuentran en ASDK, los campos que se sincronizan son:

*   **Nombre de la compañía**
*   **Código de la compañía:** NIT de la compañía
*   **Nombre de contacto**
*   **Teléfono de contacto**
*   **Correo de contacto**
*   **Dirección:** estandarizada por el control de búsqueda de direcciones de Google.
*   **Estado:** define si el estado de la compañía activa o no.

![]({{ site.baseurl }}/assets/images/image161.png)

_Compañías de ASDK sincronizadas_

### **Importando Clientes de ASDK a AFLS**

AFLS ejecuta una sincronización de los clientes que se encuentran en ASDK, los campos que se sincronizan son:

*   **Nombre del cliente**
*   **Código del cliente:** número de identificación, NIT o Nombre de usuario (único) del cliente.
*   **Número de teléfono**
*   **Correo electrónico**
*   **Dirección:** estandarizada por el control de búsqueda de direcciones de Google.
*   **Estado:** define si el estado del cliente es activo o no.
*   **Servicios:** lista de servicios asociados al cliente.


![]({{ site.baseurl }}/assets/images/image162.png)

_Clientes de ASDK sincronizados_

### **Importando usuarios especialistas de ASDK como despachadores a AFLS** 


![]({{ site.baseurl }}/assets/images/image163.png)

_Usuarios web de ASDK sincronizados_

AFLS ejecuta una sincronización de los especialistas que se encuentran en ASDK, los campos que se sincronizan son:

*   **Nombre del usuario**
*   **Usuario:** código del usuario en ASDK.
*   **Correo electrónico:** email de contacto del especialista.
*   **Teléfono:** teléfono del especialista.
*   **Contraseña:** contraseña del especialista
*   **Estado:** define si el estado del especialista es activo o no.
*   **Rol:** se asigna el rol Despachador
