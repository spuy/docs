**Perdidas y Ganancias por Diferencias de Cambio Realizada**
============================================================

Una Pérdida o Ganancia se genera cuando usted tiene transacciones de
Cuenta por Pagar o Cuenta por Cobrar en una moneda diferente a la de su
contabilidad y hay un cambio en la tasa de conversión de la moneda entre
las fechas de realización de la transacción mediante el Documento por
pagar/Cobrar y su correspondiente pago/Cobro.

Estas diferencias de cambio pueden ser:

-  Diferencias de Cambio realizadas
-  Diferencias de Cambio no realizadas

Solop ERP gestiona tanto las diferencias de cambio realizadas como las
no realizadas.

Diferencia de Cambio Realizada
------------------------------

Es la determinada entre la fecha de origen del activo o pasivo en moneda
extranjera y la fecha en que se recibe o efectúa el abono parcial o
total.

La Pérdida o Ganancia realizada se genera con base en los Pagos y Cobros
efectivamente realizados. La Pérdida o Ganancia realizada se genera
cuando:

-  se realiza un pago en una moneda diferente a su moneda contable.
-  la tasa de conversión de moneda es diferente en el momento del pago a
   la que tenía cuando el documento fue aplicado.

Ejemplo Diferencia de Cambio Realizada y No Realizada
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Por ejemplo, suponga que una factura de Proveedor se generó por 100 USD
con una tasa de conversión de 30. Esto es convertido a la moneda
contable dando un valor de 3.000 UYU.

**Diferencia No Realizada**

Si posteriormente la Tasa de Conversión es de 32, cuando se ejecuta la
conversión a la moneda contable se obtiene un valor de 3.200 UYU. Una
pérdida de 20 UYU es Aplicada a la cuenta de Pérdida no Realizada. Esto
es realizado con el Proceso de “Ganancia Pérdida Ganancia”

**Diferencia Realizada**

Posteriormente, cuando la factura es pagada. En ese momento la Tasa de
Conversión es de 27 lo que da un valor de 2.700 UYU. Cuando se aplica el
pago la pérdida no realizada se restaura y una Ganancia Realizada de 300
UYU es aplicada.

El sistema advierte en el momento de realizar el asiento contable
correspondiente a la Asignación (entre el Documento por Pagar/Cobrar y
el Pago/Cobro) si existe variación en la Tasa de cambio entre la fecha
de Factura y la fecha del Cobro (lo mismo sucede con el Pago). En caso
de existir diferencia aplicará en ese momento el ajuste correspondiente
a la Diferencia de Cambio Realizada correspondiente.

En el caso que esa diferencia de cambio realizada esté gravada por
impuestos de venta o compra, Solop ERP realizará el cargo
correspondiente a los impuestos por Pagar o Impuestos por Cobrar.