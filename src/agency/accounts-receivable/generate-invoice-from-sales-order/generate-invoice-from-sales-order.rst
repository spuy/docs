.. |Campo CFE Billing Criteria| image:: resource/cfe-billing-criteria.png
.. |Pestaña Linea de Factura CFE| image:: resource/cfe-invoice-line-tab.png
.. |Campo Detalle en Factura| image:: resource/detail-in-invoice.png
.. |Generar Factura desde Línea de Orden Sb| image:: resource/generate-invoice-from-sales-order-process.png
.. |Proceso Generar Lineas de Factura para CFE| image:: resource/process-generate-invoice-lines-for-cfe.png
.. |Opciones de Facturación| image:: resource/opciones-de-facturacion.png
.. |Error Varios Terminos de Pago| image:: resource/error-varios-terminos-de-pago.png
.. |Ordenes de Venta Grilla| image:: resource/ov-grilla.png

Generar Factura desde Orden de Venta
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Las órdenes de venta generadas en el sistema pueden ser facturadas de
manera ágil y masiva utilizando el proceso **"Generar Factura desde
Línea de Orden".**

**Precondiciones**
^^^^^^^^^^^^^^^^^^

Para poder facturar una Orden de Venta, esta tiene que estar

-  Estado: Completo
-  Con el check “Permite Facturar” = SI
-  Regla de Facturación: Inmediata

En este proceso se podrá aplicar el filtro que desee para encontrar
aquellas líneas de ordenes que cumplan con dichas condiciones.

Dentro de los filtros a definir podemos encontrar:

|Generar Factura desde Línea de Orden Sb|

**Generar Factura**
-------------------

Y comenzaremos la búsqueda, a continuación obtendremos las líneas de
Orden de Venta que cumplan con la condición.

Procederemos a marcar el check que esté como primer columna para todas
las líneas que se deseen facturar.

En la parte inferior de esta ventana veremos distintas opciones
utilizadas al momento de generar la factura:

**Fecha de Facturación:** (Obligatorio) Fecha de facturación del
Documento por Cobrar generado.

**Acción en el Documento:**

-  **Preparar:** Si desea ver la Factura antes de completarla puede
   seleccionar la opción "Preparar" de manera de que se genere el
   documento primero en estado "En Proceso" y así poder verificar que
   todo esté correctamente definido. En este caso al generar el proceso
   se creará la factura con un Nro de Borrador "DR-2222" y podrá acceder
   a la misma tanto desde el proyecto u Orden desde donde se generó,
   cómo también buscando en la ventana "Documentos por Cobrar" según el
   Nro de borrador presentado abajo a la izquieda del Proceso.
-  **Completar:** Si uno está seguro de la información que estará
   facturando también puede seleccionar la acción "Completar" de manera
   de que se completen automáticamente las facturas al correr el
   proceso.

**Organización de la Transacción:** Es la organización con la que se
está logeado, necesario cuando el documento pasa a estado completo,
debido a que no se pueden realizar envíos a DGI de un documento con una
organización que no es con la que se está logueado.

**Criterio de Agrupación:** Según el Criterio de Agrupación definido es
la forma en que el sistema agrupará las líneas de órdenes en una
Factura, estas puede ser por:

-  **Socio del Negocio:** Generará una Factura con todas las líneas de
   Orden de por cada Socio del Negocio diferente.
-  **Contrato:** Generará una factura por cada Contrato establecido en
   las Órdenes de Venta, agrupará en esa factura todas las Órdenes que
   pertenezcan al mismo contrato.
-  **Proyecto:** Si la línea tiene definido el Proyecto utilizará esta
   referencia y en caso de no tenerlo establecido tomará el de su
   respectiva orden (puede ser que en una misma agrupación algunas
   líneas tengan Proyecto relacionado y a la vez otras que se tenga que
   obtener de su respectivo Cabezal), Siguiendo este criterio se
   generará un Documentos por Cobrar por proyecto diferente.
-  **Orden:** La agrupación que agrupa menos registros, se generará cada
   factura agrupando líneas de Orden por su respectivo cabezal.
-  **Impuesto:** Agrupará por Impuesto definido en cada Línea de Orden
   seleccionada. Se generará una factura por tipo de impuesto
   encontrado. El criterio de agrupación no es por % (Ej: 22%, 10% o
   0%), sino por diferente Tipo de Impuesto.
-  **Orden de Compra Cliente:** Si se selecciona este Criterio de
   Facturación se generará una Factura por cada Número de la Orden de
   Compra Cliente que se encuentre en todas las líneas seleccionadas.
   Este criterio de agrupación incluye además la clasificación según
   diferentes clientes.

**¿Por qué motivo puede no referenciarse un Proyecto en una factura?**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

El Proyecto se referenciará en la factura siempre que el criterio de
agrupación que se haya elegido para agrupar las lineas de Orden al
correr el proceso Generar factura desde línea de Orden haya sido
“Proyecto”.

Por ejemplo se puede tener N proyectos por Contrato pero solo Un
Contrato por cada proyecto. Por lo que si se agrupa por Contrato, como
las lineas de orden pueden ser de varios proyectos, al generar la
factura no establece el campo de Proyecto en el cabezal.

|Opciones de Facturación|

Respecto al Tipo de documento, el sistema controlará si el Socio del
Negocio a quien se está facturando tiene definido un RUT o una Cédula y
le generará una e-Factura o un e-ticket según corresponda.

**Criterios Implícitos**

Además de los criterios definidos manualmente, siempre se agrupará una
factura teniendo en cuenta que deben ser:

-  Para un mismo Socio de Negocio
-  Una misma localización para ese Socio de Negocio (Su dirección de
   facturación seleccionada)
-  Misma Moneda: Tener en cuenta que es la moneda a Facturar de la Orden
   de Venta, por si la misma hace un cruzamiento de monedas.

Estos son requerimientos obligatorios por la naturaleza del CFE.

Nota: En el caso que se defina la opción para Completar el documento se
ejecutará automáticamente el proceso Generar líneas de CFE.

**Criterio de Facturación (definición de Líneas de Factura)**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El **Criterio de Facturación** permite generar líneas más resumidas de
la información que se está Facturando, adaptando así según la necesidad
de cliente, definiendo en ellas la información exacta que el cliente
desea recibir en cada "Concepto de Facturación".

Debido a que el ERP puede tener una definición muy detallada de las
"líneas de las órdenes" presentando en ellas un concepto de
**Servicios**, **Cantidades** y **Precios** que si bien puede ser de
gran utilidad para la gestión interna y el control de sus Costos, en
ciertas ocasiones a los clientes no les interesa contar con tal detalle.

De esta manera, el **Criterio de Facturación** que tendrá cada Factura
será criterio que se va a utilizar para generar las líneas que se
detallarán en el CFE (e-Factura o e-Ticket).

Facturación de Honorarios en Línea independiente
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

El Criterio de Facturación aplicará siempre para las líneas de
"Inversión" del cliente, agrupando según el criterio seleccionado. Esto
quiere decir que el criterio nunca aplicará la agrupación para aquellas
líneas que correspondan a Honorarios Variables calculados en un Proyecto
o Fase de Proyecto, estos siempre irán en una línea aparte detallando
que son Honorarios.

**Proceso automático**
^^^^^^^^^^^^^^^^^^^^^^

**Proceso automático**
^^^^^^^^^^^^^^^^^^^^^^

El Criterio que se definirá en cada factura será el que cada cliente
tenga definido en su ficha, pudiendo ser por Línea (normal), por
Proyecto, por Fase de Proyecto o por Factura. .

Al utilizar como criterio "Proyecto", el sistema agrupará en una línea a
todas las líneas del Proyecto y definirá la descripción de la misma
según el campo "Detalle Factura" ubicado en el Proyecto en cuestión.

|Campo Detalle en Factura|

|Pestaña Linea de Factura CFE|

**\*Siempre se agrupan las líneas que no sean Honorarios ya que éstos
van en otra línea a parte.**

Si utilizamos como criterio "Fase del proyecto", el sistema agrupará
todas las líneas de una fase en una línea, por lo que la factura tendrá
tantas líneas de CFE como fases se estén facturando. En la descripción
de cada línea se obtendrá  según el campo "Detalle Factura" ubicado en
cada Fase del Proyecto en cuestión.

Este proceso se puede realizar de forma automática o manual.

**Proceso Manual**
^^^^^^^^^^^^^^^^^^

Si para alguna factura en especial se desea utilizar un Criterio de
Facturación diferente al que tiene definido el Cliente por defecto, se
podrá generar el mismo desde el cabezal de la factura.

Si se desea realizar el proceso de forma manual se deben seguir los
siguientes pasos luego de generar la factura:

Elegir en el campo "Criterio de Facturación" ubicado en la Factutra el
Nuevo Criterio que se desee aplicar.

|Campo CFE Billing Criteria|

Luego procederemos a correr el proceso "Generar líneas de factura para
CFE", seleccionando la opción desde los Procesos asociados a la Factura.

|Proceso Generar Lineas de Factura para CFE|

**Posibles Errores Controlados**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Varios Términos de Pago en las Órdenes de Venta seleccionadas**

Cuando se están facturando en una misma factura varias Órdenes de Venta
que tienen diferentes Términos de Pago no permitirá generar una única
factura y figurará el siguiente mensaje de Error:

|Error Varios Terminos de Pago|

Esto se debe a que no puede determinar que término de pago se desea
definir en la Factura a Generar.

**Solución: Para solucionarlo lo ideal sería abrir en la ventana de
“Órdenes de Venta” todas las Ordenes de venta que se están intentando
facturar Varios Términos de Pago en las Órdenes de Venta
seleccionadas.**

| **Ver las mismas en formato “Grilla” para identificar qué Orden de
  Venta tiene un Término de Pago diferente.**
| **Para modificarlo deberá Rectivar la Orden, modificar el Término de
  Pago y luego completarla nuevamente.**

|Ordenes de Venta Grilla|

**Varios Agentes Comerciales definidos en las Órdenes de Venta**

En principio el proceso definirá el Agente Comercial en la Factura según
el Agente que esté definido en la Orden de Venta en cuestión.

En caso de que existan diferentes Agentes Comerciales definidos en las
Órdenes de Venta el proceso tomará el Agente Comercial definido en el
Socio del Negocio.

Si no tiene ninguno definido en el Socio del Negocio tomará el Agente
Comercial definido en las Ordenes de Venta. Si estos son diferentes dará
un error.






