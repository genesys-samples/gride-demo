---
title: "Configuración"
chapter: true
weight: 10
---
![Setup](/images/SMSsetup1-768x300.jpg)

## Configuración de SMS 
Hoy, configuraremos los conceptos básicos de SMS en Genesys Cloud CX. Comprará un número de SMS directamente desde el portal de administración de Genesys Cloud, siendo Genesys su intermediario de SMS. También importará un flujo básico de Inbound Message Architect. Por último, conectará el número de SMS que compró con el flujo de Architect que importó a través de una ruta de mensajería.

## Seguir a lo largo
1. Navegue a la pantalla **Administrador** > Busque **Inventario de números de SMS**
2. Cuando aparezca la página Inventario de números de SMS, presione **Comprar** en la esquina superior derecha
3. Complete los campos apropiados para buscar el número para comprar
4. Para ver los números disponibles para comprar, haga clic en **Buscar**
5. Haga clic en **Comprar ahora** > Cuando aparezca el cuadro de diálogo Confirmar compra de número
6. Haga clic en **Comprar** _(Tenga en cuenta el número que compró, porque es difícil de encontrar después de la compra)_

  
7. Vuelva a la cola que creó anteriormente> Configure el número de SMS que acaba de comprar como el número de SMS saliente
    ![Queue Set Outbound SMS Number](/images/QueueSetSMSOutboundNumber.jpg)

8. Siga las instrucciones a continuación para crear un flujo de mensajes entrantes:

9. En la página de inicio de Architect, haga clic o desplace el cursor sobre el menú **Flujos** y seleccione **Mensaje entrante**
10. Haga clic en ***+ Agregar**. Se abre el cuadro de diálogo Crear flujo.
11. En el campo Nombre, escriba un nombre único para el flujo de mensajes entrantes
12. Haga clic en **Crear flujo**

13. Una vez dentro del flujo, arrastre una tarea **Transferir a ACD** al **menú Inicio** como se ve en la imagen a continuación
14. Haga clic en el menú desplegable y seleccione la cola que creó al principio
15. Haga clic en los tres puntos junto a la tarea **Desconectar** para eliminar esta tarea
16. Haga clic en **Publicar** una vez que haya completado estos pasos
![Inbound Message](/images/inboundmessage1.jpg)

17. Vaya a la pantalla **Administrador** > Busque **Enrutamiento de mensajes**
18. Haga clic en **+** > Haga clic en **Seleccionar flujo** > Comience a escribir las primeras letras del flujo de mensajes entrantes que desea usar y seleccione de la lista.
19. En **Direcciones**, haga clic en **+** > Haga clic en **Seleccionar dirección** > Haga clic en el número que desea agregar
20. Haga clic en **Agregar** > Haga clic en **Guardar**
Configure una ruta de mensajería para conectar su flujo de arquitecto de mensajes entrantes y el número de SMS que compró en el paso dos

![Call Routing](/images/callrouting1.jpg)