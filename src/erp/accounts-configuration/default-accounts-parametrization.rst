Comprendiendo la Parametrización de Cuentas Contables predeterminadas
=====================================================================

Con el fin de facilitar las definiciones contables de los diferentes
"jugadores" que se encuentran en el sistema desde donde se determinan
las cuentas contables, Solop cuenta con un ágil proceso de definición
masiva de cuentas contables, de manera que uno siempre se asegurará que
los "jugadores" cuenten con una definición correcta. Dentro de este
universo de jugadores definidores de cuentas contables podremos
encontrar a Productos, Socios de Negocio y Cuenta Bancarias, Almacenes,
etc.

Asientos Contables por Tipo de Documentos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Solop logra una correcta aplicación contable en tiempo real gracias a su
poder de generar asientos exactos a medida que la operativa avanza a lo
largo de la compañía. Esto es alcanzado gracias a la correcta y
adaptable definición de asientos contables que cuenta cada Tipo de
Documento, obteniendo el Importe desde el Documento y la cuenta contable
que corresponda a partir de los "Jugadores" que estén definidos en el
documento en cuestión.

.. raw:: html

   <table>

.. raw:: html

   <tbody>

.. raw:: html

   <tr>

.. raw:: html

   <td>

.. raw:: html

   <p>

En todo asiento contable de un documento transaccional existe un asiento
contable que busca las cuenta contables para crear el asiento desde dos
lados diferentes.

.. raw:: html

   </p>

.. raw:: html

   <ul>

.. raw:: html

   <li>

Cabezal

.. raw:: html

   </li>

.. raw:: html

   <li>

Líneas del Documento

.. raw:: html

   </li>

.. raw:: html

   </ul>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

Por un lado, se basa en el cabezal del documento, donde posiblemente se
define el Socio de Negocio por ejemplo. Del otro lado del asiento,
tomará la cuenta existente en las líneas, como podría ser un Producto en
el caso de una factura o una Cuenta Bancaria o caja en el caso de ser un
Recibo.

Configuración de Cuentas contables en los "Jugadores"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

De esta manera es vital que la definición de la contabilidad en cada uno
de estos **Jugadores** sea fácil de mantener y permita a la
administración tener la confianza de que las cuentas estén siempre
correctamente definidas.

Cada tipo de Jugador tendrá su propia manera de definición de Cuentas
Contables por Defecto.

Los Tipos de Jugadores que podemos encontrar en el sistema pueden ser
los siguientes:

-  Producto
-  Socio del Negocio
-  Cuenta Bancaria
-  Tasa de Impuesto
-  Almacén
-  Cargo

Configuración de las Cuentas Contables de Productos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Los productos son un jugador muy importante en el ERP ya que los mismos
podrán cumplir diferentes posiciones a lo largo de cada proceso. Según
sea el documento que lo esté utilizando, el mismo definirá si es una
Venta, una compra o una recepción por lo tanto cada documento obtendrá
del mismo diferentes cuentas según sea la acción realizada.

La cuenta de los Productos se obtendrá siempre según la definición
contable que tenga el mismo. Esta definición se podrá encontrar en la
misma ventana de Producto, pestaña Contabilidad, teniendo un campo
exclusivo para cada acción que se podrá realizar con un producto.

.. image:: /api/v3/attachments/627/content

Dentro de Solop podrán ser definidos miles de productos, cada una con su
definición correspondiente, siendo muy importante contar con una
clasificación correcta de los mismos para facilitar así una correcta y
ágil definición contable a medida que se modifican o crean productos
nuevos.

Las cuentas contables definidas en cada uno de los productos, podrán
asignarse manera masiva según 2 niveles.

En el 1er Nivel, el más abarcativo, que podremos llamar **nivel
superior**, podremos encontrar las cuentas definidas en el "Esquema
Contable", dentro del grupo de campos de **"Producto"** encontraremos
las cuentas que hacen referencia a los Productos y será donde se definan
las cuentas por defecto que utilizará el sistema para cargar los
siguientes niveles de definición contable para los Productos. Si se
desea mantener una definición contable única para todos los productos,
sólo será necesario definir las cuentas contables en este nivel, y las
mismas se definirán en todos los productos.

.. image:: /api/v3/attachments/628/content

A partir de estas cuentas definidas por defecto en el Esquema Contable,
se definirán en el siguiente nivel de definición contable de productos,
el **2do nivel** para los productos será según la **"Categoría de
Producto".** Dentro de cada categoría podrá ver una pestaña de
Contabilidad donde se podrá, en caso que se desee, modificar las cuentas
contables que desee utilizar según la Categoría de Producto que sea. De
esta manera, es vital la correcta clasificación de los productos con su
correcta "Categoría de Producto" ya que a partir de ella, se definirá su
correspondiente definición contable.

.. image:: /api/v3/attachments/629/content

El 3er y último nivel será el de "Producto", al crear un nuevo producto
es obligatorio definir que Categoría de Producto le corresponde, a
partir de la Categoría de Producto seleccionada, el producto tomará su
definición contable definida. En caso de que se desee modificar la
definición contable específicamente de un producto, será posible
simplemente modificando la cuenta que desee de la definición contable
del Producto en cuestión.

De no encontrar una cuenta definida en el Producto, no se podrá
completar el asiento contable en cuestión, quedando dicho documento con
“Error de Posteo”.

.. image:: http://159.203.95.97:8086/api/v3/attachments/627/content

Configuración de las cuentas contables de Socios del Negocio
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Dentro de Solop podrán ser definidos tantos socios del negocio se desee,
cada una con su definición correspondiente, siendo muy importante contar
con una clasificación correcta de los mismos para facilitar así una
correcta y ágil definición contable a medida que se modifican o crean
nuevos.

Las cuentas contables definidas en cada uno de los Socios del Negocio,
podrán asignarse manera masiva según 2 niveles.

En el 1er Nivel, el más abarcativo, que podremos llamar **nivel
superior**, podremos encontrar las cuentas definidas en el "Esquema
Contable", dentro del grupo de campos de **"Socio del Negocio"**
encontraremos las cuentas que hacen referencia a los Socios del Negocio
y será donde se definan las cuentas por defecto que utilizará el sistema
para cargar los siguientes niveles de definición contable para los
Socios del Negocio. Si se desea mantener una definición contable única
para todos los Socios del Negocio, sólo será necesario definir las
cuentas contables en este nivel, y las mismas se definirán en todos los
Socios del Negocio.

.. image:: /api/v3/attachments/630/content

A partir de estas cuentas definidas por defecto en el Esquema Contable,
se definirán en el siguiente nivel de definición contable de productos,
el **2do nivel** para los productos será según la **"Grupo de Socios del
Negocio".** Dentro de cada Grupo de Socio del Negocio podrá ver una
pestaña de Contabilidad donde se podrá, en caso que se desee, modificar
las cuentas contables que desee utilizar según el Grupo de Socios del
Negocio que sea. De esta manera, es vital la correcta clasificación de
los Socios del Negocio con su correcto "grupo de Socios del Negocio" ya
que a partir de ella, se definirá su correspondiente definición
contable.

.. image:: /api/v3/attachments/631/content

El 3er y último nivel será el de "Socios del Negocio", al crear un nuevo
Socios del Negocio es obligatorio definir que Grupo de Socios del
Negocio le corresponde, a partir del mismo se tomará su definición
contable definida. En caso de que se desee modificar la definición
contable específicamente de un Socios del Negocio, será posible
simplemente modificando la cuenta que desee de la definición contable
del Socios del Negocio en cuestión.

De no encontrar una cuenta definida en el Socio del Negocio, no se podrá
completar el asiento contable en cuestión, quedando dicho documento con
“Error de Posteo”.

.. image:: /api/v3/attachments/632/content

Configuración de las cuentas contables en Bancos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Por otro lado se encuentran los Cuentas Bancarias definidos en el Solop.
Para este caso las cuentas contables sólo tendrán dos niveles.

En el 1er Nivel, el más abarcativo, que podremos llamar **nivel
superior**, podremos encontrar las cuentas definidas en el "Esquema
Contable", dentro del grupo de campos de **"Banco"** encontraremos las
cuentas que hacen referencia a las Cuentas Bancarias y será donde se
definan las cuentas por defecto que utilizará el sistema para cargar en
la definición contable para las Cuentas Bancarias que creen. Si se desea
mantener una definición contable única para todos las Cuentas Bancarias,
sólo será necesario definir las cuentas contables en este nivel, y las
mismas se definirán en todas.

.. image:: /api/v3/attachments/633/content

El 2do nivel y último estará la definición contable que tengan cada una
de las Tasas de Impuesto definidas en el sistema.

.. image:: /api/v3/attachments/636/content