---
title: "Herramietnas de Agente"
chapter: true
weight: 40
---
![Agent Tools](/images/Webchat4-768x300.jpg)
## Herramientas de interacción digital

Al manejar interacciones digitales en Genesys Cloud CX, una serie de herramientas están disponibles listas para usar. Algunos pueden depender de su nivel de licencia o permisos basados en su rol de usuario.

![Digital Interactions](/images/digitalinteraction.jpg)

***Transferencia ciega***: una transferencia ciega le permite transferir una interacción inmediatamente a una persona o cola. Si realiza una transferencia ciega a una cola, Genesys Cloud recuerda la información basada en habilidades aplicada a la llamada original de forma predeterminada.

***Colgar***: finaliza las interacciones y envía al agente a su trabajo posterior a la llamada (ACW).

***Script***: las palabras escritas y la lógica que sigue un agente mientras procesa una llamada. Un guión puede contener varias páginas de narración combinadas con campos para actualizar los datos recopilados o actualizados por el agente. Se pueden crear scripts para interacciones entrantes o salientes.

***Respuestas enlatadas***: las respuestas enlatadas son respuestas preescritas a preguntas frecuentes que puede usar durante una interacción, ya sea leyendo la respuesta a un cliente o insertando la respuesta en un chat, correo electrónico o tweet .

***Notas***: puede tomar notas sobre una interacción durante la interacción o durante el trabajo posterior a la llamada (ACW). Si ingresa notas para una interacción y luego transfiere esa interacción a otro agente, las notas permanecen con la interacción. Debido a que las notas son parte de la interacción, el agente receptor también puede verlas.

***Código de finalización***: los códigos de finalización indican la naturaleza de una interacción. Los agentes especifican códigos de finalización después de completar una interacción; por ejemplo, una venta completada, un cliente insatisfecho con el servicio o un problema de facturación.

***Pantalla compartida***: la pantalla compartida utiliza WebRTC para enviar y recibir la pantalla compartida. Los que comparten solo necesitan una aplicación compatible con WebRTC para compartir sus pantallas. Puede incluir Chromium Embedded Framework compatible con WebRTC en su aplicación de escritorio o indicar a los clientes que usen un navegador web compatible con WebRTC, como Firefox o Google Chrome. Para el chat web, Genesys Cloud comparte la clave de seguridad en segundo plano, sin necesidad de que el agente realice ninguna acción. Después de que Genesys Cloud conecta la sesión de pantalla compartida, el agente puede ver la pantalla del que comparte y el agente o el que comparte puede finalizar la pantalla compartida.

***Recorrido del cliente***: puede ver la siguiente información, según cómo esté configurado Predictive Engagement:
* Detalles del visitante, como el nombre del visitante, el estado y el número de visitas.
* Visita fechas y duración. Si el visitante tiene varias fechas, seleccione la fecha sobre la que desea ver más información.
* Visite la información del viaje, incluidas las páginas visitadas y las acciones en esas páginas durante la visita seleccionada. Para ver más información sobre las acciones realizadas, haga clic en el icono de la acción.
* Segmentos asignados a la interacción para la visita seleccionada.
* Puntuaciones de resultado para la visita seleccionada.
* Otra información del visitante, como ubicación, tipo de dispositivo, sistema operativo y tipo de navegador.


![Blind Transfer](/images/blindtransferandhangup.jpg)


**Genesys Cloud mantiene una experiencia de usuario uniforme en toda la plataforma. Por esta razón, es fácil para los agentes dominar el arte de tomar interacciones. Los guiones, el perfil del cliente, las respuestas enlatadas, las notas y la adición de códigos de resumen son exactamente iguales para las interacciones digitales y de voz.**