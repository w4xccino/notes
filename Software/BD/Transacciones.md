# Transacciones [[SQL]]
Las [[transacciones]] son operaciones que se ejecutan en un bloque. Puede tomarse como un proceso externo a la informática. Es decir, que son un conjunto de operaciones que si falla una sentencia, falla toda la transacción. 

Las transacciones cumplen con las propiedades #ACID

## #ACID
- **Atomicity** (*Atomicidad*): Se deben ejecutar todas las operaciones, o ninguna. "O es todo el atomo, o no es nada."

- **Consistency** (*Consistencia*): Las operaciones no deben de fallar, es decir no deben de tener errores ni de semántica, ni de sintaxis. La transacción primero verifica si ninguna de las sentencias tiene error y luego, finalmente, ejecutan las [[transacciones]]

- **Isolation** (*Aislamiento*): Esta propiedad garantiza que una operación no debe afectar a otras. Esto asegura que la realización de dos transacciones sobre la misma información sean independientes y no generen ningún tipo de error. 


	La primera transacción bloquea  a la segunda si la primera transacción afecta **al mismo tiempo** y la segunda debe esperar a que la primera termine.

- **Durability** (*Durabilidad*): Por cada transacción que se ejecuta, se hace un *commit* de los datos (manualmente al final de cada transacción) y si existe algun problema, se puede hacer un *rollback*. Los datos persisten porque el commit se ha ejecutado.