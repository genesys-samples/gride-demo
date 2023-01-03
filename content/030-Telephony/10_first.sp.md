---
title: "Location & Site"
chapter: true
weight: 10
---

![Title](/images/LocationSiteNew-768x300.jpg) 


## Opciones de telefonía

Genesys Cloud CX está disponible principalmente a través de dos opciones de telefonía, Genesys Cloud Voice y BYOC (Bring Your Own Carrier). Con Genesys Cloud Voice, la telefonía y el centro de contacto PBX se entregan mediante servicios proporcionados por Genesys. No se requiere hardware ni contrato de operador alternativo.

BYOC permite que un cliente permanezca con su proveedor y contrato existente mientras entrega telefonía a través de troncales SIP. El procesamiento de medios se proporciona en la nube.

En el taller de hoy, configuraremos nuestro entorno aprovechando Genesys Cloud Voice. Si desea utilizar nuestra opción BYOC, puede consultar la documentación aquí: (https://help.mypurecloud.com/articles/byoc-cloud-configuration-overview/)


## Locación
1. Esta es la ubicación física en la que residirán sus agentes como su sede. Las ubicaciones están asociadas para las capacidades de enrutamiento de emergencia; no se recomienda usar servicios de emergencia en un laboratorio de desarrollo, pero es un paso obligatorio.


2. **Vaya a Admin > Ubicaciones > Haga clic en "Agregar ubicación"**

![AdminPage](/images/Locations.jpg)

3. Asigne un nombre a su ubicación, **"Sede central"**, luego agregue una dirección. La dirección debe ser válida, a medida que comience a escribirla, aparecerá una lista desplegable.

4. Seleccione una de las opciones autocompletadas para asegurarse de que el directorio la haya identificado como válida para fines del 911.

5. Agréguese como **"Contacto del sitio"** ya que el propósito es solo de demostración.

6. Marque la casilla para **"Hacer que esta ubicación esté disponible para su uso en sitios"**.

7. Agregue un número de emergencia.


![LocationDetails](/images/LocationsPopup.jpg)

## Site


 Un site es el hogar de un conjunto de teléfonos. El sitio define las reglas de clasificación de llamadas y las reglas de enrutamiento de salida, así como las propiedades de telefonía para marcar. Aquí también es donde el enrutamiento de salida hará referencia a un plan numérico. Los sitios deben estar vinculados a las ubicaciones físicas definidas.

![AdminDirectory](/images/Site.jpg)

1. **Ir a Admin> Sitio> Hacer clic en "Crear site"**

2. Cree un nuevo sitio y asígnele el nombre **"Mi site"**.

3. Asocia tu ubicación, selecciona una zona horaria, deja Media Model como "Nube"

![SiteDetails](/images/SiteSetup.jpg)

3. Navegue a Rutas destacadas dentro del sitio recién creado y en **"Seleccionar troncales externos"** asegúrese de que la troncal "PureCloud Voice – AWS" esté asociada. Asegúrese de **"Habilitar"** el Estado también.

![OutboundRoutingDetails](/images/OutboundRoute.jpg)

4. Por último, regrese a la pestaña **"General"** y confirme que el sitio se ha seleccionado como predeterminado. Asegúrese de **Guardar site**


![SiteSettings](/images/DefaultSite.jpg)

## Grupos de bordes

Un grupo perimetral es un conjunto de dispositivos perimetrales que están conectados entre sí para acceder y compartir troncales. En el pasado, las organizaciones BYOC Prem podían tener varios grupos perimetrales para ayudar a reducir la latencia. Genesys Cloud ahora ha presentado Hybrid Media Org, que permite que una organización combine las opciones de conexión de telefonía en la nube y prem.

Para los usuarios de organizaciones híbridas de Genesys Cloud CX, una troncal telefónica no está definida de manera predeterminada. Tendremos que ubicar **Edge Groups** en el menú Telefonía. Luego, **Crear nuevo**, seleccionamos el menú desplegable debajo de Troncales telefónicos y elegimos **Genesys Cloud - Troncal telefónico CDM WebRTC**.

Nuevamente, esto será solo para organizaciones específicas de medios híbridos. Si cree que esto se ha predefinido, pero se encuentra con un error al intentar enrutar las interacciones de voz entrantes, este será un punto principal de solución de problemas. Por lo general, un error aquí hará referencia a AoR o Address of Record.

![SiteSettings](/images/Hybrid.jpg)