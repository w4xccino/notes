## Variables: (lvc)
```javascript
let a = 12 //hace que a sea leida solamente por la funcion que lo contiene ademas la variable solamente se  puede declarar una vez. 
var b = 10 //b se convierte en una variable global.
const c = 9 //c solamente puede ser declarada una vez y su valor no puede cambiar.
```

Normalmente las variables `const` se declaran con nombres en mayusculas separados por un subguion. 

## Metodos
-> `.length` sirve para medir la longitud de un elemento iterable.
-> `.pop()` elimina el ultimo elemento de un elemento iterable. 
-> `.shift()` elimina el primer elemento de un elemento iterable.
-> `unshift` agrega elemento al inicio de un elemento iterable.

## Funciones
> Es importante crear funciones con varibles `let` o `const` para que no hayan conflictos con otras variables. Asi mismo, estas variables solo existen en la funcion
```javascript
function nameFunction(attributes){
	//function content
}
```
	

## Condicionales
```javascript
7 == 7 //True
7 == '7' //True
7 === '7' //false

7 != 7 //false
7 != '7' //false
7 !== '7' //true
```

#### Sintaxis
```javascript
if (<condition>){
	//content1
}if else{
	//content2
}
else{
	//content3
}
```


## Objetos
#### Creacion
Los objetos en JS se crean de la siguiente manera:
```javascript
let dog{
	name:"Richard",
	age: 16,
	gender: "None is a dog"
}
```

#### Acceso
Los objetos tienen la caracteristica de almacenamiento **clave/valor** es decir, como un diccionario.
Se puede usar para ahorrarnos tiempo en la creacion de sentencias `if else` o `switch case`

Se pueden acceder a los objetos siguiendo esta sintaxis:
```javascript
dog.name // return Richard
dog[age] //return 15
```

#### Eliminacion de propiedades.
```javascript
delete dog.gender // elimina la propiedad gender de nuestro objeto**
```

#### Verificación de propiedades de un objeto.
Se hace con la sentencia `.hasOwnProperty(<propname>)`
```javascript
dog.hasOwnProperty(name); //return True;
dog.hasOwnProperty(gender); //return False porque lo eliminamos anteriormente

```

## Objetos complejos
Como sabemos, los objetos pueden almacenar una estructura de datos flexible, es decir, que se almacenar gran cantidad de tipos de datos en él (cadenas, booleanos, enteros, arreglos). 
```javascript
const ourMusic = [
  {
    "artist": "Daft Punk",
    "title": "Homework",
    "release_year": 1997,
    "formats": [ 
      "CD", 
      "Cassette", 
      "LP"
    ],
    "gold": true
  }
];
```

#important 
Se puede notar que este arreglo contiene un objeto dentro que, dentro del objeto mismo hay un arreglo tambien.
A este tipo de dato, se le llama objecto complejo.
Se puede almacenar mas objetos dentro del arreglo `ourMusic` añadiendo una coma(`,`) despues del objeto. 
Esto tiene la misma sintaxis que [JavaScript Object Notation](http://www.json.org/) o `JSON`este un formato de intercambio de datos relacionado utilizado para almacenar información.
```js
const myMusic = [

{

"artist": "Billy Joel",

"title": "Piano Man",

"release_year": 1973,

"formats": [

"CD",

"8T",

"LP"

],

"gold": true

}, // la coma viene a separar el objeto.

{

"artist": "Daft Punl",

"title": "Technologic",

"release_year": 2004,

"formats": [

"CD",

"8T",

"LP"]

}

];
```

### Objetos anidados
Se puede acceder a las sub propiedades de objetos encadenando la notación de puntos o corchetes.

Aquí hay un objeto anidado:

```js
const ourStorage = {
  "desk": {
    "drawer": "stapler"
  },
  "cabinet": {
    "top drawer": { 
      "folder1": "a file",
      "folder2": "secrets"
    },
    "bottom drawer": "soda"
  }
};

ourStorage.cabinet["top drawer"].folder2;
ourStorage.desk.drawer;
```

`ourStorage.cabinet["top drawer"].folder2` sería la cadena `secrets` y `ourStorage.desk.drawer` sería la cadena `stapler`

## Bucles
- While
```js
let c = 0
while (c<10){
console.log(c)
}
```

- For
```js
const arr = [10, 9, 8, 7, 6];

for (let i = 0; i < arr.length; i++) {
   console.log(arr[i]);
}
```

 ## ParseInt
 ```js
const a = parseInt("007"); //return 7 int
```

## Recursividad
> Factorial

```js
function fact(n){
	if (n==1){
		return 1;
	}
	else{
		return n * fact(n - 1);
	}
}
```

Usar [PythonTutor](https://pythontutor.com/) para una mejor comprension junto a este [video](https://www.youtube.com/watch?v=SRR4TLey2lA)


