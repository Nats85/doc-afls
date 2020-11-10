---
title: Configuración de usuario
chapter: "configurando"
---

La gestión completa de una orden de trabajo requiere definir usuarios con roles específicos quienes se encargarán de administrar las diferentes etapas del ciclo de vida de una orden de trabajo. Estos usuarios operan ya sea desde la consola web o desde la aplicación móvil de AFLS.

### Usuarios Web

Los Usuarios web definidos para la atención oportuna de un servicio son:

*   **Administrador**: Será el responsable de la configuración y definición del servicio, los repuestos a utilizar, compañías, clientes, medios de transporte, cargos, usuarios y organizaciones.
*   **Despachador**: Será responsable de la creación de la orden de trabajo asociada al servicio, asignación y programación de especialistas para la atención de la orden y asignación de los repuestos previamente configurados.
*   **Monitor**: Será responsable de supervisar los desplazamientos del especialista en campo y hacer seguimiento a la evolución del proceso del servicio.
*   **Gestor de inventario:** Podrá administrar artículos, medidas, ubicaciones, realizar movimientos de entrada o salida, transferencias entre bodegas y ver los reportes de inventario por sedes.

La creación de los usuarios con rol **Administrador**, **Monitor**, **Despachador** o **Gestor** se debe realizar por la opción de usuarios web, a estos usuarios se les puede asociar un grupo web si se requiere:

*   Para cada uno de los usuarios configurados con el rol de administrador, despachador, monitor y gestor, se debe establecer el nombre de cada **usuario** y en su información de contacto ingresar los datos de contraseña, correo electrónico, teléfono y estado.

![]({{ site.baseurl }}/assets/images/image89)

Los usuarios configurados con el rol de administrador, despachador, monitor y gestor no tendrán habilitada la opción de **Medios de Transporte**; esta solo está disponible para el usuario con rol de especialista en campo. Todos los usuarios definidos para la gestión del servicio quedarán en **estado** “Activo”, para la atención de la orden de trabajo.

### Usuarios Móvil

Para adicionar un usuario web con rol **especialista**, haga clic en el botón **Nuevo** de la categoría **Usuarios Móvil** y llene los campos de la pestaña **Información** al lado derecho de la pantalla.

*   A cada usuario con rol de especialista en campo se le asociará un **cargo** yun **proveedor** que han sido configurados previamente, y también una sede de inventario (este último campo no es obligatorio).

![]({{ site.baseurl }}/assets/images/image90.png)

#### Grupos móvil asociados al usuario

Cada usuario con el rol de especialista en campo podrá estar asociado a diferentes grupos según sus características y condiciones para la prestación del servicio.

![]({{ site.baseurl }}/assets/images/image91.png)

#### Disponibilidad del usuario

En esta pestaña podrá configurar la disponibilidad de tiempo de cada especialista para la atención del servicio.

![]({{ site.baseurl }}/assets/images/image92.png)

| **Nota:** Si el usuario se asocia a un grupo móvil que ya tiene una disponibilidad configurada, el usuario la heredará de dicho grupo. La disponibilidad heredada se visualiza de en color gris (ver convenciones). |
| --- |

#### Habilidades del usuario

En esta pestaña se configuran las habilidades específicas para cada especialista en campo.

![]({{ site.baseurl }}/assets/images/image93.png)

| **Nota:** Si el usuario se asocia a un grupo móvil que ya tiene habilidades configuradas, el usuario las heredará de dicho grupo. Las habilidades heredadas se visualizan de manera diferente (ver convenciones) |
| --- |
