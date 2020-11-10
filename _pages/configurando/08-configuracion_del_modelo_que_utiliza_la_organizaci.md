---
title: Configuración del modelo que utiliza la organización
chapter: "configurando"
---

Un **modelo** reúne diversas características comunes a los servicios. En particular estas características incluyen:

*   Flujos de trabajo
*   Campos adicionales
*   Encuesta de satisfacción
*   Acuerdos de niveles de servicio

Una vez se define un modelo con estas características es posible utilizarlo dentro de los servicios, de esta manera todos los servicios compartirán las características.

### Creando un nuevo modelo

Al crear un nuevo modelo es posible definir la información básica y asociar la encuesta de satisfacción. Para facilitar su uso, Aranda FIELD SERVICE incluye varios elementos utilizados dentro del modelo para que no sean creados desde cero.

Una vez se crea un nuevo modelo, es posible modificar sus características a través del botón “**Editar Modelo**”.


![]({{ site.baseurl }}/assets/images/image38.png)


Al ingresar a la edición de un modelo se pueden observar en el menú de la izquierda tres secciones principales que se describen a continuación:

![]({{ site.baseurl }}/assets/images/image39.png)

### Configurando un flujo de trabajo para su organización

Cada organización ejecuta sus servicios de manera diferente. La configuración de los flujos de trabajo le permitirá adecuar la herramienta para cumplir con sus procedimientos particulares. El flujo de trabajo determina el ciclo de vida de las órdenes de trabajo. Cada actividad del flujo de trabajo será un paso que el especialista en campo debe llevar a cabo hasta finalizar un trabajo.

#### Estados

Dentro de un flujo de trabajo existen tres fases o estados principales que resumen los pasos de ejecución de la orden:

*   **Abierta:** corresponden a órdenes que aún no han sido asignadas a un especialista, son las órdenes recién creadas o que deben ser reagendadas para su ejecución.
*   **En proceso:** esta fase incluye todos los pasos que debe ejecutar el especialista en campo para llevar a cabo una tarea. Los subestados definidos dentro de este estado guiarán al especialista paso por paso. Dentro de este estado puede crear los subestados que desee, sin embargo, es importante mantener la simplicidad del proceso.
*   **Ejecutada:** la orden de trabajo finaliza en este estado, con dos posibles subestados: ejecutada o cancelada.

#### Subestados

El especialista en campo recibe las órdenes en el estado “En proceso” y es aquí donde los subestados le sirven de guía para la ejecución de una orden. El ciclo de vida de las órdenes se rige por los subestados y sus transiciones.

Al crear un subestado, el administrador puede configurar diferentes opciones que permiten adecuar el modelo al proceso de negocio:

**Información Básica:** Esta información incluye el nombre del estado y el mensaje de ayuda. Este mensaje es sumamente importante ya que indica a los usuarios (especialistas y en algunos casos monitores) lo que debe hacer en cada una de las actividades.

**Roles**: Esta sección define quién tiene permiso de modificar un caso (respecto al flujo de trabajo), es decir, cuáles usuarios pueden cambiar el estado de un caso.

**Cronómetros**: Esta sección permite que los casos que estén en este subestado lleven la cuenta del tiempo que tardan. Tan pronto un caso entra en este subestado los cronómetros marcados comienzan a contar tiempo. Al salir del estado los cronómetros se detienen, así es posible llevar la cuenta del tiempo que tardan entre diferentes actividades.

**Costos**: Esta sección le permite a la aplicación saber en cuáles estados se debe llevar la cuenta del tiempo invertido por el especialista, o la distancia recorrida con el fin de calcular los costos de ejecución y desplazamiento.

![]({{ site.baseurl }}/assets/images/image40.png)

#### Transiciones

Otra parte importante del flujo de trabajo corresponde a las transiciones que se representan con flechas o caminos que van de un subestado a otro. Las transiciones tienen un contexto adicional y es que se convierten en “botones” que podrán utilizar los especialistas en campo o los agentes en la web para mover una orden de trabajo de un estado a otro.

Al configurar una transición, el nombre es importante, ya que con este dato se identificarán los botones en la consola móvil que utilizan los especialistas para la ejecución. De esta manera la recomendación es que los nombres de las transiciones sean verbos infinitivos, por ejemplo, para pasar de un estado “En proceso” a otro “Escalado”, la transición debería llamarse “Escalar”. Esta palabra, “Escalar” será utilizada en la aplicación móvil como una acción que pueden tomar los especialistas en campo para modificar la orden.

![]({{ site.baseurl }}/assets/images/image41.png)

Dentro de las transiciones también es posible crear un conjunto de razones. Esta información se solicitará al especialista en campo cuando cambie el estado de una orden de trabajo.

#### Elementos especiales del flujo de trabajo

Dentro del flujo de trabajo existen algunos elementos que requieren especial atención. Están enumerados a continuación:

**Transiciones por defecto**

Dentro de un flujo de trabajo, un estado puede tener varias transiciones de salida. Por ejemplo, un estado de aprobación puede tener la transición “Aprobar” y otra transición “No Aprobar”. El flujo de trabajo de Aranda FIELD SERVICE requiere que se marque una de las transiciones como transición por defecto. Al hacer esto, esta transición será la principal y se mostrará como un botón en la consola del especialista. Las demás transiciones aparecerán en el menú de Acciones. Las transiciones por defecto están marcadas con una estrella.

![]({{ site.baseurl }}/assets/images/image42.png)

**Subestado Sin Programar**

Este sub estado es propio del sistema. Cualquier transición que llegue a este subestado hará que el motor se encargue automáticamente de seleccionar una nueva fecha y hora, así como un nuevo especialista que pueda atender la orden.

**Subestado Programada**

Este sub estado es propio del sistema. Una orden puede pasar del estado “sin programar” a estar “programada” a través de dos eventos: a través del motor de asignación, donde la herramienta programa la orden, o a través de un agendamiento manual. En ambos casos la condición que debe cumplir una orden de trabajo para pasar de un estado a otro es tener una fecha planeada de ejecución.

**Subestado Cancelado**

Este subestado es propio al sistema. Corresponde a un estado terminal. Cuando la orden llega a este estado indica que no se cumplió el trabajo.

**Subestado Ejecutado**

Este subestado es propio del sistema. Es un estado terminal que indica que la orden se finalizó correctamente.

**Subestado de cumplimiento de cita**

Teniendo en cuenta que una orden de trabajo puede incluir múltiples actividades (subestados), y algunas de estas actividades pueden llevarse a cabo antes de tener contacto con el cliente (desplazamiento, preparación, etc), existe una actividad que indica que se inicia la labor en campo en el lugar especificado. Este estado tiene una marca en forma de estrella y corresponde al primer subestado en el que corre el tiempo de ejecución.

#### Modificando el flujo de trabajo

El administrador de la herramienta puede modificar el flujo de trabajo configurado por defecto incluyendo nuevos subestados y transiciones. Para crear una nueva actividad utilice el botón . El nuevo subestado se creará en el nivel inmediatamente inferior. Para crear una transición se debe arrastrar y soltar el cursor desde la actividad inicial hasta la final.

#### Modificando los acuerdos dentro de los modelos

Generalmente los niveles de acuerdo de servicio dentro de las organizaciones son comunes a los diferentes modelos, sin embargo, puede darse el caso de que algunos modelos requieran comportamientos singulares, por ejemplo, que los acuerdos de tiempo sean diferentes.

El módulo de acuerdos de niveles de servicio despliega todos los ANS dentro de un modelo configurado para la herramienta.

![]({{ site.baseurl }}/assets/images/image44.png)

Si es necesario, el administrador podrá entrar al detalle de los acuerdos de tiempo y sobrescribir los valores para todos los casos que utilicen el modelo. Es importante tener en cuenta que los casos creados utilizarán el detalle del modelo, si no se ha especificado de otra forma. En esta página también es posible revertir los cambios para que los casos del modelo utilicen los valores prestablecidos.

![]({{ site.baseurl }}/assets/images/image45.png)

### Configurando los campos adicionales de un modelo

Adicionalmente un modelo incluye un conjunto de campos adicionales que corresponden a información para cada una de las órdenes de trabajo creadas.

En esta pantalla se puede definir la información que se debe solicitar para cada orden, y definir los permisos y la obligatoriedad de cada campo.

![]({{ site.baseurl }}/assets/images/image46.png)

La creación de un campo adicional está dividida en dos partes. Primero, la información básica dónde es posible crear la etiqueta, el texto de ayuda y seleccionar uno de los tipos de campo adicional: texto simple, párrafo, numérico, fecha, y opciones.

Cuando un campo adicional está activo se observa como parte del concepto (orden de trabajo).

La segunda parte corresponde a las opciones avanzadas. En la pestaña de detalles se puede configurar un nombre y una descripción. Esta información corresponde a la información técnica que podrá utilizarse más adelante en la integración con otros sistemas.

![]({{ site.baseurl }}/assets/images/image47.png)

En la sección de permisos puede definir:

*   Cuáles roles pueden ver la información de los campos adicionales, ya sea monitor y/o despachador en la aplicación web, y/o especialista en la aplicación móvil.
*   Adicionalmente puede configurar estos permisos en cada uno de los estados.

![]({{ site.baseurl }}/assets/images/image48.png)

Una vez configurada la información común de los modelos, se podrán asociar a los servicios de su organización.
