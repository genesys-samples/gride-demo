---
title: "Configuración"
chapter: true
weight: 10
---
![Setup](/images/Inbound1-768x300.jpg)
## Configuración Inbound Voice 
Si bien siguen surgiendo nuevos canales de comunicación, la importancia de la voz permanece. La velocidad y la agilidad de la plataforma del centro de contacto Genesys Cloud CX™ conecta el compromiso de su cliente con la opción de telefonía que mejor se adapta a sus necesidades comerciales. La más amplia variedad de opciones de conectividad de servicios de voz en la industria brinda a los clientes una flexibilidad y elección sin igual. Los clientes pueden elegir Genesys Cloud CX Voice (Genesys telecom) para VoIP, o utilizar la opción BYOC (Bring Your Own Carrier) basada en la nube. Los clientes pueden mantener un contrato de operador o una infraestructura PBX existente, o consolidarse utilizando Genesys como un único proveedor para todas las necesidades. Los clientes que eligen Genesys Cloud CX a menudo se sienten atraídos por las tecnologías de nube y la arquitectura de microservicios que brindan velocidad, estabilidad y agilidad a su negocio. La adopción de una solución en la nube para los servicios de voz es un enfoque preparado para el futuro, ya que extiende estos mismos beneficios de la nube a todo el sistema de comunicaciones de un cliente.

![Phone](/images/phone.png)

#### Voz de Genesys Cloud CX
Genesys Cloud CX Voice es un servicio de telefonía basado en Internet proporcionado por Genesys que, cuando se activa, brinda acceso de telefonía pública a los servicios de Genesys Cloud CX.

#### Traiga su propio proveedor - Bring Your Own Carrier (BYOC)
Genesys Cloud CX BYOC hace referencia a la capacidad de los clientes para definir troncales SIP entre Genesys Cloud CX y dispositivos o servicios de terceros.

## Lo Que Construiremos Hoy
#### Colas
Hoy lo guiaremos a través de la creación de la columna vertebral de su centro de contacto. El motor ACD de Genesys Cloud CX utiliza un sistema de enrutamiento basado en cola con la capacidad de asociar habilidades, idiomas y prioridad a la lógica de enrutamiento. Lo mantendremos simple y comenzaremos con una cola básica.

Las colas de Genesys Cloud CX están equipadas de forma predeterminada para comunicaciones omnicanal. A lo largo de este taller, enrutaremos todos los tipos de medios a la misma cola.

#### Telefonía
Hoy también utilizaremos los servicios Genesys Cloud CX Voice. Como se mencionó anteriormente, le brindamos la flexibilidad de traer su propio operador o utilizar Genesys como operador. Cualquiera de las opciones dentro de Genesys Cloud CX se administra fácilmente y le permite aprovechar los servicios de voz en la nube que se pueden implementar en días sin necesidad de hardware. Los únicos pasos que deberá seguir hoy para configurar Genesys Cloud CX Voice son comprar un número de teléfono y asignar ese número a una ruta de llamada. Bastante simple, ¿verdad? Tenga en cuenta que se incurre en cargos por la compra de un número de teléfono, aunque son mínimos. Consulte este documento para conocer los precios. https://help.mypurecloud.com/articles/genesys-cloud-voice-pricing/

#### Arquitecto

La configuración de capacidades de voz entrante también requiere un flujo de Architect. De hecho, importaremos flujos de arquitectos para cada tipo de medio que configuraremos hoy. Architect es una poderosa herramienta que forma parte de Genesys Cloud CX.

Architect es una herramienta de diseño web basada en arrastrar y soltar fácil de aprender que crea flujos para tipos de medios. Architect utiliza menús y una lógica directa a la cola asociada con mayor frecuencia a los operadores automáticos tradicionales. Sin embargo, también incorpora operaciones lógicas avanzadas y ricas en funciones, como la recopilación de dígitos fuera del menú, el acceso a datos externos (inmersiones de datos), la lógica condicional y la edición de expresiones para ayudar a desarrollar la funcionalidad IVR. Architect también proporciona una gestión de avisos centralizada con soporte en varios idiomas.

Architect también tiene una opción de exportación e importación, una característica que es importante para el taller de hoy. Lo que esto nos permitirá hacer es simplemente proporcionarle un archivo descargable para un flujo de arquitecto y luego puede importar ese archivo a su flujo de arquitecto en su instancia de Genesys Cloud CX. Architect es una herramienta poderosa y es muy divertido aprender a construir flujos de Architect desde cero, pero ese no es el objetivo del taller de hoy. ¡Lo guardaremos para otro día!

## Siga a lo largo

1. Vaya a Admin> Buscar y haga clic en **Colas**> luego haga clic en **Crear cola**
2. Escriba un nombre de cola único en la pestaña **Nombre**
3. Haga clic en **Guardar** y la configuración de la cola se abra en la pestaña **General**
 

4. Navegue a la pestaña **Miembros** > cuadro **Seleccione nuevos miembros** y busque su nombre > Haga clic en el botón **Agregar +**
5. Agregue nuevos miembros según sea necesario

6. Haga clic en **Voz** > agregue un número de llamadas salientes con el número que compró para voz. Clic en Guardar**
  ![Queue Set Calling Party Number](/images/QueueSetCallingParty.jpg)
7. Navegue [Aquí](https://help.mypurecloud.com/articles/download-architect-flow-examples/) > descargue el flujo descrito en la captura de pantalla a continuación> Siga las instrucciones a continuación para **descargar un flujo de muestra**


 ![Flujo de Muestra](/images/sampleflow.jpg)
 ![Flujo de Muestra](/images/sampleinstructions.jpg)

8. Navegue hasta **Arquitecto** en la pantalla de administración como se muestra a continuación > siga las instrucciones para cargar un _Flujo de llamadas entrantes_.
 ![Architect](/images/architect.jpg)
 ![Import Flow](/images/importflow.jpg)

9. Una vez que haya importado el flujo> seleccione **Transferir a ACD**> seleccione la cola que creó anteriormente> y marque la casilla junto a **DTMF va a esta opción de menú desde cualquier menú**. _Consulte la captura de pantalla a continuación para obtener orientación_
  ![Architect Flow](/images/architectflow.jpg)

10. Elimine las tareas **Transferir a usuario** y **Marcar por extensión** siguiendo la captura de pantalla a continuación. Cuando haya terminado estos cambios, asegúrese de seleccionar **Publicar**
  ![Architect Flow](/images/architectflow1.jpg)
        
11. Vaya a la pantalla **Administrador** > busque y haga clic en **Enrutamiento de llamadas** > Haga clic en **+** > Escriba un nombre de enrutamiento de llamadas único en el campo **Nombre** > Haga clic en **+** debajo **Direcciones** > Busque el número de teléfono que compró anteriormente y seleccione **la casilla de verificación junto al número** > Haga clic en **Listo**


    