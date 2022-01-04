Las [[API]] de [[Google Cloud]] son una parte clave de Google Cloud. Al igual que los servicios, las más de 200 API (en áreas que incluyen desde administración de empresas hasta aprendizaje automático) se integran fácilmente con los proyectos y las aplicaciones de Google Cloud.

Las API son _interfaces de programación de aplicaciones_ que puede llamar directamente o través de las bibliotecas cliente. Las API de Cloud usan principios de diseño orientados a los recursos, como se describe en la [Guía de diseño de API](https://cloud.google.com/apis/design/).

Cuando [[Qwiklabs]] aprovisiona un proyecto de Google Cloud nuevo para una instancia de lab, habilita automáticamente la mayoría de las API de modo que pueda comenzar a trabajar en las tareas del lab con rapidez. Cuando cree sus propios proyectos de Google Cloud fuera de Qwiklabs, deberá habilitar ciertas API usted mismo.

### Tarea 4: Consulte las API disponibles
1.  En **Menú de navegación** (![Menú de navegación](https://cdn.qwiklabs.com/tkgw1TDgj4Q%2BYKQUW4jUFd0O5OEKlUMBRYbhlCrF0WY%3D "Menú de navegación")), haga clic en **API y servicios > Biblioteca**. En el panel izquierdo, debajo del encabezado **CATEGORÍA**, se muestran las diferentes categorías disponibles.

![apis.gif](https://cdn.qwiklabs.com/IhN1xAfMsp0KrMIwX50LGtlzcsup%2BfK45UA1wseaaa4%3D "Animación de la biblioteca de API")

2.  En la barra de búsqueda de API, escriba **Dialogflow** y, luego, haga clic en **Dialogflow API**. Se abrirá la página de descripción de Dialogflow.

![dialogflow.png](https://cdn.qwiklabs.com/TJxda7OL7Z8mAPtAWRFkf16dH2KSGWP%2FS0cEvzofT%2Fw%3D "Habilitar la API de Dialogflow")

La API de Dialogflow le permite compilar aplicaciones conversacionales eficientes (p. ej., para el Asistente de Google) sin tener que comprender el esquema subyacente de aprendizaje automático y lenguaje natural.

3.  Haga clic en **Habilitar**. Se abrirá la página de descripción de Dialogflow.
    
4.  En su navegador, haga clic en el botón Atrás para verificar que la API ahora esté habilitada.
    

![habilitado.png](https://cdn.qwiklabs.com/eTgnbsNvLaqrex7qumvUuzQEc114GwncM%2FV8xL4j594%3D "Confirmación de API habilitada")

5.  Haga clic en **Probar esta API**. Se abrirá una pestaña nueva en el navegador que mostrará la documentación de la API de Dialogflow. Explore esta información y cierre la pestaña cuando termine.
    
6.  Para regresar a la página principal de Cloud Console, en **Menú de navegación**, haga clic en **Página principal**.
    

Si le interesa obtener más información sobre las API, abra la nueva herramienta práctica de Google Cloud llamada [Explorador de API de Google](https://developers.google.com/apis-explorer/#p/). Google también tiene un lab, [Explorador de API: Qwik Start](https://google.qwiklabs.com/catalog_lab/1241), que le proporcionará experiencia práctica con la herramienta, mediante un ejemplo sencillo.