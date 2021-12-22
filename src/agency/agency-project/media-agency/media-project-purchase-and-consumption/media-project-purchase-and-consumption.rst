.. |Boton Generar Orden de Venta| image:: resource/boton-generar-ov.png
.. |Gif Completar Orden de Compra| image:: resource/completar-oc.gif
.. |Crear checking| image:: resource/crear-checking-barra-herramientas.png
.. |Generar OV| image:: resource/generar-ov.png
.. |Gif Cabezal| image:: resource/gif-cabezal.gif
.. |Gif Crear Checking| image:: resource/gif-crear-checking.gif
.. |Gif Fase| image:: resource/gif-fase.gif
.. |Gif Generar OV| image:: resource/gif-generar-ov.gif
.. |Gif 1 Lineas Fase Proyecto| image:: resource/lineas-fase-del-proyecto-gif-1.gif
.. |Gif 2 Lineas Fase Proyecto| image:: resource/lineas-fase-del-proyecto-gif-2.gif
.. |Lineas Fase Proyecto Grilla| image:: resource/lineas-fase-del-proyecto-grilla.png
.. |Lineas Fase Proyecto| image:: resource/lineas-fase-del-proyecto.png
.. |Representacion Impresa| image:: resource/representacion-impresa-oc.png
.. |Visualiza Detalle| image:: resource/visualiza-detalle.png

Se entiende como “Compra y Consumo” cuando se desee realizar una compra
a un Medio en nombre de un Cliente y a su vez, en el mismo documento se
solicita también su emisión.

-  Proyecto

   -  Compra y Consumo en Canal 4 (FASE): Orden de Venta (Compra y
      Consumo)

      -  Línea con Producto a emitir
      -  Línea con Producto a emitir
      -  Línea con Producto a emitir

Para poder generar una Orden de Compra en nombre de un Cliente, primero
se deberá generar una Orden de Venta al Cliente. A continuación se
detallan los pasos a seguir para su operativa:

**Se comienza generando un Proyecto con nivel de línea “Fase”**

|Gif Cabezal|

**Una vez con el Proyecto creado se deberá crear una Fase definiendo el
Proveedor a quien se realizará la compra. Se deberá generar una Fase por
proveedor.**

|Gif Fase|

Luego de definir el Proveedor en la Fase, se deberá ir a la pestaña
“Línea de la Fase” donde se deberán definir los Productos a ser
Emitidos. En este caso tenemos dos opciones:

-  **Crear una línea por Producto: en este Caso se deberá definir en
   cada línea:**

   -  Fechas Desde: Fecha obligatoria a definir a partir de cuando es la
      Emisión
   -  Fecha Hasta: opcionalmente si desea definir un Hasta puede
      definirlo.
   -  Descripción: Datos extra que desea aclarar del Producto.
   -  Material
   -  Producto
   -  Precio
   -  Cantidad

-  **Crear una línea por Emisión de Producto: esta opción es más
   detallada definiendo una línea por Emisión y no las cantidades
   totales en una línea. Se deberán definir los mismos datos el punto a
   tantas emisiones como hayan.**

Algunas ayudas aplicables:

**Creando una Línea:** Las líneas se desplegarán en formato grilla, para
completarlas se deberá hacer click en el primer campo “Fecha Emisión”,
para avanzar al siguiente campo podrá hacerlo con la tecla “Intro”.

**Copiar Registro:** Una vez termine de completar una línea, se podrá
copiar la misma utilizando el botón de la barra de herramientas “Copiar
Registro”, una nueva línea será generada con la misma información, sólo
deberá modificar lo que corresponda (Fecha de Emisión, Programa, etc).

|Lineas Fase Proyecto|

|Lineas Fase Proyecto Grilla|

**Producto:** En cada una de las líneas se deberá definir el producto
que será Emitido. Para seleccionar el producto puede hacer click en el
buscador del campo, abriendo la ventana de Información del Producto. En
ella podrá realizar los filtros que considere necesario para encontrar
el Producto exacto a ser consumido. Dentro de los campos que puede
utilizar se recomienda definir el Proveedor del mismo que debería ser el
mismo a quién se está generando la Orden de Compra. A su vez, también se
podrá apoyar en el campo “Medio” y “Soporte” de los productos.

|Gif 1 Lineas Fase Proyecto|

|Gif 2 Lineas Fase Proyecto|

Una vez definido el Proveedor y los Productos en las líneas, se deberá
proceder a realizar una Orden de Venta del tipo “Orden de Venta (Compra
y Consumo)” desde el botón “Generar Orden de Venta”.

|Boton Generar Orden de Venta|

|Generar OV|

Al confirmar el proceso, una Orden de Venta será generada apareciendo el
número de la misma en la esquina inferior izquierda de la ventana. Para
acceder a ella se podrá utilizar el botón de “Visualiza Detalle” en la
Barra de Herramientas de la Ventana Proyecto.

|Visualiza Detalle|

La Orden generada también aparecerá en el campo Orden de Venta de la
Fase. Para acceder a ella podrá hacer click en el campo “Orden de
Venta”.

La Orden de Venta es el Documento que se Facturará al Cliente. La misma
tendrá definido a su vez, en el campo “Socio del Negocio Entrega
Directa” el Proveedor del Medio al cual se le generará una Orden de
Compra Espejo por los Medios correspondientes.

|Gif Generar OV|

La Orden de Venta se deberá Completar, de manera que se genere
automáticamente la Orden de Compra al Proveedor del Medio.

La Orden de Compra será del Tipo “Orden de Publicidad (Compra y
Consumo)” se generará en estado Borrador por lo que se deberá navegar a
la misma y Completarla para terminar con el proceso.

|Gif Completar Orden de Compra|

**Representación impresa:**

Desde la Ventana Orden de Compra se podrá obtener la Representación
Impresa de la misma que deberá ser enviada al Proveedor del Medio.

|Representacion Impresa|

**Checkin de la Pauta**

Luego de contar con una “Orden de Publicidad (Compra y Consumo)” en
Estado “Completo”, la misma se deberá confirmar mediante el Checking.

El checking se puede acceder desde los Procesos definidos en el Proyecto
de Medios que se estará verificando. Para ver los procesos del Proyecto
se deberá oprimir el botón de proceso ubicado en la Barra de
Herramientas seleccionando “Checking”.

|Crear checking|

Al realizar la búsqueda desde el SmarBrowser de Checkin, deberá
seleccionar las líneas que han sido emitidas, confirmando a su vez la
cantidad en cuestión de dicha emisión.

|Gif Crear checking|