---
title: Proveedores Auxiliares
chapter: "configurando"
---

Son proveedores a los que se les puede asignar órdenes por restricción (órdenes cuya asignación se restringe por un criterio específico, ej. proveedor, especialista, fecha o jornada), estos proveedores no tienen especialistas y no pueden hacer gestión de órdenes desde AFLS.

Estos proveedores usan sus propios métodos para gestionar la orden y cuando la terminan de atender, el monitor web de dicho proveedor debe cerrar la orden cambiando su estado a Cancelada y seleccionando la razón: AFLS: ejecutado por proveedor.

Para AFLS las órdenes que procesen los proveedores Auxiliares son órdenes Canceladas, es decir que a los ojos de AFLS estas no han sido gestionadas bajo la lógica de AFLS.

![]({{ site.baseurl }}/assets/images/image86.png)

| **Nota**: Para que un proveedor quede configurado como proveedor auxiliar es necesario ir a la base de datos y cambiar el Tipo de Asignación para que sea nulo (Actualizar el AssinqType permitiendo NULL). |
| --- |
