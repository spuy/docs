**Diferencias de Cambio sobre Documentos por Cobrar o Pagar**
=============================================================

Si su compañía usa diferentes monedas como monedas base, es posible que
deba re expresar los saldos de las cuentas de la moneda base a cualquier
moneda extranjera configurada para su uso en contabilidad. Esta
operación se llama Conversión de Monedas.

Una cuenta de Pérdida o Ganancia se genera cuando usted tiene
transacciones de Cuenta por Pagar o Cuenta por Cobrar en una moneda
diferente a la de su contabilidad y hay un cambio en la tasa de
conversión de la moneda entre las fechas de realización de la
transacción mediante el Documento por pagar/Cobrar y su correspondiente
pago/Cobro.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

La Diferencia de Cambio Realizada es la determinada entre la fecha de
origen del activo o pasivo en moneda extranjera y la fecha en que se
recibe o efectúa el abono parcial o total.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

La Pérdida o Ganancia realizada se genera con base en los Pagos y Cobros
ya realizados. La Pérdida o Ganancia realizada se genera cuando se hace
un pago en una moneda diferente a su moneda contable y la tasa de
conversión de moneda es diferente en el momento del pago a la que tenía
cuando el documento fue aplicado.

Por ejemplo, suponga que una factura de Proveedor se generó por 100.00
USD con una tasa de conversión de 30. Esto es convertido a la moneda
contable dando un valor de 3.000 UYU.

| **Diferencia No Realizada**
| Si posteriormente la Tasa de Conversión es de 32, cuando se ejecuta la
  conversión a la moneda contable se obtiene un valor de 3.200 UYU. Una
  pérdida de 20 UYU es Aplicada a la cuenta de Pérdida no Realizada.
  Esto es realizado con el Proceso de “Ganancia Pérdida Ganancia”

| **Diferencia Realizada**
| Posteriormente, cuando la factura es pagada. En ese momento la Tasa de
  Conversión es de 27 lo que da un valor de 2.700 UYU. Cuando se aplica
  el pago la pérdida no realizada se restaura y una Ganancia Realizada
  de 300 UYU es aplicada.

El sistema advierte en el momento de realizar el asiento contable
correspondiente a la Asignación (entre el Documento por Pagar/Cobrar y
el Pago/Cobro) si existe variación en la Tasa de cambio entre la fecha
de Factura y la fecha del Cobro (lo mismo sucede con el Pago). En caso
de existir diferencia aplicará en ese momento el ajuste correspondiente
a la Diferencia de Cambio Realizada correspondiente.

El Documentos que presentan las conversiones y realizan estos cálculos
es la Asignación

**Asignación**
--------------

El documento “Asignación” es el responsable de realizar el cálculo de
Diferencia de Cambio Realizada al momento de cancelar el saldo abierto
de los Documentos (DxC, DxP, Pago, Cobro, Pago Diferido, Cobro
Diferido).

El Ajuste se realiza siempre según la fecha de la Asignación realizada.
A dicha fecha se comparará los Montos Fuentes de las transacciones que
se estén cancelando según el % de la misma (Pueden ser asignaciones
parciales donde se calculará el % correspondiente o bien asignaciones
totales) por la Tasa de Cambio de Tipo “Spot” de a la fecha de la
Asignación contra el importe que dicho documento fue originalmente
contabilizado en su creación.

Muy importante considerar que el Ajuste se realizará llevando los Montos
Fuentes a la TASA DE CAMBIO DE LA ASIGNACIÓN, no necesariamente siendo
la misma que la del Pago/Cobro con quién se esté asignando.

**Asientos Contables Documentos por Diferencia de Cambio**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Documento por Cobrar (Moneda USD)**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Cuenta

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Fecha

.. raw:: html

   </td>

.. raw:: html

   <td>

Moneda

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Tasa

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

21610 - IVA Ventas

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

11.957,02

.. raw:: html

   </td>

.. raw:: html

   <td>

23/04/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

277,20

.. raw:: html

   </td>

.. raw:: html

   <td>

43,135

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

41000 - Ventas Productos

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

54.350,10

.. raw:: html

   </td>

.. raw:: html

   <td>

23/04/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

60.00

.. raw:: html

   </td>

.. raw:: html

   <td>

43,135

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

12110 - Cuentas por Cobrar Comerciales

.. raw:: html

   </td>

.. raw:: html

   <td>

66.307,12

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

23/04/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

1.537,20

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

43,135

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Cobro (Moneda USD)**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Cuenta

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Fecha

.. raw:: html

   </td>

.. raw:: html

   <td>

Moneda

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Tasa

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

11110 - Cheques en Tránsito

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

1.537,20

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

11130 - Cheques Depósitos No Asignados

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

1.537,20

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Asignación**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Cuenta

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Fecha

.. raw:: html

   </td>

.. raw:: html

   <td>

Moneda

.. raw:: html

   </td>

.. raw:: html

   <td>

Débito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Crédito Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Tasa

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

21620 - Impuestos Contabilizados

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

18,85

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

UYU

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

80540 - Ganancia Realizada

.. raw:: html

   </td>

.. raw:: html

   <td>

18,85

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

UYU

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

11130 - Cheques Depósitos No Asignados

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

1,537.20

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

12110 - Cuentas por Cobrar Comerciales

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

1,537.20

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

12110 - Cuentas por Cobrar Comerciales

.. raw:: html

   </td>

.. raw:: html

   <td>

104,53

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

UYU

.. raw:: html

   </td>

.. raw:: html

   <td>

104.53

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

1.00

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

80540 - Ganancia Realizada

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

104,53

.. raw:: html

   </td>

.. raw:: html

   <td>

28/05/2020

.. raw:: html

   </td>

.. raw:: html

   <td>

UYU

.. raw:: html

   </td>

.. raw:: html

   <td>

0.00

.. raw:: html

   </td>

.. raw:: html

   <td>

104.53

.. raw:: html

   </td>

.. raw:: html

   <td>

1.00

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Explicación del Ajuste**
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Documento

.. raw:: html

   </td>

.. raw:: html

   <td>

Importe Fuente

.. raw:: html

   </td>

.. raw:: html

   <td>

Moneda

.. raw:: html

   </td>

.. raw:: html

   <td>

Tasa de Cambio Asignación

.. raw:: html

   </td>

.. raw:: html

   <td>

Importe Actualizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Importe Contabilizado

.. raw:: html

   </td>

.. raw:: html

   <td>

Actualización

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

DxC

.. raw:: html

   </td>

.. raw:: html

   <td>

1.537,20

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

66.307,12

.. raw:: html

   </td>

.. raw:: html

   <td>

104,53

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Impuesto

.. raw:: html

   </td>

.. raw:: html

   <td>

277,20

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   <td>

11.975,87

.. raw:: html

   </td>

.. raw:: html

   <td>

11.957,02

.. raw:: html

   </td>

.. raw:: html

   <td>

18,85

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Cobro

.. raw:: html

   </td>

.. raw:: html

   <td>

1.537,20

.. raw:: html

   </td>

.. raw:: html

   <td>

USD

.. raw:: html

   </td>

.. raw:: html

   <td>

43,203

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

66.411,65

.. raw:: html

   </td>

.. raw:: html

   <td>

0,00

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

**Ajuste del Impuesto**

Para los Ajustes de Impuesto se tomará la Cuenta Contable definida en el
Campo “Impuesto Pagado” o “Impuesto Acreditado según sea Documentos por
Cobrar o Documentos por Pagar correspondientemente.

.. image:: https://lh4.googleusercontent.com/sh_GgfbzcWtObFj8OZa2GzQ38KaeqUz6eIkr36_5RvH2Qyc3LTGgGLeaPmEbmbrLwXlF6A0mMgTpF97NVgAtKkMzHEQWvW5d-7Sg_9ucIe9s-L3x6C7uqosl0HytuEkqo5KyD78h

**Criterio de Definición de Cuentas Contables Resultado**

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Condición

.. raw:: html

   </td>

.. raw:: html

   <td>

DEBE

.. raw:: html

   </td>

.. raw:: html

   <td>

HABER

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

Transacción de Ventas = SI

.. raw:: html

   </p>

.. raw:: html

   <p>

&amp;amp;amp;amp;amp;amp;amp;gt; 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td>

.. raw:: html

   </td>

.. raw:: html

   <td>

Cuenta de Ganancia

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

Transacción de Ventas = SI

.. raw:: html

   </p>

.. raw:: html

   <p>

&amp;amp;amp;amp;amp;amp;amp;lt; 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td>

.. raw:: html

   </td>

.. raw:: html

   <td>

- Cuenta de Pérdida

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

Transacción de Ventas = NO

.. raw:: html

   </p>

.. raw:: html

   <p>

&amp;amp;amp;amp;amp;amp;amp;gt; 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td>

Cuenta de Ganancia

.. raw:: html

   </td>

.. raw:: html

   <td>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

Transacción de Ventas = NO

.. raw:: html

   </p>

.. raw:: html

   <p>

&amp;amp;amp;amp;amp;amp;amp;lt; 0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td>

- Cuenta de Pérdida

.. raw:: html

   </td>

.. raw:: html

   <td>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>