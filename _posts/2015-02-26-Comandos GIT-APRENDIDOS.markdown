---
layout: post
title:  "Comandos GIT y JEKYLL"
date:   2015-02-26 17:51:34
---

##INSTALACIÓN DE GIT
Para instalar GIT en tu linux (ubuntu) debes usar el comando: `$ apt-get install git`
Comandos usados durante para la creación de mi primer Blog en Git-Hub com Jekyll.

##COMANDOS GIT

* __git init__
    ----> para inicializar el git en el directorio de trabajo.

* __git status__
    ----> ver el status del git

* __git add .__
    ----> se añaden los archivos a la zona de Stagin. Al usar el "." se dice que queremos añadir todos los ficheros de ese directorio. Pero se pueden usar expresiones regulares o escribir un fichero en concreto.

* __git commit -m "My hello world"__
    ----> Se hace un commit de todo lo que hay en la zona de Stagin. 
    _NOTA = el parámetro "-m" es para escribir un comentario del commit._

* __git remote add origin https://github.com/frantwo/frantwo.github.io.git__
    ----> Esto se usa cuando queremos crear un repositorio remoto para subir el código. Una vez creasdo si seguimos usando el mismo ya no hace falta.
    _NOTA = "origin" es el alias para la web "https://github.com/frantwo/frantwo.github.io.git"_

* __git remote__
    ----> saca el listado de los repositorios que tengo

* __git remote show origin__
    ----> muestra la dirección web del alias "origin"

* __git push -u origin master__
    ----> se sube todo lo que tenemos commiteado a la rama "master"
    _NOTA = usando el parámetro "-u" establecemos por defecto que todos los "git push" que hagamos vayan al alias "origin" y la rama "master". Se podría usar "git push origin master2" para hacer un PUSH a la rama "master2" pero no la estaríamos poniendo por defecto como cuando usamos el parámetro "-u"_


##INSTALACIÓN JEKYLL
Para instalar Jekyll en tu linux (Ubuntu) debes usar el siguiente comando: ` sudo gem install jekyll`
Aunque es posible que nuestro linux nos diga que nos faltan componentes antes de instalarlo. Como siempre en Linux deberemos leer lo que nos pone pero lo más lógico es que tengamos que actualizar nuestro sistema operativo y los paquetes previamente. Y despúes de eso instalar ruby y sus gemas.

Comenzamos:

    Para actualizar la lista de paquetes de software:

    `sudo apt-get update`

    Ahora actualizamos el sistema operativo y los paquetes:

    `sudo apt-get upgrade`

    Instalamos Ruby:

    `sudo apt-get install ruby`

    Instalamos Gems:

    `sudo apt-get install rubygems`

    Finalmente instalamos Jekyll:

    `sudo gem install jekyll`

##COMANDOS JEKYLL

* __jekyll new Frantwo-Blog__
  	----> creación de un proyecto con Jekyll

* __jekyll serve__
  	----> inicializa el servidor de Jekyll.

* __jekyll build Frantwo-Blog__
  	----> creación del html estático.


