# Scrap_Ciencia_J.Sampedro

## Motivación

Descargar las publicaciones en abierto de Javier Sampedro en ElPais.com sobre ciencia.
Los libros que las recopilan están agotados

## Objetivo

Crear un script para descargar y generar con ellas un ebook

## Datos

Al hacer una búsqueda sobre el autor se llega a una página

[https://elpais.com/autor/javier_sampedro/a/](https://elpais.com/autor/javier_sampedro/a/)

A partir de ahí se puede pasar a las distintas páginas añadiendo un número, que el 22 de Julio puede ser hasta 74, siendo el 74 la última que contiene las más recientes.
La [1](https://elpais.com/autor/javier_sampedro/a/1) contiene publicaciones desde Dicembre de 1977 hasta Agosto de 1994, si bien no todas tratan sobre temas científicos.

## Objetivos

1. Generar un listado de publicaciones
1. Descargar las publicaciones desde las más recientes
1. Crear un ebook con los artículos


## Detalles

Se han descargado manualmente las paǵinas [74](./pagina_test1_74.html), [73](./pagina_test2_73.html), [72](./pagina_test3_72.html) y [25](./pagina_testX_25.html)

Una inspección rápida nos muestra que basta hacer

    grep "articulo-titulo" *.html

Para recuperar:
* Url del articulo: enlace de la etiqueta <a>
* Fecha: de la url
* Título: del texto de la etiqueta <a>
