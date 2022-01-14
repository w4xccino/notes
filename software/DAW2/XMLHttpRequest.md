## Funciones 
- Intercambiar datos con un [[Servidor]] web en segundo plano.


### Creacion del objeto:
- **Fetch API**
`<variable> = new XMLHttpRequest();`
- **IE5 o 6**
` <variable> = newActiveXObject(Microsoft.XMLHTPP);`

## Metodos

- `XMLHttpREquest()` -> Construct
- `abort()` -> Cancela el requerimiento
- `getAllResponseHeaders` -> Devuelve la informacion de la cabecera. 
- `getResponseHeader()` -> Retorna la informacion especifica de una cabecera
- `open(metodo, url, async)` -> determinar la apertura de la conexion
- `open(metodo, url, async, usuario, password)`
- `send()` -> envia el requerimiento al servidor #GET 
- `send(string)` -> envia el requerimiento al servidor #POST .
- `setRequestHeader()` -> adicionar un valor (par) a la cabecera.

## Propiedades.
- `onreadystatechange` -> va a definir una funcion a llamar cuando la propiedad readyState cambie.
- `readyState` -> contiene el estado del ob (`0,1,2,3,4`) en [[AJAX#Ready State]]
- `responseText` 
- `responseXML`
- `status` retornar el numero de conexion con el [[Servidor]] en [[AJAX#Status]]
- `statusText` 


### Example:
```js
if (window.XMLHttpRequest){
	xhttp = new XMLHttpRequest();
}else
{
	xhttp = new activeXObject("microsoft.XMLHttp");
}
```


## Request (Solicitud)

```js 
xhttp.open("GET", "url.asp", true);
xhttp.send();

xhttp.open("POST", "url.asp", true);
xhttp.send();

xhttp.open("POST", "url.php", true);
xhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded")
xhttp.send("dato=valor&dato2=valor2");
```

## Response (Respuesta)\

```js
xhhtp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200){
     //codigo JS que queremos ejecutar
     //incluir responseText / resposeXML
  }
}
```


