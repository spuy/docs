.. |Completar OV Inversion| image:: resource/completar-ov-a-facturar.gif
.. |Generar OV Inversion| image:: resource/generar-ov-a-facturar.gif
.. |Generar OV Inventario| image:: resource/generar-ov-inventario.png
.. |Gif Cabezal| image:: resource/gif-cabezal.gif
.. |Gif Completar OC| image:: resource/gif-completar-oc.gif
.. |Gif Crear Checking| image:: resource/gif-crear-checking.gif
.. |Gif Fase| image:: resource/gif-fase.gif
.. |Gif Generar OV Inventario| image:: resource/gif-generar-ov-inventario.gif
.. |Gif Linea de Tarea| image:: resource/gif-linea-de-tarea.gif
.. |Gif Tarea| image:: resource/gif-tarea.gif
.. |Proceso Crear Checking| image:: resource/proceso-crear-checking.png
.. |Gif 1 Consumo de Inventario| image:: resource/consumo-de-inventario-gif-1.gif
.. |Gif 2 Consumo de Inventario| image:: resource/consumo-de-inventario-gif-2.gif
.. |Gif 3 Consumo de Inventario| image:: resource/consumo-de-inventario-gif-3.gif

Creación de un “Proyecto de Medios” donde realizará la Inversión del
cliente. La idea es que dentro de un mismo Proyecto se controle lo
**Ordenado con lo Facturado**. Como se manejan diferentes criterios de
Facturación que de recepción de Productos a inventario, se decide
manejar mediante la FASE la “\ *Inversión”*, y mediante la Tarea y
líneas de la Tarea la *“Recepción”*.

**Compra Inventario**
~~~~~~~~~~~~~~~~~~~~~

**Se comienza generando un Proyecto con nivel de línea “Tarea”**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-  En la ventana de Proyecto de Medios se deberá crear un proyecto
   definiendo:

   -  **Cliente**
   -  **Marca del Cliente**
   -  **Nombre del Proyecto**
   -  **Nivel de Línea:** Tarea
   -  **Lista de Precios**
   -  **Campos Automáticos:** Según el Cliente seleccionado se cargarán
      los siguientes Campos:

      -  Contrato de Servicio
      -  Sello
      -  Sello Origen

-  Término de pago
-  Almacén del cliente

|Gif Cabezal|

**Definición del Proveedor de la Inversión:**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**En la Fase del Proyecto se deberá definir el Proveedor donde se realizará la inversión**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para que el sistema permita elegir un Proveedor en el campo **Socio del
negocio Entrega Directa** es importante que el mismo:

-  Esté creado con la Organización con la que se encuentra logueado el
   usuario o con Organización (*).
-  En la ventana Socio de negocio, en su cabezal debe tener marcado el
   check de "activo" y en la pestaña Proveedor el check de "Proveedor".

|Gif Fase|

**Orden de Inventario:**
~~~~~~~~~~~~~~~~~~~~~~~~

| Desde la Tarea se crea la **Orden de Inventario** donde se definirán
  los Productos a comprar. El proceso de generar una Compra de
  Inventario deberá comenzar realizando la definición de todos los
  Productos que se estarán adquiriendo para consumir en el futuro dentro
  las líneas de una Tarea de Proyecto.  
| Para ello se deberá detallar cada uno de los productos que se estarán
  adquiriendo en “Líneas de Tarea” con el Precio acordado de los mismos.
  Una vez se tengan todos los Productos definidos en Líneas de Tarea, se
  podrá ver el TOTAL en el campo “Total Planeado” de la Tarea.

|Gif Tarea|

|Gif Linea de Tarea|

Una vez confirmado el importe se deberá generar la “Orden de Inventario”
desde el Proceso “Generar Orden”. IMPORTANTE la Orden de Inventario es
una orden de Sub tipo de OV “Propuesta”.

|Generar OV Inventario|

|Gif Generar OV Inventario|

La Orden de Venta se definirá en el Campo Orden de Venta de la Tarea. Se
debe navegar hacia la Orden de Venta para poder Completarla.

Al Completar la Orden de Venta se generará la Orden de Compra al
Proveedor definido. Se podrá navegar a la Orden de Venta desde el campo
“Orden enlazada” desde la Orden de Venta.

|Gif Completar OC|

Al completar la Orden de Compra de tipo de documento “Orden de Compra
Inventario”, los Productos definidos en ella se habrán recepcionado
automáticamente en el Almacén definido en el Proyecto. Ésta Almacén
debería ser el Almacén definido para el Cliente por el cual se compró
los productos.

**Reporte “Detalle de Almacenamiento Simple”**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se podrá confirmar el ingreso de los productos al almacén mediante el
reporte de “Detalle de Almacenamiento Simple” seleccionando el Almacén
en cuestión.

**Orden de Venta y Orden de Compra a Facturar**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Desde la **FASE**  se deberá crear una “Orden de Venta Inversión”, ésta
será realizada según el Producto genérico definido en la FASE (Ej:
Inversión TV) y por el Importe Total. Este producto será el que
finalmente será facturado, tanto al Cliente como por el Proveedor.

Para el caso que una Orden de Venta u Orden de Compra deba ser Facturada
en diferentes “Cuotas” se deberá:

-  **Producto a Facturar:** Como la facturación no se realizará producto
   a Producto que fue solicitado, se debe definir un Producto Genérico
   que será el que finalmente será facturado.
-  **Descripción:** Escribir en la Descripción de la FASE cómo se desea
   que sea Facturado para que Administración se entere.
-  **Cantidad:** Además se deberá definir en Cantidad las diferentes
   Cuotas que tendrá. Además en el Campo “Cantidad” de la Fase se deberá
   definir la Cantidad de Cuotas que se desea Facturar, ya sea por el
   Medio o al Cliente. Ver que como Precio Unitario se deberá visualizar
   el importe de cada una de las cuotas a ser Facturado.

|Generar OV Inversion|

|Completar OV Inversion|

**Consumo de Inventario**
~~~~~~~~~~~~~~~~~~~~~~~~~

Cuando un cliente cuente con inventario previamente comprado y se quiera
consumir parte del mismo, se deberá crear directamente una Orden de
Venta del tipo “Orden de Pauta”. En la misma se deberá definir el *Proveedor* y el *Almacén* del Cliente definiendo “Entrega
Directa” = N. En las líneas se deberá definir cada uno de los Productos
que se desean emitir así como su Cantidad correspondiente. Esta Orden de
Pauta una vez se confirme es la que generará la Entrega del Inventario
bajándolo de stock.

-  Pendiente de definir: Ver cómo se quiere gestionar el Precio en las
   Órdenes de Pauta.
-  Esta Orden de Pauta no será facturada nunca ya que se entiende que ya
   se facturó mediante la Orden de Venta Inversión que se compró el
   Inventario.

|Gif 1 Consumo de Inventario|

|Gif 2 Consumo de Inventario|

|Gif 3 Consumo de Inventario|

**Checking**
~~~~~~~~~~~~

|Proceso Crear Checking|

|Gif Crear Checking|
