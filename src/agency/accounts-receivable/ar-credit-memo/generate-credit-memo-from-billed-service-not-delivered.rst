**Servicio Facturado pero No Entregado**
========================================

Para este caso, debido a que el importe que se deberá generar una Nota
de Crédito aún no fue Entregado, es decir no se realizó Checking, para
solicitar la creación de una Nota de Crédito por las Cantidades que
fueron Facturadas pero no fueron Entregadas bastará que el Usuario
“Cierre” la Orden de Venta correspondiente. Al Cerrar una Orden de Venta
las “Cantidad Ordenada” de sus líneas son llevadas a la “Cantidad
Entregada”.

**Control de Facturación correcta en Órdenes de Venta**
-------------------------------------------------------

El sistema, luego de Cerrar una Orden, realizará un control de verificar
si la Orden de Venta está Correctamente Facturada. Este Control implica
2 verificaciones:

Control de Cantidades: En cada una de sus líneas se verificará que su
“Cantidad Facturada” NO sea SUPERIOR a la “Cantidad Ordenada”. En caso
de encontrar alguna línea que sea superior, es decir que se haya
Facturado más de lo Ordenado y que la Orden esté Cerrada, se generará
automáticamente una “Solicitud de Nota de Crédito” detallando la Orden
de Venta y Factura vinculada y se le asignará al Departamento
“Administración”. Este control se aplicará siempre y cuando dicha Orden
no haya sido “Modificada”

1. Control de Totales (Orden Modificada): Si en el primer control no
   encontró nada por lo que deba realizar una Solicitud de NC, se deberá
   continuar con el siguiente paso que será analizar el “Total de
   Líneas” de la Orden es Menor que el “Total de Líneas” del Documento
   por Pagar vinculado a la misma. En caso de que la Orden sea Menor que
   el DxP entonces deberá correr el proceso de “Solicitud de NC”.