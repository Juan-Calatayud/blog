
# PRIMEROS PASOS EN GIT

## [Aprendiendo javascript con "MentoringJS Pretraining Step 2"](http://mentoringjs.com/)

El control de versiones.

El control de versiones es un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas recuperar versiones espec�ficas de tus archivos.

Breve historia de Git

El n�cleo de Linux es un proyecto de software de c�digo abierto. En 2002, el proyecto del n�cleo de Linux empez� a usar un DVCS propietario llamado BitKeeper.

En 2005, la relaci�n entre la comunidad que desarrollaba el n�cleo de Linux y la compa��a que desarrollaba BitKeeper se vino abajo, y la herramienta dej� de ser ofrecida gratuitamente. Esto impuls� a la comunidad de desarrollo de Linux (y en particular a Linus Torvalds, el creador de Linux) a desarrollar su propia herramienta basada en algunas de las lecciones que aprendieron durante el uso de BitKeeper.

Instalando Git.

GIT es una herramienta creada para el proyecto Linux. No es de extra�ar que sea una herramienta a base de comandos pensada y preparada para ejecutarse en un Shell Linux. Por tanto, para instalar GIT es habitual hacer uso de apt-get otro gestor de paquetes equivalente. El comando concreto para instalar GIT mediante apt-get es:  sudo aptget install gitcore.

Sin embargo, tambi�n es posible ejecutar GIT en un entorno Windows. Para ello basta con descargar el instalador de 
https://git-scm.com/downloads/ y ejecutarlo.

Primeros pasos para crear un repositorio


�C�mo creo un repositorio y c�mo s� que se ha creado correctamente?. Sencillo, se busca la carpeta de nuestro repositorio en el terminal, y iniciamos con el primer comando �git init�. Esta carpeta ser� nuestro repositorio y en ella se almacenar� toda la informaci�n del mismo.

Esta es la primera vez que utilizamos GIT y nos va a pedir un nombre de usuario y un
correo electr�nico.  Para configurar correctamente estos par�metros el sistema nos sugiere ejecutar los comandos:

git config --global user.name �Nuestro nombre�
git config --global user.email �Nuestro email�


A continuaci�n, vamos a escribir el comando �git status� para ver cual es el estado actual de nuestro proyecto. Luego creamos un fichero, por ejemplo, hola.txt. Se vuelve a comprobar el estado. 

Para indicar a Git que comience a realizar el seguimiento de los cambios realizados en hola.txt, primero debemos a�adirlo al �rea de preparaci�n mediante �git add hola.txt�. Ahora ejecutamos el comando �git status� para ver como va.

Para almacenar los cambios realizados, ejecutamos el comando commit con un mensaje que describe lo que hemos cambiado  (git commit -m �Hemos a�adido hola al repositorio�).

Si queremos tener un registro de los cambios que hemos realizado y en el orden que los cometimos, utilizamos el comando �git log�.

Para enviar nuestro repositorio local al servidor GitHub, tendremos que a�adir un repositorio remoto. Este comando toma un nombre remoto y una URL de repositorio, que en su caso es https://github.com/nombre-de-usuario/nombre-repositorio.git. Y el comando ser�a �git remote add origin https://github.com/nombre-usuario/nombre-repositorio.git�.

Com el comando push le decimos a Git donde poner nuestros commits. Con esto subimos nuestros archivos locales al repositorio en GitHub y este es el comando �git push -u origin master�. Estos se suben a una rama local llamada master.

Si hay m�s gente en nuestro repositorio, para saber si han hecho alguna modificaci�n y queremos tener los cambios en nuestro repositorio, utilizamos el comando �git pull origin master�.

Si al hacer un pull queremos saber si hay algo diferente en nuestros archivos, utilizamos el comando �git diff HEAD�.

Para eliminar alg�n archivo podemos utilizar el comando �git reset hola.txt�.

Cuando diferentes personas est�n trabajando en un mismo proyecto, para que sus archivos no choquen los unos con los otros, se crean diferentes ramas para poder trabajar mejor, as� no estropear el trabajo que est� realizando el otro. Las ramas se crean mediante el comando �git branch nombre_rama�. Ahora con �git branch� podemos ver las ramas que tenemos en nuestro proyecto, y podemos elegir la rama que queramos con �git checkout nombre_rama�. 

Para volver a la rama principal, despu�s de haber realizado nuestro trabajo, lo hacemos con �git checkout master�. Y cuando est� todo preparado para fusionarse con la rama principal, utilizamos el comando �git merge nombre_rama�. 

Una vez est� todo el trabajo subido al repositorio, lo que hacemos es borrar la rama en la que hemos estado trabajando, y para ello utilizamos �git branch -d nombre_rama�.

Para finalizar, lo �ltimo que nos queda es subirlo todo a nuestro repositorio en GitHub, as� que para ello utilizamos �git push�.


Para realizar este trabajo he consultado los apuntes del curso impartido por la fundaci�n telef�nica de Desarrollo web en PHP. Tambi�n he realizado el curso Try git que hay en Codeschool(https://try.github.io/levels/1/challenges/1). Y he consultado este libro https://git-scm.com/book/en/v2


Un saludo!!
