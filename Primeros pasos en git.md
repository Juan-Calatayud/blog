
# PRIMEROS PASOS EN GIT

## [Aprendiendo javascript con "MentoringJS Pretraining Step 2"](http://mentoringjs.com/)

El control de versiones.

El control de versiones es un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas recuperar versiones específicas de tus archivos.

Breve historia de Git

El núcleo de Linux es un proyecto de software de código abierto. En 2002, el proyecto del núcleo de Linux empezó a usar un DVCS propietario llamado BitKeeper.

En 2005, la relación entre la comunidad que desarrollaba el núcleo de Linux y la compañía que desarrollaba BitKeeper se vino abajo, y la herramienta dejó de ser ofrecida gratuitamente. Esto impulsó a la comunidad de desarrollo de Linux (y en particular a Linus Torvalds, el creador de Linux) a desarrollar su propia herramienta basada en algunas de las lecciones que aprendieron durante el uso de BitKeeper.

Instalando Git.

GIT es una herramienta creada para el proyecto Linux. No es de extrañar que sea una herramienta a base de comandos pensada y preparada para ejecutarse en un Shell Linux. Por tanto, para instalar GIT es habitual hacer uso de apt-get otro gestor de paquetes equivalente. El comando concreto para instalar GIT mediante apt-get es:  sudo aptget install gitcore.

Sin embargo, también es posible ejecutar GIT en un entorno Windows. Para ello basta con descargar el instalador de 
https://git-scm.com/downloads/ y ejecutarlo.

Primeros pasos para crear un repositorio


¿Cómo creo un repositorio y cómo sé que se ha creado correctamente?. Sencillo, se busca la carpeta de nuestro repositorio en el terminal, y iniciamos con el primer comando “git init”. Esta carpeta será nuestro repositorio y en ella se almacenará toda la información del mismo.

Esta es la primera vez que utilizamos GIT y nos va a pedir un nombre de usuario y un
correo electrónico.  Para configurar correctamente estos parámetros el sistema nos sugiere ejecutar los comandos:

git config --global user.name “Nuestro nombre”
git config --global user.email “Nuestro email”


A continuación, vamos a escribir el comando “git status” para ver cual es el estado actual de nuestro proyecto. Luego creamos un fichero, por ejemplo, hola.txt. Se vuelve a comprobar el estado. 

Para indicar a Git que comience a realizar el seguimiento de los cambios realizados en hola.txt, primero debemos añadirlo al área de preparación mediante “git add hola.txt”. Ahora ejecutamos el comando “git status” para ver como va.

Para almacenar los cambios realizados, ejecutamos el comando commit con un mensaje que describe lo que hemos cambiado  (git commit -m “Hemos añadido hola al repositorio”).

Si queremos tener un registro de los cambios que hemos realizado y en el orden que los cometimos, utilizamos el comando “git log”.

Para enviar nuestro repositorio local al servidor GitHub, tendremos que añadir un repositorio remoto. Este comando toma un nombre remoto y una URL de repositorio, que en su caso es https://github.com/nombre-de-usuario/nombre-repositorio.git. Y el comando sería “git remote add origin https://github.com/nombre-usuario/nombre-repositorio.git”.

Com el comando push le decimos a Git donde poner nuestros commits. Con esto subimos nuestros archivos locales al repositorio en GitHub y este es el comando “git push -u origin master”. Estos se suben a una rama local llamada master.

Si hay más gente en nuestro repositorio, para saber si han hecho alguna modificación y queremos tener los cambios en nuestro repositorio, utilizamos el comando “git pull origin master”.

Si al hacer un pull queremos saber si hay algo diferente en nuestros archivos, utilizamos el comando “git diff HEAD”.

Para eliminar algún archivo podemos utilizar el comando “git reset hola.txt”.

Cuando diferentes personas están trabajando en un mismo proyecto, para que sus archivos no choquen los unos con los otros, se crean diferentes ramas para poder trabajar mejor, así no estropear el trabajo que está realizando el otro. Las ramas se crean mediante el comando “git branch nombre_rama”. Ahora con “git branch” podemos ver las ramas que tenemos en nuestro proyecto, y podemos elegir la rama que queramos con “git checkout nombre_rama”. 

Para volver a la rama principal, después de haber realizado nuestro trabajo, lo hacemos con “git checkout master”. Y cuando está todo preparado para fusionarse con la rama principal, utilizamos el comando “git merge nombre_rama”. 

Una vez está todo el trabajo subido al repositorio, lo que hacemos es borrar la rama en la que hemos estado trabajando, y para ello utilizamos “git branch -d nombre_rama”.

Para finalizar, lo último que nos queda es subirlo todo a nuestro repositorio en GitHub, así que para ello utilizamos “git push”.


Para realizar este trabajo he consultado los apuntes del curso impartido por la fundación telefónica de Desarrollo web en PHP. También he realizado el curso Try git que hay en Codeschool(https://try.github.io/levels/1/challenges/1). Y he consultado este libro https://git-scm.com/book/en/v2


Un saludo!!
