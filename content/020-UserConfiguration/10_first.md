---
title: "Roles y Permisos"
chapter: true
weight: 10
---
![Title](/images/UserConfig2-768x300.jpg)
## Roles y Permisos

>Cada rol en Genesys Cloud contiene uno o más permisos. Los permisos permiten a los usuarios con ese rol realizar varias tareas, como crear grupos, configurar integraciones y supervisar la actividad del centro de contacto.

>El rol de empleado tiene el nivel más bajo de permisos y se asigna a todos los usuarios. Este rol no se puede eliminar. Un administrador de Genesys Cloud debe asignar roles adicionales a un usuario para tener permisos adicionales.
>El rol de administrador tiene permisos para realizar cualquier cambio en una organización de Genesys Cloud. Este rol se asigna automáticamente a quien configura la organización. Esta persona es responsable de invitar a otras personas a una organización de Genesys Cloud y de asignar roles a los invitados.





**Asignación del Rol de Administrador Maestro al usuario**

1.	Click Admin > Personas > **seleccione su Cuenta de Usuario**
2.	En el lado derecho de la pantalla Roles, cambie "Ver:" de **Asignado** a **Todo**
3.	Asignar **administrador maestro** permisos y guardar la cuenta

![Add Role](/images/RolesPic.png)

Crear Rol para los permisos de Genesys Cloud Voice

1.  Click Admin > Roles / Permisos > Click **"Agregar Rol"**
2.	Asigne un nombre al rol, por ejemplo: usuario de GCV o algo que pueda encontrar fácilmente.
3.	Cambie a la pestaña de permisos a la derecha y busque **“PureCloud Voice”** en el campo Permiso
4.	Marque la casilla para todos los permisos y guarde
5.	Regrese a Personas y seleccione su usuario nuevamente 
6.	Vaya al lado derecho de la pantalla Roles y cambie "Ver" de **Asignado** a **Todo**
7.  Asígnate el usuario de GCV que acabas de crear

![Permissions](/images/Permission.png)

**Agregar usuarios adicionales a su organización**

**Nota: La información a continuación sobre cómo agregar usuarios adicionales es para configurar entornos de desarrollo reales y no para talleres presenciales dirigidos por Genesys.**

Cuando crea nuevos usuarios, todo lo que se necesita es un nombre y un correo electrónico (para enviar la invitación). También puede expandirse a **Campos Opcionales** para asignar campos como Título, Departamento, Ubicación, Colas, etc. si conoce esos detalles antes. También existe la opción de importar usuarios de forma masiva en lugar de agregar usuarios de uno en uno. 

Si elige enviar invitaciones a nuevos usuarios más tarde y establece manualmente su estado en inactivo, cuando envía las invitaciones, Genesys Cloud cambia automáticamente su estado a activo.<br>
1.	Haga clic en Administrador <br>
2.	En Personas y permisos, haga clic en Personas <br>
3.	Haga clic en Agregar persona. Se abre el cuadro de diálogo Agregar personas a la organización. <br>

 

![People](/images/People.png)


4.	Haga clic en la pestaña **Persona** .
5.	Complete los campos obligatorios Nombre y Correo electrónico.
6.	(Opcional) Ingrese información adicional haciendo clic en Campos opcionales. 
7.	Note: The Manager field is optional but recommended. Genesys Cloud uses manager assignments to create hierarchy views
8.	(Opcional) Para agregar a la persona a una cola, haga lo siguiente:
9.	En Asignar colas, comience a escribir las primeras letras de la cola deseada
10.	Seleccionarlo de la lista
11.	Nota: asegúrese de asignar la función Empleado, junto con cualquier otra función. Normalmente, el rol de empleado se asigna de forma predeterminada. Sin embargo, agregar roles manualmente durante la creación de usuarios anula el valor predeterminado asignado al empleado.
12.	(Opcional) Para agregar roles para la persona, haga lo siguiente:
13.	En Asignar funciones, comience a escribir las primeras letras de la función deseada
14.	Seleccionarlo de la lista
15.	Asigne roles adicionales según sea necesario
16.	Envía la invitación automáticamente seleccionando Enviar invitación ahora
17.	Nota: Las personas que agregue no pueden unirse a Genesys Cloud hasta que reciban una invitación. Si no haces esto ahora, recuerda hacerlo más tarde
18.	Haga clic en Crear

#### Contactos Externos
Ahora que tenemos nuestro agente del centro de contacto, creemos un cliente para identificarlo durante nuestras interacciones de voz, SMS y correo electrónico (durante nuestra prueba de chat web, configuraremos un contacto en el widget). 
Los contactos externos le permiten crear un repositorio sólido de datos de clientes que sus agentes pueden aprovechar mientras ayudan a sus clientes. Con los contactos externos, un agente puede comunicarse rápidamente con un cliente por correo electrónico, llamada telefónica o mensaje de Twitter. Durante una interacción, un agente construye el historial de interacciones para un cliente al verificar los datos de contacto clave. El agente puede ver rápidamente quién ha interactuado con el cliente y puede leer sobre la relación de su empresa con ellos.

Al igual que con la mayoría de las funciones de Genesys Cloud, se puede agregar un contacto externo desde varias ubicaciones.

En el taller de hoy, 

1. Ubique el **Directorio** en la parte superior izquierda de su interfaz de usuario y haga clic en un menú desplegable.
2. Seleccione **Contactos externos**, en el extremo derecho, elija **+Agregar** y luego **Contacto**.

![External Contact](/images/External.jpg)

Siéntase libre de usar un nombre ficticio aquí, siempre que sea uno que se identifique fácilmente cuando se produzca la interacción. Después de ingresar un nombre y seleccionar la flecha, se abrirá una nueva pantalla con campos adicionales.

3. Agreguemos un **Correo electrónico** y un **Número de teléfono**.

*NOTA: Estos campos deben ser válidos, no ficticios, ya que esto es a lo que Genesys Cloud hará referencia cuando llame, envíe un mensaje de texto y envíe un correo electrónico. La mejor práctica sería usar su correo electrónico de trabajo y cualquier número de teléfono que usará para llamar o enviar mensajes de texto. a la organización*

4. Asegúrese de **Guardar** en la parte inferior izquierda y nos despediremos de nuestro cliente por el momento. 

![External Contact](/images/Contact.jpg)