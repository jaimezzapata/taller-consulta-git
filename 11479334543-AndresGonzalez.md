1: git es un sistema de control distribuido, guarda el historial de los cambios para que si los algo salen mal sepueda volcer atras para recuperar los trabajos ya hechos. resuelve los caos de trabajar en equipos sin pisar los cambios y permite volver atras para recuperar datos si estos fallan 

2: git es un sistema de control distribuidos que permite registrar,organizar y controlar los cambios que se realicen en un proyecto de software y en cambio GitHub es un sitio web donde se suben el proyecto de Git para compartir y ver los proyectos de los demas 


3: una nube de repositorios es un servicio de internet donde se guarda respositorios de codigo para compartirlo, respaldarlo y trabajar sin enredos. GitHub es un ejemplo claro de una nube de respositorios ya que es un espacio donde la gente sube sus repositorios y las demas personas pueden verlo, manejarlo e incluso mejorarlo



4: Glosario de papabras con ejemplos 

commit
Definicion: es guardar un cambio en el historial de cualquier proyecto
Ejemplod: cambias una línea en tu archivo, luego escribes "git add ."  para preparar el cambio, y después "git commit -m "los cambios hechos" para guardar esa versión

branch:
Definicion: es una rama o copia aparte del proyecto para probar cambios sin arfectar la version principal
Ejemplos: marca una rama, se escribe un cambio y si funciona se une a la rama principal, si sirve se concerva, si no sirve se descarta. es como al escribir una carta de amor, se hace una copia de esa carta, se agrega lo que se desee agregar, si eso funciona se para para la carta principal, si no funciona se puede descartar


Merge:
Definicion: es unir los cambios de la rama copia a la rama principal, juntar lo que se propo en la rama de prueba y luego juntarlo a la rama principal
Ejempolo: es como tener dos proyectos, uno principal y el otro es una copia, si se hacen cambios en el proyecto copia y son buenos esos cambios se utiliza un merge 

pull y push:
definicion: push es enviar los cambios en linea y pull es traer los cambios nuevos hacia el ordenador
Ejemplos: es como tener un proyecto con un amigo, yo hago cambios y los envio con "push" y si mi compañero hace cambios yo hago un "pull" para traer esos cambios


pull request:
Definicion: es uan solicitud para revisar y mezclar los cambios desde una rama principal, asi las demas personas lo revisan antes de aceptarlo
Ejemplos:es como tener una lista de regalos y revisarlo antes de salir a repartirlos, es ver que todo este bien para que no hayas problemas al momento de salir

clone:
definicion: es clonar un repositorio, es bajar una copia completa con todo y historial al computador que tengo en ese momento, para trabajar localmente sin depender de internet
Ejemplo: se clona el repositorio del profe con todo e historial, se hacen los cambios localmente y luego se le envia al profesor


upstream
Definicion: es el repositorio original del que se clona o se actualiza y su diferencia con origin es que origin es la copia propia del que clono, origin baja del repositorio y upstream sube al repositorio
Ejemplo: es como encontrar un libro de recetas en una estanteria, ese libro de recetas es el "upstream" luego con ese libro yo le hago fotocopias, las fotocopias serian el origin, luego yo agregaria notas a las fotocopias y las subiria al upstream si es que me las aceptan

5: la importancia de las ramas
branches:
Definicion: sirve para trabajar en funciones o ideas aparte, sin modificar la version principal del proyecto, es para probar, fallar, y corregir y si todo sale correcto se sube al principal. en unntrabajo indiviual es que permite concentrarse en el trabajo uno mismo sin depender de los demas, entender cada paso a fondo y corregir a mi manera. para el trabajo en equipo la ventaja es que las ideas se suman, se pueden rapartir tareas para avanzar mas rapido, se permiten mejoras desde otra perspectiva que ayudan a mejorar la calidad
Ejemplo:es como tener un pagina web y cambiar el color de un boton, es branch se crea para probar eso y si queda bien se une con el merge, si no queda bien simplemente se descarta


6: es un modelo de trabajo con ramas en Git, se definen las ramas claras para organizar el desarrollo, las correcciones y las versiones que salen a produccion 
main/master es la version estable la que ya funciona y se entrega
Develop es donde se juntan las cosas que estan en construccion
Feature son ramas temporales para cada funcion, estas se crean desde develop y cuando funciona se mezclan
Release es una rama para preparar una version antes de salir a produccion, se corrigen detalles finales y despues se funciona con main
Hotfix es para arreglos urgentes en produccion, sale desde main y regresa a main apenas el arreglo esta listo
