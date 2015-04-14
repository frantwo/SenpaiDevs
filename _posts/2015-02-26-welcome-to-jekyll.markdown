---
layout: post
title:  "Welcome to Jekyll!"
date:   2015-02-26 17:51:34
categories: jekyll update
---
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
  	----> inicializa el servidor de Jekyll generando una web con los posts escritos. Además nos da una dirección web local donde está de forma temporal.

* __jekyll build Frantwo-Blog__
  	----> creación del html estático.

Los posts se encuentran en el directorio `_posts`. Para añadir uno simplemente creamos un nuevo fichero con la nomenclatura `YYYY-MM-DD-name-of-post.ext` 


Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
