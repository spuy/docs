**Gestión de Medios**
=====================

**Proyecto de Medios**
----------------------

El Proyecto de Medios centraliza el pedido realizado por el cliente,
asociando todo tipo de documentos que hayan sido generados a lo largo de
toda la organización, por ejemplo:

-  Orden de Compra
-  Orden de Venta
-  Cotizaciones
-  Tareas

En un Proyecto de Medios se gestionará la Inversión que un cliente
quiera realizar sobre los Tipos de Medio y Medios que desee.

Sobre cada proyecto se podrá asignar Órdenes de Compra realizadas a los
Medios, Órdenes de Venta (Órdenes de Facturación) a los Clientes así
como también el registro de las correspondientes Facturas tanto de
compra como de venta.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Las Compras a los medios realizadas para los clientes podrán ser
realizadas de dos maneras, solicitando tanto la compra como la
publicación en conjunto o bien se podrá realizar una Pre-Compra para
luego ir consumiendo el saldo mediante Órdenes de Publicidad
independientes. 

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

La idea es que mediante el Proyecto se pueda obtener un vistazo de
situación de la compra de medios solicitada por el cliente.

En cada proyecto se definirá los siguientes puntos:

**Clasificación según diferentes “Etiquetas”:** estas pueden ser
Cliente, Marca del Cliente, Tipo de Trabajo, Sello, etc.

**Gerente de Proyecto:** este normalmente es el “Ejecutivo de Cuenta”
que tenga el cliente pero puede cambiar en algunos proyectos.

**Generación de Órdenes de Venta:** sobre las cuales se podrá gestionar
su Facturación.

**Detalle de Línea de Factura:** Opcionalmente

**Reportes:** se podrá generar diferentes Reportes financieros sobre el
estado de los proyectos.

**Campos del Proyecto**
~~~~~~~~~~~~~~~~~~~~~~~

Campos Manuales
^^^^^^^^^^^^^^^

Se deberán definir manualmente de forma obligatoria los siguientes
campos:

-  **Socio del Negocio**
-  **Nombre**
-  **Marca Cliente**
-  **Lista de Precios:** Es según la Lista de Precios que se define la
   Moneda que se manejará en el Proyecto.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

La moneda del Proyecto la determina la moneda que Facturará el Proveedor

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

\_En caso que al Cliente se le deba Facturar en otra moneda, la Orden de
Venta deberá ser en la misma moneda que se comprará al Proveedor, pero
se podrá definir en la Orden de Venta una moneda diferente a ser
Facturado junto con su Tasa de Cambio acordada. \_

**Campos Automáticos:**
^^^^^^^^^^^^^^^^^^^^^^^

Los siguientes campos, entre otros, se definirán de manera automática
(igualmente se podrán modificar si se desea).

-  **Moneda**
-  **Agente Comercial:** El campo “Agente Comercial” en el cabezal de un
   Proyecto tomará de forma automática al usuario logueado en el sistema
   siempre que este tenga el check de "Agente comercial" en "Y", en la
   Pestaña "Empleado" de la ventana "Socio de negocio".
-  **Sello Origen:** Cuando se guarda un proyecto se realiza lo
   siguiente:

   Según la Categoría de Proyecto se definirá el Sello Origen
correspondiente que tenga definido el Contrato del Cliente en sus
“Partes del Contrato”.

Según las siguientes Categoría de Proyecto se obtendrá el sello definido
para el siguiente tipo de empresa:

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Categoría de Proyecto

.. raw:: html

   </td>

.. raw:: html

   <td>

Tipo de Empresa

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Proyecto de Agencia

.. raw:: html

   </td>

.. raw:: html

   <td>

Agencia Creativa

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Proyecto de Medios

.. raw:: html

   </td>

.. raw:: html

   <td>

Agencia de Medios

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Proyecto RRPP

.. raw:: html

   </td>

.. raw:: html

   <td>

Agencia RRPP

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr>

.. raw:: html

   <td>

Proyecto de Medios Digitales

.. raw:: html

   </td>

.. raw:: html

   <td>

Agencia de Medios Digitales

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

\*Si no se obtuvo sello de origen se lanza una excepción.

-  **Almacén:** El almacén en un proyecto se definirá de manera
   automática según el almacén que tenga definido el Cliente en la
   pestaña Cliente ventana Socio del Negocio.

**Tamaño del Proyecto (Campo “Nivel de Línea”)**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Un Proyecto podrá tener diferentes niveles según su complejidad o
tamaño. Dentro del Nivel seleccionado, se contará con una pestaña de
Líneas donde se podrá definir cada uno de los Productos que se estará
manejando. Sobre estos Productos definidos se generará una Orden de
Venta al Cliente y una Orden de Compra al Proveedor del Medio.

Los diferentes niveles posibles son: Proyecto, Fase y Tarea.

**Nivel PROYECTO:** No usar Nivel Proyecto para los Proyectos de Medios

**Nivel FASE:** Se utilizará cuando el Proyecto sea de Compra y Consumo
(mismo momento).

**Nivel TAREA:** Se utilizará cuando el Proyecto sea de Pre-Compra o
Inversión y luego su Consumo (En momentos diferentes).