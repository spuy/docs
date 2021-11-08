.. |Boton Generar Orden de Venta| image:: resource/generate-sales-order-button.png
.. |Gif Completar Orden de Venta| image:: resource/gif-completar-orden-de-venta.gif
.. |Gif Generar Orden desde Fase| image:: resource/gif-generar-orden-desde-fase.gif
.. |Gif Cargar Lineas Fase del Proyecto 2| image:: resource/gif-lineas-fase-del-proyecto-2.gif
.. |Gif Cargar Lineas Fase del Proyecto| image:: resource/gif-lineas-fase-del-proyecto.gif
.. |Gif Completar Cabezal| image:: resource/header-gif.gif
.. |Lineas Fase del Proyecto Grilla| image:: resource/lineas-fase-del-proyecto-grilla.png
.. |Gif de la Fase| image:: resource/phase-gif.gif
.. |Proceso Generar Orden de Venta| image:: resource/proceso-generar-orden-de-venta.png
.. |Pestaña Lineas Fase del Proyecto| image:: resource/project-phase-lines-tab.png
.. |Documentos Relacionados| image:: resource/view-details-button.png

Se entiende como “Compra y Consumo” cuando se desee realizar una compra
a un Medio en nombre de un Cliente y a su vez, en el mismo documento se
solicita también su emisión.

Para poder generar una Orden de Compra en nombre de un Cliente, primero
se deberá generar una Orden de Venta al Cliente. A continuación se
detallan los pasos a seguir para su operativa:

**Se comienza generando un Proyecto con nivel de línea “Fase”**

|Gif Completar Cabezal|

Una vez con el Proyecto creado se deberá crear una Fase definiendo el
Proveedor a quien se realizará la compra. Se podrá generar tantas Fases
por proveedor se cuente.

|Gif de la Fase|

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

|Pestaña Lineas Fase del Proyecto|

|Lineas Fase del Proyecto Grilla|

**Producto:** En cada una de las líneas se deberá definir el producto
que será Emitido. Para seleccionar el producto puede hacer click en el
buscador del campo, abriendo la ventana de Información del Producto. En
ella podrá realizar los filtros que considere necesario para encontrar
el Producto exacto a ser consumido. Dentro de los campos que puede
utilizar se recomienda definir el Proveedor del mismo que debería ser el mismo a quién se está generando
la Orden de Compra. A su vez, también se podrá apoyar en el campo
“Medio” y “Soporte” de los productos.

|Gif Cargar Lineas Fase del Proyecto|

|Gif Cargar Lineas Fase del Proyecto 2|

Una vez definido el Proveedor y los Productos en las líneas, se deberá
proceder a realizar una Orden de Venta del tipo “Orden de Venta (Compra
y Consumo)” desde el botón “Generar Orden de Venta”.

|Boton Generar Orden de Venta|

|Proceso Generar Orden de Venta|

Al confirmar el proceso, una Orden de Venta será generada apareciendo el
número de la misma en la esquina inferior izquierda de la ventana. Para
acceder a ella se podrá utilizar el botón de “Visualiza Detalle” en la
Barra de Herramientas de la Ventana Proyecto.

|Documentos Relacionados|

La Orden generada también aparecerá en el campo Orden de Venta de la
Fase. Para acceder a ella podrá hacer click en el campo “Orden de
Venta”.

La Orden de Venta es el Documento que se Facturará al Cliente. La misma
tendrá definido a su vez, en el campo “Socio del Negocio Entrega
Directa” el Proveedor del Medio al cual se le generará una Orden de
Compra Espejo por los Medios correspondientes.

|Gif Generar Orden desde Fase|

La Orden de Venta se deberá Completar, de manera que se genere
automáticamente la Orden de Compra al Proveedor del Medio.

La Orden de Compra será del Tipo “Orden de Publicidad (Compra y
Consumo)” se generará en estado Borrador por lo que se deberá navegar a
la misma y Completarla para terminar con el proceso.

|Gif Completar Orden de Venta|

Desde la Ventana Orden de Compra se podrá obtener la Representación
Impresa de la misma que deberá ser enviada al Proveedor del Medio.