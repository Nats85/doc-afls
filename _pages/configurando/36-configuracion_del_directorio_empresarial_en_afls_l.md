---
title: Configuración del directorio empresarial en AFLS (LDAP)
chapter: "configurando"
---

Esta funcionalidad le permite configurar la conexión con un directorio empresarial ya existente, para que la información de los empleados esté sincronizada con la base de datos de AFLS. También es posible importar un usuario del directorio empresarial y asignarle un rol dentro de la aplicación, y así, el administrador evita la tarea de diligenciar todo el formulario al crear los roles.

Para esto, es necesario activar primero la opción de LDAP y configurar la información básica de conexión al directorio empresarial. Luego ingrese los filtros, que se tendrán en cuenta al momento de sincronizar la información y son de carácter obligatorio.

![]({{ site.baseurl }}/assets/images/image164.png)

_Pantalla de configuración de conexión al directorio empresarial_

La sincronización de datos puede ser manual (inmediata) o se puede programar para sincronización automática mensual, semanal o diaria, trayendo las actualizaciones de los datos de los usuarios previamente sincronizados y/o nuevos. Se debe tener en cuenta que la fecha y hora de inicio para programar la sincronización debe ser mayor o igual a la fecha y hora actual.

![]({{ site.baseurl }}/assets/images/image165.png)

_Pestaña para configurar la sincronización de datos con el directorio empresarial_

En la pestaña **Unificación de campos**, se configuran los campos necesarios para la sincronización. Los campos obligatorios son: usuario, nombre, correo electrónico, teléfono, y nombre de grupos. El sistema no permite guardar la información sin diligenciar estos campos obligatorios. Los demás campos son opcionales, para el caso en el que el usuario desee sincronizar información adicional.


![]({{ site.baseurl }}/assets/images/image166.png)

_Pestaña para configurar el mapeo de campos con el directorio empresarial_

### **Importando usuarios de LDAP como usuarios web en AFLS**

Una vez configurada la integración del directorio empresarial y sincronizada la información con la base de datos de AFLS, el sistema le permitirá importar usuarios a la aplicación. Ingrese a **Administración** **&gt; Usuarios &gt; Usuarios Web**, luego haga clic en el menú desplegable al lado del botón **Nuevo** y allí se presentará la opción **Importar usuarios LDAP**, en este caso, usuarios Web.


![]({{ site.baseurl }}/assets/images/image167.png)

_Opción para importar usuarios_

Al seleccionar la opción de importar, el sistema despliega el formulario de importación, donde el administrador puede seleccionar el rol o roles que tendrán los usuarios a importar. También puede asociar los usuarios que va a importar a un grupo web.


![]({{ site.baseurl }}/assets/images/image168.png)

_Pantalla inicial para importación de usuarios_

En el área de texto, digite el nombre del usuario o usuarios a importar y que previamente fueron sincronizados de su directorio empresarial. Al momento de digitar el nombre del usuario, el sistema desplegará una lista con las coincidencias encontradas.


![]({{ site.baseurl }}/assets/images/image169.png)

_Lista de usuarios disponibles para importar_

Aquí es posible seleccionar la cantidad de usuarios que desee. Estos usuarios seleccionados se irán presentando en la zona **Usuarios Asociados** y tendrá la posibilidad de removerlos de la lista en caso de error.


![]({{ site.baseurl }}/assets/images/image170.png)

_Lista de usuarios a importar como usuarios web a AFLS y Rol definido_

Los usuarios que se encuentren en la zona de usuarios asociados se importarán a la aplicación tomando el rol o roles que se les configure.

Luego de hacer clic en **Importar**, el sistema mostrará un mensaje de éxito de la importación.

### **Importando usuarios de LDAP como Usuarios Móvil en AFLS**

AFLS también permite crear usuarios móviles importándolos desde el directorio empresarial. Una vez configurada la integración del directorio empresarial y sincronizada la información con la base de datos de AFLS, ingrese a **Administración** **&gt; Usuarios &gt; Usuarios Móvil**, luego haga clic en el menú desplegable al lado del botón **Nuevo**, allí encontrará la opción **Importar usuarios LDAP**, en este caso, usuarios Móvil.


![]({{ site.baseurl }}/assets/images/image171.png)

_Opción de importación_

![]({{ site.baseurl }}/assets/images/image172.png)


_Pantalla importación (LDAP)_

![]({{ site.baseurl }}/assets/images/image173.png)

_Lista de usuarios a importar (LDAP)_

Una vez importados, estos usuarios se verán en la lista con la etiqueta LDAP y algunos de sus campos no serán modificables en AFLS, pues esta información solo se modifica directamente en el directorio empresarial.

![]({{ site.baseurl }}/assets/images/image174.png)

_Usuarios importados_

Al igual que en la creación de usuarios móviles, los usuarios LDAP que se importan toman la configuración existente, es decir, toman la disponibilidad, habilidades, grupos móviles asociados, cargo de especialista y medio de transporte que ya están configurados para los usuarios móvil.

### **Importando Grupos de LDAP como Grupos Web en AFLS**

Una vez configurada la integración del directorio empresarial y sincronizada la información con la base de datos de AFLS, el sistema le permitirá importar grupos a la aplicación.

Ingrese a **Administración &gt; Grupos &gt; Grupos Web**, luego haga clic en el menú desplegable al lado del botón **Nuevo**, allí encontrará la opción **Importar grupos LDAP**, en este caso, grupos Web.

![]({{ site.baseurl }}/assets/images/image175.png)

_Opción para importar Grupos LDAP_

| **Nota**: Para importar grupos LDAP, debe configurarse el filtro de grupos en el módulo de LDAP. |
| --- |


![]({{ site.baseurl }}/assets/images/image176.png)

_Pantalla inicial para importación de Grupos_

Al hacer clic en **Importar**, el sistema despliega el formulario de importación. Aquí el administrador puede seleccionar el rol o roles que tendrán los grupos a importar.

![]({{ site.baseurl }}/assets/images/image177.png)

_Lista de grupos a importar como usuarios web a AFLS y rol definido_

En el área de texto, digite el nombre del usuario o usuarios a importar y que previamente fueron sincronizados del directorio empresarial. Al momento de digitar el nombre del usuario, el sistema desplegará una lista con las coincidencias encontradas.

![]({{ site.baseurl }}/assets/images/image178.png)

_Zona de grupos disponibles para importar_

Aquí es posible seleccionar la cantidad de grupos que desee. Estos grupos seleccionados se irán presentando en la zona **Usuarios Asociados** y tendrá la posibilidad de remover los grupos que no desee en la lista.

Los grupos que se encuentren en la zona de usuarios asociados se importarán a la aplicación tomando el rol o roles que se le configure. Los campos **Nombre del grupo** y **Descripción** estarán bloqueados.

![]({{ site.baseurl }}/assets/images/image179.png)

_Mensaje de importación_

Si el grupo LDAP a importar incluye usuarios en el directorio empresarial, estos usuarios se importarán con el grupo y heredarán los roles configurados además de tener la característica de ser usuarios Web. Se listarán en la pestaña **Usuarios**.

![]({{ site.baseurl }}/assets/images/image180.png)

_Usuarios importados como usuarios web con rol definido que estaban incluidos en el grupo del directorio empresarial_

| **Nota**: Si se remueve un usuario de la lista de usuarios a importar, el sistema no lo tendrá en cuenta para importarlo a AFLS. Si uno de los usuarios relacionados al grupo ya ha sido previamente importado, este se relacionará al grupo correspondiente al momento de importarlo. |
| --- |

### **Importando Grupos de LDAP como Grupos Móvil en AFLS** 

Una vez configurada la integración del directorio empresarial y sincronizada la información con la base de datos de AFLS, el sistema le permitirá importar grupos a la aplicación.

Ingrese a **Administración &gt; Grupos &gt; Grupos Móvil**, luego haga clic en el menú desplegable al lado del botón **Nuevo**, allí encontrará la opción **Importar grupos LDAP**, en este caso, grupos Móvil.

![]({{ site.baseurl }}/assets/images/image181.png)

_Opción para importar Grupos LDAP_

| **Nota**: Para importar grupos LDAP, debe configurarse el filtro de grupos en el módulo de LDAP. |
| --- |

![]({{ site.baseurl }}/assets/images/image182.png)

_Pantalla inicial para importación de Grupos_

Al hacer clic en **Importar**, el sistema despliega el formulario de importación. Aquí el administrador puede seleccionar la disponibilidad, habilidades, cargo, medio de transporte y servicios asociados que tendrán los grupos a importar.

![]({{ site.baseurl }}/assets/images/image183.png)

_Configuración Habilidades (Pestaña de habilidades)_

![]({{ site.baseurl }}/assets/images/image184.png)

_Configuración de Disponibilidad_ (Pestaña de Disponibilidades)

En el área de texto, digite el nombre del grupo o grupos a importar y que previamente fueron sincronizados del directorio empresarial. Al momento de digitar el nombre del grupo, el sistema desplegará una lista con las coincidencias encontradas.

![]({{ site.baseurl }}/assets/images/image185.png)

_Lista de grupos disponibles para importar_

Aquí es posible seleccionar la cantidad de grupos que desee. Estos grupos seleccionados se irán presentando en la zona **Usuarios Asociados** y tendrá la posibilidad de remover los grupos que no desee en la lista.

![]({{ site.baseurl }}/assets/images/image186.png)

_Zona de grupos disponibles para importar_

Los grupos que se encuentren en la zona de usuarios asociados, se importarán a la aplicación tomando las propiedades de los parámetros que se le configure. Los campos **Nombre del grupo** y **Descripción** estarán bloqueados.

![]({{ site.baseurl }}/assets/images/image187.png)

_Mensaje de importación_

Si el grupo LDAP a importar incluye usuarios en el directorio empresarial, estos usuarios se importarán con el grupo y heredarán las propiedades de los parámetros que se le configure, además de tener la característica de ser usuarios Móvil.

![]({{ site.baseurl }}/assets/images/image188.png)

_Usuarios importados como usuarios web con rol definido que estaban incluidos en el grupo del directorio empresarial_

| **Nota**: Si se remueve un usuario de la lista de usuarios a importar, el sistema no lo tendrá en cuenta para importarlo a AFLS. Si uno de los usuarios relacionados al grupo ya ha sido previamente importado, este se relacionará al grupo correspondiente al momento de importarlo. |
| --- |
