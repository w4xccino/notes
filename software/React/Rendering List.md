# Rendering Lists
Para renderizar una lista en react, es distinto a como se haria en Js nativo. ES decir, React no es un motor de iteraci'on pero hay otras maneras.
Si tenemos una lista de datos, por ejemplo:
```jsx 
let state = {
	list: ["item1", "item2", "item3"]
}
```
Y queremos renderizarlo en el dom, no podemos usar `for` porque React , como dije, no es un motor de iteracion

Se puede solucionar de esta manera.
```jsx
render(){
	return(
		<ul>{this.state.list.map(tag => {
			<li>{tag}</li>)}</ul>
)};
```
Estamos usando `map` para poder obtener todos los elementos de la lista e iterarlos en una *arrow function* que tiene los elementos `<li>` y los renderiza con `{tag}`, osea, el parametro de la arrow function y elemento iterativo.

Pero tendremos un problema si revisamos la consola.
![[Pasted image 20220402181258.png]]
Para solucionar este error, necesitamos agregar claves a nuestros elementos, esto se hace de la siguiente manera:

```jsx
render(){
	return(
		<ul>{this.state.list.map(tag => {
			<li key="{tag}">{tag}</li>)}</ul>
	)};
```

Ahora no tendremos ningun problema si ningun elemento se repite en nuestra lista.

