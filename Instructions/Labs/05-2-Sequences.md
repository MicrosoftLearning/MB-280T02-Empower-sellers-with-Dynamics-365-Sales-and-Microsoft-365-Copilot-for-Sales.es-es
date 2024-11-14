---
lab:
  title: 'Laboratorio 5.2: Creación de una secuencia'
---

# Módulo 5: Trabajar con Dynamics 365 Sales Insights y el Acelerador de ventas 

## Laboratorio de práctica 5.2: Creación de una secuencia

### Escenario
Los vendedores de Contoso Coffee sugieren que las ventas podrían mejorarse si los "procedimientos recomendados" de la organización fueran más fáciles de seguir. Tras un examen, los jefes de ventas de Contoso han determinado una secuencia ideal de eventos de ventas para vendedores. Quieren aplicar procedimientos recomendados configurando una serie de actividades consecutivas para que los vendedores sigan mientras califican a los clientes potenciales. Quieres asegurarte de que sea lo más fácil de seguir posible para los vendedores durante su día. Has determinado que una secuencia es la mejor manera de lograrlo.

Al completar este laboratorio, podrás hacer lo siguiente:

-   Crear un segmento
-   Crear una secuencia
-   Definir actividades de secuencia
-   Activar y conectar secuencias con registros

## Ejercicio 1: Crear y adjuntar secuencias a registros

### Tarea 1: Habilitar el Acelerador de ventas

1.  En el grupo Sales Insights, selecciona **Configuración global.**
2.  En el grupo Acelerador de ventas, selecciona la pestaña **Secuencias**.
3.  Se te pedirá que configures el área de trabajo para poder usar Secuencias. Selecciona el botón **Configurar espacio de trabajo**.
4.  Selecciona el botón **Configuración rápida**.
5.  En la sección Tipo de registro y formulario, selecciona **+ Agregar tipo de registro**. Selecciona **Oportunidades**.
6.  Para el formulario predeterminado para cada tipo de registro, configura de la siguiente manera:
    -   Clientes potenciales: Sales Insights
    -   Oportunidades: Sales Insights
7.  Seleccione el botón **Publicar**.
    -   Nota: los cambios pueden tardar varios minutos en aplicarse.

### Tarea 2: Crear un segmento

1.  Si aún no lo has hecho, cambia el área a **Configuración de Sales Insights.**
2.  En el grupo Sales Insights, selecciona **Configuración global.**
3.  En el subgrupo Acelerador de ventas, selecciona la pestaña **Asignación de trabajo**.
4.  Asegúrate de que el **Tipo de registro** está establecido en **Clientes potenciales** y selecciona el botón **Nuevo segmento**.
5.  En el campo **Nombre**, escribe el texto **Trade Show Leads** y, después, selecciona el botón **Siguiente**.
6.  En la pestaña **Definición de segmento**, selecciona el botón **Agregar**.
7.  En el menú que aparece, seleccione **Agregar fila**.
8.  Configure la condición de la siguiente manera:
    1.  **Fuente de cliente potencial**: **Igual a**: **Feria comercial**
9.  Selecciona **Simular resultados**.

    Deberías ver una pantalla de simulación de miembro del segmento que incluirá los clientes potenciales que cumplan tus criterios.

10. Cierra la ventana **Simulación de miembro del segmento**.
11. Selecciona el botón **Guardar**.
12. Selecciona el botón **Activar**.

## Ejercicio 2: Crear y adjuntar secuencias a registros

### Tarea 1: Crear una secuencia nueva

1.  Si aún no lo has hecho, cambia el área a **Configuración de Sales Insights.**
2.  En el grupo Sales Insights, selecciona **Configuración global.**
3.  En el grupo Acelerador de ventas, selecciona la pestaña **Secuencias**.
4.  Si es necesario, selecciona **Habilitar** en la notificación para habilitar el flujo de trabajo para que las secuencias funcionen correctamente.
5.  En la pestaña Secuencias, selecciona **+ Nueva secuencia.**
6.  Tienes la opción de crear una secuencia a partir de una serie de plantillas comunes. Puedes explorar las plantillas disponibles. Cuando estés listo, selecciona **Empezar desde cero.**
7.  A continuación, asignarás un nombre, una descripción y elegirás el tipo de tabla para el que estará disponible la secuencia. En el cuadro de texto Nombre de secuencia, escribe el nombre de secuencia, *Secuencia de seguimiento de feria comercial.*
8.  En el cuadro de texto Descripción, escribe la descripción de la secuencia: "Se trata de una secuencia de prueba para Test Coffee. Esta secuencia se usará para realizar un seguimiento de los clientes potenciales después de las ferias comerciales".
9.  En Tipo de registro, selecciona **Cliente potencial** (si aún no está seleccionado).
10. Haga clic en **Next**.

### Tarea 2: Elegir la primera actividad que el vendedor debe realizar

Elige el primer paso que deben realizar tus vendedores. Puede tratarse de enviar un correo electrónico, realizar una llamada telefónica o agregar una tarea propia. En nuestro ejemplo, comenzaremos con un correo electrónico.

1.  Debajo del icono Inicio de secuencia, selecciona el botón **+** para agregar una acción u otro elemento.
2.  Haz clic en **Enviar un correo electrónico.**
3.  En Título, escribe: *Correo electrónico de presentación.*
4.  En Descripción, escribe opcionalmente una descripción: *Presentación del cliente potencial al equipo de ventas.*
5.  Si hay plantillas de correo electrónico (plantillas específicas de tabla o globales) disponibles en tu organización, puedes elegir una plantilla de correo electrónico. En este caso, asumiremos que el vendedor escribirá su propio correo electrónico de presentación.
6.  Selecciona la **X** para cerrar el panel Actividad.
7.  En la barra de comandos de la secuencia, selecciona **Guardar**.

### Tarea 3: Agregar actividades adicionales para que las realice el vendedor

Agrega actividades adicionales para que realicen los vendedores de forma ordenada ; por ejemplo, el vendedor debe realizar primero la primera actividad, después la segunda y la tercera, etc.

1.  Haga clic en el botón **+**.
2.  Elige la siguiente actividad que debe realizar el vendedor, puede ser enviar un correo electrónico, realizar una llamada telefónica o agrega una tarea propia. Selecciona **Establecer tiempo de espera** para definir un intervalo de tiempo entre actividades. En nuestro ejemplo, agregaremos un intervalo de tiempo de 1 hora.
3.  Haga clic en Save(Guardar).
4.  Haga clic en el botón **+**.
5.  Selecciona **Llamada de teléfono**.
6.  En el Título, escribe *Llamada de seguimiento.* (Puedes agregar una descripción si quieres).
7.  Seleccione **Guardar** en la barra de comandos.

### Tarea 4: Activar la secuencia

Para que la secuencia esté disponible para que la usen los vendedores, activa la secuencia.

1.  Selecciona **Activar** en la barra de comandos.
2.  Selecciona **Entiendo** y, a continuación, **Activar** en el elemento emergente.
3.  Tu secuencia tendrá ahora una barra verde en la parte superior que te indica que la secuencia se ha activado correctamente.

### Tarea 5: Conectar la secuencia a un segmento

1.  Asegúrate de que estás en el área **Configuración de Sales Insights**.
2.  Con el panel de navegación de la izquierda, selecciona **Secuencias**.
3.  Abre la secuencia **Seguimiento de feria comercial** que creaste anteriormente.
4.  Seleccione la pestaña **Clientes potenciales conectados**.
5.  Selecciona **+ Conectar segmentos**
6.  Busca y selecciona el segmento **Clientes potenciales de feria comercial** que creaste anteriormente.
7.  Seleccione **Conectar**.

### Tarea 6: Conectar la secuencia al registro (de registro)

1.  Cambia el área al área **Ventas** mediante el menú desplegable de la parte inferior izquierda.
2.  Selecciona **Clientes potenciales** en el menú de navegación del sitio.
3.  Selecciona uno de los clientes potenciales que creaste antes.
4.  En la barra de comandos, selecciona la **flecha abajo** situada junto a Secuencias. En el menú que aparece, selecciona **Conectar secuencia** en la barra de comandos.
5.  Selecciona la secuencia que creaste anteriormente y selecciona **Conectar.**
6.  Aparece un mensaje de confirmación en la parte inferior de la página y la secuencia se conecta al registro del cliente potencial seleccionado.
7.  Si se te pide que asignes un vendedor, selecciona el botón **Asignar**. Ahora, los vendedores que tienen acceso al registro del cliente potencial pueden ver las actividades conectadas con él.
8.  Actualiza la página: deberías ver las tareas que creaste en la sección **Arriba siguiente**.

