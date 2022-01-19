.. |Check multimoneda| image:: resources/multimoneda1.png
.. |Asignacion de Pagos| image:: resources/asignacion-de-pagos.png

**Asignación Manual de Pagos y Cobros**
=======================================

Si la Asignación entre un Pago y una Factura no se realiza al momento de
generarlo, también puede asignarlo posteriormente mediante el proceso de
Asignación de Pagos.

Mediante el proceso de Asignación de Pagos se asocia una Factura por
Pagar o Cobrar con su Pago/Cobro o Nota de Crédito que corresponda.

Como aclaración, este proceso visualiza los Medios de Pago realizados a
dicho Socio del Negocio.

**Moneda:** Se puede seleccionar una sola moneda o marcar el check
de “Multimoneda” para que se visualice documentos en todas las monedas.

|Check multimoneda|

**Fecha:** En la fecha seleccionada se aplicará la Asignación a generar.

CP – CC: Este campo define los tipos de documentos que se visualizará en
el proceso. Las opciones son CxC & CxP, Sólo CxP, Sólo CxC. (CxC=
Cuentas por Cobrar, CxP= Cuentas por Pagar).

En la parte inferior de la ventana se ven los campos de Diferencia,
Cargo, Organización y Descripción. En Diferencia se definirá
automáticamente según la diferencia que exista entre los documentos que
se hayan seleccionado para que la Asignación “Cierre”. **El sistema no
permitirá generar ninguna Asignación mientras exista una diferencia y no
se seleccione Cargo.**

Al definir un Cargo se realizará la asignación aplicando la diferencia a
dicho cargo.

Descripción: En el campo descripción podrá agregar adicionalmente una
descripción a la Asignación a generar. Por defecto las asignaciones que
sean generadas desde este proceso definirán el nombre del usuario que la
generó en la descripción de la asignación.

|Asignacion de Pagos|

**Asignación Multi-moneda:** este check deberá ser marcado en Y si se
desea realizar una Asignación entre dos documentos de diferente moneda.
Al marcarlo, no sólo se mostrarán documentos en la Moneda definida en el
campo "Moneda", sino que mostrará todos los documentos con saldo en
todas las monedas.

Además se agregara en la ventana nuevas columnas con el importe
Convertido a la moneda definida en el campo moneda.

**Tipo de Conversión:** Opcionalmente se podrá definir el Tipo de
Conversión deseado. Normalmente el sistema tomará por defecto el Tipo de
Conversión "Spot" que es la conversión utilizada por la contabilidad,
pero adicionalmente podrán definir una Conversión "Documento" (utilizada
para setear una tasa de cambio manual que se pudo haber acordado con el
Socio del negocio para hacer la conversión entre ambas monedas) o
también Tasa de Cambio "Compañía" si es que la empresa define una tasa
de cambio por defecto para realizar las conversiones de moneda al
momento de realizar asignaciones.

**Tasa de Cambio:** Si se define el tipo de Conversión "Documento" se da
la opción de definir manualmente la tasa de cambio deseada para aplicar
la conversión.

Se adjunta gif del proceso

.. only:: html

    .. figure:: resources/gif-asignacion.gif

    Video 1. Proceso de Asignación