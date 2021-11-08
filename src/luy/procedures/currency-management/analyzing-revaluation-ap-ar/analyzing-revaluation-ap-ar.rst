.. |Ejemplo| image:: resource/example.png
.. |Saldos Abiertos a la Fecha| image:: resource/open-items.png

Analizando la Diferencia de Cambio no Realizada
===============================================

El proceso para realizar la verificación Contable con los Saldos
Abiertos que existe en los Auxiliares se puede realizar mediante los
siguientes pasos:

Verificación del Ajuste Cuentas por Pagar y por Cobrar
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

1. Verificar que todos dan igual según Importe Fuente (Opcional)

   1. Obtención de Reporte de Saldos Abiertos cuentas por Cobrar
   2. Balance de Prueba Cuenta “Cuentas por Cobrar Comerciales”
   3. Obtención de Reporte de Saldos Abiertos cuentas por Pagar
   4. Balance de Prueba Cuenta “Cuenta por Pagar Comerciales”

2. Proceso de “Ajuste de Diferencia de Cambio No Realizada” (Factura
   Pérdida/Ganancia No Realizada)
3. Verificar que da igual reportes Auxiliares y Balance

   1. Obtención de Reporte de Saldos Abiertos cuentas por Cobrar
   2. Balance de Prueba Cuenta “Cuentas por Cobrar Comerciales”
   3. Obtención de Reporte de Saldos Abiertos cuentas por Pagar
   4. Balance de Prueba Cuenta “Cuenta por Pagar Comerciales”

Explicación del Ajuste realziado por el Proceso de DIferencia de Cambio No Realizada
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El proceso de diferencia de cambio No Realizada puede controlarse, para
ello deberá exportar a Excel el Reporte que brinda el proceso del
cálculo de Diferencia de Cambio No Realizada al momento que la ejecuta.
Cuidado, este reporte presentará el cálculo realizado y no podrá
obtenerse nuevamente a menos que genere el proceso una vez más,
generando así el Asiento del Ajuste nuevamente.

En la planilla verá documento por documento sus aplicaciones en moneda
fuente, en moneda esquema, los importes revaluados considerando la tasa
de cambio seleccionada y las diferencias a revaluar.

Ejemplo:

|Ejemplo|

Comprobación de Cálculo de Diferencia de Cambio no Realizada
------------------------------------------------------------

Como forma de comprobación del proceso realizado usted podrá emitir los
siguientes reportes:

En Documentos por Pagar y Documentos por Cobrar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Emitir Reportes de Saldos Abiertos a la Fecha del proceso de:

-  Transacciones de Ventas incluyendo Cheques Diferidos
-  No Transacciones de Venta incluyendo Cheques Diferidos

Considerar sólo las operaciones en Monedas Extranjeras (no hay filtro de
MONEDA, las deberá excluir en una planilla externa)

Verificación de Diferencias de Cambio Cuentas por Pagar  y Cuentas por Cobrar
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Obtener el Informe Financiero “Balancete de Cuentas Contables” a fecha
de Cierre de Ejercicio

Verificación de Saldos Contables de Cuentas de Documentos:

En estos casos, las líneas de Ganancia/Pérdida por Diferencia de Cambio
Realizada se realizan SIEMPRE con Moneda del Esquema Contable, de manera
que no estarán clasificadas como con Moneda USD sino con UYU si su
esquema contable está en UYU.

|Saldos Abiertos a la Fecha|

1. Seleccione Organización
2. Transacción de Ventas: SI
3. A Fecha de cierre de fecha de Período Financiero
4. Con Cheques Diferidos