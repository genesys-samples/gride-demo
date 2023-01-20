---
title: "Configuración"
chapter: true
weight: 10
---

---
![Setup](/images/Email1-768x300.jpg)

## Configuración de correo electrónico
El correo electrónico sigue siendo una de las formas más confiables y deseadas para que los clientes interactúen con las empresas en busca de soporte. Genesys Cloud CX distribuye automáticamente los correos electrónicos al agente más adecuado según el análisis de contenido y las palabras clave. El enrutamiento de correo electrónico de Genesys agiliza su proceso de respuesta mediante la funcionalidad de automatización de correo electrónico que le permite monitorear, medir y optimizar su flujo de correo electrónico para crear una mejor experiencia para el cliente.

Genesys Cloud enruta los mensajes de correo electrónico entrantes a través de ACD del mismo modo que enruta las llamadas y los chats, utilizando los mismos métodos de enrutamiento y evaluación. Al enrutar mensajes de correo electrónico, Genesys Cloud considera las habilidades, el idioma, la prioridad y la utilización del agente.

Su cuenta de Genesys Cloud puede tener un máximo de dos dominios de correo electrónico con hasta 500 direcciones de correo electrónico asociadas por dominio. Usted asigna cada dirección de correo electrónico a una cola y puede configurarla para que tenga asociado un idioma, una habilidad y una prioridad. Genesys Cloud ACD enruta cada mensaje entrante a un miembro de la cola. Los métodos de enrutamiento y evaluación configurados ayudan a determinar el mejor agente disponible para manejar la interacción.

Cuando un agente maneja una interacción por correo electrónico, se le enrutará como cualquier otro canal digital. Una vez que respondan, la interacción se borrará de su panel de interacción. Sin embargo, es común que la comunicación por correo electrónico tenga múltiples respuestas que deban enviarse al cliente. Debido a esto, cuando un cliente responde al correo electrónico, Genesys Cloud CX se enrutará al agente que respondió para una comunicación fluida siempre que ese agente esté disponible.

![Email](/images/email.png)

## Lo que construiremos hoy
Hoy configuraremos un dominio de correo electrónico dentro de Genesys Cloud CX que se enruta automáticamente a una cola. Los dominios de correo electrónico tienen la opción de enrutar directamente a una cola o a un flujo de arquitecto para un procesamiento adicional. Es posible que desee que su dominio de correo electrónico se enrute a un flujo de arquitecto si desea realizar respuestas automáticas, inmersiones de datos o adjuntar habilidades al correo electrónico. Para nuestro escenario, solo haremos que el correo electrónico vaya directamente a la cola G Ride que configuramos anteriormente.

## Seguir a lo largo

  1. Navegue a la pantalla **Administrador** > Busque **Correo electrónico** en **Centro de contacto**

  2. Haga clic en **Agregar dominio** > De la lista **Tipo de dominio**, seleccione **Genesys Cloud** > En el cuadro **Nombre de dominio**, ingrese el subdominio de correo electrónico (por ejemplo, su nombre de cuenta), que con **.myPureCloud.com**

  3. Haga clic en **Guardar**. Se abre la página de dirección de correo electrónico para el nuevo dominio.

  2. A continuación, agregue la dirección de correo electrónico entrante al dominio.
  3. Haga clic en **Agregar dirección de correo electrónico** > En el cuadro **Dirección de correo electrónico**, escriba la dirección de correo electrónico que usa el cliente para enviar un correo electrónico.
  4. En **Enrutamiento de correo electrónico**, seleccione **Enrutar siempre a esta cola**
  5. Haga clic en la lista **Cola** y elija la cola deseada > En el cuadro **Habilidades**, agregue opcionalmente cualquier habilidad de ACD para asegurarse de que los correos electrónicos asociados se dirijan a un agente con habilidades coincidentes.
 
  6. Haga clic en la lista **Idioma** y, opcionalmente, elija un idioma > En **Enrutamiento de spam**, elija "Desconectar todos los correos electrónicos detectados como spam" > Haga clic en **Guardar**

 
**_Para el taller de hoy, asegúrese de enrutar a una cola en lugar de a un flujo como se describe en esta captura de pantalla_**
    
 ![Email Domain Set Up](/images/EmailSetUp.jpg)

 3. Vuelva a la cola > actualice la **Dirección de correo electrónico saliente** al dominio de correo electrónico que acaba de configurar

    ![Queue Set Outbound Email Domain](/images/SetOutboundEmail.jpg)
 
 4. Vaya a **Administrador** > Buscar **Utilización**
 5. En **Capacidad máxima**, especifique la cantidad de interacciones que se permitirán para cada tipo de interacción. Por ejemplo, si desea que un agente trabaje con hasta cuatro correos electrónicos a la vez, establezca la capacidad máxima de correo electrónico en 4 > Para asegurarse de que las interacciones que no son de ACD no se vean interrumpidas por las interacciones de ACD, seleccione **Bloquear llamadas cuando esté activado. casilla de verificación de una llamada que no es ACD (excluye transferencias)** >
  **Asegúrese de que la utilización coincida con la captura de pantalla a continuación**
 6. Haga clic en **Guardar**
  
 
    ![Utilization Settings](/images/Utilization.jpg)