## Const
Se pueden alterar los valores de las variables const si accedemos intrinsecamente a ellos:

**Por Ejemplo:**
```js
const a = [1,3,2];
a[0]=34;
```
El valor de `a` se convertira a `[34,3,2`] .
Para evitar ello se puede usar el metodo `Object.freeze(a)`. Asi el objecto queda "congelado" y sus valores no se podran alterar.

## Funciones flecha
Normalmente en ES6 o en JS en general, no se suelen nombrar las funciones, especialmente cuando son el parametro de otras funciones.
```js
const a = console.log(function()){
//contenido 
}
```

Para ahorrarnos espacio y simplificar las cosas, se usan funciones flecha, por ejemplo:
```js
const a = () => //return contenido;
```
No es necesario usar el return.

Para poder tener argumentos dentro de una funcion flecha =>   

- Con un solo argumento:
```js
const a = arg => //return contenido;
```
- Para dos o mas argumentos.

```js
const a = (arg1,arg2) => //return contenido;
```

## Parametro Rest
Los parametros rest permiten crear funciones mas flexibles. Los parametros ingreados se convierten en un arreglo. El numero de argumentos de esta funcion son indefinidos.

```js
function howMany(...args) {
  return "You have passed " + args.length + " arguments.";
}
console.log(howMany(0, 1, 2));
console.log(howMany("string", null, [1, 2, 3], { }));
```

La consola mostrará las cadenas `You have passed 3 arguments.` y `You have passed 4 arguments.`.

### Operador de propagación para evaluar los arreglos en el lugar.
Asi tambien, el parametro rest, puede usarse para funciones que solamente esperan un argumento. Por ejemplo:
```js
const arr = [6, 89, 3, 45];
const maximus = Math.max(...arr);
```

`maximus` tendría un valor de `89`.

Asi tambien, si se desea agregar o copiar un arreglo:
```js
a = [1,2,3,5]
b = [...a]
```

> Eso hara que `b` tenga los valores de `[1,2,3,5]`

## Desestructuración de objetos.
En ES5, para desestructurar un objeto se hacia lo siguiente:
```js
const user = { name: 'John Doe', age: 34 };

const name = user.name;
const age = user.age;
```
Las variables `name` y `age` tendrian los valores de `John Doe` y `34` respectivamente. 

Pero con ES6, esto se vuelve mas sencillo.

```js
const { name, age } = user;
```
De nuevo, `name` tendrá una cadena con valor `John Doe`, y `age` tendrá el número `34`.

### Sintaxis de desestructuración para asignar variables desde objetos
Usando el mismo objeto del ejemplo anterior:

```js
const user = { name: 'John Doe', age: 34 };
```

Así es como puedes dar nuevos nombres de variables en la asignación:

```js
const { name: userName, age: userAge } = user;
```

Puedes leerlo como "obtén el valor de `user.name` y asígnalo a una nueva variable llamada `userName`" y así sucesivamente. El valor de `userName` sería la cadena `John Doe`, y el valor de `userAge` sería el número `34`.

### Objetos anidadados:
Usando un objeto similar a los ejemplos anteriores:

```js
const user = {
  johnDoe: { 
    age: 34,
    email: 'johnDoe@freeCodeCamp.com'
  }
};
```

Así es como se extraen los valores de propiedades de objetos y se los asigna a variables con el mismo nombre:

```js
const { johnDoe: { age, email }} = user;
```

Y así es como se puede asignar los valores de las propiedades de un objeto a variables con diferentes nombres:

```js
const { johnDoe: { age: userAge, email: userEmail }} = user;
```


## Sintaxis de desestructuración para asignar variables desde arreglos
Una diferencia clave entre el operador de propagación y la desestructuración de arreglos es que el operador de propagación desempaca todos los contenidos de un arreglo en una lista separada por comas. En consecuencia, no puedes elegir qué elementos deseas asignar como variables.

Desestructurar un arreglo nos permite hacer exactamente eso:

```js
const [a, b] = [1, 2, 3, 4, 5, 6];
console.log(a, b);
```

La consola mostrará los valores de `a` y `b` como `1, 2`.

A la variable `a` se le asigna el primer valor del arreglo, y a `b` se le asigna el segundo valor del arreglo. También podemos acceder al valor en cualquier índice de un arreglo con la desestructuración usando comas para alcanzar el índice deseado:

```js
const [a, b,,, c] = [1, 2, 3, 4, 5, 6];
console.log(a, b, c);
```

La consola mostrará los valores de `a`, `b`, y `c` como `1, 2, 5`.

> **EJEMPLO**
Utiliza la sintaxis de desestructuración para intercambiar los valores de `a` y `b` para que `a` reciba el valor almacenado en `b`, y `b` reciba el valor almacenado en `a`.

>```js
let a = 8, b = 6;
[a,b] = [b,a] //solucion

## Cadenas usando plantillas literales

Una nueva característica de ES6 es la plantilla literal. Este es un tipo especial de cadena que facilita la creación de cadenas complejas.

Las plantillas literales te permiten crear cadenas multilínea y usar características de interpolación, para crearlas.

Fíjese en el código debajo:

```js
const person = {
  name: "Zodiac Hasbro",
  age: 56
};

const greeting = `Hello, my name is ${person.name}!
I am ${person.age} years old.`;

console.log(greeting);
```

La consola mostrará las cadenas `Hello, my name is Zodiac Hasbro!` y `I am 56 years old.`.

