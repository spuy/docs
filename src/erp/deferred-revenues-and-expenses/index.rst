.. _src/erp/deferred-revenues-and-expenses:

=======================================
**Reconocimiento de Ingresos y Gastos**
=======================================

**Generalidades**
-----------------

De acuerdo con los principios básicos de contabilidad, los ingresos no
deben reconocerse hasta que se hayan logrado, y los gastos no deben
reconocerse hasta que se hayan gastado. Para estos fines, el término
"diferimiento" se utiliza en la contabilidad. Se refiere al acto de
posponer el reconocimiento de ciertos ingresos o gastos en el estado de
resultados por un tiempo previamente determinado y registrarlos en las
cuentas de balance (pasivo o activo, respectivamente) cuando
verdaderamente se logran o gastan. En los siguientes períodos, se irán
reconociendo en las fracciones planificadas las cuentas de balance
(activo y pasivo) a las cuentas de resultados  (ingresos o gastos) en el
estado de resultados.

**La idea de esta funcionalidad es que en todo momento el Balance de la
empresa refleje de manera exacta lo que corresponda en relación a los
servicios suministrados y recibidos por la empresa.**

Estarán vinculadas en esta funcionalidad las cuentas contables de:

-  Activo y Pasivo correspondientes a los contratos (o servicios)
-  Ganancias y Pérdidas que reflejarán lo realmente suministrado o
   recibido

**Etapas de la Funcionalidad del Reconocimiento**
-------------------------------------------------

**Método de Reconocimiento:** Determinación del Método de Reconocimiento
en cada línea de la Orden (determinación de la manera que se deberá
reconocer los ingresos de cada producto)

-  Por Porcentaje de Avance
-  Por evento (no alcanzado)
-  Por período (no alcanzado)
-  Por Cobro (no alcanzado)

**Plan de Reconocimiento:** Según el Método definido, en cada
Transacción de Venta (Orden de Venta) se definirá líneas con los
importes a ser reconocidos por período.

**Proceso de Reconocimiento**: Proceso de Run

**Proceso de Diferencia de Cambio:** Diferencias de Cambio relacionadas
al reconocimiento de ingresos de operaciones en Moneda Extranjera.

.. toctree::
    :maxdepth: 2

    recognition-process/index
    deferred-revenue-recognition-types/index