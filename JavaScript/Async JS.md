## Que es?
La programacion asincronica permite al equipo "pasar" a otra tarea mientras espera que se complete la operacion asincronica. 
Es decir que, las operaciones asincronicas que requieren mucho tiempo, no tiene por que detener todo lo demas de nuestros programas.

Hay innumerables ejemplos de asincronicidad en nuestra vida cotidiana. Limpiar nuestra casa, por ejemplo, implica operaciones asíncronas como un lavavajillas lavando nuestros platos o una lavadora lavando nuestra ropa. Mientras esperamos la finalización de esas operaciones, somos libres de hacer otras tareas.

![[Pasted image 20220117214629.png]]

Del mismo modo, el desarrollo web hace uso de operaciones asincrónicas. Operaciones como hacer una solicitud de red o consultar una base de datos pueden llevar mucho tiempo, pero JavaScript nos permite ejecutar otras tareas mientras esperamos su finalización.


### Promesas:
#important 
Las promesas **son objetos que representan el resultado final de una operación asincrónica**. Un objeto puede estar en uno de los tres estados:

-   **Pendiente:** El estado inicial: la operación aún no se ha completado.
-   **Cumplido:** La operación se ha completado con éxito y la promesa ahora tiene un _valor resuelto._ Por ejemplo, la promesa de una solicitud podría resolverse con un objeto JSON como valor.
-   **Rechazado:** La operación ha fallado y la promesa tiene una razón para el fracaso. Esta razón suele ser de algún tipo.`Error`

Nos referimos a una promesa como _resuelta_ si ya no está pendiente, ya sea que se cumpla o se rechace. Pensemos en un lavavajillas como si tuviera los estados de una promesa:

-   **Pendiente:** El lavavajillas está funcionando pero no ha completado el ciclo de lavado.
-   **Cumplido:** El lavavajillas ha completado el ciclo de lavado y está lleno de platos limpios.
-   **Rechazado:** El lavavajillas encontró un problema (¡no recibió jabón!) y devuelve platos sucios.

Si nuestra promesa de lavado de platos se cumple, podremos realizar tareas relacionadas, como descargar los platos limpios del lavavajillas. Si es rechazado, podemos tomar medidas alternativas, como volver a correrlo con jabón o lavar los platos a mano.

Todas las promesas eventualmente se resuelven, lo que nos permite escribir la lógica de qué hacer si la promesa se cumple o si se rechaza.



![[Pasted image 20220117222906.png]]

> Ejemplo

```js
const inventory = {
  sunglasses: 3,
  pants: 1088,
  bags: 1344
};
const myExecutor = (resolve, reject) =>{
  if (inventory["sunglasses"] > 0){
    resolve("Sunglasses order processed.");
  }
  else{
    reject("That item is sold out.");
  }
}

const orderSunglasses = () => new Promise(myExecutor);
let orderPromise = orderSunglasses();
console.log(orderPromise);
```

Para repasar conceptos click en este [link](https://www.codecademy.com/learn/asynchronous-javascript/modules/javascript-promises/cheatsheet)


### Async and Await
