## Semana 1

Acá no hay mucho de clases solo la info del Pre-work

### Instalación en Windows con WSL (Windows 10, 11)
- Abre la terminal de Ubuntu.
- Ejecuta `sudo apt update` para actualizar la info del repositorio de dependencias.
- Ejecuta `sudo apt install git-all`
- Asegurate que haya instalado ejecutando `git --version`
- Actualiza tu nombre y correo ejecutando los siguientes comandos:

<pre>
git config --global user.name "Tú nombre"
git config --global user.email "tu_correo@ejemplo.com"
</pre>

Cuando se realicen los commit, éstos van a generar un HASH que irá añadido a tu Nombre y Correo, para poder manejar y controlar quién sube qué cosas y en qué momento. (Versionar)

Fuente: [Undefined Shell](https://undefinedshell.notion.site/2-Instalar-Git-2a65a86fc7d648cb83aaeb7ef2743d8c).

## Semana 2

Acá empezó la parte de GIT y GitHub

Repositorio es como un restaurante.

- Working Directory es la cocina donde se hacen los ajustes.
- Staging Area: Es el área donde los platos están listos para ser llevados al cliente.
- Commit History: Todo lo que esté en el Staging Area se va al cliente *commit*

### Secuencia Básica de un Commit:

| Comando | Accion |
|-|-|
| git init| Iniciar control de versiones |
| git status | Muestra el estado actual del proceso de versionado |
| git add -archivo- | Agrega el archivo al Staging Area | 
| git commit -m "mensaje" | Haces el commit con un mensaje descriptivo |
| git log | Revisamos  el log de commits realizados | 

Vamos a hacer el primer repo local.

`IMPORTANTE`
Revisar y comprobar en qué carpeta estás parado antes de hacer el 'git init'. Recién casi la cago.

Pero por si la cagas, puedes hacer 
<pre>
>rm -rf .git
</pre>

Para borrar los archivos de git que pusiste en la carpeta equivocada.

`Empecemos`

Vamos a el-mundo-del-markdown.
>git init

