

Procesando transacciones de Caja/Bancos
=======================================

En ADempiere puede agregar rápidamente transacciones que registran los
cobros de los clientes, los pagos a los proveedores, los reembolsos
recibidos de proveedores, cargos y comisiones bancarias, retiros de
Caja/Banco y diversos ajustes. Además, puede controlar las cuentas de
Caja/Banco y administrar efectivamente estas transacciones.

Aquí, leerá cómo registrar rápidamente las transacciones en dinero de
cualquier tipo y cómo el sistema las procesa.

Comprender los tipos de transacciones de Caja/Banco
---------------------------------------------------

Dependiendo del propósito de la transacción, puede registrar y procesar
transacciones de Caja/Banco de los siguientes tipos:

*Pago/Cobro* : crea una transacción tipo Pago para registrar una
operación realizada en Caja/Banco, como un cargo bancario, intereses, un
pago de un cliente, un pago a un proveedor o un pago desconocido.

*Transferencia recibida* : se crea una transacción de tipo Cobro cuando
registra una transferencia de fondos entre cuentas en Caja/Banco;
corresponde a los fondos recibidos a la cuenta de destino.

*Transferencia* emitida: se crea una transacción de tipo Pago cuando
registra una transferencia de fondos entre cuentas en Caja/Banco;
corresponde a los fondos enviados desde la cuenta de origen.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   </td>

.. raw:: html

   <td>

Para una transferencia de fondos, siempre hay una transacción del tipo
Transferencia recibida y una transacción del tipo Transferencia emitida
.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

*Pago anticipado* : crea una transacción de este tipo para registrar un
anticipo o pago inicial a un proveedor si el pago se realizó en
Caja/Banco. Las transacciones de este tipo afectan las cuentas contable
y las cuentas de proveedores en Cuentas por pagar.

*Reembolso del proveedor* : crea una transacción de este tipo para
registrar un reembolso por un pago anticipado o un ajuste de débito si
el reembolso se realizó en Caja/Banco. Las transacciones de este tipo
afectan las cuentas contable y las cuentas de proveedores en el módulo
Cuentas por pagar.

*Cobro Cliente* : crea una transacción de tipo Cobro para registrar el
cobro de un cliente entrante que se realizó en Caja/Banco. Las
transacciones de este tipo afectan las cuentas del Libro mayor y las
cuentas de clientes en el módulo Cuentas por cobrar.

*Cobro* : crea una transacción de tipo Cobro para registrar una
operación realizada en Caja/Banco, como un ingreso bancario, ingresos
por intereses.

*Depósito Bancario* : crea una transacción de este tipo Pago si desea
depositar pagos de clientes o reembolsos de proveedores en una cuenta de
Caja/Banco. Las transacciones de este tipo afectan las cuentas
contables.

*Depósito Bancario* anulado: crea una transacción de este tipo si desea
anular un depósito. Las transacciones de este tipo afectan a las cuentas
contables que participaron en el depósito relacionado.

Ingresando Transacciones de Pago/Cobro
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Dependiendo el Tipo de Transacción que desee ingresar debe tener claro
que siempre deberá ingresar:

-  Tipo de Documento
-  Cuenta Bancaria
-  Moneda
-  Fecha
-  Socio de Negocio

Procesando Pagos de  Documentos por Pagar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Al momento de ingresar un Pago, si éste está vinculado a un Documento
por Pagar,  puede asignarlo en ese momento.

También puede asignarlo posteriormente de manera manual en Asignación de
Pagos.

En ambos casos se realizará el asiento contable de asignación.

Procesando Cobro de  Documentos por Cobrar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Al momento de ingresar un Cobro, si éste está vinculado a un Documento
por Cobrar,  puede asignarlo en ese momento.

También puede asignarlo posteriormente de manera manual en Asignación de
Pagos.

En ambos casos se realizará el asiento contable de asignación.

Procesamiento de una entrada de Caja/Banco
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Registro de un Pago/Cobro
~~~~~~~~~~~~~~~~~~~~~~~~~

Usted crea una entrada de Caja/Banco utilizando la ventana de
Pago/Cobro. Selecciona una cuenta Bancaria y un tipo de entrada, moneda,
 cambia la fecha de la transacción. A continuación, agregue los detalles
de la transacción.

Para cada detalle de transacción, puede seleccionar un SDN y un cargo si
corresponde.

-———————————————————————————————————–

Ingreso rápido de un Cobro
''''''''''''''''''''''''''

Aprobar una entrada de efectivo
'''''''''''''''''''''''''''''''

Visualización de una entrada de efectivo
''''''''''''''''''''''''''''''''''''''''

Monitoreo de una Transacción de Caja
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Cuenta Caja/Banco detallada
'''''''''''''''''''''''''''

Puede ver información resumida o la lista completa de transacciones
relacionadas con efectivo realizadas en la cuenta durante este período.
La información se recopila de los módulos Administración de efectivo,
Libro mayor, Cuentas por pagar y Cuentas por cobrar.

Seleccionando la vista
''''''''''''''''''''''

Entrada rápida de transacciones
'''''''''''''''''''''''''''''''