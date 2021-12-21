Proyecto de Agencia Creativa
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El Proyecto de Agencia Creativa será donde se deba ingresar todo pedido
realizado por el cliente. Desde el Proyecto se vinculará todos los
documentos que se haya generado a causa dicho Pedido a lo largo de toda
la organización (Solicitudes, Orden de Compra, Orden de Venta,
Cotizaciones, Tareas, etc) y será desde donde se defina la facturación a
realizar.

Cada Proyecto de Agencia podrá tener un Brief, este será la descripción
del servicio solicitado por el Cliente. Este se puede definir tanto en
un Campo Texto o bien adjuntando un archivo directo en el Proyecto.
Según el tamaño y complejidad del mismo, este podrá Fases, Tareas y
Solicitudes vinculadas separando así el trabajo a realizar.

A su vez, directo desde un Proyecto se podrá generar las Órdenes de
Venta definiendo lo que deberá facturar en relación al mismo.

Se deberán definir obligatoriamente en el cabezal los siguientes Campos:

Socio del Negocio Nombre Marca Categoría del Proyecto Nivel de línea
Fecha Inicio (creación) Fecha Límite Lista de Precios

Campos Automáticos:

Según la Lista de precio seleccionada:

Moneda

Según el Cliente seleccionado:

Término de pago. Almacén del Cliente: El almacén en un proyecto se
definirá de manera automática según el almacén que tenga definido el
Cliente en la pestaña Cliente ventana Socio del Negocio. Contrato de
Servicio: (En caso que el Cliente posea más de uno, el sistema tomará el
primer Contrato creado que encuentre, por lo que se sugiere en estos
casos elegir el Contrato en este campo de forma manual). Sello. Sello
Origen: Cuando se guarda un proyecto se realiza lo siguiente:

Según la Categoría de Proyecto se definirá el Sello Origen
correspondiente que tenga definido el contrato en sus “Partes del
Contrato”.

Según las siguientes Categoría de Proyecto se obtendrá el sello definido
para el siguiente tipo de empresa:

Categoría de Proyecto

Tipo de Empresa

Proyecto de Agencia

Agencia Creativa

Proyecto de Medios

Agencia de Medios

Proyecto RRPP

Agencia RRPP

Proyecto de Medios Digitales

Agencia de Medios Digitales

\*Si no se obtuvo sello de origen se lanza una excepción.

Según el usuario logueado en el sistema:

Agente Comercial: Este campo en el cabezal de un Proyecto tomará de
forma automática al usuario logueado en el sistema siempre que este
tenga el check de “Agente comercial” en “Y”, en la Pestaña “Empleado” de
la ventana “Socio de negocio”.