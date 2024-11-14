---
lab:
  title: 'Laboratorio 3.2: Elaborar ofertas'
---

# Módulo 3: Administración de pedidos y del catálogo de productos con Dynamics 365

## Laboratorio de prácticas 3.2: Elaborar ofertas

### Escenario
Como analista de ventas para la implementación de Dynamics 365 Sales en Contoso Coffee, quieres asegurarte de que los vendedores podrán aprovechar las mejoras del catálogo de productos durante todo el ciclo de vida de ventas. Para asegurarte de que la funcionalidad funciona correctamente, probarás el proceso de creación de una oferta a partir de una nueva oportunidad.

Al completar este laboratorio, podrás hacer lo siguiente:
- Crear oportunidades y agregar elementos de línea de oportunidad
- Generar una oferta a partir de una oportunidad

### Ejercicio 1: Crear una oferta

#### Tarea 1: Agregar elementos de línea de productos
En esta tarea, crearás una oportunidad y agregarás elementos de línea de productos.
1. Vaya a su aplicación Centro de ventas de Dynamics 365.
2. En el menú izquierdo, en el grupo Ventas, selecciona **Oportunidades.**
3. Haga clic en **+ Nuevo**.
4. Escribe *Interesado en accesorios Airpot XL* en Tema y selecciona **Jon Doe** en Contacto.
5. En el encabezado del registro en la parte superior selecciona la **flecha abajo** junto al campo Propietario, y elige **Test Coffee Shop, Inc.** en Cuenta. Seleccione **Guardar**.
6. Seleccione la pestaña **Productos**.
7. Debes seleccionar una lista de precios para poder agregar productos de oportunidad. Selecciona **Filtrar directo** en Lista de precios.
8. Selecciona **Calculado por el sistema** en Ingresos.
9. Encima de la subcuadrícula, haz clic en **+ Agregar productos.**
10. En la lista Todos los productos, busca **Airpot XL 6 Month Filter**, escribe *6* en Cantidad, selecciona **Agregar.**
11. Busca **AirpotXL Pot Extender** en la lista de productos, escribe *1* en Cantidad y selecciona **Agregar.**
12. Busque **Airpot XL Reservoir Extension** en la lista de productos, escribe *1* en Cantidad y selecciona **Agregar.**
13. Verás que se han agregado tres productos. Seleccione **Guardar**.
14. Haz doble clic en el producto **Airpot XL 6 Month Filter**.
15. Busca el campo Descuento por volumen. Verás que no hay ningún descuento.
16. Cambia la Cantidad a *15* y haz clic fuera del campo. El descuento se iniciará ahora y el campo Descuento por volumen mostrará el valor con descuento.
17. Seleccione **Guardar y cerrar**.

#### Tarea 2: Crear oferta
En esta tarea, crearás una oferta a partir de Oportunidad que has creado en la tarea 1.
1. Si aún no está ahí, ve a tu aplicación del centro de Dynamics 365 Sales.
2. Si es necesario, abre la oportunidad que has creado en la tarea anterior. Se llamará **Interesado en accesorios de Airpot XL.**
3. Selecciona la pestaña **Ofertas**.
4. Encima de la subcuadrícula, haz clic en **+ Nueva oferta.**
5. Se abrirá el formulario Oferta y se copiará la información pertinente de Oportunidad.
6. En la página de la oferta Interesados en accesorios de Airpot XL, examina la subcuadrícula de productos y asegúrate de que los productos y sus cantidades se muestran como esperabas. Puedes cambiar las cantidades y descontar el precio de cada artículo de línea.
7. En la barra de comandos, selecciona **Activar oferta.** (Según el tamaño del explorador, es posible que tengas que seleccionar los puntos suspensivos para ver esta opción).
8. Haz clic en **Exportar a PDF** ubicado en la barra de comandos y selecciona **Imprimir oferta para cliente.** Haga clic en **Descargar**.
9. Abre el documento generado y ve el aspecto de la oferta.
10. Cierra el PDF.
11. Cierre la ventana Exportar a PDF.

