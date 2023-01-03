---
title: "Troubleshooting"
chapter: true
weight: 30
---


![Test](/images/Inbound3-768x300.jpg)

## Voice Troubleshooting
Si las interacciones de voz no se enrutan al agente/cola correcto o no aparecen en el panel de interacción, siga los siguientes consejos para la resolución de problemas:

* [Confirme que el agente es miembro de la cola que se creó al comienzo del taller](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/10_first.html#Followalong)

* [Confirme que el número que llama está vinculado al flujo](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/10_first.html)

* [Confirme que el estado del agente está establecido en "En cola"](https://workshop.genesys.com/workshops/gride-demo/040-inbound-voice/20_second.html)

* Los nuevos sitios híbridos no tienen una troncal telefónica definida de forma predeterminada. Deberá definir uno manualmente en Edge Groups. Si recibe este mensaje de error a continuación cuando intenta enrutar una interacción de voz, confirme que se ha definido un Edge Group. Puedes encontrar esas instrucciones. [Aquí](https://workshop.genesys.com/workshops/gride-demo/030-telephony/10_first.html)

![Address of Reference](/images/AoR.jpg)

 Si las interacciones aún no se enrutan correctamente, contáctenos en Workshops@genesys.com.

