---
lab:
  title: 'Laboratorio 1.1: Configuración de aplicaciones compatibles'
---

# Módulo 1: Configuración de Dynamics 365 for Sales

## Laboratorio de práctica 1.1: Configuración de aplicaciones compatibles

## Escenario

Los vendedores de Contoso Coffee informan de que, aunque Dynamics 365 Sales es muy útil para aumentar la productividad del vendedor, la aplicación parece muy aislada en relación con su flujo diario de trabajo. Tienen los siguientes requisitos para su departamento de TI:

-   Los vendedores desean realizar un seguimiento y administrar la correspondencia por correo electrónico relacionada con las ventas en CRM.
-   Los vendedores quieren almacenar documentos relacionados con las ventas (como artículos de conocimientos de productos, investigación de clientes e informes de tendencias de mercado) en CRM. Quieren poder acceder, compartir y administrar estos documentos directamente desde la aplicación Sales.
-   A los vendedores les gustaría colaborar con otros departamentos, como inventario, suministro de pedidos y marketing a medida que persiguen sus oportunidades de ventas. Les gustaría que estos otros departamentos pudieran colaborar en un registro de cliente dentro de un chat o canal de Teams.
-   Los vendedores han oído mucho sobre las características de Copilot dentro de Dynamics 365 Sales, incluyendo resumen de registros, ponerse al día de los cambios en los registros, preparar las reuniones y redactar correspondencia. Quieren asegurarse de que las características de Copilot están activadas en su entorno para que puedan empezar a aprovechar la inteligencia artificial dentro de la aplicación para mejorar su productividad.

En este laboratorio, activaremos y configuraremos las características que ayudarán a nuestra organización de CRM a cumplir los requisitos de estos vendedores.

## Ejercicio 1: Configuración de la integración de correo electrónico, SharePoint y OneDrive

### Tarea 1: Configuración de la integración de correo electrónico

1.  En un explorador web, ve a [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  En el panel de navegación del sitio del lado izquierdo de la pantalla, selecciona **Entornos**.
3.  Selecciona el entorno **Prueba de Sales** para abrirlo.
4.  Busca y selecciona **Configuración** entre los comandos que aparecen en la parte superior.
5.  Selecciona el encabezado de correo electrónico para expandirlo y selecciona **Buzones**.
6.  Abre el registro del buzón de **Administrador MOD**.
7.  Configura el buzón de administrador **MOD** de la siguiente manera:
    -   **Perfil de servidor**: Microsoft Exchange Online
    -   **Correo electrónico entrante**: Sincronización del lado del servidor o E-mail Router
    -   **Correo electrónico saliente**: Sincronización del lado del servidor o E-mail Router
    -   **Citas, contactos y tareas**: sincronización del lado del servidor
8.  Guarde los cambios mediante **Guardar**. Después, haz clic en **Aprobar correo electrónico**. (**Nota:** Debes aprobar el buzón antes de poder enviar y recibir correo electrónico).
9.  Se te preguntará si deseas aprobar el correo electrónico principal. Seleccione **Aceptar**.
10. Haz clic en **Probar y habilitar buzón**.
11. En la pantalla emergente de prueba y habilitación, asegúrate de que, si este buzón se ha configurado previamente para sincronizarse con otra organización, marcar esta opción hará que se sincronice con esta organización.
12. Seleccione **Aceptar**.

**IMPORTANTE:** No salgas de esta página mientras se completan las pruebas. Si deseas trabajar en la tarea 2 mientras se completan las pruebas, puedes abrir una nueva pestaña o explorador.

## Tarea 2: Habilitar la integración de SharePoint basada en servidor

En esta tarea, habilitarás la integración de SharePoint basada en servidor para tu organización de Dynamics 365.

1.  En un explorador web, ve a [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  En el panel de navegación del sitio del lado izquierdo de la pantalla, selecciona **Entornos**.
3.  Abre el entorno **Prueba de Sales** en el que has estado trabajando para abrirlo.
4.  Busca y selecciona **Configuración** entre los comandos que aparecen en la parte superior.
5.  En el encabezado Integración, selecciona **Configuración de administración de documentos**.
6.  Deberías ver una opción para habilitar **Integración de SharePoint basada en servidor**. (Si no está allí, la integración de SharePoint ya se ha habilitado y puedes ir al paso once).
    -   Si la integración de SharePoint no está configurada, selecciona **Habilitar integración de SharePoint basada en servidor**.
7.  En la pantalla Habilitar integración de SharePoint basada en servidor, haz clic en el botón **Siguiente**.
8.  Selecciona **En línea** en el tipo de implementación, haz clic en el botón **Siguiente**.
9.  Escribe la dirección URL del sitio de SharePoint que deseas usar. (Ejemplo: https://"Orgname".sharepoint.com), haz clic en el botón **Siguiente**.

    **Nota:***Para encontrar la dirección URL de SharePoint, selecciona el icono del comprobador de aplicaciones en la esquina superior izquierda de la pantalla. (Parece un cuadrado de 3 x 3). mantén presionada la tecla CTRL y selecciona SharePoint.*

10. Una vez validado el sitio, haz clic en el botón **Habilitar**.
11. Haz clic en **Configuración de administración de documentos**.
12. Selecciona las entidades para las que quieras habilitar la administración de documentos, como clientes potenciales, cuentas, oportunidades y haz clic en **Siguiente**.
    -   **IMPORTANTE**: Si planeas configurar la interacción con el correo electrónico en Sales Insights, selecciona la entidad Correo electrónico.
13. En el campo Dirección URL del sitio de SharePoint, escribe la dirección URL del sitio de SharePoint que has usado en la tarea anterior.
14. Haga clic en el botón **Next** (Siguiente).
15. Haz clic en el botón **Finalizar** para completar la configuración.

### Tarea 3: Configurar la integración de OneDrive para la Empresa

En esta tarea, configurarás la integración de OneDrie para tu organización de Dynamics CRM. (Desde la publicación de este curso, la configuración de administración de documentos no estaba disponible desde el Centro de administración de Power Platform. Tendrás que configurar la integración de OneDrive para la Empresa desde el área de configuración de Dynamics 365 clásico).

1.  En un explorador web, ve a [admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com/).
2.  En el panel de navegación del sitio del lado izquierdo de la pantalla, selecciona **Entornos**.
3.  Abre el entorno **Prueba de Sales** en el que has estado trabajando para abrirlo.
4.  Busca y selecciona **Configuración** entre los comandos que aparecen en la parte superior.
5.  En el encabezado Integración, selecciona **Configuración de administración de documentos**.
6.  Haz clic en el icono **Habilitar OneDrive para la Empresa**.
7.  Selecciona la casilla **Habilitar OneDrive para la Empresa** y, después, selecciona **Aceptar**.
8.  Después de que se actualice la pantalla, haz clic en **Configuración de la carpeta de OneDrive para la Empresa**.
9.  Acepta el nombre de carpeta predeterminado o escribe un nombre de tu elección y haz clic en **Aceptar**.

## Ejercicio 2: Configuración de Teams y Copilot

### Tarea 1: Configuración de la integración de Teams

1.  Si es necesario, abre la aplicación Centro de ventas.
2.  Mediante la navegación de la izquierda, selecciona el área **Ventas** (parte inferior izquierda).
3.  En el menú que aparece, seleccione **Configuración de la aplicación**.
4.  En el grupo Configuración general, selecciona **Chat y colaboración**.
5.  Establece **Activar la vinculación de registros de Dynamics 365 con canales de Microsoft Teams** en **Sí**.
6.  Establece **Activar integración de Microsoft Teams mejorada** en **Sí**. (Es posible que tengas que seleccionar la cuenta de administrador MOD. Si se te solicitan permisos, selecciona **Aceptar**).
7.  En **Activar chats de Microsoft Teams dentro de Dynamics 365**, selecciona **Activar para todas las aplicaciones de Dynamics 365**.
8.  Selecciona el botón **Guardar**.  
    **IMPORTANTE**: Los cambios pueden tardar varios minutos en guardarse.

### Tarea 2: Configurar Copilot

1.  Asegúrate de que estás en el área **Configuración de la aplicación**.
2.  En el grupo Configuración general, selecciona **Copilot**.
3.  Activa la casilla situada junto a **Probar las características de versión preliminar más recientes antes de que se implementen para todos los usuarios** para habilitarla.
4.  En **Características de Copilot**, cambia **Todas las aplicaciones de Dynamics 365 Sales** de la siguiente manera:
    -   **Chat**: activado
    -   **Correo electrónico (versión preliminar):** activado
5.  Selecciona el botón **Guardar**.

