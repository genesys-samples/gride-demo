---
title: "Configuración del teléfono WebRTC"
chapter: true
weight: 30
---
![Title](/images/WebRTC-768x300.jpg)
## Crear una configuración base de WebRTC

Antes de poder crear un teléfono, cree una configuración básica para ese modelo de teléfono. La configuración básica contiene un grupo de configuraciones que se encuentran en las pestañas Base Phone y Base Line Appearance que definen cómo debe funcionar un modelo de teléfono en particular en Genesys Cloud. Una vez que crea una configuración de configuración básica, puede guardarla con la configuración predeterminada o puede personalizar la configuración. Se puede hacer referencia rápidamente a estas configuraciones para agilizar el aprovisionamiento de nuevos teléfonos.


1. Haga clic en Admin> Administración del teléfono> Haga clic en "Configuración base"

2. Seleccione **"Agregar configuración básica"**. Ingrese un nombre como **"General WebRTC"** y luego busque en el campo "Marca y modelo del teléfono" **Teléfono Genesys Cloud WebRTC"**.

3. Haga clic en **"Guardar configuración básica"**


![BaseSettingsConfig](/images/BaseSettings.jpg)

## Cree un teléfono WebRTC para su usuario

 Genesys Cloud admite la tecnología WebRTC con el teléfono Genesys Cloud WebRTC. Al aprovisionar un teléfono Genesys Cloud WebRTC para un usuario, se crea una línea telefónica específica para ese usuario. El teléfono Genesys Cloud WebRTC no requiere la instalación de un cliente de software en la PC. Utilice los controles de llamadas de Genesys Cloud para las llamadas telefónicas de WebRTC.

1. Haga clic en Admin> Administración del teléfono> Haga clic en "Agregar teléfono"** *La mejor práctica es nombrar su teléfono con el nombre del usuario que se asociará con él.*
 
2. Seleccione la **Configuración base de WebRTC** que creó en el paso anterior.
 
3. Seleccione el **sitio** que creó en el capítulo anterior.
 
4. Seleccione el **agente** que utilizará el teléfono WebRTC.  


![WebRTCPhoneSettings](/images/PhoneSetup.jpg)

## Activación de su teléfono

1. Localice el icono del teléfono en la barra de herramientas izquierda. Nota: El teléfono puede estar rojo con una línea que lo atraviesa porque no tiene un teléfono asignado.

2. Seleccione el ícono **"Detalles del teléfono"** en el menú deslizable.

3. Haga clic en **"Seleccionar teléfono"** para buscar el nombre de su teléfono. Su configuración de WebRTC ahora está completa, asignada al agente apropiado y lista para manejar interacciones de voz. 


![PhoneAssignment](/images/PhoneSelect.jpg)