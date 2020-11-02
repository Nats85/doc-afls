---
title: Configuración de la integración con terceros
chapter: "configurando"
---

AFLS puede integrarse con el sistema que el cliente desee, siempre que se haga un desarrollo que cumpla con el contrato definido en algunas interfaces contenidas en un archivo .dll suministrado por Aranda.

Para que AFLS pueda sincronizar información con otro sistema, se deben configurar los parámetros en el módulo **Integración &gt;** **Otras aplicaciones** en la pestaña **Sincronización de información**.

[]({{ site.baseurl }}/assets/images/image189.png)

_Ejemplo de configuración de integración con terceros_

Campos a diligenciar:

*   **Información del componente:** archivo .dll con clases que implementan las interfaces definidas en la dll proveída por Aranda.
*   **Sigla del componente de sincronización:** sigla con la que se marcarán los datos sincronizados.
*   **Fecha y hora de inicio:** fecha y hora en la cual se empieza el proceso de sincronización con los datos del otro sistema (Compañías, clientes y despachadores o especialistas).
*   **Periodicidad:** frecuencia de la sincronización
*   **Estado:** indica si el proceso de sincronización se debe ejecutar o no.
*   **Actualizar ahora:** es un botón de una sola ejecución, que inicia el proceso al siguiente minuto.

### **Importando compañías de terceros a AFLS** {#importando-compa-as-de-terceros-a-afls}

AFLS ejecuta una sincronización de las compañías que se encuentran en otros sistemas por medio del componente ya configurado, los campos que se sincronizan son:

*   **Nombre de la compañía**
*   **Código de la compañía:** NIT o identificación de la compañía.
*   **Nombre de contacto**
*   **Teléfono de contacto**
*   **Email de contacto**
*   **Dirección:** estandarizada por el control de búsqueda de direcciones de Google.

[]({{ site.baseurl }}/assets/images/image190.png)

_Compañías de terceros sincronizadas_

### **Importando clientes de terceros a AFLS** {#importando-clientes-de-terceros-a-afls}

AFLS ejecuta una sincronización de las compañías que se encuentran en otros sistemas por medio del componente ya configurado, los campos que se sincronizan son:

*   **Nombre del cliente**
*   **Código del cliente:** cédula o identificación del cliente.
*   **Teléfono**
*   **Email de contacto**
*   **Compañía:** nombre de la compañía asociada al cliente.
*   **Dirección:** estandarizada por el control de búsqueda de direcciones de Google.
*   **Estado:** define si el estado del cliente es activo o no.
*   **Servicios:** lista de servicios asociados al cliente.


[]({{ site.baseurl }}/assets/images/image191.png)

_Clientes de terceros sincronizados_
