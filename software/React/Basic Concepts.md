## Installation
To install React, first we need to instal NodeJs.
After that, we gonna use this command:
```
npx create-react-app <name-app>
```

## Elementos
React, puede actualizar componentes y elementos dentro de de los componentes sin necesidad de actualizar  toda la pagina.
Las aplicaciones basadas en **React** son arboles. ES decir, que cada componente, puede contener otros componentes.

### Jsx
Jsx fue desarrollado por Facebook para ofrecernos facilidad al crear componentes de React. 
es decir, con Jsx, podemos hacer esto.
```jsx
let element = <p> Hello World! </p>
```

### Importaciones
Para usar react, debemos importar estos modulos.

```jsx
import React from 'react';

import ReactDOM from 'react-dom';
```

### Clases
Usamos `extend` para heredar los componentes de `React` a una clase.

```jsx 
class App extends React.Component{}
```
#### Elementos basicos de la clase
- `render()` nos sirve para renderizar o mostrar a la vista.
- `state{}` es un objeto que muestra el estado de los parametros en react.
- 