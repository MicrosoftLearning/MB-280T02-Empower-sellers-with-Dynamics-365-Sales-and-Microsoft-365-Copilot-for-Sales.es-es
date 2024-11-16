---
lab:
  title: 'Laboratorio 2.1: Administración de clientes potenciales y oportunidades'
---

# Módulo 2: Administración de posibles clientes y oportunidades con Dynamics 365 for Sales

## Laboratorio de prácticas 2.1: Administración de clientes potenciales y oportunidades

### Escenario
Contoso Coffee desea Dynamics 365 Sales para formalizar su proceso de ventas, así como abordar un trabajo pendiente de clientes potenciales intactos importados por el equipo de marketing de las ferias comerciales y las campañas. Como analista de ventas de Contoso Coffee, se te ha pedido que evalúes y actualices los registros de clientes principales para asegurarte de que el equipo ejecutivo trabajará con un informe de canalización preciso en la próxima reunión de liderazgo.

Al completar este laboratorio, podrás hacer lo siguiente:
- Crea y actualiza los registros de clientes potenciales
- Calificar o descalificar clientes potenciales.
- Reactivar registros de clientes potenciales

### Ejercicio 1: Administración de clientes

#### Tarea 1: Creación de clientes potenciales
En esta tarea, crearás tres clientes potenciales, uno sin información sobre la compañía y dos con información sobre la compañía.
1. Vaya a su aplicación Centro de ventas de Dynamics 365. Asegúrate de que estás en el área Ventas con el menú desplegable de la parte inferior izquierda.
2. Usando la navegación de la izquierda, en el grupo Ventas, selecciona **Clientes potenciales.**
3. En el panel Elementos de trabajo, selecciona **Cuadrícula de solo lectura** para cambiar el tipo de vista.
4. En el menú que aparece, selecciona el botón **+ Nuevo**.
5. Escribe *Cliente potencial de cafetera sin compañía* en Tema, *Jane* en Nombre, *Doe* en Apellido.
6. Acepta la sugerencia **Administrador de cafeterías** que se ha rellenado en el campo Puesto.
7. Selecciona el botón **Guardar**. En la barra de comandos de la parte superior, selecciona de nuevo **+ Nuevo**.
8. Escribe *Cliente potencial de cafetera con compañía* en Tema, *Jon* en Nombre, *Doe* en Apellido, *Doe Inc.* en Compañía y haz clic en **Guardar.**
9. En la barra de comandos, selecciona el botón **+ Nuevo** una vez más.
10. Escribe *Otro cliente potencial de cafetera* en Tema, *Jack* en Nombre, *Rogers* en Apellido, *Test Coffee Shop, Inc.* en Compañía y haz clic en **Guardar.**

### Ejercicio 2: Calificaciones de liderazgo
En este ejercicio, calificarás o descalificarás a los clientes potenciales y verás qué registros se crean cuando un cliente potencial pase por el proceso de calificación.

#### Tarea 1: Calificar cliente potencial de cafetera sin información sobre la compañía
1. Ve a tu aplicación Centro de ventas.
2. Selecciona **Clientes potenciales.**
3. En el panel Elementos de trabajo, haz clic en el botón **Cuadrícula de solo lectura**.
4. Busca **Cliente potencial de cafetera sin empresa** y selecciónalo.
5. Haz clic en **Calificar** en el menú superior.
6. El cliente potencial se calificará en un nuevo registro de oportunidad.
   - **NOTA:** Si la nueva oportunidad no se abre automáticamente, selecciona Oportunidades en el menú izquierdo para ver todas las oportunidades abiertas. Después, abre el cliente potencial de cafetera sin la oportunidad de la compañía.
7. Busca el campo Contacto. Verás que Jane Doe es ahora un registro de contacto en la aplicación que puedes abrir.
8. Busca el campo Cuenta (en el encabezado del registro de oportunidad). Observa que el campo está vacío.
9. Haga clic en **Save**(Guardar).

#### Tarea 2: Calificar cliente potencial de cafetera con compañía
1. Ve a tu aplicación Centro de ventas.
2. Selecciona **Clientes potenciales**.
3. Busca Cliente potencial de cafetera con empresa y ábrelo.
4. Haz clic en **Calificar** en el menú superior.
5. El cliente potencial se calificará como el cliente potencial anterior y se te dirigirá al registro de oportunidad recién creado del cliente potencial calificado.
6. Busca el campo Contacto. Verás que Jon Doe es ahora un registro de contacto.
7. Busca el campo Cuenta. Verás que Doe, Inc. es ahora un registro de cuenta.

#### Tarea 3: Descalificar un cliente potencial
1. Si es necesario, ve a tu aplicación Centro de ventas.
2. Selecciona **Clientes potenciales.**
3. Busca otro cliente potencial de cafetera y ábrelo.
4. Haz clic en **Descalificar** (es posible que tengas que seleccionar el botón de puntos suspensivos verticales para que se muestre).
5. Después, en el menú que aparece, selecciona **Sin interés**.
6. El cliente potencial se descalificará, el estado cambiará a Sin interés y el registro pasará a ser de solo lectura.

#### Tarea 4: Reactivar un cliente potencial
1. Si es necesario, ve a tu aplicación Centro de ventas.
2. En la navegación del sitio, en el grupo Ventas, selecciona **Clientes potenciales.**
3. El cliente potencial que descalificaste ya no está en la vista Mis clientes potenciales abiertos. Selecciona la flecha abajo situada junto a Mis clientes potenciales abiertos y cambia la vista a **Clientes potenciales cerrados.**
4. Busca el cliente potencial de cafetera y ábrelo.
5. Haz clic en **Reactivar cliente potencial**.
6. El cliente potencial se reactivará, el estado cambiará a Nuevo y el registro se volverá modificable.

### Ejercicio 3: Trabajar con oportunidades
En este ejercicio, recorrerás el proceso de trabajo de una oportunidad a través del proceso de ventas.

#### Tarea 1: Administrar cliente potencial de cafetera con compañía
1. Si es necesario, ve a tu aplicación Centro de ventas.
2. En la navegación de la izquierda, selecciona **Oportunidades** en el grupo Ventas.
3. Busca y abre la oportunidad **Cliente potencial de cafetera con compañía**.
4. En el panel Oportunidad que aparece, selecciona el **botón Acceso a main** (ubicado junto al botón X (Cerrar)).
5. Completa el registro de oportunidad como sigue:
   - Importe del presupuesto: 17 000 $
   - Período de tiempo de compra: este trimestre
   - Proceso de compra: Comité
   - Descripción: desean actualizar sus cafeteras actuales en varias ubicaciones.
6. Expande el encabezado de registro en la parte superior y complétalo de la siguiente manera:
   - Ingresos Fecha de cierre: escribe la fecha de mañana.
   - Ingresos Ingresos: 16 500 $
7. En el control Escala de tiempo, selecciona el **+** (agregar un registro de escala de tiempo).
8. En el menú que aparece, selecciona **Llamada de teléfono.**
9. Completa la llamada de teléfono como se muestra a continuación:
   - Asunto: Llamada inicial a Jon.
   - Límite: escribe la fecha de hoy a las 16:30
10. Seleccione el botón **Guardar y cerrar**.
11. Con la oportunidad abierta, selecciona la **Fase de desarrollo** en el flujo de proceso de negocio de cliente potencial a oportunidad. Realice los pasos siguientes:
   - Necesidad del cliente: desean actualizar sus cafeteras en varias ubicaciones.
   - Solución propuesta: recomendar varias máquinas AirPot Duo.
   - Identificar partes interesadas: completado
   - Identificar competidores: completado
12. Selecciona el botón **Fase siguiente**.
13. En la fase Proponer, establece todos los campos en **Completado.**
14. Selecciona el botón **Fase siguiente**.
15. Selecciona cualquier lugar fuera de la fase de proceso de negocio para cerrarlo.
16. En la sección Asistente, en Notificaciones, selecciona el elemento **Llamada telefónica** que has creado anteriormente para abrirlo.
17. Seleccione **Complete**. (Observa que el elemento desaparece de tus notificaciones).
18. Selecciona **Cerrar fase** en el Proceso de ventas de cliente potencial a oportunidad.
19. Marca todos los elementos de Cerrar fase como **Completado.**
20. Seleccione el botón **Finalizar**.
21. En la barra de comandos de la parte superior, selecciona el botón **Cerrar como ganada**.
22. En la pantalla Cerrar oportunidad, selecciona el botón **Aceptar**.

Enhorabuena, has creado y administrado correctamente clientes potenciales y oportunidades en Dynamics 365 Sales.
