## Cómo acceder a Cloud Console

### Comience el lab

-   Ahora que comprende las características y los componentes clave de un lab, haga clic en **Comenzar lab**.

Es posible que el entorno de [[Google Cloud]] y las credenciales tarden un momento en iniciarse. Cuando el temporizador comienza la cuenta regresiva y el botón Comenzar lab cambia a rojo y dice Finalizar lab, significa que todo está listo y ya puede acceder a Cloud Console.

**Nota:** No haga clic en el botón Finalizar lab hasta que haya completado todas las tareas del lab. Si hace clic en el botón, sus credenciales temporales ya no serán válidas, y usted no podrá acceder al trabajo que realizó en el lab. Debe hacer clic en este botón cuando termine. Si no lo hace, no podrá realizar otro lab. (Qwiklabs cuenta con protecciones que impiden la inscripción simultánea)

### Panel Detalles de la conexión

Ahora que la instancia de su lab está en funcionamiento, observe el panel de la izquierda. Contiene el botón Abrir Google Console, las credenciales (nombre de usuario y contraseña) y un campo ID del proyecto.
![](https://cdn.qwiklabs.com/%2FtHp4GI5VSDyTtdqi3qDFtevuY014F88%2BFow%2FadnRgE%3D)

#### Abre Google Console

Este botón abre [Cloud Console](https://cloud.google.com/cloud-console/): la consola web y el centro de desarrollo principal de Google Cloud. Realizará la mayor parte del trabajo en Google Cloud desde esta interfaz. Todos los Qwiklabs de Google Cloud usan Cloud Console de alguna forma.

#### ID del proyecto

Un [proyecto de Google Cloud](https://cloud.google.com/docs/overview/#projects) es una entidad que le permite organizar los recursos allí incluidos. A menudo, contiene recursos y servicios; por ejemplo, puede incluir un grupo de máquinas virtuales, un conjunto de bases de datos y una red que los conecta entre sí. Los proyectos también contienen configuraciones y permisos que especifican las reglas de seguridad y quiénes tienen acceso a cada recurso.

El _ID del proyecto_ es un identificador único que se utiliza para vincular los recursos de Google Cloud y las API con su proyecto específico. Los ID de proyecto son únicos en Google Cloud: solo puede haber un **qwiklabs-gcp-xxx…**, que identifica al proyecto a nivel global.


#### Nombre de usuario y contraseña

Estas credenciales representan una identidad en el servicio de Cloud Identity and Access Management (Cloud IAM). Esta identidad tiene permisos de acceso (una o más funciones) que le permiten trabajar con recursos de Google Cloud en el proyecto que se le haya asignado. Estas credenciales son _temporales_ y solo funcionan durante el período de acceso al lab. Cuando el temporizador llegue a 00:00:00, ya no tendrá acceso a su proyecto de Google Cloud con esas credenciales

### Tarea 1: Acceda a Google Cloud

Ahora que comprende mejor el panel Detalles de la conexión, use su contenido para acceder a Cloud Console.

1.  Haga clic en **Abrir Google Console**.

Esta acción abrirá la página de acces	o de Google Cloud en una pestaña nueva del navegador.

![SignInPage.png](https://cdn.qwiklabs.com/VkUIAFY2xX3zoHgmWqYKccRLwFrR4BfARLd5ojmlbhs%3D "Página de Acceso con Google")

Si alguna vez accedió a una aplicación de Google, como Gmail, esta página debería resultarle familiar.

**_Sugerencia:_** Abra las pestañas en ventanas separadas, una junto a la otra.

Si se abre la página **Elegir una cuenta**, haga clic en **Usar otra cuenta**. ![Usar otra cuenta](https://cdn.qwiklabs.com/eQ6xPnPn13GjiJP3RWlHWwiMjhooHxTNvzfg1AL2WPw%3D)

2.  Copie el **Nombre de usuario** del panel Detalles de la conexión, péguelo en el campo **Correo electrónico o teléfono** y haga clic en **Siguiente**.

***!_¡Un momento! Asegúrese de usar el correo electrónico googlexxxxxx_student@qwiklabs.net para acceder, NO su dirección de correo electrónico personal o corporativo._***

3.  Copie la **Contraseña** del panel Detalles de la conexión, péguela en el campo **Contraseña** y haga clic en **Siguiente**.
    
4.  Haga clic en **Aceptar** para indicar que está de acuerdo con las Condiciones del Servicio y la Política de Privacidad de Google.
    
5.  En la página **Protege tu cuenta**, haga clic en **Confirmar**.
    

Dado que esta cuenta es temporal, no se preocupe por actualizar los números de teléfono ni los correos electrónicos de recuperación.

6.  En la página **Welcome student!**, marque las **Condiciones del Servicio** para aceptar las Condiciones del Servicio de Google Cloud y haga clic en **Aceptar y continuar**.

Accedió correctamente a Cloud Console con sus credenciales de Qwiklabs. Ahora su página debería ser similar a la siguiente:

![35a55968748df7c0.png](https://cdn.qwiklabs.com/vPsOw690IZhUlPPxZk3asDaXQBRVZRiyr%2B6nBXCqEf4%3D "Se accedió a Google Cloud Console")

Hay siete categorías de servicios de Google Cloud #important :
 
-   **Procesamiento:** Incluye una variedad de tipos de máquinas que admiten cualquier tipo de carga de trabajo. Las diferentes opciones de procesamiento le permiten decidir cuánto control quiere sobre la infraestructura y los detalles operativos.
-   **Almacenamiento:** Incluye opciones de bases de datos y almacenamiento para datos estructurados o no estructurados, relacionales o no relacionales.
-   **Herramientas de redes:** Incluye servicios que balancean el tráfico de las aplicaciones y aprovisionan reglas de seguridad.
-   **Operaciones:** Incluye un paquete de herramientas de confiabilidad de registro, supervisión, seguimiento y otros servicios, aplicables entre nubes diferentes.
-   **Herramientas:** Incluye servicios que ayudan a los desarrolladores a administrar las implementaciones y las canalizaciones de compilación de aplicaciones.
-   **Macrodatos:** Incluye servicios que le permiten procesar y analizar grandes conjuntos de datos.
-   **Inteligencia artificial:** Incluye un paquete de API que ejecutan tareas específicas de inteligencia artificial y aprendizaje automático en Google Cloud.

## Finalice su lab

Ahora que terminó el lab, haga clic en **Finalizar lab** y, luego, en **Aceptar** para confirmarlo.

![end_lab.gif](https://cdn.qwiklabs.com/W%2B4SnUeJ5uNFmTjaRFdsBrUHr0SSyl%2BFkgc3i%2B6Eyxc%3D "Animación de finalización del lab")

Califique cada lab que realice en Qwiklabs. ![five_stars.png](https://cdn.qwiklabs.com/LZUBJPyOLYREWQFfmfqWDA%2Ftgxsb4hvRrg32UipHjD0%3D "Calificación de cinco estrellas")

Califique el lab con la nota máxima si está satisfecho o con una puntuación menor si no lo está. Deje comentarios sobre sus experiencias en la ventana “Comentario”. Google aprecia los comentarios considerados.

Cuando finalice un lab, perderá su acceso al proyecto de Google Cloud y al trabajo que realizó en él. Si regresa a Cloud Console, verá que su sesión se cerró automáticamente. Ahora puede cerrar esa pestaña.

