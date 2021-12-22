.. |Pestaña Fase| image:: resource/phase-tab.png
.. |Pestaña Orden de Venta| image:: resource/sales-order-tab.png
.. |Pestaña Proveedor| image:: resource/supplier-tab.png

**Compra Directa a un Proveedor en nombre de Cliente**
------------------------------------------------------

Cuando el Proyecto incluya realizar una compra específica a un proveedor
pero que no es necesario pasar por el proceso de generar una Solicitud
de Cotización (RFQ), se podrá gestionar la misma de forma directa desde
una Fase.

En este caso, los pasos a seguir serán:

Definir el Proyecto mínimo con Nivel de Línea “Fase”

En la Fase activar el check Entrega Directa

Definir un Proveedor como “Socio del Negocio de Entrega Directa”

En las Líneas de Tarea definir el Producto, precio y cantidad

Desde la Fase generar una Orden de Venta al Cliente pero Generar la
Orden desde el botón de Generar Orden de Venta ubicado en la Fase.

Seleccionar Tipo de Orden “Orden de Venta con Aprobación”

|Pestaña Fase|

Dicho Proceso generará una Orden de Venta con el Proveedor definido como
Entrega Directa. Esto hará que al completarse la Orden de Venta, se
genera automáticamente una Orden de Compra al Proveedor enlazada con
esta Orden de Venta.

La Orden de Compra se podrá encontrar en el campo “Orden enlazada” de la
Orden de Venta.

|Pestaña Orden de Venta|

IMPORTANTE: Tener en cuenta que el Producto definido en la línea de la
Orden de Venta, deberá estar definido tanto en la Lista de Precios de la
Orden de Venta, como también en la Lista de Precios que el Proveedor
tenga definida por defecto en su definición de Socio del Negocio. Para
evitar esto podemos dejar el campo Lista de Precios de Compra del
Proveedor vacío.

|Pestaña Proveedor|

**Checking**
~~~~~~~~~~~~

Luego de contar con una “Orden de Compra” en Estado “Completo”, la misma
se deberá confirmar mediante su delivery mediante el Checkin.

El checking se puede acceder de dos maneras:

1. Barra de Herramientas/Procesos (engranaje). Desde los Procesos
   definido en el Proyecto que se estará verificando el delivery. Para
   ver los procesos del Proyecto se deberá oprimir el botón de proceso
   ubicado en la Barra de Herramientas seleccionando “Checkin”.
2. Menú. Desde el proceso Checkin ubicado en el menú, en este caso se
   podrá filtrar según desee pudiendo ver más de un proyecto a la vez
   para confirmar.

Barra de Herramientas/ Procesos:

.. image:: https://lh5.googleusercontent.com/0S0ogDdsbUZzeqJ8zX17SWPIZOFp_v6BbiuSd19i8_QVjX2i9Fi1BMqKfN4PWNGPSiBhB2fBJPyTMYwhNTDB2ufy2e_k6ZP99PMmru3b7TDJN3xEBIStD8xEfHlzT6Et4yTdJps5

Documentos sobre los que se debe realizar checking:

-  Se debe realizar checking sobre todas las órdenes de venta inversión
   del cliente menos la "OV compra paquete" dónde el checking se realiza
   sobre las órdenes de consumo.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Los Procesos desde la Barra de Herramientas no se actualizan
automáticamente, por lo que si lo presionó desde la Fase, recordará los
Procesos de la Fase. para solucionarlo deberá ingresar nuevamente a la
ventana y presionar “Procesos” desde la pestaña de proyecto.

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>