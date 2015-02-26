---
layout: post
title:  "Comandos GIT-APRENDIDOS"
date:   2015-02-26 17:51:34
---
Comandos usados durante para la creación de mi primer Blog en Git-Hub com Jekyll.

jekyll new Frantwo-Blog
  	----> creación de un proyecto con Jekyll

jekyll server
  	----> inicializa el servidor de Jekyll.

jekyll build Frantwo-Blog
  	----> creación del html estático.

git init
  	----> para inicializar el git en el directorio de trabajo.

git status
  	----> ver el status del git

git add .
  	----> se añaden los archivos a la zona de Stagin. Al usar el "." se dice que queremos añadir todos los ficheros de ese directorio. Pero se pueden usar expresiones regulares o escribir un fichero en concreto.

git commit -m "My hello world"
  	----> Se hace un commit de todo lo que hay en la zona de Stagin. 
  	NOTA = el parámetro "-m" es para escribir un comentario del commit.

git remote add origin https://github.com/frantwo/frantwo.github.io.git
  	----> Esto se usa cuando queremos crear un repositorio remoto para subir el código. Una vez creasdo si seguimos usando el mismo ya no hace falta.
  	NOTA = "origin" es el alias para la web "https://github.com/frantwo/frantwo.github.io.git"

git remote
  	----> saca el listado de los repositorios que tengo

git remote show origin
  	----> muestra la dirección web del alias "origin"

git push -u origin master
  	----> se sube todo lo que tenemos commiteado a la rama "master"
  	NOTA = usando el parámetro "-u" establecemos por defecto que todos los "git push" que hagamos vayan al alias "origin" y la rama "master". Se podría usar "git push origin master2" para hacer un PUSH a la rama "master2" pero no la estaríamos poniendo por defecto como cuando usamos el parámetro "-u"

