**Actualización de Cálculo de comisiones para Honorarios**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se deberán seguir los siguientes pasos:

-  Desde el Contrato de servicio, pestaña Honorarios modificaremos el
   campo “Multiplicador” al Honorario en cuestión que queramos
   modificar, indicando aquí el nuevo valor. Guardamos el registro.
-  Luego desde la Orden de venta a la que se aplicaron los honorarios
   correremos el proceso “Actualizar Cálculo de Comisión de Orden”

De esta manera los Cálculos de comisiones generados antes de aplicar
este proceso serán Cerrados al igual que su Orden de venta Honorarios.

Se generarán los nuevos  Cálculos de comisiones aplicando los nuevos
porcentajes definidos y una nueva Orden de venta honorarios en estado
Completo.

**Actualización de Cálculo de comisiones por Comisiones al proveedor**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se deberán seguir los siguientes pasos:

-  Desde el proveedor en la ventana Socio del negocio, pestaña
   Comisiones del proveedor modificaremos el campo “Multiplicador” a la
   comisión en cuestión que queramos modificar, indicando aquí el nuevo
   valor. Guardamos el registro.
-  Luego desde la Orden de compra a la que se aplicaron los honorarios
   correremos el proceso “Actualizar Cálculo de Comisión de Orden”

De esta manera los Cálculos de comisiones generados antes de aplicar
este proceso serán Cerrados al igual que su Orden de venta por la
comisión.

Se generarán los nuevos Cálculos de comisiones aplicando los nuevos
porcentajes definidos y una nueva Orden de venta en estado Completo.

**¿Por qué motivo puede que un Cálculo de comisión solo considere la línea que está facturada de una Orden?**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El cálculo de comisión que se genera desde la Orden de Compra para que
funcione correctamente no debe tener facturado parcialmente ninguna
línea, ya que si lo tiene, el cálculo se realizará considerando dicha
cantidad facturada y no la totalidad.

SOLUCIÓN: Si esto sucede se sugiere realizar una Orden de Venta Comisión
MANUALMENTE por el total. Recordar definir todos los campos que tienen
las Ordenes de Venta Comisión automáticas (Proyecto y Contrato de
Servicios).