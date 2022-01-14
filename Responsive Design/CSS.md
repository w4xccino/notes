# CSS 
CSS es un lenguaje estilo cascada que permite mejorar el aspecto de los elementos de un archivo `HTML`

Hay aspectos #important sobre CSS como por ejemplo:

## Margin
Sirve para establecer la distancia de un elemento entre un `border` para fuera

## Padding
Sirve para establecer la distancia de un elemento entre un `border` para dentro
Cada uno de los elementos puede especificarse como:
`padding-top`
`padding-left`
`padding-right`
`padding-bottom`
Pero tambien puede establecerse como:
```css
padding: 10px 20px 10px 20px
```
Esto se establecer deacuerdo a las agujas del reloj.

### Ejemplo:
![[Pasted image 20211221135313.png]]

## **Usa selectores de atributos para dar estilo a elementos**
Hasta ahora, has añadido atributos `id` o `class` a elementos para aplicarles estilos específicos. Estos se conocen también como selectores de ID y de clase. Sin embargo, existen otros selectores CSS que puedes utilizar para seleccionar grupos personalizados de elementos a los que quieras aplicar el mismo estilo.

Para este desafío, usarás el selector de atributos `[attr=value]` para aplicar estilo a las casillas de verificación (checkboxes).

**EJEMPLO**
```css
[type='radio'] {
  margin: 20px 0px 20px 0px;
}
```

## **Unidades absolutas y relativas de medida**
Varios de los últimos desafíos establecen el "margin" o "padding" de un elemento usando píxeles (`px`). Los píxeles son un tipo de unidad de longitud que le indica al navegador qué tamaño o cuánto espaciado asignarle a un elemento. Además de `px`, CSS cuenta con variedad de opciones de unidades de longitud que puedes utilizar.

Los dos tipos principales de unidades de longitud son las unidades absolutas y relativas. Las unidades absolutas están relacionadas con unidades físicas de longitud. Por ejemplo, `in` y `mm` se refieren a pulgadas y milímetros, respectivamente. Las unidades de longitud absoluta aproximan la medición real sobre una pantalla, pero existen cierta variación que depende de la resolución de la pantalla utilizada.

Las unidades relativas, como `em` o `rem` son relativas a otro valor de longitud. Por ejemplo, `em` se basa en el tamaño de fuente de un elemento. Si la utilizas para establecer la propiedad `font-size`, es relativa al `font-size` del elemento padre.

**Nota:** Hay varias opciones de unidades relativas que están vinculadas al tamaño del viewport. Veremos estas unidades relativas de medida en la sección de principios de diseño web responsivo.

## **Utiliza código hexadecimal (hex code) para mezclar colores**

Repasemos: En código hexadecimal se utilizan 6 dígitos hexadecimales para representar los colores, dos para el componente rojo (R), verde (G) y azul (B).

¡A partir de estos tres colores puros (rojo, verde y azul) podemos variar las cantidades de cada componente de color para crear más de 16 millones de colores distintos!

Por ejemplo, el naranja es rojo puro mezclado con algo de verde y nada de azul. En hex code, esto se traduce como `#FFA500`.

El dígito `0` es el número más bajo en hex code, y representa la ausencia total de color.

El dígito `F` es el número más alto en hex code, y representa el brillo máximo.

## **Crea una variable de CSS personalizada**

Para crear una variable CSS, solo tienes que darle un nombre que comience con dos guiones (--) y asignarle un valor, como se muestra a continuación:

```css
--penguin-skin: gray;
```

Esto creará una variable llamada `--penguin-skin` y le asignará el valor `gray`. Ahora puedes usar esa variable en cualquier otro lugar de tu código CSS para cambiar el valor de otros elementos a "gray" (gris).

Esto creará una variable llamada `--penguin-skin` y le asignará el valor `gray`. Ahora puedes usar esa variable en cualquier otro lugar de tu código CSS para cambiar el valor de otros elementos a "gray" (gris).

## **Cambia la posición de los elementos superpuestos con la propiedad z-index**
#important 
Cuando los elementos son posicionados para superponerse (i.e. usando `position: absolute | relative | fixed | sticky`), el elemento que viene después dentro del marcado HTML aparecerá, por defecto, encima de los otros elementos. Sin embargo, la propiedad `z-index` puede especificar el orden de cómo los elementos están apilados unos sobre otros. Debe ser un entero (i.e. un número entero y no un decimal), y los elementos que mayor valor tengan en `z-index` serán movidos más arriba en la pila de elementos que aquellos con valores menores.

