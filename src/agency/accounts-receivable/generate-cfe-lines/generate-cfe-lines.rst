.. |Criterio de Facturación DxC| image:: resource/dxc.png
.. |Criterio de Facturación SDN| image:: resource/sdn.png

**Generar Líneas de CFE**
~~~~~~~~~~~~~~~~~~~~~~~~~

En vista a que las líneas del Documento por Cobrar no siempre se
corresponden con las líneas a enviar en el CFE e imprimir en la
representación impresa, además de disponer en esta venta a de las líneas
del documento (la pestaña convencional), se ha agregado una pestaña
donde figuran las líneas que deberán enviarse en el CFE.

A grandes rasgos es la misma información que las líneas convencionales
del Documento por Cobrar solo que en un estado más resumido.

**Precondición:** Para generar o Modificar las líneas CFE, la factura no
puede estar completa porque en este caso ya estaría enviada a DGI y no
tendría sentido realizar modificaciones sobre sus respectivas líneas.

**Observación:** No aplica para Resguardos

En el cabezal del Documento por Cobrar en la sección Facturación hay un
campo llamado **“Criterio de Facturación”**, este campo indica dentro de
este documento cómo deben agruparse sus respectivas líneas (en orden
jerárquico).

|Criterio de Facturación DxC|

-  Factura: Realizará solo una línea agrupando todas las líneas de este
   documento: Descripción de línea queda vacío, deberá completarse
   manualmente
-  Contrato: Descripción de línea: (Línea Factura) -> Proyecto ->
   Contrato.Nombre (Ver Nota 1)
-  Proyecto: Descripción de línea: (Línea Factura) -> Descripción del
   Proyecto (Ver Nota 1)
-  Fase de Proyecto: Descripción de línea: (Línea Factura) ->
   Descripción de Fase (Ver Nota 2)
-  Línea: Descripción de línea: (Línea Factura) -> Si tengo Producto
   utilizo su nombre y descripción, Si no tengo Producto pero si Cargo
   utilizo Nombre y Descripción del Cargo. Si no tengo ninguno retornará
   un error.

**Nota 1: Siempre que para todas las líneas de Factura tenga el mismo
proyecto, en caso contrario quedará vacío**

**Nota 2: Siempre que para todas las líneas de Factura tenga la misma
fase de proyecto, en caso contrario quedará vacío**

**Configuración del Socio del Negocio**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Criterio de Líneas en Factura**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

En cada Socio del Negocio se podrá pre configurar el criterio de
facturación que se desee. Esto se debe definir en la pestaña Cliente de
la ventana Socio del Negocio en el campo Criterio de Facturación.

|Criterio de Facturación SDN|