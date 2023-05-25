# Ejercicio GIT - GITHUB
modulo de GIT - GITHUB.


## Primeros pasos:
1. Crearemos un repositorio en GITHUB.
	-  **suma (+)** que se encuentra en la parte superior derecha y presionaremos en **"New repository"**.

	-![](https://github.com/StivenBerrio/devjumpers.git)



2. Clonar el repositorio:
	- en una carpeta de nuestro pc entramos  **"Git Bash Here"**, teniendo instalado ya **GIT** 

	-utilizo el comando it clone seguido del enlace
    $ git clone https://github.com/StivenBerrio/devjumpers.git 

------------

### Pasos para el README.md


Para la creación del archivo **README.md** Escribimos el comando **touch** con el nombre de archivo **README.md** quedando **touch README.md**
utilizamos **ls** para comprobar que se encuentre allí.




## .GITIGNORE
Documentación [GIT - GITIGNORE](https://git-scm.com/docs/gitignore "GIT - GITIGNORE").

Ahora haremos lo siguiente:
- Investigar sobre **.gitignore**.
- Crear en el repositorio local un fichero llamado **privado.txt**.
- Crear en el repositorio local una carpeta llamada **privada**.

**Acerca .gitignore:** 

El objetivo principal de un archivo .gitignore es evitar que Git rastree los archivos necesarios o generados automáticamente (como archivos de compilación, registros o archivos temporales). Esto ayuda a mantener el repositorio limpio y evita los conflictos necesarios.

Para utilizarlo, tenemos que crear un archivo llamado .gitignore en el que escribiremos cada línea que queramos evitar que sea rastreada por GIT.

Para crear el archivo, hacemos lo siguiente: Dentro de la carpeta del repositorio, abrimos Git Bash

Para carpetas: escribiremos el comando  mkdir privado
Para otros archivos: podemos escribir touch .gitignore privado.txt en una línea o para cada archivo escribimos touch .gitignore y luego touch privado.txt


**Para la creación de los archivos seguiremos los suiguientes pasos:** 
En la carpeta del repositorio abrimos **Git Bash**
- Escribiremos el comando **mkdir privada**
- En una nueva linea **touch .gitignore privado.txt** 

ya los nuevos archivos estan en el repositorio


luego agregaremos los archivos dentro del .gitignore, desde **Visual Stuido Code** 
- Línea 1: privado.txt
- Línea 2: privada

Haciendo un push enseguida.


------------
## RAMAS, FICHEROS, MERGE, CONFLICTOS

##### fichero y rama:

1. Para añadir fichero **1.txt** al repositorio local.
	- Lo haremos desde la rama master/main usando el comando **touch 1.txt**
2.  Crear una rama con el nombre** v0.2**. e ingresa a la rama.
	-  agregamos  el comando **git checkout -b v0.2**, el cual creara la rama con el nombre **v0.2** y nos posicionará en dicha rama al mismo tiempo.
3. Para añadir un fichero **2.txt** en la rama **v0.2** y subir los cambios al reposiorio remoto.
	- Para crear el nuevo fichero usaremos el comando **touch 2.txt** y luego a esto usaremos ** git add . ** para agregar los nuevos archivos al área de preparación, usaremos **git commit -m "[comentario]"** y para finalizar enviamos los cambios al repositorio remoto utilizando el comando **git push origin -u v0.2**.
	//

##### Merge 

1.  En la rama **master/main** y un merge de la **rama v0.2** en la **rama master**.
	- nos posicionamos en una rama difierente **git checkout master**, ya para hacer el merge escribimos **git merge [rama a fusionar]**, por lo que quedaría **git merge v0.2**

##### Merge con conflicto:

*Nota: Estos puntos los podemos hacer de varias formas, uno sería desde algún editor de texto como **Visual Studio Code**, ingresando directamente al **bloc de notas** o desde la misma consola de **git bash**.*

1. En la rama **master** poner **Hola** en el fichero **1.txt** y hacer commit.
	- Desde la rama **master** y estando en git bash escribimos lo siguiente: 
		**echo "Hola" > 1.txt** y finalizamos con un commit.
2. en la rama **v0.2** y poner **Adios** en el fichero **"1.txt"**; y hacer commit.
	- Luego de haber realizado el paso anterior, nos vamos a posicionar en la rama **v0.2** usando el comando **git checkout v0.2**, escribimos "Adios"con el comando **echo "Adios" > 1.txt"** y hacemos commit.
3. n la rama **master** y hacer un merge con la rama **v0.2**
	- ingresamos en la rama master usando el comando **git checkout master** y haremos el merge: **git merge v0.2** 
	modificamos el archivo dejado el **"Hola"** en la línea #1 y el **"Adios"** en la línea #3  


Para arreglar el conflicto modificaremos el archivo,hacemos  un commit,  usamos **git add .** y luego **git commit -m ""** y de está manera ya habremos solucionado el conflicto.



##### Borrar rama:

Para eliminar la rama, lo podemos hacer utilizando el siguiente codigo **git branch -D [nombreDeLaRama]**


### Comandos utilizados en el proceso:

- git clone 
- cd [nombreDeLaCarpeta] 
- touch README.md
- touch 1.txt
- ls
- git checkout -b v0.2
- touch 2.txt
- mkdir 
- gid add .
- clear
- git status
- git commit -m
- git merge v0.2
- echo "Hola" > 1.txt
- echo "Adios" > 1.txt
- git push
- gid log
- git checkout -b




------------







------------

## Compañeros Devjumps

|  NOMBRE | GITHUB  |
| :------------: | :------------: |
|  Esteban Garcia | [github.com/egarcia9543](https://github.com/egarcia9543 "github.com/egarcia9543")  |
| Isabella E  |[github.com/i-echeverri22](https://github.com/i-echeverri22 "github.com/i-echeverri22") |
| Jeremmy Rojas  |[github.com/J-Rojas29](https://github.com/J-Rojas29 "github.com/J-Rojas29") |
| Jhonatan Toro   |[github.com/jtorova5](https://github.com/jtorova5 "github.com/jtorova5") |
| Michell  |[github.com/michell20](https://github.com/michell20 "github.com/michell20") |
|  Santiago Meneses |[github.com/santiaoomC](https://github.com/SantiagoomC "github.com/santiagoomC") |


## Colaborador
|  NOMBRE | GITHUB  |
| :------------: | :------------: |
|  Santiago Meneses |[github.com/santiaoomC](https://github.com/SantiagoomC "github.com/santiagoomC") |