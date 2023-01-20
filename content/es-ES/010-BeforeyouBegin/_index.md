---
title: "Antes de Empezar"
chapter: true
weight: 10
---

![Title](/images/DevLabSetup.jpg)
## Objetivo

Este taller pretende ser una guía documentada y resumida para configurar una nueva organización de desarrollo de Genesys Cloud y enrutar las interacciones de voz y digitales. Este tutorial describirá cómo configurar los aspectos básicos con el objetivo de agregar usuarios, colas, enrutamiento de interacciones, etc. El objetivo final es poder enviar interacciones entrantes a través de un IVR al ACD y finalmente entregarlas a un Agente. Aprenderá qué herramientas tienen los agentes a su disposición cuando manejan las interacciones y cómo aprovechar mejor esas herramientas. Este documento es una recomendación y es posible que no sea igual para todos.


**Notas antes de empezar**: <br>

Se recomienda utilizar la función de búsqueda en el panel de administración en lugar de intentar navegar manualmente a cualquiera de las secciones de administración (consulte la imagen a continuación)
![Search](/images/gcadmin.png)

Se recomienda altamente utilizar convenciones de nomenclatura al crear cualquier elemento (aparte de la configuración de ubicación, sitio y base) para asegurarse de que no está desarrollando sobre implementaciones de colegas. Ej: JaneDoe_Queue o JaneDoe_Inboundflow, etc. En este taller, usaremos la convención, "YourLastName_Item", para que sea rápidamente identificable. También le convendría anotar cada uno, de modo que pueda consultarlos sin navegar por la plataforma Genesys Cloud CX. 

## Activación de su cuenta
1. Haga clic en el enlace en su correo electrónico de bienvenida para activar la cuenta. _Se recomienda que ingrese en una cuenta compartida para esta configuración inicial, en lugar de una cuenta personal, para simplificar la recuperación para futuros usuarios_

2. **Admin** > **Genesys Add Ons** > **Asegúrese de que Genesys Cloud Voice Tile esté activo**
![Activate ](/images/activate.jpg)

_Esto debería estar habilitado de forma predeterminada, sin embargo, los pedidos de organizaciones que no sean GCV requerirán activación manual <br>
If activation is required, select the tile and activate GCV- this can take around 10 minutes to fully activate_

**Nota**: Es posible que deba omitir y volver a "Asegurarse de que Genesys Cloud Voice esté activado", ya que es posible que primero deba asegurarse de que se hayan asignado los roles y permisos adecuados al usuario.
