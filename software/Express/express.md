## Conceptos básicos de Express y Node.

```js
let express = require('express');
let app = express();

console.log("Hello World")

app.get("/",(req,res)=> {
  // res.send("Hello Express")
  route = __dirname + "/views/index.html"
  res.sendFile(route)
  res.send
})
```

![[Pasted image 20220504012350.png]]

Revisar bien la variable global de node `__dirname` y tambien el metodo get para asignar rutas.

¡Sirvamos nuestra primer cadena! En Express, las rutas toman la siguiente estructura: `app.METHOD(PATH, HANDLER)`. METHOD es un método http en minúsculas. PATH es una ruta relativa en el servidor (puede ser una cadena, o incluso una expresión regular). HANDLER es una función que Express llama cuando la ruta coincide. Los Handlers toman la forma `function(req, res) {...}`, donde req es el objeto de la solicitud, y res es el objeto de respuesta. Por ejemplo, el handler


### Qué es un middleware?

