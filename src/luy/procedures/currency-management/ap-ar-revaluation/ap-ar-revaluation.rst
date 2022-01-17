.. |Completar Asiento Diario| image:: resource/accounting-application-.png
.. |Diario Contable Completo| image:: resource/diario-contable-completo-.png
.. |Factura Perdida Ganancia No Realizada| image:: resource/perdida-ganancia-no-realizada-.png
.. |Reporte Diferencia de Cambio DxC y DxP No Realizada| image:: resource/reporte-de-diferencia-de-cambio-dxc-y-dxp-no-realizada-.png

Revaluaciones de Cuentas por Cobrar y Cuentas por Pagar
=======================================================

Debido a que la tasa de cambio cambia con el tiempo, es posible que deba
determinar el valor actual de estos documentos en la fecha especificada
de revaluación (generalmente al final del período financiero).

Solop ERP puede calcular las ganancias o pérdidas no realizadas
realizando la revalorización de los documentos abiertos de Cuentas por
Pagar y Cuentas por Cobrar creados en moneda extranjera de forma
simultánea. Cuando el sistema realiza la revaluación, vuelve a calcular
los saldos abiertos de clientes y proveedores utilizando el tipo de
cambio vigente en la fecha de revaluación.

Este proceso revalúa los saldos abiertos en ME de la siguientes Cuentas
por Cobrar:

-  Documentos por Cobrar (no considera Notas de Crédito)
-  Cheques Diferidos por Cobrar

Este proceso revalúa los saldos abiertos en ME de la siguientes Cuentas
por Cobrar:

-  Documentos por Pagar (no considera Notas de Crédito)
-  Cheques Diferidos por Pagar

Este proceso se realiza en la ventana *Factura Pérdida/Ganancia no Realizada*
-----------------------------------------------------------------------------

|Factura Perdida Ganancia No Realizada|

-  **Esquema Contable:** Seleccionar el Esquema Contable que se quiere
   registrar la Diferencia de Cambio.
-  **Tipo de Conversión de Revaluación:** Tipo de Conversión de la
   revaluación.
-  **Fecha de Revaluación:** Fecha a realizar proceso
-  **CP-CC: Cuentas por Pagar:** (incluye documentos a Pagar como son
   los cheques diferidos , Cuentas por Cobrar o ambas.
-  **Incluir Todas las Monedas:** No hacer click. Dejar Vacío
-  **Moneda:**  Dejar Vacío
-  **Revalorización Tipo de Documento:** donde genera el asiento de
   revaluación (GL Document)- General Ledger (Contabilidad)

Dicho proceso realizará el cálculo necesario para actualizar la
aplicación contable de los Saldos de todos aquellos Documentos por
Cobrar y Documentos por Pagar que se encuentren Pendientes de Pago/Cobro
a la fecha de Revaluación.

El Resultado lo mostrará en el Reporte de Diferencia de Cambio No
Realizada detallando línea a línea los Documentos con el cálculo
realizado.

Reporte de Diferencia de Cambio Documentos por Cobrar y Documentos por Pagar no Realizada
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|Reporte Diferencia de Cambio DxC y DxP No Realizada|

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

La emisión del Reporte genera un Asiento Contable en borrador detallando
línea a línea los ajustes que se estarían realizando documento por
documento.

.. raw:: html

   </p>

.. raw:: html

   <p>

Este mismo lo podrán encontrar en la Ventana de Diario Contable, en
forma de Asiento Contable

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

El Lote del  Asiento Contable deberá completarse

|Completar Asiento Diario|

Anular el Asiento de Revaluación
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si desea anular un Asiento ya Completo deberá Anular y Corregir para que
la fecha de anulación sea la misma que la del asiento.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

CUIDADO La acción Anular y Causación crea el asiento con la fecha de
hoy.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

|Diario Contable Completo|

Si es necesario, puede realizar la revaluación de las cuentas de Cuentas
por cobrar más de una vez durante el mismo período. La revaluación
posterior en el mismo período ajusta los resultados de la revaluación
anterior, y cada revalorización genera un lote de asientos de extorno
automáticamente.

Asiento de revaluación de Cuentas por Cobrar
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Cuando se realiza una revaluación de Cuentas por cobrar, el sistema crea
un lote de Contabilidad general con los resultados de la revaluación. El
lote actualiza la cuenta de ganancia (o pérdida) no realizada
especificada para la moneda con el monto de ganancia (o pérdida)
calculada en el formulario

Como resultado del proceso de revaluación, el sistema calcula las
ganancias y pérdidas no realizadas y crea un asiento de revaluación con
inversión automática. Las ganancias y pérdidas no realizadas resultantes
se registran en las cuentas del Libro que especifique

Usted especifica las cuentas en las que se publican las ganancias y
pérdidas no realizadas en los recuadros Cuenta de ganancia no realizada
y Cuenta de pérdida no realizada .