.. |Boton Generar Orden de Venta| image:: resources/generate-sales-order-button.png
.. |Numero de Orden de Venta| image:: resources/numero-ov-esquina-inferior-pantalla.png
.. |Crear Checking Barra de Herramientas| image:: resources/proceso-crear-checkin-barra-de-herramientas.png
.. |Proceso Generar Orden de Venta Consumo| image:: resources/proceso-generar-orden-de-venta-consumo.png
.. |Documentos Relacionados| image:: resources/visualiza-detalle-barra-de-herramientas.png

Compra paquete por importe

Se considera una Pre-Compra o Compra con Inversión cuando se realiza una
compra a un Medio en nombre de un Cliente para que la misma pueda ser
Consumida en un momento diferente a la Compra en cuestión.

El **Nivel de Línea “TAREA”** se deberá utilizar para realizar una
**Pre-Compra** en Nombre de un Cliente para su posterior **Consumo**.
Esto sería cuando sólo se realiza la compra en un medio de determinado
*Importe de Inversión*, sin especificar los Productos que se estarán
Consumiendo.

En este caso los niveles serán clasificados de la siguiente manera:

**FASE:** A Nivel de Fase se deberá definir el *Proveedor del Medio* que
se realizará la Compra. En caso de ser una Pre-Compra, también se deberá
definir en el Producto el correspondiente de “Inversión”. Importante
seleccionar un producto con la Tasa de Impuesto que corresponda (Iva
Básico o Exento).

**TAREAS:** Dentro de cada Fase se crearán las diferentes TAREAS por
cada Consumo que se consumirá la Inversión en cuestión. Los Productos se
deberán definir en las Líneas de Tarea, definiendo Producto, Fecha
Emisión, Descripción del Programa, Cantidad y Precio.

**Pre-Compra**
~~~~~~~~~~~~~~

Se comienza generando un Proyecto con nivel de línea “Tarea”:

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

.. only:: html

    .. figure:: resources/cabezal.gif

    Video 1. Cabezal

La inversión se debe definir desde una FASE del Proyecto de Medios.

En la misma, se deberá definir el Proveedor del Medio que se realizará
la Compra.

Para que el sistema permita elegir un Proveedor en el campo **Socio del
negocio Entrega Directa** es importante que el mismo:

-  Esté creado con la Organización con la que se encuentra logueado el
   usuario o con Organzación (*).
-  En la ventana Socio de negocio, en su cabezal debe tener marcado el
   check de "activo" y en la pestaña Proveedor el check de "Proveedor".

En el Campo de Producto se deberá definir el correspondiente de
“Inversión” junto con su correspondiente Importe en el campo “Total
Planeado”. Importante seleccionar un producto con la Tasa de Impuesto
que corresponda (Iva Básico o Exento).

Una vez definido el Proveedor, el Producto y el importe, se deberá
proceder a realizar una Orden de Venta del tipo “Orden de Venta
(Inversión)” desde el botón “Generar Orden de Venta”.

|Boton Generar Orden de Venta|

.. only:: html

    .. figure:: resources/gif-generar-orden-de-venta-inversion.gif

    Video 2. Generar Orden de Venta Inversión

Al confirmar el proceso, una Orden de Venta será generada apareciendo el
número de la misma en la esquina inferior izquierda de la ventana. Para
acceder a ella se podrá utilizar el botón de “Visualiza Detalle” en la
Barra de Herramientas de la Ventana Proyecto.

|Documentos Relacionados|

La Orden de Venta es el Documento que se Facturará al Cliente. La misma
tendrá definido a su vez, en el campo “Socio del Negocio Entrega
Directa” el Proveedor del Medio al cual se le generará una Orden de
Compra Espejo por los Medios correspondientes.

La Orden de Venta se deberá Completar, de manera que se genere
automáticamente la Orden de Compra al Proveedor del Medio. Para
Completar la Orden de Venta el sistema controlará que la misma tenga el
Check de “Aprobado por Cliente” en “Y” y que tenga adjunto la aprobación
en cuestión. Esta Orden de Compra se definirá en el campo “Orden
Enlazada”. La Orden de Compra se generará en estado Borrador a la espera
que el Departamento de Compras verifique la misma y la complete.

Desde la Orden de Compra se podrá obtener la Representación Impresa de
la misma que deberá ser enviada al Proveedor del Medio.

.. only:: html

    .. figure:: resources/gif-completar-ov-y-oc.gif

    Video 3. Completar Orden de Venta y Orden de Compra

**Consumo**
~~~~~~~~~~~

Desde la tarea se deberá crear una Orden de Venta del Tipo “Orden de
Venta (Consumo)” tomando los datos definidos en la misma y en sus
líneas. En las Líneas de la Tarea se deberá definir los Productos a ser
Consumidos, definiendo Fecha Emisión, Producto, Descripción del
Programa, Cantidad y Precio.

| Las líneas se desplegarán en formato grilla, para completarlas se
  puede ir definiendo uno a uno los campos utilizando “Intro” para pasar
  al siguiente campo. Una vez termine de completar una línea, se podrá
  copiar la misma utilizando el botón de la barra de herramientas
  “Copiar Registro”, una nueva línea será generada con la misma
  información, sólo deberá modificar lo que corresponda (Fecha de
  Emisión, Programa, etc).
| **Producto:** en cada una de las líneas se deberá definir el producto
  que será Emitido. Para seleccionar el producto puede hacer click en el
  buscador del campo, abriendo la ventana de Información del Producto.
  En ella podrá realizar los filtros que considere necesario para
  encontrar el Producto exacto a ser consumido. Dentro de los campos que
  puede utilizar se recomienda definir el Proveedor del mismo que
  debería ser el mismo a quién se está generando la Orden de Compra. A
  su vez, también se podrá apoyar en el campo “Medio” y “Soporte” de los
  productos.

.. only:: html

    .. figure:: resources/gif-consumo.gif

    Video 4. Consumo

Una vez definidas todas las líneas que se desea pautar, se deberá
proceder a realizar una Orden de Venta del tipo “Orden de Venta
(Consumo)” desde el botón “Generar Orden de Venta”.

|Proceso Generar Orden de Venta Consumo|

Al confirmar el proceso, una Orden de Venta será generada apareciendo el
número de la misma en la esquina inferior izquierda de la ventana. Para
acceder a ella se podrá utilizar el botón de “Visualiza Detalle” en la
Barra de Herramientas de la Ventana Proyecto.

|Numero de Orden de Venta|

|Documentos Relacionados|

La Orden de Venta (Consumo) se deberá Completar, de manera que se genere
automáticamente la Orden de Compra (Consumo) correspondiente. Una vez
con la Orden de Compra (Consumo) completa, la misma podrá ser enviada al
Proveedor del Medio en cuestión mediante su representación impresa.

Ambas consumirán sus Órdenes de Pre-Compra correspondientes (Orden de
Venta y Orden de Compra), quedando a la espera de ser confirmados
mediante el “Checking”.

.. only:: html

    .. figure:: resources/consumo-gif-linea-de-tarea.gif

    Video 5. Línea de Tarea

**Checking**
~~~~~~~~~~~~

Luego de contar con una “Orden de Publicidad (Consumo)” o una “Orden de
Publicidad (Compra y Consumo)” en Estado “Completo”, la misma se deberá
confirmar mediante el Checking.

El checking se puede acceder de dos maneras, una opción es directo desde
los Procesos definidos en el Proyecto de Medios que se estará
verificando. Para ver los procesos del Proyecto se deberá oprimir el
botón de proceso ubicado en la Barra de Herramientas seleccionando
“Checking”. Otra opción es directo desde el proceso Checkin ubicado en
el menú, en este caso se podrá filtrar según desee pudiendo ver más de
un proyecto a la vez para confirmar.

|Crear Checking Barra de Herramientas|

Al realizar la búsqueda desde el SmarBrowser de Checkin, deberá
seleccionar las líneas que han sido emitidas, confirmando a su vez la
cantidad en cuestión de dicha emisión.

En caso de querer confirmar la No Emisión se deberá seleccionar la
línea, definir la cantidad en 0.

En caso de que dicha Cantidad a su vez deberá Liberar Saldo de una
Pre-Compra además se deberá marcar el Check de “Liberar Saldo” en Y.

.. only:: html

    .. figure:: resources/gif-checking.gif

    Video 6. Checking