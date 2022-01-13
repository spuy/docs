.. _ERPyA: http://erpya.com
.. _src/adempiere/open-items/payment-selection:

=====================
**Selección de Pago**
=====================

Una selección de pagos en Solop ERP no es más que la agrupación de documentos de CxP o de compras que se necesitan ser cancelados ya sean en su totalidad o de manera parcial, dentro de la selección de pagos se encuentran los tipos de documentos "**Orden de Pago**" y la "**Selección de Pagos de Cuentas por Pagar**", los cuales son utilizados para seguir los canales regulares entre los departamentos de compras, cuenta por pagar y tesorería.

La "**Orden de Pago**" es utilizada para crear aquellas solicitud de pago de los documentos pendientes por pagar, comúnmente es utilizada por los departamentos de compras y de cuentas pagar, ya qué ellos solo se encargan de agrupar aquellos documentos los cuales necesitan qué sean cancelados.

La "**Selección de Pagos de Cuentas por Pagar**" es utilizada cuando se define cuales son los documentos que sí se les generará el pago y desde qué cuenta bancaria de la compañía saldrán la cancelación de los documentos seleccionados; la selección parte de la agrupación de facturas asociadas en la "**Orden de Pago**" este procedimiento es comúnmente realizado por el departamento de tesorería, ya qué ellos son los encargados de llevar los saldos en banco lo cual le permite tener una toma de decisión del banco a utilizar para saldar una factura de CxP o realizar un anticipo a proveedores.


.. toctree::
    :maxdepth: 2

    payment-order-from-purchase-order
    pay-order
    payment-selection-payroll
    payment-selection-cxp