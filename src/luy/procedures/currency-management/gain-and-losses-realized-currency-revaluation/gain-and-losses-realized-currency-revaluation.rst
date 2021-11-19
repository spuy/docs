Diferencia de Cambio Ganancia/Pérdida
=====================================

Si su compañía usa diferentes monedas como monedas base, es posible que
deba re expresar los saldos de las cuentas de la moneda base a cualquier
moneda extranjera configurada para su uso en contabilidad. Esta
operación se llama Conversión de Monedas.

Los Documentos que presentan estas conversiones y realizan estos
cálculos son los siguientes:

**Asignación**
~~~~~~~~~~~~~~

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

1.00</s