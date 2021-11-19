# AJAX (Asynchronous JavaScript and XML).

- Leer datos de un **[[Servidor]] WEB** despues de haber cargado la pagina
- Actualizar paginas sin recargar la pagina.
- Enviar datos a un servidor web en segundo plano.

## Pasos
1. Se produce un evento en la pagina emisora.
2. JS crea un objeto XmlHttpRequest.
3. El objeto XmlHttpRequest enviara una solicitud a un [[Servidor]] Web.
4. EL [[Servidor]] va a procesar la solicitud.
5. EL servidor va a enviar una respuesta a la pagina web.
6. La respuesta es leida por medio de JS.
7. JS va a realizar la accion requerida.

LOs pasos en el codigo no se ejecutan en un orden secuencial porque AJAX es **asincrono**. 

## Estados de recepcion y envio. #important

### Ready State.
1. Requerimiento no inicializado.
2. Establece una conexion con el servidor
3. El requerimiento ha sido recibido.
4. El requerimiento esta procesandose
5. EL reuqerimiento finalizo y la respuesta esta lista\


### Status
1. El canal esta abierto
2. La pagina esta perdida (Forbidden 403)
3. No se ha encontrado (Not Found 404).
