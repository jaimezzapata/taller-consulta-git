1: ¿Qué es Git y qué problema resuelve en el desarrollo de software?
Git es un sistema de control de versiones distribuido y de código abierto diseñado para registrar los cambios en el código fuente de un proyecto a lo largo del tiempo, facilitando el trabajo ordenado y colaborativo entre desarrolladores.

En el desarrollo de software, esta herramienta resuelve problemas críticos como el caos de los archivos duplicados con nombres confuso, reemplazándolos por un historial estructurado de commits que permite auditar y revertir modificaciones. Asimismo, previene que los equipos se sobrescriban el trabajo al permitir el uso de ramas independientes que luego se fusionan de forma segura al tronco principal. Al ser distribuido, cada copia local almacena el historial completo del proyecto, evitando la pérdida de información ante fallos y sirviendo como respaldo junto con plataformas en la nube. Finalmente, simplifica el debugging al identificar con exactitud qué usuario, fecha y cambio introdujeron una línea específica de código.

2: Diferencias clave entre Git y GitHub. (Explique por qué no son lo mismo).
Git y GitHub suelen confundirse o utilizarse como si fueran lo mismo, pero en realidad cumplen funciones totalmente diferentes en el flujo de desarrollo. Git es la herramienta fundamental: un software de control de versiones local que se instala en tu computadora para rastrear cada modificación, guardar historiales de cambios, manejar ramas y permitirte viajar en el tiempo a versiones anteriores de tu código fuente sin necesidad de estar conectado a internet.

Por otro lado, GitHub es una plataforma web de alojamiento en la nube construida alrededor de Git. Funciona como un servidor centralizado donde los desarrolladores pueden subir (push) y compartir sus repositorios locales para respaldarlos de forma segura en internet y facilitar el trabajo colaborativo en equipo mediante herramientas visuales como solicitudes de extracción (pull requests), revisiones de código y control de incidencias (issues). En resumen, Git es el motor que rastrea y gestiona el código en tu máquina, mientras que GitHub es el punto de encuentro en la nube para almacenar, compartir y colaborar en esos proyectos con otras personas.

3: ¿Qué es una nube de repositorios? Expliquen este concepto y mencionen al menos tres alternativas diferentes en el mercado (por ejemplo, además de GitHub, ¿qué otras plataformas existen?).

Una nube de repositorios (también conocida como servicio de alojamiento de código fuente o plataforma de control de versiones basada en la nube) es un servicio en línea que almacena y gestiona repositorios de Git de forma remota. Funciona como un centro neurálgico en internet donde los equipos de desarrollo pueden respaldar su código, sincronizar los avances individuales de cada integrante, realizar copias de seguridad automáticas y colaborar de manera fluida sin depender exclusivamente de una máquina local. Además de guardar el historial de cambios, estas plataformas integran herramientas de gestión de proyectos, control de versiones visual, revisión de código (code review), automatización de pruebas y despliegues (CI/CD).

4: Glosario básico: Definan con sus propias palabras, de forma clara y agregando un ejemplo práctico para cada uno, los siguientes conceptos fundamentales de Git: commit, branch, merge, pull y push, pull request (PR), clone y upstream (y su diferencia con origin).

Definiciones:

commit: Es como guardar un punto de control de tu proyecto. Cuando modificas archivos y haces un commit, congelas ese momento exacto en el tiempo y le pones una nota corta para recordar qué hiciste.

branch: Es como sacar una copia temporal de tu proyecto para trabajar en algo nuevo (una función o un arreglo) sin tocar ni arriesgar el código principal que ya está funcionando.

merge: Es el paso final de unir lo que hiciste en una rama de prueba con la rama principal del proyecto.

pull y push: Son los comandos para comunicarte con la nube. Push es enviar (empujar) tus cambios locales hacia internet, y Pull es descargar (jalar) a tu computadora los cambios que hayan subido tus compañeros.

pull request (PR): Es una petición formal que haces en internet (como en GitHub) para avisarle a tu equipo que terminaste una tarea y pedirles que revisen tu código antes de juntarlo con el proyecto principal.

clone: Es descargar por primera vez una copia completa de un proyecto que está en internet (con todo su historial y sus ramas) directamente a tu computadora.

upstream y su diferencia con origin: Son los nombres o apodos que se usan para identificar los lugares en internet donde guardas tu código. Origin es tu propia copia o el lugar donde tú estás subiendo tus cosas habitualmente. Upstream es el proyecto original y principal (muy usado en código abierto cuando colaboras en proyectos de otras personas).

Ejemplos prácticos:

commit: Terminas de escribir la barra de navegación de tu página, haces un commit con el mensaje "agrego menú de navegación" y así guardas ese avance en la historia del proyecto por si luego necesitas consultarlo.

branch: Tu aplicación funciona bien, pero quieres probar un carrito de compras. Creas una rama llamada carrito para programarlo con total libertad sin que afecte el programa principal hasta que esté listo.

merge: El carrito de compras que programaste en la rama carrito ya quedó perfecto y sin errores; entonces haces un merge para unirlo con la rama principal y que ya forme parte oficial de la aplicación.

pull y push: Al terminar de programar en la tarde, ejecutas git push para respaldar tu código en GitHub. Al día siguiente, antes de empezar, ejecutas git pull para asegurarte de tener en tu PC lo último que hizo tu equipo.

pull request (PR): Creaste una nueva sección de contacto, la subes a GitHub y abres un Pull Request para que tus compañeros le echen un vistazo, den su visto bueno y aprueben la unión.

clone: Entras a un nuevo proyecto, copias el enlace de GitHub y escribes git clone en tu terminal para traerte todos los archivos y carpetas a tu PC de un solo golpe.

upstream y su diferencia con origin: Si sacas una copia de un repositorio público para aportar mejoras, tu propia copia en la nube es origin, y el repositorio principal de la persona que creó el proyecto es el upstream.

5: La importancia de las ramas (Branches): ¿Por qué se deben crear ramas en un proyecto de software? Expliquen para qué sirven y qué ventajas ofrecen tanto en el trabajo individual como en equipo.

Las ramas (branches) son líneas de desarrollo independientes que permiten aislar el código en un repositorio para trabajar en nuevas funcionalidades, experimentos o correcciones de errores sin alterar la versión principal ni comprometer la estabilidad del sistema. Su uso es una de las prácticas más importantes en el control de versiones, ya que ofrecen ventajas fundamentales tanto en proyectos individuales como colaborativos. En el trabajo individual, permiten organizar las tareas por partes y probar cambios arriesgados con la total tranquilidad de que, si algo sale mal, la rama principal o de producción se mantiene intacta y se puede descartar el experimento sin dañar lo avanzado. Por su parte, en el trabajo en equipo, las ramas evitan que varios desarrolladores interfieran o sobrescriban el trabajo de los demás al mismo tiempo, permitiendo que cada quien desarrolle su tarea en su propia ruta aislada para luego unificar todo de forma segura mediante fusiones (merges) o revisiones de código (pull requests).


