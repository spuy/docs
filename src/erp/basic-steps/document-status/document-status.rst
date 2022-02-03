.. |Anulado| image:: resources/anulado.png
.. |Borrador| image:: resources/borrador.png
.. |Completo| image:: resources/completo.png
.. |Estados de Documentos| image:: resources/estados-de-documentos.jpg
.. |Reversado| image:: resources/reversado.png

Estados del Documento
=====================

En Solop, los *Documentos* -al contrario de los *Datos Maestros-* tienen
estados, y un flujo definido dentro de Solop para pasar de un estado a
otro.

|Estados de Documentos|

Además, dependiendo del estado del documento, ciertos campos del
documento son editables y otros no.

| Un documento pasa de un *Estado* a otro por medio de una *Acción*. 
| Por ejemplo para pasar del estado de *Borrador* a *En Progreso*, se
  debe ejecutat la acción *Preparar*, y para pasar del estado *En
  Progreso* al estado *Completado*, se debe ejecutar la acción
  *Completar*.

Todos los documentos comienzan en el estado de *Borrador*.

En Solop son *Documentos*:
~~~~~~~~~~~~~~~~~~~~~~~~~~

-  Órdenes de Compra y Venta
-  Facturas de Compra y Venta
-  Recibos y Despachos de Material
-  Pagos y Cobros
-  Traslados de Material
-  Asientos Contables
-  Producción
-  \**etc.*\*

Documento Borrador
~~~~~~~~~~~~~~~~~~

|Borrador|

En el cabezal de la ventana en el Estado, Estado del Documento indicará
Borrador.

Documento En Progreso
~~~~~~~~~~~~~~~~~~~~~

| Se llega al estado *En Progreso* luego de ejecutar la acción
  *Preparar*.
| La acción *Preparar* realiza pruebas lógicas previas a ejecutar el
  documento (o "completarlo", en el idioma de Solop).
| Por ejemplo en una Factura, la acción *Preparar* verifica entre otras
  cosas que el período correspondiente a la fecha indicada esté abierto.

Documento Completo
~~~~~~~~~~~~~~~~~~

| Se llega al estado *Completo* luego de ejecutar la acción *Completar*.
| La acción *Completar* ejecuta el documento, es decir ejecuta una Orden
  de Compra, ejecuta una Factura, ejecuta un Pago, etc.
| Esto incluye las transacciones definidas para el documento, como por
  ejemplo en el documento Recibo de Material, incrementar la existencia
  del Almacén.

Importante: la acción *Completar* no incluye la afectación contable! El
resultado de completar un documento lo coloca en la lista de documentos
por contabilizar, y que el procesador contable cuando corra, ejecutará
contablemente.

Es posible ejecutar el procesador contable de manera *Inmediata* al
Completar un documento. En este caso sí aplicará contablemente
simultáeamente al completar.

|Completo|

-  Estado del Documento indicará Completo.
-  El Botón de Proceso indicará que puede Anular el documento.

Documento Anulado
~~~~~~~~~~~~~~~~~

|Anulado|

En Solop los documento NO se borran, se anulan, creando automáticamente una transacción negativa llamada Reverso.

1. Nro. del Documento
2. Indica que el Documento está Anulado y pone el Nro del Reverso con
   estos símbolos para su identificación <.)
3. Estado de Documento: Anulado

Documento Reversado
~~~~~~~~~~~~~~~~~~~

|Reversado|

1. Nro. del Documento
2. Indica que el Documento está Reversado y pone el Nro del Documento
   Anulado con estos símbolos para su identificación {->
3. Estado de Documento: Reversado

Documento Cerrado
~~~~~~~~~~~~~~~~~

Con esta acción el Documento queda “Bloqueado” y no será posible
accionar sobre él. El asiento queda intacto.

Documento Reversar-Corregir
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Revierte el Documento realizando el asiento contable inverso con la
fecha en que se realizó la acción.

Documento Reversar - Causación
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Revierte el Documento realizando el asiento contable inverso con la
fecha de hoy.