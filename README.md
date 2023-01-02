# gitGuide
# GUÍA DE COMANDOS GIT

En esta guía vas a aprender los comandos
necesarios para poder trabajar con git, pero antes que nada necesitas manejarte por el sistema operativo a través de terminal. 

Vas a aprender a manejarte y trabajar con directorios y ficheros. (un **directorio** es una **carpeta** y un **fichero** es un **archivo**, acostumbrate a usar esos nombres)

primero hay que ver el directorio en el que nos encontramos

***para eso hacemos el comando:***

```
pwd
```

y nos saldrá el directorio en el que nos encontramos actualmente

ej:

```
/home/omar13/Escritorio
``` 

(eso es un ejemplo para Linux, en Windows sale con backslashes si usas powershell, osea con una barra trasera (C:\Users\User\Desktop), pero si usas ***GIT BASH***, la terminal que te da git al instalartelo en el PC, saldrá algo así ```c/Users/User/Desktop```)


Ahora, para ver los archivos del directorio en el que nos encontramos, ***hacemos este comando***:

```
ls
```

y nos saldrán todos los ficheros y directorios que se encuentran en el directorio actual: 

```
Projectos\, Fichero1
```

Ahora vamos a crear directorios y ficheros
suponiendo que usas como shell ***Git Bash*** (NO SE SI EN POWERSHELL FUNCIONA) (que es el shell que se te instala al instalarte GIT), para crear archivos se usa el comando:

``` 
touch <nombredelarchivo>.<extension>
```

vamos a suponer que creamos un archivo de texto llamado ***hola***
y se crea en el directorio actual en el que estás.
Hacemos el mismo comando:

```
touch hola.txt
```

para comprobarlo, lanzamos el comando

```
ls
```

y veremos que efectivamente se encuentra el fichero que acabamos de crear

``` 
Projectos/, Fichero1, hola.txt
```

y para eliminarlo simplemente hacemos este comando:

```
rm hola.txt
```

y comprobamos que ha sido eliminado con el comando ```ls```:

```
Projectos/, Fichero1 
```

PERFECTO!!!, ya sabes mirar en que directorio de te encuentras, su contenido, y crear y eliminar ficheros dentro de él

Ahora vas a aprender a crear y a eliminar directorios.

Es muy facil, para crear un directorio en el directorio actual en el que te encuentras tienes que hacer este comando:

```
mkdir <nombre del directorio>
```

vamos a poner un ejemplo:

```
mkdir miDirectorio
```

y hacemos un ```ls``` para comprobar que efectivamente hemos creado un directorio en el directorio que nos encontramos actualmente

```
Projectos/, Fichero1, miDirectorio/ 
```

Ahora, para moverte a ese directorio tendrás que hacer este comando

```
cd <nombreDeDirectorio>
```

Lo haremos con el directorio que hemos creado ```miDirectorio```:

```
cd miDirectorio
```

y para comprobar que efectivamente estamos en ese directorio haremos el comando ```pwd```

```
C:\Users\User\Desktop\miDirectorio
```
o ```c/Users/User/Desktop/miDirectorio``` si lo hacemos en ***GIT BASH***

ahora supongamos que quieres irte al Directorio anterior, algo asi como 
"ir para atrás", tendrás que hacer este comando:

```
cd ..
```
(el espacio entre el ```cd``` y el ```..``` es obligatorio, si no el comando no funcionará)

Y podemos comprobar con los comandos ```ls``` y ```pwd``` no estamos en ese directorio ya, sino en su anterior.

```
input: pwd
output: C:\Users\User\Desktop
```

```
input: ls
output: Projectos/, Fichero1, miDirectorio/ 
```

Ahora, si queremos ***eliminar un directorio***, tendremos que hacer este comando:

```
rmdir <nombreDirectorio>
```
por ejemplo:

```
rmdir miDirectorio
```

y si hacemos un ```ls``` veremos que se ha borrado ese directorio

```
Projectos/, Fichero1
```

Ya tienes los comandos básicos para navegar por directorios y trabajar con ellos

Ahora vas a aprender los comandos de git básicos para poder trabajar con git con la terminal de manera rápida.

## COMANDOS DE GIT

los comandos más importantes de git son:

- ```git add <directorio>```  para añadir el directorio al staging area
- ```git commit -m "<nombre del commit>"``` para añadirlos al repositorio local
- ```git log --oneline```  para ver los commits que has hecho en el proyecto

Y también están push y eso pero con hacer esas funciones desde el programa github desktop ya vale xd
