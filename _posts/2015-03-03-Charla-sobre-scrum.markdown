---
layout: post
title:  "Introducción a las Metodologías Ágiles para el desarrollo de Software"
date:   2015-03-03 17:30:34
---
Presentación de las metodologías Ágiles por Teresa Oliver. Sé que hay millones de webs explicándo todos estos temas, pero éstas son mis notas sobre una magnífica charla expuesta por Teresa, a la cual le agradezco mucho su tiempo y dedicación al grupo de Senpai Devs.

##METODOLOGÍA TRADICIONALES
En las metodologías tradicionales se trabaja en forma de cascada (Ver Imagen 1). Como consecuencia de ésto, no se tiene nada de valor para el cliente hasta el final del ciclo (implantación). 

:![Alt text](/images/Metod_Agil_01.jpg "Imagen 1")

Pero antes, empecemos por el principio, 
###¿Cuáles son los ciclos de una metodología tradicional?

* __ANÁLISIS__

Durante la esta fase se toma el 100% de los requerimientos del cliente. Esta fase es importantísima ya que entender lo que el cliente quiere será necesario para organizar y planificar los pasos siguientes.

* __DISEÑO__

Durante esta fase se comienza diseñar en papel toda la infraestructura de la aplicación (BD, UI, Eventos, entorno, etc...). 

* __IMPLEMENTACIÓN__

Durante esta fase se codifica todo lo diseñado en la fase anterior.

* __PRUEBAS__

En esta fase se hacen las pruebas de todo el código generado en la fase anterior. En esta fase, el desarrollo de la aplicación está terminado pero aún no tiene valor para el cliente ya que puede contener errores que deben ser subsanados.

* __IMPLANTACIÓN__

En esta fase el cliente recibe su poducto software y ve los resultados obtenidos.


###__¿QUÉ PROBLEMAS TIENE ESTA METODOLOGÍA?__

Normalmente el grupo de trabajo está especializado en cada una de las fases y recibe las instrucciones de lo que tiene que hacer de fases anteriores. Esto hace que los requerimientos del cliente puedan llegar "descafeinados" a cada uno de los grupos. Y por lo tanto el producto final llegue a la implementación de una forma que nuestro cliente no ha requerido.  
Por otro lado, si se produce un fallo en una de las fases, se arrastra en todas las siguientes. Es por ésto por lo que las fases de análisis y diseño cobran especial importancia en estas metodologías.
La consecuencia de todo ésto, como bien se decía al principio es que durante todo el ciclo el cliente no tiene nada de valor. Sólamente al final (IMPLANTACIÓN) es cuando obtiene algo tangible (Ver linea roja Imagen 2).  

:![Alt text](/images/Metod_Agil_02.jpg "Imagen 2")  


##__ENTRADA DE LAS METODOLOGÍAS ÁGILES__
Es entonces donde las metodologías ágiles cobran especial importancia. Ya que se trata de metodologías iterativas que van desarrollando pequeñas porciones definitivas del producto hasta llegar al producto completo. En la siguiente ilustración se puede ver la idea. El cliente nos pide un coche, y en cada una de las iteraciones nos vamos acercando al concepto final, de tal forma que siempre podemos entregar al cliente algo funcional y definitivo y él puede ver la evolución hasta sus requerimientos.

:![Alt text](/images/Metod_Agil_02b.jpg "Objetivo de las metodologías ágiles.")  


###__ROLES EN UNA METODOLOGÍA SCRUM__  

Los roles que podemos encontrar en una metodología SCRUM son los siguientes:  
* PRODUCT OWNER (PO):
Persona que está en contacto con el cliente y el equipo. Regula e intercede en los requerimientos y necesidades del cliente.  
* EQUIPO:
Es un grupo de personas con roles heterogéneos y autoorganizados que desempeñan todas la funcionalidades cada uno de ellos.  
* SCRUM MASTER:
Es un facilitador. Es la persona que ayuda a que el Equipo y el Product Owner funcionen correctamente. Intercede en disputas, y facilita que el trabajo siga su curso sin ningún impedimento. (Ver Imagen 3).
:![Alt text](/images/Metod_Agil_03.jpg "Imagen 3")  


###__ACTIVIDADES__

Para la realización de ese proceso iterativo, primeramente se realiza una historia de usuario. Comparándolo con las metodologías tradicionales, sería la recogida de requisitos del cliente. Pero para las metodologías ágiles, se trata de un listado de cosas necesarias a hacer, ordenadas de mayor importancia a menos (basando la importancia en el valor que tiene para el cliente), y que recoje de forma atomizada funcionalidades que se van a realizar y que se podrán enseñar al cliente de forma definitiva una vez terminadas (ver Imagen 4).
:![Alt text](/images/Metod_Agil_04.jpg "Imagen 4")

Utilizando más metodologías Ágiles como es la de KANBAN (ver Imagen 5) vamos gestionando las tareas para el equipo. Siendo el PO el que "achucha" al equipo para que las tareas se vayan haciendo según el orden establecido en la historia de usuario. El Equipo irá haciendo cada una de las tareas de la columna "DOING" durante un plazo apróximado de 2 semanas que se conoce con el nombre de SPRINT (ver Imagen 5). Durante este tiempo el Equipo se autoorganiza para que las tareas salgan adelante y estén acabadas al final del SPRINT. De no ser así, se verían las razones y se pasaría las tareas no realizadas al siguiente SPRINT. Mientras, en reuniones diarias de no más de 15 min. en los que el equipo y el PO se juntan, se debaten las actividades y su estatus. Estas reuniones suelen hacerse de pie, para que no se dilanten en el tiempo.
![Imagen 1][1]  ![Imagen 2][2]

 [1]: /images/Metod_Agil_05.jpg "Imagen 5"
 [2]: /images/Metod_Agil_06.jpg "Imagen 6"

Después de la finalización de cada SPRINT se le hace una DEMO al cliente con las funcionalidades acabadas. Además se hace una retrospectiva de cómo ha ido el SPRINT para ver errores cometidos y mejoras para futuros SPRINTS.

###__TODO MUY BONITO PERO...¿CÓMO SE COBRA AL CLIENTE DE ESTA FORMA?__

 De una forma tradicional (ver linea roja de Imagen 7) al principo del proyecto, durante la fase de análisis se calcula un presupuesto que el cliente de aprobar y se cobra a la entrega del producto. Esto significa que durante todo el ciclo no se cobra ningún euro. Además de que estamos aventurando una serie de horas y recursos en la primera fase y que no sabemos si podremos cumplirlos. En la mayoría de los proyectos esas estimaciones son erroneas y se acaban metiendo más horas de las presupuestadas (con su correspondiente pérdida de ganancias).  
 ¿Cómo se hacen con Scrum? Se estipula un precio por SPRINT, de tal forma que con cada uno de ellos el cliente recibe una funcionalidad que quiere en su proyecto software y así mientras en los primeros SPRINTS recibe las funcionalidades más importantes que el cliente requiere, en los últimos recibe los que menos importancia le ha dado. Y de esta forma, el cliente puede dar por finalizado incluso antes de terminar todo, en caso de que su presupuesto no de para maś o tenga la necesidad de implantarlo cuanto antes con lo que hasta esa fecha se le ha entregado.
:![Alt text](/images/Metod_Agil_07.jpg "Imagen 7")

Espero que os haya gustado este autoresumen.
