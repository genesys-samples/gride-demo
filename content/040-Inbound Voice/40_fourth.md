---
title: Herramientas de Agente
chapter: true
weight: 40
---
![Test](/images/Inbound4-768x300.jpg)

## Herramientas de interacción de voz

Al manejar interacciones de voz en Genesys Cloud CX, una serie de herramientas están disponibles listas para usar. Algunos pueden depender de su nivel de licencia o permisos basados en su rol de usuario. Cada uno desempeña su papel al proporcionar al agente datos relevantes para manejar con éxito la interacción y crear una experiencia personalizada y fluida para el cliente.

![Voice Interaction](/images/Voiceinteractiontools.jpg)

***Teclado de marcación***: el teclado de marcación le permite ingresar números que los sistemas de llamadas automatizados reconocen, como un número de cuenta o una selección de menú. Genesys Cloud reproduce un sonido DTMF para cada número que seleccione.

***Silenciar/Activar***: silenciar desactiva el micrófono del agente. El cliente no puede escuchar lo que dice el agente, pero el agente puede escuchar al cliente.

***Espera***: Espera pone al cliente en espera. El agente no puede escuchar al cliente y el cliente no puede escuchar al agente.

![Dialpad](/images/Dialpad.jpg)

Genesys Cloud CX admite dos tipos de transferencias: una transferencia ciega (todos los tipos de interacción) y una transferencia de consulta (interacciones de llamadas). Ambos tipos de transferencia le permiten ver el estado de un agente antes de realizar la transferencia para asegurarse de que habrá alguien al otro lado para ayudar al cliente. Al transferir a una cola, tendrá una línea de visión del tiempo de espera estimado de la cola, cuántos agentes están vinculados a la cola y cuántas interacciones se están manejando actualmente por tipo de medio.

***Transferencia ciega***: una transferencia ciega le permite transferir una interacción inmediatamente a una persona o cola.

***Transferencia con consulta***: una transferencia con consulta le permite conectarse con una persona o cola antes de transferir una llamada.

![Consult](/images/Consulttransfer.jpg)

***Iniciar/finalizar pausa segura***: puede presionar la "pausa segura" para detener la grabación de la llamada (tanto audio como grabaciones de pantalla), ingresar el número de tarjeta de crédito y finalizar la " pausa segura" para reanudar la grabación. Esto asegura que no se registre información confidencial. Todavía puede escuchar al cliente y hablar con él durante esta pausa segura, pero el sistema no registra la interacción en este momento. Esta pausa segura también se puede incrustar en el script, del que hablaremos más adelante. Las pausas seguras también se pueden activar a través de API y terceros.
https://appfoundry.genesys.com/filter/genesyscloud


***Colgar***: cuando haya terminado con la interacción, puede presionar este botón para finalizar la llamada y comenzar su trabajo posterior a la llamada.

![SecurePause](/images/securepause.jpg)


***Script***- Los Scripts son una forma de que los supervisores le den palabras y lógica a seguir al realizar interacciones. Los scripts pueden contener las palabras exactas que se supone que debe decir cuando habla con un cliente, sitios web de terceros que tiene que visitar con frecuencia, datos de clientes de un sistema de terceros, ¡y más! Esto es útil para los agentes más nuevos que pueden no saber qué decir cuando atienden una llamada o incluso para los agentes experimentados como referencia, y ahorra tiempo al tener las herramientas más importantes en la misma página. Los scripts son completamente personalizables y configurables por cola y tipo de interacción. ¡A continuación se muestra un ejemplo de cómo puede verse un script!

![Script](/images/script.jpg)

***Pantalla emergente***- Una aplicación de pantalla emergente entrega una llamada entrante a un agente, junto con datos relacionados con la llamada o la persona que llama. Por ejemplo, un cliente con Salesforce.com u otra aplicación CRM puede usar la información de identificación de llamadas para buscar el registro del cliente en CRM. El agente recibe una "pantalla emergente" de la cuenta de la persona que llama a través de su navegador web Salesforce.com. O bien, el script para una campaña de marcación saliente puede llenar la pantalla del agente con información relacionada con la llamada, el cliente y la campaña.
![Screen Pop](/images/screenpop.jpg)

***Pantalla compartida***: compartir la pantalla le permite ver la pantalla del cliente en tiempo real, con su permiso, por supuesto. Los agentes deben solicitar y recibir permiso de un cliente para iniciar un chat de pantalla. Para la voz, puede comunicar verbalmente la clave de seguridad al cliente, quien luego escribirá ese número en un formulario en su sitio web. Para el chat web, Genesys Cloud comparte la clave de seguridad en segundo plano, sin necesidad de que usted realice ninguna acción. Una pantalla compartida siempre está vinculada a la interacción original, en este caso una interacción de voz. Para fines de gestión de calidad, esta interacción se mostrará como una sola interacción.

![Screen Share](/images/screenshare.jpg)

***Agent Assist***: Agent Assist brinda transcripción en tiempo real de una llamada de cliente y sugerencias de conocimiento que se actualizan automáticamente según el contexto de la conversación. Las sugerencias de conocimiento incluyen preguntas frecuentes o recomendaciones de artículos de conocimiento que hacen que los agentes sean más eficientes y conocedores. No tiene que perder el tiempo buscando información y puede concentrarse en sus discusiones con los clientes.

![Agent Assist](/images/agentassist.jpg)

***Perfil***: los perfiles de clientes brindan más información sobre el cliente. Puede ver más detalles del cliente y notas que otros agentes han hecho sobre este cliente. Siempre es mejor tener la mayor cantidad de información posible sobre el cliente para asegurarse de que está brindando una experiencia *personalizada*.

***Notas***: puede tomar notas sobre una interacción durante la interacción o durante el trabajo posterior a la llamada (ACW). Si ingresa notas para una interacción y luego transfiere esa interacción a otro agente, las notas permanecen con la interacción. Debido a que las notas son parte de la interacción, el agente receptor también puede verlas.

![Profile](/images/profile.jpg)

***Programar una devolución de llamada***: una devolución de llamada es una llamada saliente solicitada por un contacto. Los agentes pueden programar una devolución de llamada durante una interacción de voz. En la fecha y hora programadas, Genesys Cloud enruta la interacción a un agente. Para enrutar la devolución de llamada a usted, seleccione Enrutar la devolución de llamada a mí si es posible. De forma predeterminada, las devoluciones de llamada programadas se enrutan a la cola que recibió la interacción original. Si su administrador ha habilitado las devoluciones de llamada propias, para tomar posesión de una devolución de llamada, seleccione Tomar posesión. La devolución de llamada espera a que esté disponible durante el tiempo configurado por su administrador.

![Callback](/images/callback.jpg)

***Códigos de finalización***: los códigos de finalización indican la naturaleza de una interacción. Los agentes especifican códigos de finalización después de completar una interacción; por ejemplo, una venta completada, un cliente insatisfecho con el servicio o un problema de facturación.

![Wrapup](/images/wrapup.jpg)
&nbsp;

#### Ha terminado de enrutar su primera interacción entrante a Genesys Cloud CX. Ahora que hemos completado la voz, pasemos a las interacciones digitales. Recuerde, Genesys Cloud CX tiene la capacidad de enrutar voz, chat web, mensajería web, correo electrónico, SMS y redes sociales, todo de forma nativa. 

