.. |Generar Cuotas a Facturar desde Contrato de Servicio| image:: resource/generate-fees-to-bill-from-the-service-contract-process.png
.. |Generar OV desde Cuota de Contrato| image:: resource/generate-sales-order-from-contract-fee.png

**Generar Órdenes de Venta recurrente desde Contrato de Servicios**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A partir de la definición de las líneas de un contrato se puede generar
Órdenes de Venta según los Servicios Recurrentes que deban ser
facturados según determinada recurrencia. De esta manera se podrán
generar Órdenes de Venta según las mensualidades definidas en los
Contratos.

El proceso será el siguiente:

Definición correcta del Contrato de Servicios: el primer paso para
comenzar el proceso es verificar que todos los contratos estén
correctamente definidos, tanto según las fechas del mismo como también
las líneas.

Crear “Cuotas a Facturar”: a partir de la definición de líneas en los
contratos con su recurrencia correspondiente e importe, se deberá
proceder a generar las “Cuotas a Cobrar” a partir del mismo. Este
proceso puede generarse tanto desde la ventana “Contrato de Servicios”
mediante el Proceso “Generar Cuotas desde Contrato” ubicado en los
procesos asignados al registro, de esta manera se generarán TODAS las
Cuotas a Facturar desde 1 solo contrato. También se tiene la opción de
realizarlo de manera masiva para todos los contratos desde el proceso
“Generar Cuotas a Facturar desde Contrato” ubicado en el menú, en este
caso podrá no seleccionar ningún Contrato de Servicios en especial
generando así Cuotas para Todos los Contratos.

|Generar Cuotas a Facturar desde Contrato de Servicio|

Generar Orden de Venta desde Cuota a Facturar de Contrato de Servicios:
Una vez se tienen todas las “Cuotas a Facturar de los Contratos de
Servicios” creadas, se podrá generar a partir de las mismas las Órdenes
de Venta para que puedan ser ingresadas luego al Proceso de Facturación.
Estas Órdenes de Venta se sugiere utilizar el Tipo de Documento “Orden
de Venta Fee”. En el Proceso se podrán filtrar según el Socio del
Negocio, la Organización o la Fecha de la Cuota a facturar. En este
proceso se podrá definir un sólo Socio del Negocio o todos los que
desee. Se recomienda filtrar según Fecha para asegurarse que se está
generando las cuotas correspondiente al mes que desea. En los parámetros
del proceso podrá ver que está editable la Fecha del Documento que desea
generar.

|Generar OV desde Cuota de Contrato|

IMPORTANTE: Para poder generar las Órdenes de Venta FEE desde el proceso
“Generar OV desde Cuota de Contrato” es obligatorio que el Cliente tenga
creado un Proyecto en el cuál tenga definido el check de “Es por defecto
para FEE”.