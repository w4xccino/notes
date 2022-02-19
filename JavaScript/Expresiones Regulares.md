# Concepto
Las expresiones regulares se utilizan en lenguajes de programación para coincidir con partes de cadenas. Creas patrones para ayudarte a hacer esa coincidencia.

---

### Test Method

Si quieres encontrar la palabra `the` en la cadena `The dog chased the cat`, puedes utilizar la siguiente expresión regular: `/the/`. Ten en cuenta que las comillas no son requeridas dentro de la expresión regular.

JavaScript tiene múltiples formas de usar expresiones regulares. Una forma de probar una expresión regular es usando el método `.test()`. El método `.test()` toma la expresión regular, la aplica a una cadena (que se coloca dentro de los paréntesis), y devuelve `true` o `false` si tu patrón encuentra algo o no.

```js
let testStr = "freeCodeCamp";
let testRegex = /Code/;
testRegex.test(testStr);
```

El método `test` aquí devuelve `true`.

##### Busqueda de múltiples valores: 
En el ejemplo anterior, podemos buscar valores en cadenas. Esto es potente, pero no se puede usar con multiples valores. A no ser que usemos los  operadores: `|`

```js
let petString = "James has a pet cat.";

let petRegex = /dog|cat|bird|fish/;

let result = petRegex.test(petString); //true
```

##### Ignora la capitalización al coincidir
Que pasaria si queremos coincidir valores y que no importen si estos valores no son semejantes en la capitalizacion. Es decir, que `Diego` sea igual a `dieGo`.
Para ello, se agrega la expresion regular `/text/i`.

```js
let myString = "freeCodeCamp";

let fccRegex = /freeCodeCamp/i; 

let result = fccRegex.test(myString); //true
```

---

### Match Method
Hasta ahora solamente podemos comprobar si un patrón existe dentro o no de una cadena.
Pero también se pueden extraer los valores que coinciden encontradas con el método `.match()`

Para utilizar el método `.match()`, aplica el método a una cadena y pasa la expresión regular dentro de los paréntesis.

Este es un ejemplo:

```js
"Hello, World!".match(/Hello/);
let ourStr = "Regular expressions";
let ourRegex = /expressions/;
ourStr.match(ourRegex);
```

Aquí el primer `match` devolverá `["Hello"]` y el segundo devolverá `["expressions"]`.

Ten en cuenta que la sintaxis `.match` es lo "opuesto" al método `.test` que has estado utilizando hasta ahora:

```js
'string'.match(/regex/);
/regex/.test('string');
```


##### Encuentra más que la primera coincidencia

Para buscar o extraer un patrón más de una vez, puedes utilizar la bandera `g`.

```js
let repeatRegex = /Repeat/g;
testStr.match(repeatRegex);
```

Y aquí `match` devuelve el valor `["Repeat", "Repeat", "Repeat"]`



