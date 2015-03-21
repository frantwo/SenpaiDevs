---
layout: post
title:  "Sinatra y otros cantantes"
date:   2015-03-10 17:51:34
categories: Introducción a Sinatra
---

##__INSTALACION__

gem install sinatra

gem install sinatra-reloader
*(NOTA: esta gema sirve para instalar el requiere reloader que ayuda a no tener que tirar y levantar de nuevo el servidor)*


##__¿QUÉ ES SINATRA?__
Sinatra es un framework para aplicaciones web de software libre y código abierto, y lenguaje específico del dominio escrita en Ruby. Es una alternativa a otros frameworks para aplicaciones web como Ruby on Rails, Merb, Nitro, Camping, y Rango. Sinatra depende de Rack interfaz de servidor web.Ç


##__PRIMER CONTACTO CON SINATRA: HOLA MUNDO!__

Con este código fuente, y runeándolo con el comando: 
~~~
ruby hello_world.rb
~~~
podemos hacer nuestro primero "Hello World" con Sinatra.

~~~
# myapp.rb
require 'sinatra'

get '/' do
  'Hello world!'
end
~~~

Vamos al navegador y con el puerto que nos haya dicho Sinatra podemos ver el resultado en la dirección del local host:
~~~
http://localhost:4567
~~~
*(NOTA: Suponiendo que el puerto devuelto por Sinatra fue 4567)*

El siguiente paso es meterle parámetros a nuestro código:
~~~
# myapp.rb
require 'sinatra'
require 'sinatra/reloader'

get '/' do
  'Hello world!'
end


get '/hello/:name' do
  # matches "GET /hello/foo" and "GET /hello/bar"
  # params[:name] is 'foo' or 'bar'
  "Hello #{params[:name]}!"
end
~~~
De esta forma metiendo en la URL lo siguiente: ~~~ http://localhost:4567/hello/Francho ~~~
obtendremos un "Hello Francho" en nuestro navegador.

##__SE NOS VA LA OLLA, VIEWS!__
Añadiendo una carpeta views en nuestra carpeta de trabajo y ahí creamos un fichero ".erb". Estos ficheros sirve de capa visual de lo que el usuario va a ver.