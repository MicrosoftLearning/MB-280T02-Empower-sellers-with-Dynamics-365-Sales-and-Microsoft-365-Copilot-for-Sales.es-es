---
lab:
  title: 'Laboratorio 5.1: Personalizar un flujo de proceso de negocio'
---

# Módulo 5: Trabajar con Dynamics 365 Sales Insights y el Acelerador de ventas 

## Laboratorio de práctica 5.1: Personalizar un flujo de proceso de negocio

## Escenario

Contoso Coffee quiere agregar algunos pasos adicionales a su proceso de negocio de ventas probado y verdadero. Aunque los vendedores han tenido éxito después de este marco en el pasado, informan de que algunas sugerencias nuevas ayudarían a estimular clientes potenciales y conseguir de contratos de alto valor.

Los vendedores quieren agregar los pasos siguientes a su proceso de negocio:

-   En el caso de clientes potenciales de alto valor con un presupuesto superior a \$1.000.000, haz que el cliente potencial se ponga en contacto personalmente para confirmar el interés antes de pasar a la calificación.
-   En la fase de desarrollo, asegúrate de que los vendedores están realizando un seguimiento de los puntos de dificultad existentes de los clientes para ayudar a identificar posibles áreas para ventas de complementos que pueden haberse perdido anteriormente.

En este laboratorio, personalizaremos el flujo de proceso de negocio para satisfacer las solicitudes de nuestros vendedores.

## Ejercicio 1: Personalizar el flujo de proceso de negocio

### Tarea 1: Crear un flujo de proceso de negocio

En esta tarea, crearás un nuevo flujo de proceso de negocio desde el proceso de ventas de la oportunidad y, a continuación, probarás el nuevo BPF.

1.  Vaya a [https://make.powerapps.com](https://make.powerapps.com/).
2.  Asegúrate de que te encuentras en el entorno de **prueba de ventas**.
3.  Seleccione **Soluciones**.
4.  En la barra de comandos dela parte superior, selecciona el botón **+ Nueva solución**.
5.  En el campo **Nombre para mostrar**, escribe **Contoso**.
6.  Selecciona **+ Nuevo publicador**.
7.  Configura el nuevo publicador de la siguiente manera.
    1.  **Nombre para mostrar:** Contoso
    2.  **Nombre:** Contoso
    3.  **Prefijo:** Contoso
    4.  **Prefijo de valor de elección:** 10000
8.  Seleccione **Guardar**.
9.  En Publicador, selecciona el nuevo publicador **Contoso** que acabas de crear.
10. Seleccione **Crear**.
11. En la **barra de comandos**, selecciona **Agregar** existente.
12. En el menú que aparece, selecciona **Automatización**\>**Proceso**.
13. Ahora, encontraremos el **Proceso de venta** en la lista de procesos. (Ahora puedes usar el cuadro de búsqueda en la esquina superior derecha para buscar). Cuando lo encuentres, selecciónalo.
14. Selecciona el botón **Agregar**.
15. Selecciona el **Proceso de venta** para abrirlo.
16. Una nueva pestaña abrirá el editor de BPF. (Mantén abierta la pestaña anterior con la lista Soluciones). Ahora, vamos a agregar los pasos que nuestros vendedores han estado solicitando.
17. En primer lugar, agregaremos una condición para comprobar el presupuesto del cliente e identificar a nuestros clientes potenciales de alto valor con presupuestos superiores a \$1.000.000. Arrastra **Condición** desde la pestaña **Componentes** y colócala entre las fases **Calificar** y **Desarrollar**.
18. Selecciona la **Condición**, ve a la pestaña **Propiedades** y escribe **Comprobar presupuesto** para **Nombre para mostrar**.
19. En **Reglas,** selecciona **Importe presupuestado** para **Campo**.
20. Selecciona **Es mayor o igual que** para **Operador**.
21. Selecciona **Valor** para **Tipo**.
22. Escribe **1.000.000** para **Valor** y haz clic en **Aplicar**.
23. Ahora es necesario agregar una nueva fase para completar la condición. En el panel Componentes, agrega una nueva fase a la derecha de la Condición.
24. Seleccione la pestaña **Propiedades**.
25. Escribe **Confirmar interés** para **Nombre para mostrar**. Seleccione **Aplicar**.
26. Haz clic en el botón **Detalles** de la fase **Confirmar interés**.
27. Selecciona el **Paso de datos \# 1 Nuevo paso** dentro de la fase **Confirmar interés**.
28. En la pestaña **Propiedades**, abre la lista desplegable **Campo de datos.** Selecciona **Confirmar interés**. El nombre del paso se actualizará automáticamente.
29. Activa la casilla **Obligatorio** y haz clic en **Aplicar**.
30. A continuación, agregaremos un nuevo paso para pedir puntos de dificultad del cliente en la fase de desarrollo, tal y como solicitan nuestros vendedores. Selecciona la fase **Desarrollar** y expande **Detalles.**
31. En el panel Componentes, arrastra un **paso de datos** debajo del paso de datos \#4.
32. En la lista desplegable Campo de datos, selecciona **Puntos de dificultad del cliente.** Ahora será un paso sugerido en la fase de Desarrollo para identificar los puntos de dificultad del cliente. No marcaremos este campo como obligatorio.
33. Seleccione **Aplicar**.
34. Haz clic en **Validar** para asegurarte de que los cambios que has realizado son válidos y que el BPF funcionará según lo previsto.
35. Si no hay problemas, haz clic en **Actualizar**.
36. Cierra la pestaña con el editor de flujo de proceso de negocio.
37. De nuevo en la pestaña anterior, haz clic en **Listo** en el elemento emergente en el área Solución predeterminada. En el menú superior, selecciona **Publicar todas las personalizaciones.** (Es posible que tengas que eliminar la búsqueda de "oportunidad" en el cuadro de texto de la esquina superior derecha para poder ver este botón).
38. Espera a que las personalizaciones se **publiquen**.

### Tarea 2: Probar el flujo de proceso de negocio

1.  Regresa a la aplicación Centro de ventas.
2.  Ve a la sección **Oportunidades** y haz clic en **+Nuevo** para crear una nueva oportunidad. Escribe un tema como **Interesado en máquinas nuevas**.
3.  Selecciona un contacto existente para el campo de contacto.
4.  Abre la fase **Calificar** del flujo de proceso de negocio del proceso de venta. Escribe *\$800.000* para Presupuesto estimado.
5.  El flujo de proceso de negocio debe tener 4 fases: **Calificar**, **Desarrollar**, **Proponer** y **Cerrar**. La fase Confirmar interés no formará parte del proceso si el importe presupuestado es inferior a \$1.000.000.
6.  Cambia el **Importe del presupuesto** a *\$1.200.000.*
7.  El flujo de proceso de negocio debe tener ahora 5 fases: **Calificar**, **Confirmar interés**, **Desarrollar**, **Proponer** y **Cerrar**. Pasa de la fase Calificar a la siguiente.
8.  **Guarda** la oportunidad.
9.  Selecciona la fase **Calificar** y selecciona el botón **Fase siguiente** para pasar a la fase **Confirmar interés**.
10. Para confirmar el interés, selecciona **No** y, a continuación, **Sí.**
11. Haz clic en el botón **Fase siguiente** para avanzar a la fase **Desarrollar**.
12. Confirma que el campo Puntos de dificultad del cliente aparece en la parte inferior de la fase Desarrollar.
13. Escribe *Las máquinas actuales no pueden controlar el volumen del cliente* en el campo Puntos de dificultad del cliente.
14. Seleccione **Fase siguiente**.
15. **Guardar** el registro.

