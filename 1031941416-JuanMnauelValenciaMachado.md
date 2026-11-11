# Guía de Actividad: Dominando Git, GitHub y GitFlow

**Respuestas**

1. ## Git es un control de versiones distribuido, de codigo abierto. Su principal funcion es registrar y rastrear cambios que se realizan en el codigo fuente de un proyecto a lo largo de su construccion

* Puede solucionar estos problemas:

## Eliminar archivos duplicados (adiós a los sufijos tipo _v2_final).

## Permitir colaboración simultánea sin que nadie sobrescriba el código de otro mediante ramas (branches).

## Ofrecer trazabilidad total para saber quién, cuándo y por qué se modificó cada línea.

## Garantizar seguridad y descentralización (cada copia local contiene todo el historial).

## Permitir experimentar de forma segura sin arriesgar la versión estable del proyecto.

2. ## Git es como la app o el programa que usas en tu compu sin internet. Cada vez que le das a "Guardar versión", el programa toma una foto de cómo va tu trabajo. Si la cagas borrando algo por accidente, puedes presionar un botón y devolverte exactamente a como lo tenías ayer o hace tres horas.

## GitHub es literalmente el Google Drive de los programadores. Es una página web a la que subes las carpetas donde Git tomó esas fotos. Sirve para que tu proyecto no se pierda si a tu laptop le pasa algo, y para que tus compañeros se conecten, descarguen tu avance en sus propias compus y todos trabajen al mismo tiempo sin tirarse el código del otro.

3. ## Una nube de repositorios es un servicio en la nube que te permite almacenar, respaldar y gestionar tus proyectos de código que usan Git.

* Alternativas ademas de GitHub:

## GitLab: Es una de las plataformas más completas del mercado. A diferencia de otras, destaca por integrar de forma nativa herramientas muy potentes de CI/CD (integración y despliegue continuo), gestión de proyectos ágiles y seguridad directamente en su interfaz.

## Bitbucket: Desarrollada por Atlassian, es una alternativa muy elegida por empresas que ya utilizan herramientas de la misma familia como Jira o Trello, ya que se integra perfectamente con ellas. Además, ofrece repositorios privados gratuitos para equipos pequeños.

## Gitea / Forgejo: Si buscas una opción más ligera o la posibilidad de alojar tu propio servidor de Git en tu propia computadora o servidor privado (auto-hospedaje) en lugar de depender de una gran empresa, estas alternativas de código abierto son excelentes y muy rápidas.

4. ## Commit: Una "foto" o guardado de los cambios actuales en tu código con un mensaje. (Ej: git commit -m "Agregué el menú").

## Branch (Rama): Una línea de trabajo independiente para programar sin afectar el código principal. (Ej: crear feature/login).

## Merge (Fusión): Unir los cambios de una rama con otra. (Ej: pasar el login terminado a la rama principal main).

## Pull y Push: Sincronizar tu PC con la nube. Push sube tus cambios a GitHub; Pull descarga los cambios de otros a tu computadora.

## Pull Request (PR): Una solicitud en GitHub para que revisen tu código antes de unirlo al proyecto oficial.

## Clone (Clonar): Descargar por primera vez un repositorio completo de GitHub a tu computadora.

## Origin y Upstream: Nombres de repositorios remotos. Origin es tu repositorio personal (de donde clonas o subes), y Upstream es el repositorio original del dueño principal en proyectos colaborativos externos.

5. ¿Para qué sirven las ramas?

## Las ramas sirven para aislar los cambios que realizas en el código. En lugar de modificar directamente la versión de producción o la rama principal (main o master), creas un entorno de trabajo paralelo donde puedes:

## Desarrollar una nueva característica de principio a fin de forma controlada.

## Investigar, probar y descartar soluciones experimentales sin compromiso.

## Aislar la corrección de un error urgente (hotfix) mientras otras tareas siguen su curso en paralelo.

*Ventajas en el Trabajo Individual*
## Trabajar con ramas no es exclusivo de los equipos grandes; incluso en proyectos personales ofrece beneficios clave:

## Experimentación sin miedo: Si una prueba o un cambio experimental rompe todo el código, puedes descartar la rama con un simple comando sin dañar tu progreso anterior ni arriesgar el funcionamiento estable.

## Organización por objetivos: Te permite separar claramente cada tarea (por ejemplo, una rama para la interfaz de usuario, otra para la conexión a la base de datos). Esto facilita retomar el desarrollo después de unos días sabiendo exactamente en qué estabas enfocándote.

## Historial limpio y trazable: Cada commit en una rama específica documenta de forma ordenada los pasos seguidos para resolver una tarea o implementar una característica concreta.

*Ventajas en el Trabajo en Equipo*
## Cuando se colabora con más desarrolladores, las ramas se convierten en la columna vertebral de la productividad y la calidad del software:

## Desarrollo en paralelo (Concurrencia): Varios desarrolladores pueden trabajar al mismo tiempo en la misma base de código sin pisarse ni sobreescribir el trabajo de los demás, ya que cada uno opera en su propio espacio aislado (feature branch).

## Revisiones de código seguras (Code Review / Pull Requests): Antes de integrar los cambios de una rama al tronco principal, el equipo puede revisar, probar y discutir las modificaciones, asegurando estándares de calidad y detectando bugs anticipadamente.

## Protección de la rama principal (main): La rama principal se mantiene siempre limpia, estable y lista para producción, mientras que las pruebas, iteraciones y errores ocurren en entornos controlados y separados.

6. GitFlow se basa en dos ramas principales de vida permanente y tres ramas de soporte temporal:

1. *Ramas Principales (Permanentes)*
## master (o main): Contiene el código oficial que está actualmente en producción. Cada fusión (merge) en esta rama representa un nuevo lanzamiento y suele estar etiquetada con un número de versión (ej. v1.2.0).

## develop: Es la rama de integración principal. Contiene todo el código nuevo que se está preparando para el siguiente lanzamiento. Los desarrolladores la toman como base para sus nuevas tareas.

 *Ramas de Soporte (Temporales)*
## feature/... (Características): Se crean a partir de develop para desarrollar nuevas funcionalidades de forma aislada. Una vez terminada la característica, se vuelve a fusionar (merge) en develop y la rama se elimina.

## release/... (Lanzamientos): Cuando develop ya tiene suficientes características para una nueva versión, se crea una rama de lanzamiento a partir de ella. Permite realizar pruebas finales de QA, corrección de pequeños bugs y empaquetado sin interrumpir el desarrollo de la siguiente versión. Al finalizar, se fusiona tanto en master como en develop.

## hotfix/... (Correcciones urgentes): Son ramas creadas directamente desde master para solucionar un error crítico detectado en producción. Una vez resuelto el problema, el cambio se fusiona de inmediato tanto en master como en develop para evitar que el fallo reaparezca en el futuro.