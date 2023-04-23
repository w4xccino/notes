## Containers 

El concepto de los contenedores tiene que ver con la abstraccion de un SO. No necesariamente tienen que instalarse todas las herramientas de un SO base, al contrario, solamente se instalan las dependencias necesarias para poder ejecutar un deploy facil de compartir. 

- Fáciles de compartir. 
- Se almacenan en un repositorio de contenedores. 

### Repositorio de contenedores.
Los contenedores se almacenan en un repositorio de contenedores; más o menos parecido a Github.  Estos pueden ser de tipos **Públicos** o **Privados**.

El repositorio público más conocido es: https://hub.docker.com/ y dentro del mismo hay aplicaciones como NodeJS, Python, Postgress, Mysql, entre otros. 

## Antes de los contenedores. 
Antes de los contenedores existía el problema de que, al trabajar con varios desarrolladores era complicado unififcar las versiones de las distintas herramientas. Podemos poner el ejemplo con desarrolladores que trabajan en WIndows y Linux. Se sabe que unificar las versiones de NodeJS es complicado, y mucho más cuando se usan distintos sistemas operativos. Esto es a razón de qué a veces los desarrolladores quieren actualizar sus versiones previas o las formas de instalación son distintas. 
Esto podría causar errores al momento de inicializar proyectos, deployarlos, etc.

## Después de los contenedores. 

Ahora con Docker es mucho más sencillo y se puede unificar el problema anterior usando sólamente líneas de comando. Un ejemplo podría ser este:
- Descargar una imagen basada en Linux.
- Configurar las herramientas necesarias. 

## Imagenes
Es el empaquetado de las dependencias de código y es lo que se comparte. 

- Dependencias
- Código
- Lo que se comparte

Esto normalmente es ejecutado en un contenedor. Es decir, un contenedor es un conjunto de capas de imágenes. Imagen sobre imagen y sobre otra. Lo que normalmente la capa que va más abajo es una distribución de Linux. La gracia de estos containers es que estos pesan poco a comparación de una VM. 


