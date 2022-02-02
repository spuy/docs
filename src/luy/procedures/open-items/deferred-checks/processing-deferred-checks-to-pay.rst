.. |Proceso Cheque Diferido por Pagar| image:: resources/payment-deferred-check-process.png

**Gestión Avanzada de Cheques Diferidos**
=========================================

**Cheque Diferido por Pagar**
-----------------------------

Tanto la Factura como el Cheque Diferido a Pagar son Documentos por
Pagar, que se diferenciar por el grado de certeza del Pago o por
aspectos jurídicos (con  diferente forma y con diferentes atributos).

Un Cheque Diferido por Pagar (C_Invoice), es un Documento por Pagar tipo
 “Factura” que tiene el mismo signo de la Factura por Pagar que se
quiere cancelar.  Es decir es una Factura Cheque Diferido.

Es por eso que para Cancelar la Factura Común mediante un Documento de
Pago Diferido, se genera automáticamente por detrás un “Pago Diferido”,
esto no es otra cosa que una “Nota de Crédito Diferida”.

Este Documento de Pago Diferido tendrá 1 sola línea con el mismo “Cargo”
definido que el que tiene el Cheque Diferido por Pagar de manera que el
mismo se netee entre sí y reclasifique el Documento por Pagar (Abierto)
a Documento por Pagar (cheque de pago Diferido)

El Pago Diferido (Nota de Crédito Diferida) es el que se asignará con el
Documento por Pagar que se está cancelando, reduciendo así su saldo,
tanto Contablemente como su Saldo Abierto.

Este paso será solamente para cancelar el Saldo Abierto del Documento
por Pagar ya que Contablemente como se puede apreciar, al ser Nota de
Crédito descuenta el importe de la misma de la cuenta de Cuentas por
Pagar.

**Proceso de Cheque Diferido a Pagar**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|Proceso Cheque Diferido por Pagar|

Asignaciones:
-------------

Asignación de Documento por Pagar y Cheque Diferido por Pagar
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El Pago Diferido generado por el cheque es el que será Asignado con el
Documento por Pagar que está cancelando. Dicha asignación se realizará
cuando se asigne el Pago Diferido con el Documento por Pagar. Esta
asignación puede ser automática desde el recibo o bien realizarse luego
desde el proceso de Asignación de Recibos.

**Asignación de Cheque Diferido por Pagar y Pago Diferido**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El Cheque Diferido por Pagar será asignado cuando el mismo sea
Cancelado, esto será cuando se realice el Débito del mismo en el Banco o
en su Vencimiento (la empresa decide si el procedimiento de generar el
Débito correspondiente al cheque sea Automático o manual).

Asientos Contables:

| Ejemplo (pago mixto):
| Documento por Pagar: 7700

Pago Contado: 4700

Pago Cheque Dif.  por Pagar 3000

**Documentos por Pagar**

74100-Impuestos  D 700

51400-Inventario  D 7.000

21100 - Cuentas por Pagar H 7.700

**Pago (contado)**

21300 Pagos seleccionados D 4.700

11110 - Cheques en Tránsito  H 4.700

**Cheque Diferido**

**Emisión de Cheque**

Cuenta Puente Diferidos  D 3.000

Documentos por pagar Diferidos  H  3.000

**Pago Diferido**

**Nota de Crédito Automática**

21100 Cuentas por Pagar D 3.000

Cuenta Puente Diferidos   H  3.000

**Consulta de Asignación Factura/Cheque diferido**

21100 - Cuentas por Pagar D    4.700      (por el Pago Contado)

21300 - Cuentas Seleccionadas H   4.700 (por el Pago Contado)

21100 - Cuentas por Pagar D 3.000           (Por el Pago Diferido)

21100 - Cuentas por Pagar  H 3.000          (Por el Pago Diferido)

**Consulta de Asignación Cheque diferido/Débito**

21100 - Cuentas por Pagar D 3.000          por el Débito

21100 - Cuentas por Pagar  H 3.000

**Pagos no Comerciales con Cheques Diferidos**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si se requiere emitir y pagar una transacción no comercial, es decir que
no corresponde al pago de Documentos por Pagar de proveedores, se deberá
utilizar la ventana de Recibo de Pago y desde allí, emitir el Cheque
Diferido por Pagar  imputándolo al cargo que requiera.

Si no se desea utilizar el Recibo de Pago con la numeración correlativa
del documento oficial, utilice la numeración correlativa del sistema o
ingrese la numeración manual que desee.