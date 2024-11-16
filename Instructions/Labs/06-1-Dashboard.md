---
lab:
  title: 'Laboratorio 6.1: Configurar un panel'
---

# Módulo 6: Análisis de datos de Dynamics 365 Sales

## Laboratorio de práctica 6.1: Configurar un panel

### Escenario
Los jefes de ventas de Contoso Coffee quieren supervisar el éxito del equipo de ventas de forma más eficaz, especialmente en torno a las oportunidades cerradas. Un jefe de ventas ha solicitado un panel personal que les proporcionará una visión general de las oportunidades cerradas recientemente y las acciones de sus vendedores en ellas. Además, les gustaría que este panel fuera su panel predeterminado cuando abran la sección Paneles de la aplicación.

Al completar este laboratorio, podrás hacer lo siguiente:
- Creación de paneles personales
- Agregar componentes a paneles

## Ejercicio 1: Configurar un panel 
### Tarea 1: Creación de un panel
1. Asegúrate de que te encuentras en el área Ventas de la aplicación, si aún no lo estás. Usa el menú desplegable de la parte inferior izquierda para cambiar el área a **Ventas** si necesitas cambiar.
2. En el grupo Mi trabajo, selecciona **Paneles** en el menú de navegación izquierdo.
3. De forma predeterminada, aparecerá el panel social de actividad de ventas. No dudes en explorar los distintos componentes. Además, puedes usar el icono desplegable <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>˅<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> junto al título del panel para explorar los demás paneles del sistema.
4. Cuando estés listo para crear tu propio panel, selecciona **+ Nuevo** y luego selecciona **Panel de Dynamics 365**:
5. Explora los distintos diseños del panel. En esta tarea, crearemos un panel normal de 2 columnas. Cuando estés listo, selecciónalo de la lista y selecciona **Crear.**

### Tarea 2: Agregar componentes
1. El diseñador de paneles se abrirá en una nueva ventana. (Si el nuevo panel no se abre en una nueva ventana, asegúrate de que el bloqueador de elementos emergentes está deshabilitado). El diseñador puede tardar un minuto en cargarse.
2. En el cuadro de texto Nombre, escribe *Panel del jefe de ventas*.
3. Vamos a agregar un componente a la sección superior izquierda. Los jefes de ventas solicitan una manera fácil de ver la cantidad de ganancias frente a los ingresos perdidos de las oportunidades. Les gustaría esta información en una vista gráfica. Para ello, agregaremos un gráfico seleccionando el icono **Insertar gráfico** en el centro de la sección superior izquierda.
4. Selecciona los detalles siguientes para el gráfico:
   - Tipo de registro: Oportunidad
   - Vista: Oportunidades cerradas
   - Gráfico: Operaciones ganadas frente a operaciones perdidas
   - Seleccione **Agregar**.
5. El gráfico aparecerá en la sección superior izquierda.
6. A continuación, vamos a agregar un componente a la sección superior derecha. Los jefes de ventas solicitan una manera de ver fácilmente las oportunidades recientemente cerradas para que puedan comunicar a los vendedores las lecciones aprendidas. Les gustaría que la vista incluya oportunidades ganadas y perdidas, pero solo las oportunidades cerradas en el año fiscal actual. Selecciona el icono **Insertar lista** para la sección superior derecha.
7. Selecciona los detalles siguientes para tu lista:
   - Tipo de registro: Oportunidades
   - Vista: Oportunidades cerradas en el año fiscal actual
   - Haga clic en **Agregar**.

### Tarea 3: Guardar y editar el panel
1. Selecciona **Guardar** y luego **Cerrar**. La ventana se cerrará y se te devolverá al formulario Paneles, donde se mostrará el nuevo panel.
2. En la barra de comando, selecciona **Establecer como predeterminado**. Este panel ahora será el panel predeterminado al navegar a la sección Paneles.
3. Haz clic en **Editar** en el menú superior. Volverás al diseñador de paneles en otra ventana nueva. Agrega dos componentes más debajo del gráfico. Los componentes que selecciones deben resolver los siguientes requisitos empresariales solicitados por los jefes de ventas:
   - Los jefes de ventas quieren tener una idea de cómo lo están haciendo los vendedores individuales en función de sus ingresos de oportunidades cerradas. Les gustaría un gráfico que muestra los nombres de los vendedores y sus ingresos totales de oportunidades cerradas.
   - Los jefes de ventas quieren supervisar las tareas diarias de los vendedores en su equipo. Les gustaría ver una lista que muestre las actividades de sus equipos de ventas.
