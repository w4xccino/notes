## Cómo acceder a Cloud Console

### Comience el lab

-   Ahora que comprende las características y los componentes clave de un lab, haga clic en **Comenzar lab**.

Es posible que el entorno de Google Cloud y las credenciales tarden un momento en iniciarse. Cuando el temporizador comienza la cuenta regresiva y el botón Comenzar lab cambia a rojo y dice Finalizar lab, significa que todo está listo y ya puede acceder a Cloud Console.

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