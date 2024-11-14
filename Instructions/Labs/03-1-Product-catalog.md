---
lab:
  title: 'Laboratorio 3.1: Configurar el catálogo de productos'
---

# Módulo 3: Administración de pedidos y del catálogo de productos con Dynamics 365

## Laboratorio de práctica 3.1: Administrar el catálogo de productos

### Escenario
A medida que crece Contoso Coffee, desea estandarizar su estructura de precios y permiten la creación más sencilla de ofertas, pedidos y facturas con precios y detalles de producto más precisos. Contoso Coffee acaba de presentar su cafetera inteligente más reciente. Como consultor funcional de su implementación de Dynamics 365 Sales, se te ha pedido que configures el catálogo de productos.

Al completar este laboratorio, podrás hacer lo siguiente:
- Creación de grupos de unidad
- Definición de listas de precios
- Creación de listas de descuentos
- Define productos y familias de productos

### Ejercicio 1: Catálogo de productos

#### Tarea 1: Crear unidad de venta
En esta tarea, crearás unidades de venta para una línea de filtros de cafetera.
1. Vaya a su aplicación Centro de ventas de Dynamics 365.
2. Haz clic en el menú Cambiar área (ubicado en la parte inferior izquierda de la pantalla). De forma predeterminada, las ventas se mostrarán en la parte inferior del menú izquierdo.
3. En el menú que aparece, seleccione **Configuración de la aplicación**.
4. Selecciona **Unidades de venta** en la sección Catálogo de productos del menú izquierdo.
5. Haga clic en **+ Nuevo**.
6. Escribe **Filtros** en Nombre, escribe **Cada** en Unidad principal y haz clic en **Aceptar.**
7. Una vez abierta la unidad de ventas, selecciona la pestaña Relacionado y elige **Unidades.**
8. Verás que solo tiene la unidad predeterminada Cada ahora; agregarás tres unidades más. Haz clic en **+Nueva unidad.**
9. Escribe <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</bpt></bpt>Filtro<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</ept></ept> en Nombre, <bpt ctype="x-unknown" id="3" rid="2"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</bpt></bpt>1<ept id="4" rid="2"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</ept></ept> en Cantidad, selecciona <bpt ctype="x-unknown" id="5" rid="3"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</bpt></bpt>Cada<ept id="6" rid="3"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</ept></ept> en Unidad base y haz clic en <bpt ctype="x-unknown" id="7" rid="4"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</bpt></bpt>Guardar y crear nuevo<ept id="8" rid="4"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</ept></ept> seleccionando el <bpt ctype="x-unknown" id="9" rid="5"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</bpt></bpt>icono desplegable ˅<ept id="10" rid="5"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</ept></ept> situado a la derecha del botón Guardar y cerrar.
10. Escribe *Pack* en Nombre, *2* en Cantidad, selecciona **Filtrar** en Unidad base y haz clic en **Guardar y crear nuevo.**
11. Escribe *Paquete de valores* en Nombre, *2* en Cantidad, selecciona **Paquete** en Unidad base y haz clic en **Guardar y cerrar.**
12. Ahora deberías tener cuatro grupos de unidades en la lista.

#### Tarea 2: Crear lista de descuentos
En esta tarea, crearás una lista de descuentos para personas que compren 15 o 20 filtros o más. Los 15 filtros obtendrán un descuento del 15 % y de 20 a 50 filtros obtendrán un descuento del 25 %.
1. Selecciona **Listas de descuentos** en la sección Catálogo de productos del menú izquierdo.
2. Haga clic en **+ Nuevo**.
3. Escribe *Descuento por cantidad* en Nombre, selecciona **Porcentaje** en Tipo y haz clic en **Guardar.**
4. Haz clic en **Relacionado** y elige **Descuentos.**
5. Haz clic en **+ Nuevo descuento.**
6. Asegúrate de que Descuento por cantidad está seleccionado para Tipo de descuento, escribe *15* en Cantidad inicial, *19* en Cantidad final, *15* en Porcentaje y haz clic en **Guardar.**
7. Vuelva a hacer clic en **+ Nuevo**.
8. Selecciona **Descuento por cantidad** en Tipo de descuento. Después, escribe *20* en Cantidad inicial, *50* en Cantidad final, escribe *25* en Porcentaje y haz clic en **Guardar.**

#### Tarea 3: Crear lista de precios
En esta tarea, crearás una lista de precios para los filtros.
1. Selecciona **Listas de precios** en la sección Catálogo de productos del menú izquierdo.
2. Haga clic en **+ Nuevo**.
3. Escribe *Filtro directo* en Nombre, selecciona **Dólar estadounidense** en Moneda y haz clic en **Guardar y cerrar.**

#### Tarea 4: Crear productos
En esta tarea, crearás productos.
1. Haz clic en el área de cambios **Configuración de la aplicación**.
2. Selecciona **Ventas.**
3. Selecciona **Productos** en la sección Garantía del menú izquierdo.
4. Haga clic en **Agregar producto.**
5. Escribe *Airpot XL 6 Month Filter* en Nombre, *AXL6MF-1234* en Id. de producto, **Filtros** en Grupo de unidades, **Filtro** en Unidad predeterminada, *2* en Decimales admitidos y haz clic en **Guardar.**. (Es posible que tengas que seleccionar la marca de verificación azul junto a los decimales admitidos para aceptar la sugerencia).
6. Selecciona la pestaña **Detalles adicionales**.
7. Haz clic en los **puntos suspensivos verticales** de la parte superior derecha de la sección Artículos de lista de precios. Haz clic en el elemento **+ Nueva lista de precios**.
8. Selecciona **Filtro directo** en Lista de precios, selecciona **Descuento por cantidad** en Lista de descuentos y selecciona **Completa** en Opción de la unidad de venta.
9. Selecciona la pestaña **Información de precios**, escribe *25* en Importe y selecciona **Guardar y cerrar.**
10. Si la publicación automática está habilitada, omite este paso. (Publicar no aparecerá en la barra de comandos). De lo contrario, selecciona **Publicar** y **Confirmar** para publicar el producto.
11. En el menú de la izquierda, selecciona **Productos** en el grupo Garantía.
12. Haga clic en **Agregar producto.**
13. Escribe *Airpot XL Reservoir Extension* en Nombre, escribe *AXLRE-4321* en Id. de producto, selecciona **Unidad predeterminada** en Grupo de unidades, selecciona **Unidad principal** en Unidad predeterminada, selecciona la marca de verificación azul junto al 2 en Decimales admitidos y haz clic en **Guardar.**
14. Selecciona la pestaña **Detalles adicionales**.
15. Haz clic en los **puntos suspensivos verticales** de la parte superior derecha de la sección Artículos de lista de precios. Haga clic en **+ Nuevo elemento de lista de precios.**
16. Selecciona **Filtrar directo** en Lista de precios. Selecciona **Completa** en Opción de la unidad de venta.
17. Selecciona la pestaña **Información de precios**, escribe *299 $* en Importe y selecciona **Guardar y cerrar.**
18. Si la publicación automática está habilitada, omite este paso. De lo contrario, selecciona **Publicar** y **Confirmar** para publicar el producto.
19. Selecciona **Productos** en el menú de la izquierda.
20. Haga clic en **Agregar producto.**
21. Escribe *Airpot XL Pot Extender* en Nombre, escribe *AXPLE-7894* en Id. de producto, selecciona **Unidad predeterminada** en Grupo de unidades, selecciona **Unidad principal** en Unidad predeterminada, marca la casilla azul junto al 2 en Decimales admitidos y haz clic en **Guardar.**.
22. Selecciona la pestaña **Detalles adicionales**.
23. Haz clic en los **puntos suspensivos verticales** de la parte superior derecha de la sección Elementos de lista de precios. Haga clic en **+ Nuevo elemento de lista de precios.**
24. Selecciona **Filtrar directo** en Lista de precios. Selecciona **Completa** en Opción de la unidad de venta.
25. Selecciona la pestaña **Información de precios**, escribe *199* en Importe y selecciona **Guardar y cerrar.**
26. Si la publicación automática está habilitada, omite este paso. De lo contrario, selecciona **Publicar** y **Confirmar** para publicar el producto.
27. En el menú de la izquierda, selecciona **Productos.**
28. Los productos que has creado deben aparecer en la vista Todos los productos, familias y agrupaciones. Para cambiar a esta vista, selecciona el <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>icono desplegable ˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> situado junto al título de vista predeterminada. 
