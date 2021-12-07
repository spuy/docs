.. _ERPyA: http://erpya.com
.. _src/adempiere/performance-analysis:

====================
**Gestión Contable**
====================

En publicaciones previas hemos dejado claro la importancia que ha tenido para las pequeñas y medianas empresas la intervención de un ERP como ADempiere para automatizar y aceleran los procesos, y finalmente obtener información financiera confiable que facilite la toma de decisiones. Definitivamente las tareas manuales y los software  aislados no satisfacen las necesidades que tienen los departamentos de contabilidad, en especial para las empresas en constante crecimiento donde el volumen de tareas aumenta notoriamente.

Tu empresa puede obtener incontables mejoras en la gestión contable con ADempiere ERP, puesto que esta herramienta permite obtener desde la gestión administrativa los registros contables de una manera efectiva e inmediata a través de un mismo software.

ADempiere ofrece la posibilidad de contar con cierres contables ágiles, automatizando los procesos contables que permite agilizar el cierre mensual y anual de las operaciones financieras gracias al acceso de la información en tiempo real.

Asimismo, ofrece opciones con las cuales la empresa puede acceder a datos estadísticos, para crear informes personalizados, preparar presupuestos, manejo de costos de material, costos adicionales, distribuciones contables automáticas, centro de costos, actividades ABC y manejar todas las cuentas bajo dimensiones contables, y así, tener un mayor control sobre las operaciones financieras de la empresa y los costos en los que incurre cada una de las actividades del negocio.

El propósito de `ERPyA`_ es apoyar a nuestros clientes, dar respuestas rápidas y eficientes a sus problemas con el manejo de información para permitir la toma de decisiones y minimizar los costes.

Generalidades
-------------

A continuación se explicará la filosofía de la contabilidad en Solop. Se
responde a la pregunta: ¿Qué es la Contabilidad en Solop?

No se va a explicar aquí detalladamente cómo funciona la Contabilidad ni
cómo manejarla porque ése será el enfoque de otros capítulos.

La contabilidad de Solop está altamente automatizada; eso concretamente
significa que al ejecutarse cualquiera de los siguientes
Procesos/Documentos Solop automáticamente crea los asientos contables,
realizando cálculos de costos, impuestos, etc.

-  Compras
-  Ventas
-  Recibo de material
-  Entrega de material
-  Pagos
-  Cobros
-  Inventario
-  procesos de Nómina
-  procesos de Activos fijos
-  Producción
-  etc.

Para poder lograrlo, se requiere configurar previamente a Solop como se
desea contabilizar. Una vez que Solop haya sido configurado, los
usuarios sólo necesitan ejecutar los procesos arriba mencionados
(Compras, Ventas, etc.) y la Contabilidad se generará automáticamente
sin necesitar prácticamente gestión humana.

**Asientos Diarios Manuales**

Se requerirán asientos contables manuales cuando sea preciso ejecutar
movimientos especiales, como por ejemplo cuando se requiera mover
cuentas de ganancias de capital o semejantes o que el auditor sugiera
ejecutar ciertos movimientos contables. En los demás casos, Solop maneja
la Contabilidad automáticamente.

Contabilidad en Solop
---------------------

La Contabilidad es el centro de cualquier sistema ERP donde se recopila
toda la información financiera para posteriormente analizarla de forma
resumida mediante estados financieros y así poder tomar decisiones
empresariales.

El objeto central de la Contabilidad es el *Catálogo de Cuentas*, que se
define en la ventana *Elemento Contable*, pestaña *Valor de Elemento*.

Comúnmente,  el *Catálogo de Cuentas* es importado durante la
implementación de Solop, y sólo se modifica para añadir una cuenta
cuando sea requerido. Por ejemplo, si se añade una cuenta bancaria, o un
nuevo impuesto.

Los datos maestros sujetos a configuración y ajustes en las cuentas
contables son:

-  Grupo de Socios Del Negocio
-  Socios Del Negocio
-  Categoría de Producto
-  Producto
-  Cargo
-  Cuentas bancarias
-  Impuestos

En cada uno de estos datos maestros existe una pestaña *Contabilidad*
donde se puede configurar la contabilidad de cada registro.

Las reglas contables de Solop operan solamente sobre la configuración
contable de los siguientes datos maestros:

-  Socios Del Negocio
-  Producto
-  Cargo
-  Cuentas bancarias
-  Impuestos

En la ventana *Esquema Contable*, pestaña *Por Defecto*, se encuentran
las cuentas (en realidad combinaciones contables, pero por simplicidad,
llamémosles cuentas) de las cuales se alimentan los datos maestros
arriba mencionados.

Detalle de los asientos contables
---------------------------------

Los asientos contables en Solop no son comprimidos, sino que son tan
detallados como uno desee, es decir, cuantan con información muy atómica
de cada acción desde donde son generados.

Esto trae como consecuencia que los reportes contables en Solop sean un
resumen de muchos asientos contables. Eso es una diferencia con también
con las otras contabilidades que prácticamente del asiento contable ya
está resumido, en Solop no; el asiento contable es muy detallado.

**Cuentas Puente**
------------------

Debido a la alta automatización con la que cuenta Solop permitiendo que
cada Documento genere el impacto contable que le corresponde, esto
ocasiona que en varios de los procesos normales empresariales, Solop
maneje Cuentas Puente que irán regularizando lo que "El Documento" en sí
sabe que puede aplicar contablemente. Esto permite que siempre se cuente
con una realidad exacta, permitiendo cada una de las acciones que pueden
ser posibles de darse en el ambito empresarial, puedan ser reflejada
automáticamente en la contabilidad y no requiera de ningún ajuste
posterior ni control de que ocurra alguna acción adicional para poderlo
contabilizar.

Estas Cuentas Puente serán completamente controladas y verificadas con
reportes auxiliares que explicarán en términos más simples, cómo se
ocasiona cierto saldo en cada una de ellas.

.. toctree::
    :maxdepth: 2

    type-of-application
    accounting-element/index
    opening-accounting-period
    unposted-documents
    accounting-dimensions
    accounting-combination
    currency-conversion/index
    gl-distribution/index
    accounting-setup-master/index
    transaction-accounting/index
    re-posting-accounting-data-from-profit-and-loss-accounts
    costing/index
    gl-journal-batch/index
    accounting-reports/index
