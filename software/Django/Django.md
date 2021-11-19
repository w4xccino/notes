# Que es Django?
[[Django]] es un framework de codigo abierto para construir aplicaciones web con Python. 

## Features de Django
 - The admin Site
 - Object-relational mapper
 - Authentication
 - Caching
 - more...

**Django trabaja en el servidor, y no se peude comparar con otros frameworks como ANgular o REact porque esos trabajan en el cliente.

## Dependencias
- Para instalar [[Django]], primero es necesario tener Python instalado. Luego es necesario instalar `pip`, que es el gestor de paquetes de Python. 

- Luego con `pip`, se debe instalar `pipenv` con el comando `pip3 install pipenv`

- `pipenv` es una herramienta de gestor de manejo de las dependencias para instalar las dependencias de nuestra aplicacion en ambientes virtuales. 

- Sirve para que nuestras dependencias de nuestra aplicacion, no entren en conflicto con dependencias de otras aplicaciones. 

## Installation
 - Se crea una subcarpeta donde alojará nuestro proyecto Django con el comando `mkdir` si es necesario.
- Luego nos ubicamos en nuestra carpeta y se usa `pipenv` para instalar Django con el comando `pipenv install Django`.
- Se instalará un ambiente virtual que estará especificado en consola que contiene que contiene archivos `bin` como python, pip3, django-admin, etc
- Luego necesitamos activar el ambiente virtual con el comando `pipenv shell` y entrar al shell de `pipenv` y ejecutar el comando 
- Luego usamos el comando de `django-admin`, que es la utilidad de Django para administrar el proyecto.
- Se usa el comando `django-admin startproject` seguido del nombre del proyecto, por ejemplo: `django-admin startproject Gaa .`.
- El `.` al final indica que no se quiere crear una subcarpeta para el proyecto, sino la misma. 
- Para ejecutar el servidor se usa: `manage.py runserver` 

## Modules
 - `Pipfile` incluye lo que necesita nuestro proyecto, como la version de Django o Python usada. 
 - `__init__.py` Define el directorio como un paquete
 - `settings.py` Donde se establecen las configuraciones de nuestra aplicacion.
 - `urls.py` Donde se definen las url's de nuestro proyecto
 - `asgi.py` and `wsgi.py` Son usados para el lanzamiento de la aplicacion
 - `manage,py` Es un wrapper que usa `django-admin` que es instalado previamente por `pipenv`