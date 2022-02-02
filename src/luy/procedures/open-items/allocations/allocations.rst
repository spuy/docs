.. |Asignacion Factura Pago Cobro 1| image:: resources/asignacion-factura-pago-cobro-1.png
.. |Asignacion Factura Pago Cobro 2| image:: resources/asignacion-factura-pago-cobro-2.png
.. |Asignacion Factura Pago Cobro 3| image:: resources/asignacion-factura-pago-cobro-3.png
.. |Asignacion Factura Pago Cobro 4| image:: resources/asignacion-factura-pago-cobro-4.png
.. |Asignacion Factura Pago Cobro 5| image:: resources/asignacion-factura-pago-cobro-5.png
.. |Asignacion Factura Pago Cobro 6| image:: resources/asignacion-factura-pago-cobro-6.png
.. |Asignacion Cliente Proveedor| image:: resources/asignacion-cliente-proveedor.png
.. |Asignacion Pago Cobro| image:: resources/asignacion-pago-cobro.png
.. |Asignacion de Pagos| image:: resources/asignacion-pagos.png
.. |Asignacion por Deposito| image:: resources/asignacion-por-deposito.png
.. |DxP| image:: resources/dxp.png
.. |Emision Cheque| image:: resources/emision-cheque.png
.. |Nota de Credito Automatica| image:: resources/nota-de-credito-automatica.png
.. |Pago Contado| image:: resources/pago-contado.png

**Asignación**
==============

Es un documento que vincula dos o más elementos, de forma que se pueda
tener una trazabilidad perfecta a causa de esta vinculación.

**Tipos de Documentos de Asignación**
-------------------------------------

-  Asignación Factura - Pago/Cobro
-  Asignación Factura - Nota de Crédito
-  Asignación por Anulación
-  Asignación por Documento Diferido

**Asignación Factura Pago/Cobro**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+---------------------------+---------------+
|                           |Pago/Cobro     |
|Documento por Cobrar/Pagar |               |
|                           |Cargo Contable |
+---------------------------+---------------+

Asignación entre Facturas a Pagar y Pagos o entre Facturas a Cobrar y
Cobros.

La Asignación disminuirá el Saldo Pendiente del Documento por
Pagar/Cobrar.

|Asignacion Factura Pago Cobro 1|

|Asignacion Factura Pago Cobro 2|

|Asignacion Factura Pago Cobro 3|

|Asignacion Factura Pago Cobro 4|

|Asignacion Factura Pago Cobro 5|

|Asignacion Factura Pago Cobro 6|

**Asignación por Nota de Crédito**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+----------------------------+-----------------------------------------------+
|Documentos por Cobrar/Pagar |Nota de CRédito de Documentos por Cobrar/Pagar |
+----------------------------+-----------------------------------------------+

|Asignacion Nota de Credito 1|

|Asignacion Nota de Credito 2|

|Asignacion Nota de Credito 3|

Asignación por Anulación
~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+-----------------------------------------+
|Documentos por Cobrar/Pagar |Anulación de Documentos por Cobrar/Pagar |
+----------------------------+-----------------------------------------+

En cada oportunidad que un documento completo es Anulado el Sistema crea
el Reverso de ese mismo documento y lo asigna mediante este documento.

.. only:: html

    .. figure:: resources/asignacion-por-anulacion.gif

    Video 1. Asignación por Anulación

Asignación por Documento Diferido
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+---------------------------+---------------------------------------------------------------+
|                           |Cobro Diferido/Pago Diferido                                   |
|Documento por Cobrar/Pagar |                                                               |
|                           |Contra Documento quye genera el Pago/Cobro con Cheque DIferido |              |
+---------------------------+---------------------------------------------------------------+

Es la que se realiza cuando el Documento a  Pagar / Cobrar se sustituye
por un Documento por Pagar/Cobrar de otro Tipo Diferido (por ejemplo una
Factura se paga o cobra con un Documentos Cheque de Pago/Cobro
Diferido).

De esta manera el saldo del Documento por Pagar/Cobrar  original
(Facturas) disminuye por la sustitución con otro Documento de diferente
Tipo y características, como por ejemplo un Cheque Diferido por Pagar.

El Documento por Pagar (Factura de Proveedor) se sustituye por otro
Documento a  Pagar (Cheque Diferido por Pagar).

El Saldo Abierto del Documento por Pagar que se estará Cancelando con el
documento Pago Diferido.

El Documento por Cobrar (Factura Cliente) se sustituye por otro
Documento a  Cobrar (Cheque Diferido a Cobrar)

.. only:: html

    .. figure:: resources/asignacion-por-documento-diferido.gif

    Video 2. Asignación por Documento Diferido

Asignación Automática de Nota de Crédito
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se utilizan los campos en pestaña "CFE Referidos" de "Total Abierto" y
"Total Asignado". Estos campos, cuando las líneas en esta pestaña son
generadas mediante un proceso, se cargan de la siguiente manera:

- Desde botón "Crear Desde" (desde Factura) en cabezal de documento: se
setea el importe abierto de la factura y el importe total asignado,
según el total de líneas agregadas a la nota de crédito.

- Desde proceso "Generar Nota de Crédito desde Factura" (en el ícono del
engranaje en cabezal de factura): se setea el importe abierto de la
factura y el importe total asignado, según el total de líneas agregadas
a la nota de crédito.

- Desde proceso "Generar Nota de Crédito desde Devolución": se setea el
importe abierto de la factura y el importe total asignado se toma del
importe total del cabezal de RMA (Autorización de Devolución)

Si se genera una línea manualmente en pestaña "CFE Referidos", también
se carga el importe abierto, y el importe asignado con igual valor.

Luego, al momento de completarse la NC, se genera la asignación
automática creando una línea por la NC, y las N líneas por cada una de
las facturas presentes en los CFE Referidos, por el importe asignado
indicado en cada una.

Al momento de ejecutarse este proceso, se verifica que cada una de las
facturas siga teniendo un saldo abierto igual o mayor al indicado en la
NC, y también que la moneda sea la misma de la NC, de lo contrario se
retorna mensaje de error indicando el motivo.

CONTROLES:

- No se permite guardar una línea en CFE referidos, si hay una factura
seleccionada y al menos uno de los campos de importe (total abierto o
total asignado) es menor o igual a cero.

- No se permite completar la NC si el monto total de facturas asignadas
es mayor al importe de la NC. En el caso que sea menor, entonces la NC
se asigna con el importe de las facturas asignadas, quedando un
pendiente en la NC.

En ningún caso se toman en cuenta las lineas de CFE referidos que no
tienen factura seleccionada.

**Documentos por Pagar**
------------------------

+----------------------------------+--------------+--------------+
|Cuenta Contable                   |DEBE          |HABER         |
+==================================+==============+==============+
|74100 - Tax e xpense              |700,00        | 0.00         |
+----------------------------------+--------------+--------------+
|51400 - Inventory Clearing        |4000,00       |0.00          |
+----------------------------------+--------------+--------------+
|51400 - Inventory Clearing        |3000,00       |0.00          |
+----------------------------------+--------------+--------------+
|21100 - Accounts Payable Trade    |0.00          |7.700,00      |
+----------------------------------+--------------+--------------+

**Pago (contado)**
------------------

+=============================+============+==========+
|21300 - Payment Selection    |4.700,00    |0.00      |
+-----------------------------+------------+----------+
|11110 - Checking In-Transfer |143.459,81  |4.700,00  |
+-----------------------------+------------+----------+

**Cheque Diferido**
-------------------

**Emisión de Cheque**


+=============================+===========+==========+
|Cuenta Puente Diferidos      |3.000,00   |0.00      |
+-----------------------------+-----------+----------+
|Documentos a Pagar Diferidos |0.00       |3.000,00  |
+-----------------------------+-----------+----------+


**Nota de Crédito Automática.**

+===============================+===================+
|21100 - Accounts Payable Trade |3.000,00 |0.00     |
+-------------------------------+---------+---------+
|Cuenta Puente Diferidos        |0.00     |3.000,00 |
+-------------------------------+---------+---------+


**Asignación de Pagos**
-----------------------

+===============================+======+=====+
|21100 - Accounts Payable Trade |500   |0.00 |
+-------------------------------+------+-----+
|21300 - Payment Selection      |0.00  |500  |
+-------------------------------+------+-----+

**Asignación por Depósito**
~~~~~~~~~~~~~~~~~~~~~~~~~~~

+---------------------------------+--------------------------------+
|Cheque diferido por cobrar/pagar |Depósito Cheque / Débito Cheque |
+---------------------------------+--------------------------------+


**Asignación Cliente Proveedor**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+--------------------+---------------------+
|                    |Documento por cobrar |
|Documento por pagar |                     |                     |
|                    |Cargo                |
+--------------------+---------------------+

**Asignación Pago Cobro**
~~~~~~~~~~~~~~~~~~~~~~~~~

+------+------+
|      |Cobro |
|Pago  |      |
|      |Cargo |
+------+------+