## Pregunta 1: ¿Qué es Git y qué problema resuelve en el desarrollo de software?

## Para mí, Git es una herramienta que sirve para llevar un control de los cambios que se hacen en un proyecto de software. Es como tener un historial de todo lo que voy haciendo en el código, para poder regresar a una versión anterior si cometo algún error o algo deja de funcionar.

## También permite que varias personas trabajen en un mismo proyecto sin perder los cambios que hace cada una.

## El problema que resuelve es la desorganización al momento de desarrollar un programa, ya que evita perder código, facilita trabajar en equipo y permite saber qué cambios se han realizado y quién los hizo.


# Pregunta 2: Diferencias clave entre Git y GitHub

Para mí, la principal diferencia entre Git y GitHub es que Git es una herramienta que permite controlar las versiones de un proyecto, mientras que GitHub es una plataforma donde podemos guardar esos proyectos y compartirlos con otras personas.

## Diferencias principales


| Git | GitHub |
| --- | --- |
| Es un sistema de control de versiones. | Es una plataforma para alojar proyectos. |
| Funciona desde nuestro computador. | Funciona principalmente a través de internet. |
| Permite guardar el historial de cambios. | Permite compartir el código con otros desarrolladores. |
| Permite crear ramas y unir cambios. | Facilita el trabajo en equipo y la colaboración. |
| No necesita internet para trabajar localmente. | Necesita internet para sincronizar los repositorios remotos. |


## Pregunta 3: ¿Qué es una nube de repositorios?

Una nube de repositorios es una plataforma en internet que permite almacenar, organizar y administrar proyectos de programación, especialmente su código fuente. También permite que varias personas trabajen en un mismo proyecto desde diferentes lugares, compartan cambios y mantengan un registro de las modificaciones realizadas.

## Tres alternativas

1. GitLab: Es una plataforma que permite guardar código de programación en internet, trabajar en equipo y controlar los cambios que se realizan en los proyectos.

2. Bitbucket: Es una herramienta que permite almacenar repositorios de código y compartir proyectos con otros programadores. También ayuda a organizar el trabajo en equipo.

3. SourceForge: Es una plataforma que permite publicar, almacenar y compartir proyectos de software. Es utilizada principalmente para proyectos de código abierto.


## Pregunta 4: Glosario básico:

Glosario básico de Git
1. Commit: Es guardar los cambios realizados en un proyecto para tener un registro de los avances.

Ejemplo: Guardar el diseño de una página web después de terminarlo.

2. Branch (Rama): Es una línea de trabajo independiente que permite hacer cambios sin afectar el proyecto principal.

Ejemplo: Crear una rama para agregar un formulario a una página web.

3. Merge (Fusión): Es unir los cambios de una rama con otra.

Ejemplo: Unir el formulario terminado con el proyecto principal.

4. Pull y Push:

Pull: Descargar los cambios más recientes del repositorio remoto.

Push: Subir nuestros cambios al repositorio remoto.

Ejemplo: Hacer pull para recibir el trabajo de un compañero y push para compartir el nuestro.

5. Pull Request (PR): Es una solicitud para que revisen nuestros cambios antes de unirlos al proyecto principal.

Ejemplo: Pedirle a un compañero que revise nuestro código antes de aprobarlo.

6. Clone (Clonar): Es copiar un repositorio de internet a nuestro computador.

Ejemplo: Descargar un proyecto de GitHub para trabajar en él.

7. Upstream y Origin:

Upstream: Es el repositorio original del proyecto.

Origin: Es el repositorio remoto que normalmente corresponde a nuestra propia copia.

Ejemplo: Si hacemos una copia (fork) de un proyecto de otra persona, nuestra copia es origin y el proyecto original es upstream.

## Pregunta 5: La importancia de las ramas (Branches)

La importancia de las ramas (Branches)
Las ramas son importantes en un proyecto de software porque nos permiten trabajar en diferentes funciones sin afectar el proyecto principal. Sirven para probar nuevas ideas, corregir errores y realizar cambios de manera más organizada.

Cuando trabajamos solos, las ramas nos ayudan a experimentar y hacer modificaciones sin dañar el trabajo que ya tenemos. Cuando trabajamos en equipo, permiten que cada persona se encargue de una parte diferente del proyecto sin interferir con el trabajo de los demás.

Sus principales ventajas son:

Permiten trabajar de forma más organizada.

Evitan dañar el proyecto principal.

Facilitan el trabajo en equipo.

Ayudan a corregir errores y probar nuevas funciones.

## Pregunta 6: ¿Qué es GitFlow?

GitFlow es una forma de organizar el trabajo en Git mediante diferentes ramas. Sirve para mantener el proyecto ordenado y facilitar el desarrollo de nuevas funciones, las pruebas y la corrección de errores.

Sus ramas principales son:

Master: Es la rama principal donde se encuentra la versión estable del proyecto.

Develop: Es donde se van uniendo los cambios y avances antes de publicarlos.

Feature: Se utiliza para desarrollar nuevas funciones sin afectar las demás partes del proyecto.

Release: Se usa para preparar y revisar una nueva versión antes de publicarla.

Hotfix: Sirve para corregir errores urgentes que aparecen en la versión publicada.