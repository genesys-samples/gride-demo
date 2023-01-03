---
title: "Telefonía"
chapter: true
weight: 20
---
![Title](/images/Telephony2New-768x300.jpg)

## Comprar un número de teléfono

>Compre números de teléfono directamente desde Genesys Cloud Voice mediante el portal de compra de números. **NOTA: Compraremos un número de teléfono en este módulo. Es importante que anote el número antes de hacer clic en "Completar compra"."**

## Follow along

**Nota**: Se requiere pedir un mínimo de un número, pero se recomienda pedir 1 número para cada usuario que utilizará Dev Lab. Los cargos de telefonía se le facturan, así que cómprelos en su organización: https://help.mypurecloud.com/articles/genesys-cloud-voice-pricing/

1. Haga clic en Admin > Administración de números > **Haga clic en "Comprar número"** <br>

	(Si no ve Administración de números en el panel de administración, es necesario que cierre la sesión y vuelva a iniciarla para actualizar los permisos recién agregados)
	
2.	Busque un número DID por código de área o ciudad/estado _(Escriba este número de teléfono ya que no podrá encontrarlo más adelante)_

3. Marque las casillas junto a cada número que vaya a comprar (con al menos uno apto para emergencias) y complete la compra

6. Marque la casilla para **"Hacer que esta ubicación esté disponible para su uso en sitios"**.

7. Agregue un número de emergencia.


![LocationDetails](/images/LocationsPopup.jpg)

## Site


Un site es el hogar de un conjunto de teléfonos. El sitio define las reglas de clasificación de llamadas y las reglas de enrutamiento de salida, así como las propiedades de telefonía para marcar. Aquí también es donde el enrutamiento de salida hará referencia a un plan numérico. Los sitios deben estar vinculados a las ubicaciones físicas definidas.

![AdminDirectory](/images/Site.jpg)

1. **Vaya Admin> Site> Clic "Crear Site"**

2.  Crear un nuevo site y nombrarlo **"Mi Site"**. 

3. Asocia tu ubicación, selecciona una zona horaria, deja Media Model como "Nube"

![SiteDetails](/images/SiteSetup.jpg)

3.Navegue a Rutas salientes dentro del sitio recién creado y en **"Seleccionar troncales externas"** asegúrese de que la troncal "PureCloud Voice - AWS" esté asociada. Asegúrese de **"Habilitar"** el Estado también.

![OutboundRoutingDetails](/images/OutboundRoute.jpg)

4. Por último, regrese a la pestaña **"General"** y confirme que el sitio se ha seleccionado como predeterminado.


![SiteSettings](/images/DefaultSite.jpg)
