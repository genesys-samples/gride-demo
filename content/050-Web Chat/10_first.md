---
title: "Setup"
chapter: true
weight: 10
---
![Setup](/images/Webchat1-768x300.jpg)
## Configuración de Web Chat 

El canal de chat web es una herramienta invaluable para comunicarse e interactuar con los clientes a fin de brindar un mejor servicio para responder preguntas, completar pedidos, orientación general sobre los productos y características de la empresa y atención personalizada al cliente. Con esta solución, Genesys mejora el tiempo de atención, la resolución en el primer contacto, la utilización de agentes y la satisfacción del cliente.

![Web Chat](/images/webchat.png)

## Flujo de web chat

De manera similar a nuestro módulo de voz entrante, necesitaremos un flujo entrante para aprovechar las capacidades de enrutamiento y enviar webchats a la cola adecuada según la intención del cliente.

1. Haga clic en **Página de administración**.
2. Haga clic en la herramienta **Architect** y seleccione **Inbound Chat** en el menú desplegable.
3. Haga clic en **+ Agregar**. Continuaremos usando la misma convención de nomenclatura que usamos anteriormente en este taller, luego **Crear flujo**.

Profundizaremos en las capacidades de enrutamiento en nuestro Taller Archiect, pero la barra de herramientas de chat es similar a lo que encontrará en otros tipos de flujos de medios también. Al implementar el autoservicio, Genesys Cloud se integra fácilmente con Google DialogFlow y Amazon Lex junto con nuestros propios Bot Flows nativos para chat y voz.

Por ahora, mostraremos lo simple que puede ser un flujo, y simplemente.

1. Elija **Transferir a ACD** arrastrándolo y soltándolo en el flujo.
2. Todo lo que queda es decidir a qué **Cola** nos enrutaremos. Ahora **Guardar** y **Publicar**

![Web Chat](/images/ChatFlow1.jpg)

## Genesys Widgets

Genesys ofrece tres versiones nativas de widgets, así como la opción de integrarse con un tercero. Las diferentes versiones de los widgets vienen con diferentes beneficios y funciones que puede habilitar. Le recomendamos que consulte nuestro documento de comparación de nuestros widgets de chat. https://help.mypurecloud.com/articles/widget-feature-comparison/

Los widgets le permiten agregar chat web a su sitio web para que los clientes puedan chatear con agentes directamente desde sus navegadores. Cuando crea un widget en la consola de administración de Genesys Cloud CX, se crea una clave de implementación. La clave de implementación ayudará a identificar los ajustes de configuración del widget cuando coloque el widget en su sitio web.

Tener un sitio web no es un requisito previo para este taller. En su lugar, enrutaremos las interacciones de chat a través de nuestra herramienta Genesys Cloud Demo Extension. Antes de instalar la herramienta de extensión, primero configuremos nuestro widget dentro de la organización Genesys Cloud CX. **Nota:** La cantidad máxima de implementaciones de widgets en una organización es 25.

1. Haga clic en Administrador, busque **Widgets**.
2. Haga clic en **Crear widget** y asígnele un nombre utilizando nuestra convención de nomenclatura estándar. No es necesaria ninguna descripción en este taller.
3. Asigne **Versión 2** en **Tipo de widget**.
4. Elija el flujo al que enrutar, creado arriba y finalmente asegúrese de **Guardar**

>## Herramienta de extensión de DEMO
>
>La extensión de demostración es ideal para mostrar rápidamente a su cliente cómo sería tener su sitio web corporativo impulsado por Genesys Cloud. La extensión de demostración muestra Genesys GX Widgets, Predictive Engagement y le permite interactuar con PureCloudNow o con su propia organización de Genesys Cloud.
>
>La extensión ofrece 2 categorías de características principales:
   Canales basados en Widgets v1: chat v1, cobrowse/screenshare, correo electrónico, devolución de llamada
   Chat de Widgets v2 con Predictive Engagement (Predictive Engagement)
>
>La extensión puede estar en tres estados de trabajo. El estado aplica por ficha. Estos estados son:

* "OFF": tanto Inspección como Inyección están en rojo. La extensión no tiene impacto en el sitio navegado.
* Modo "Edición de demostración": tanto Inspección como Inyección son verdes. En este modo, puede agregar HotSpots (acciones adjuntas a los elementos seleccionados) haciendo clic con el botón derecho del mouse y eligiendo la acción para ejecutar. Cualquier par {elemento, acción} se resalta con una línea de borde verde para que pueda identificar lo que se ha creado.

* Modo "Ejecución de demostración": la inyección es verde y la inspección es roja. Este modo no tiene los elementos resaltados que activan las acciones de clic. El sitio parece completamente normal, pero las acciones asociadas a los elementos se activarán cuando haga clic en ellos. Para ayudarlo a recordar dónde hacer clic y en qué orden, el icono de la extensión mostrará el nombre de la acción cuando se desplace sobre los elementos activos. Además, un contador se incrementará en el icono de la extensión para indicar que la acción se activó cuando se hizo clic en el elemento.

#### Instalación

Haga clic en https://chrome.google.com/webstore/detail/genesys-gdemo-extension/jiilhcbdojcdonkigflgmdnljialgmfh para agregar la herramienta Genesys Cloud Demo Extension a su navegador Chrome.

![DemoExtension Installer](/images/DemoExtension.jpg)

1. Abra Genesys Extension Tool ó ña herramienta de extensión y seleccione **Opciones**
2. Haga clic en 'Agregar organización'
3. Seleccione la región de su organización (menú desplegable Entorno)
4. Haga clic en 'Iniciar sesión en la organización': se abrirá una nueva pestaña en la página de inicio de sesión de su organización.
5. En la nueva pestaña, inicie sesión en su organización: la extensión extraerá los datos de configuración necesarios de su organización y la pestaña se cerrará automáticamente después de unos segundos.
6. Seleccione la cola apropiada
7. Marque la casilla para habilitar **Web Chat V2** y seleccione el widget en **Clave de implementación (V2)**
8. Presiona 'Guardar'

![DemoExtension Installer](/images/ExtensionOptions.jpg)