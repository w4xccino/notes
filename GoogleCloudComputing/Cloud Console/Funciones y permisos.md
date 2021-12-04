Anteriormente, aprendió que, además de los servicios de computación en la nube, [[Google Cloud]] también contiene una colección de permisos y funciones que definen quiénes tienen acceso a cada recurso. Puede usar el servicio [Cloud Identity and Access Management (Cloud IAM)](https://cloud.google.com/iam/) para inspeccionar y modificar tales funciones y permisos. [[Cloud Console]]

### Tarea 3: Visualice sus funciones y permisos

1.  En **Menú de navegación** (![Menú de navegación](https://cdn.qwiklabs.com/tkgw1TDgj4Q%2BYKQUW4jUFd0O5OEKlUMBRYbhlCrF0WY%3D "Menú de navegación")), haga clic en **IAM y administración**. Esta acción abrirá una página que contiene una lista de usuarios y especifica los permisos y las funciones otorgados a cuentas específicas.

![87534f555ed17b88.png](https://cdn.qwiklabs.com/v5er%2BfG4yURAeD9YUOKNuDgtD9KdMi9Sg2Ph9XThkZA%3D "Animación del administrador de IAM")

2.  Busque el nombre de usuario "@qwiklabs" con el que accedió:

![iam.png " Encuentra miembro de Qwiklabs"](https://cdn.qwiklabs.com/zchfMWz4f12cRb%2BV73VmuS75Io5iFtKItiK7dRXnyDo%3D "Encontrar el nombre de usuario")

En la columna Miembro, se muestra `_googlexxxxxx_student@qwiklabs.net_` (que coincide con el nombre de usuario con el que accedió). En la columna Nombre, se muestra `_googlexxxxxx_student@qwiklabs.net student_`. En la columna Función, se muestra _Editor_, que es una de las tres _funciones básicas_ que ofrece Google Cloud. Estas funciones establecen permisos a nivel de proyecto y, a menos que se especifique lo contrario, controlan el acceso a todos los servicios de Google Cloud y su administración.

En la siguiente tabla, se extraen definiciones de la [documentación de funciones](https://cloud.google.com/iam/docs/understanding-roles/#primitive%5C_roles) que ofrecen una descripción general breve de los permisos de las funciones de visualizador, editor y propietario: #important 

| Nombre de la funcion | Permisos |
| --- | ----------- |
| visor | Permisos para acciones de solo lectura que no afectan el estado, como leer (pero no modificar) los recursos o datos existentes |
| editor | Todos los permisos de la función de visualizador y permisos adicionales para acciones que modifican el estado, como cambiar recursos existentes (***solamente pueden editar algunos recursos que son establecidos por el propietario del proyecto***)|
| propietario |Todos los permisos de la función de editor y aquellos necesarios para realizar las siguientes acciones: administrar las funciones y los permisos de un proyecto y todos sus recursos correspondientes; configurar la facturación de un proyecto |

Como editor, puede crear, modificar y borrar recursos de Google Cloud. Sin embargo, no puede agregar ni borrar miembros de los proyectos de Google Cloud.


