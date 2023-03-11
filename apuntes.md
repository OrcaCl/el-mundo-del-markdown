<!-- ---
layout: /Code/el-mundo-del-markup/layout.liquid
title: Apuntes de OrcaCL
description: la fuente de la juventud
--- -->

# Este es mi libro de anotaciones.

Acá voy a ir anotando las cosas que vaya aprendiendo durante el Bootcamp de Guillermo Rodas

## Markdown

Muy interesante he encontrado esto del Markdown pero más aún, el uso de WSL Ubuntu, y volver a juguetear con un terminal de linux.

Acabo de aprender a hacer aliases y entender además, por qué no me querían funcionar unos cuantos varios que traté de hacer andar y no pasaba ni un carajo.


## 05-03-2023

Acabo de tomar la decisión de que en este archivo voy a ir anotando todo, y posteriormente voy a ir ordenando los apuntes en sus respectivos archivos separados.

Así no me preocupo tanto del orden en un principio y después el limpiar me servirá para estudiar y repasar las cosas que voy aprendiendo. Además que puedo ir incorporando las cosas que descubro o busco por separado a lo que viene en los cursos del bootcamp.

Ahora seguiré poniendome al día con el video de S1C4

## 06-03-2023

Si tengo echo "Blabla" > nombrefile.md me va a generar un archivo que incluya lo que puse dentro del echo.

Si uso cat puedo ver en consola lo que tiene un archivo dentro.

En algún momento del stream hablaron de @11ty o Eleventy. No alcancé a cachar que era y ahora llegué a esta parte.

Ya. Después que vi en vivo como la cagaba ya entendí.
Primero, **NPM o Node Package Manager** instala paquetes. Como globales (para usar) o como dependencias de lo que sea que esté escribiendo (una app, por ejemplo).

Por otro lado **NPX o Node Package Execute**, me permite descargar un paquete y ejecutarlo sin necesidad de instalarlo como global o dependencia. Es como para probar algo sin estar seguro si me sirve o no.

Y @11ty/eleventy es una herramienta para crear sitios HTML estáticos super fácil, que trae además un servidor local de archivos hml estáticos.

<pre>
> npx @11ty/eleventy -serve
</pre>

Este comando descarga el temporal, y convierte mis archivos base de Markdown en HTML, y los guarda en la carpeta por omisión, "_site".

Hay formas de ajustar parámetros, pero porongas. Eso lo veré después si es que lo necesito.

Si después repito el comando, me levanta el server en:

<pre>
> http://localhost:8080/
</pre>

Un detalle es que si hay más archivos en la carpeta, los va a convertir todos y dejar en subcarpetas separadas.  Si quiero que sólo convierta un archivo, es mejor especificarlo. Hay que usar el parámetro --input

<pre>
>npx @11ty/eleventy --input mark.md --serve
</pre>

"ls folder" lista el contenido del folder

**Bash**
Acá hay otro listado de alias que Guillermo comparte:

Top 10 comandos más usados:

La línea tal cual Guillermo no me funcionó. Supongo que por la diferencia de teclados y uso de " o '.

La modifiqué un poco con ayuda de ChatGPT y quedó así.

<pre>
alias mostused="history | awk '{print \$2}' | sort | uniq -c | sort -nr | head -n 10"
   
</pre>

Estos son mis 10 comandos más utilizados:

| comando | descripcion |
|-|-|
| ls | listar el contenido |
| cd | cambiar de directorios |
| nano | editor de texto de consola |
| code | llamar a VS CODE |
| mimark | saltar con alias a el-mundo-del-markdown |
| exit | cerrar terminal |
| mostused | llamar al alias que arma esta lista |
| cl | limpiar consola |
| npx | ejecutar NPX |
| alias | listar los alias |

## Git y Github

Master y Branches