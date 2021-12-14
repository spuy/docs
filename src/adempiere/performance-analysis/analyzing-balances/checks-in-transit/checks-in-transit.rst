Cheques en Tránsito (Activo)
============================

La cuenta Cheques en tránsito es utilizada por Solop para dejar registro
de todo movimiento Financiero que esté registrado en el sistema pero que
aún no fue verificado en la cuenta bancaria utilizada. El hecho de que
se registre un Pago/Cobro en el sistema significará que por un lado,
debería aumentar o reducir un Activo monetario (ej. Saldo del Banco) y
por otro lado, cancelar una deuda o activo generado por un Documento por
Pagar o Cobrar. La parte "Monetaria" de una Pago/Cobro es la que
manejará la cuenta "cheques en tránsito" siendo una cuenta intermedia
antes de confirmar su correspondiente Ingreso/Egreso del
banco.Movimientos de la cuenta contable:

La cuenta Cheques en Tránsito se parametriza en la Cuenta Bancaria,
campo Cheques en Transito.

(FOTO)

**Cuando la Empresa cobra:**

Debita con: Cobros                                 Acredita con:
Conciliación Bancaria

**(FOTO ASIENTO COBRO)**

**(FOTO ASIENTO CONCILIACIÓN COBRO)**

**Cuando la Empresa Paga:**

Debita con Conciliación Bancaria        Acredita con: Pagos

**(FOTO ASIENTO PAGO)**

**(FOTO ASIENTO CONCILIACIÓN PAGO)**

Reporte de Pagos/Cobros sin concilar
------------------------------------

La composición de la Cuenta Contable Cheques en Tránsito se analiza en
el **Reporte de Pagos sin Conciliar.**

Dicho reporte mostrará aquellos documentos de Pago/Cobro que involucren
a Cuentas Bancarias y que no han sido conciliados aún.

Analizando Pagos/Cobros sin conciliar mediante el Balance de Prueba.
--------------------------------------------------------------------

Podrá realizar los siguientes pasos que le ayudará a comprender y
verificar el saldo de esta cuenta:

Transacciones con una sola moneda
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Emitir el Balance de Prueba de la cuenta contable "Cheques en
   Tránsito" por Socio de Negocio.
2. Exportar con formato XLSX.
3. Identifique las contabilizaciones que correspondan a transacciones
   anuladas. Píntar las anuladas.
4. Sumar las filas identificadas y verificar que sumen 0.
5. Vincular Pagos con Conciliaciones. Pintarlos. Verificar que sumen 0.
6. Vincular Cobros con Conciliaciones. Pintarlos. Verificar que semen 0.
7. Las transacciones que quedaron sin identificar corresponderá al saldo
   de la cuenta. Es decir a los Pagos/Cobros sin Conciliar.
8. También podrá emitir el Reporte de Pagos sin Conciliar (le mostrará
   los pagos no conciliados a la fecha, cualquier estado).

Transacciones en varias monedas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Emitir el Balance de Prueba de la cuenta contable "Cheques en
   Tránsito" por Socio de Negocio y Moneda.
2. Exportar con formato XLSX.
3. Identifique las contabilizaciones que correspondan a transacciones
   anuladas. Píntar las anuladas.
4. Sumar las filas identificadas y verificar que sumen 0.
5. Vincular Pagos con Conciliaciones. Pintarlos. Verificar que sumen 0.
6. Vincular Cobros con Conciliaciones. Pintarlos. Verificar que semen 0.
7. Las transacciones que quedaron sin identificar corresponderá al saldo
   de la cuenta. Es decir a los Pagos/Cobros sin Conciliar.

Cuenta Cheques en Tránsito con Moneda Extranjera
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si la cuenta contable Cheques en Tránsito se utiliza para realizar
transacciones en varias monedas o sólo en Moneda Extranjera, se deberá
parametrizar el elemento contable como:

**(AGREGAR FOTO)**

-  Cuenta Banco
-  Maneja Moneda Extranjera SI
-  Moneda USD

De esta manera participará en el proceso de revaluación de saldos en
Moneda Extranjera Cheques.