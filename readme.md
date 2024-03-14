# Programando tareas

En este proyecto conoceremos como programar tareas en linux, con un ejemplo practico

## Vamos a empezar

Si te gustaria tener una copia del tutorial para realizar este proyecto puedes entrar a la siguiente liga (https://github.com/Ericktati1234/My_Pro_Git.git)
y descargar el archivo "Practicar bash script -"

### Prerequisitos

Debemos de tener instalado linux en nuestro computador, sea cual sea la version de linux (debian, ubuntu, linux mint), nos debe de funcionar 
lo siguiente que vamos a utilizar. Yo que utilizo ubuntu puedo observar su version con el siguiente comando

```
/etc/lsb-release
```

### Instalando y verificando version (funcionamiento)

Si no poseemos de ninguna version de linux en los siguientes links encontraremos tutoriales para las siguientes versiones, con los comandos
siguientes podremos verificar la version de nuestro SO:

Ubuntu (https://www.youtube.com/watch?v=airSSg1Ut0g)

```
/etc/lsb-release o /etc/os-release
```

Debian (https://www.youtube.com/watch?v=jd3f6Pq4wfg&t=27s)

```
lsb_release –a
```

Linux Mint (https://www.youtube.com/watch?v=5q7NfbRdeW0)

```
lsb_release -d
```
Para la consulta de la version debemos ejecutar el comando en nuestra consola

Nos enfocamos en una instalacion en donde deseemos conservar nuestro windows y asi poder trabajar con los 2 SO al mismo tiempo

### Ejecutando nuestro archivo

En la misma liga donde descargamos nuestro tutorial (https://github.com/Ericktati1234/My_Pro_Git.git) encontraremos un archivo llamado "ScriptCP.sh"
Lo vamos a descargar y vamos a crear las respectivas Carpetas para su correcto funcionamiento:

Vamos a crear en nuestra carpeta un archivo llamado "readme.txt" para ello podemos utilizar el comando

```
touch readme.txt
```
Despues de creado este archivo, ahora crearemos una carpeta en nuestra raiz llamada "Carpeta2", de la siguiente forma

```
mkdir Carpeta2
```
Despues creamos una carpeta dentro de esta carpeta (Carpeta2) y la llamamos "Docs", de la siguiente forma

```
cd Carpeta2 #Para entrar a la carpeta "Carpeta2"
mkdir Docs
```
Ya habiendo creado estas 2 carpetas y nuestro documento, vamos a ejecutar nuestro Script descargado, asi que vamos a buscar en que carpeta tenemos 
nuestro Script y lo ejecutaremos de la siguiente forma:

```
./ScriptCP.sh
```
Al ejecutar el script podemos confirmar su ejecucion verificando en la direccion ~/Carpeta2/Docs/, si existe el archivo llamado "readmeCopy.txt"
Si no es asi, vuelve a leer los pasos e intentalo de nuevo

### Terminando tutorial

Por ultimo vamos a ejecutar los comandos clave de nuestro proyecto, el cual nos permite crear tareas programadas, el comando a utilizar es:

```
Crontab -e
```
Al ejecutar nuestro comando observaremos una gran cantidad de comentarios que nos explican la manera de programar tareas, nosotros vamos a ignorar 
esto y vamos a escribir al fondo de nuestro documento (Sin continuar ninguna linea ya hecha) el siguiente comando:

```
*/80 * * * * ~/ScriptCP.sh
```
La direccion donde esta nuestro Script puede variar, debemos nosotros verificar en donde se encuentra nuestro documento ScriptCp.sh y escribir la 
direccion completa de este terminando siempre con el nombre de nuestro archivo ScriptCP.sh

Felicidades, acabamos de programar una tarea, la cual se ejecutará cada 80 minutos o 1 hora y 20 minutos

## Implementacion

Si queremos comprender como realizar nuestras propias tareas programadas y como funciona los comandos dentro de crontab, en la siguiente liga 
podremos comprender que significa cada * del comando dentro de crontab (https://crontab.guru)

## Hecho con

* [VsCode](https://code.visualstudio.com) - Como editor de nuestro codigo fuente
* [GitHub](https://github.com) - Como repositorio remoto que contiene nuestros archivos tutorial

## Contribucion

Si desea contribuir y mejorar el siguiente documento, favor de contactarnos en el siguiente correo (ContactoBinBash@coolmail.com)

## Versionado

Para el versionado y consulta de documento hacemos el uso de [GitHub](https://github.com) en el cual actualizamos, verificamos y probamos 
cada mejora en los codigos y tutoriales realizados

## Authors

* **Erick Nevarez** - *Totalidad del trabajo* - [Ericktati1234](https://github.com/Ericktati1234)

Por el momento a la fecha 14/05/2024 no existen colaboradores que hayan participado en el proyecto

## License

Este proyecto es usado solamente para usos didacticos, no nos hacemos responsables ninguno de los autores por el mal uso del codigo anexado
Todos los documentos y links son una via para obtener mayor conocimiento, no se obtiene ningun beneficio personal por el compartir los links

## Reconocimientos

* Un agradecimiento a los youtubers: [Herschel González](https://www.youtube.com/@HerschelGonzalez), [Adolfo Lobos](https://www.youtube.com/@Lamdolf), [TutosPC](https://www.youtube.com/@TutosPCyoutube) los cuales tienen tutoriales muy bien explicados para la instalacion de linux


