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
    ----> Si estás empezando el seguimiento en Git de un proyecto existente, necesitas ir al directorio del proyecto y escribir este comando.Esto crea un nuevo subdirectorio llamado .git que contiene todos los archivos necesarios del repositorio —un esqueleto de un repositorio Git. Todavía no hay nada en tu proyecto que esté bajo seguimiento.

* __git clone__
    ----> Si deseas obtener una copia de un repositorio Git existente —por ejemplo, un proyecto en el que te gustaría contribuir— el comando que necesitas es éste.

* __git status__
    ----> Este es el principal comando para determinar qué archivos están en qué estado es el comando.Cuando lo ejecutas puedes recibir las siguientes cabeceras:
        - “Cambios a confirmar” (“Changes to be committed”).
        - “Modificados pero no actualizados” (“Changes not staged for commit”). Esto significa que un archivo bajo seguimiento ha sido modificado en el directorio de trabajo, pero no ha sido preparado todavía.

* __git diff__
    ----> Este comando sirve para ver lo que has modificado pero aún no has preparado. Compara lo que hay en tu directorio de trabajo con lo que hay en tu área de preparación. El resultado te indica los cambios que has hecho y que todavía no has preparado.

* __git diff --cached // git dif --staged__
    ----> Comando que sirve para ver los cambios que llevas preparados hasta ahora. Si quieres ver los cambios que has preparado y que irán en tu próxima confirmación, puedes usarlo 

* __git add .__
    ----> se añaden los archivos a la zona de Stagin. Al usar el "." se dice que queremos añadir todos los ficheros de ese directorio. Pero se pueden usar expresiones regulares o escribir un fichero en concreto.

* __git commit -m "My hello world"__
    ----> Este comando confirma los cambios en la zona de Stage.
    _NOTA = el parámetro "-m" es para escribir un comentario del commit.

* __git commit -a__
    ----> Aunque puede ser extremadamente útil para elaborar confirmaciones exactamente a tu gusto, el área de preparación es en ocasiones demasiado compleja para las necesidades de tu flujo de trabajo. Si quieres saltarte el área de preparación, Git proporciona un atajo. Pasar la opción -a al comando git commit hace que Git prepare todo archivo que estuviese en seguimiento antes de la confirmación, permitiéndote obviar toda la parte de git add.

* __git rm -f__
    ----> Este comando borra tanto del área de trabajo como del área de preparación (STAGE) el fichero en cuestión. El parámetro "-f" fuerza a que se borre.

* __git rm --cached -f__
    ----> Este comando borra el fichero en cuestión del área de preparación (STAGE). El parámetro "-f" fuerza a que se borre.

* __git remote add [nombre] [url]:__
    ----> Esto se usa cuando queremos crear un repositorio remoto para subir el código. Una vez creasdo si seguimos usando el mismo ya no hace falta.
    Ejemplo: git remote add origin https://github.com/frantwo/frantwo.github.io.git
    _NOTA = "origin" es el alias para la web "https://github.com/frantwo/frantwo.github.io.git"_

* __git remote__
    ----> saca el listado de los repositorios que tengo. Con la opción "-v" se muestran las URLs asociadas a cada repositorio remoto.

* __git remote show origin__
    ----> muestra la dirección web del alias "origin"

* __git fetch [remote-name]__
    ----> Este comando recupera todos los datos del proyecto remoto que no tengas todavía. Después de hacer esto, deberías tener referencias a todas las ramas del repositorio remoto, que puedes unir o inspeccionar en cualquier momento.

* __git push -u origin master__
    ----> se sube todo lo que tenemos commiteado a la rama "master"
    _NOTA = usando el parámetro "-u" establecemos por defecto que todos los "git push" que hagamos vayan al alias "origin" y la rama "master". Se podría usar "git push origin master2" para hacer un PUSH a la rama "master2" pero no la estaríamos poniendo por defecto como cuando usamos el parámetro "-u"_


