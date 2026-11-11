1. ¿Qué es Git y qué problema resuelve en el desarrollo de software?
Git es un sistema de control de versiones distribuido (DVCS) creado por Linus Torvalds en 2005. Permite registrar los cambios realizados en archivos a lo largo del tiempo para que se pueda recuperar versiones específicas más adelante.

Problema que resuelve:

Pérdida de código y duplicación: Elimina la necesidad de crear copias manuales como proyecto_v1, proyecto_final, proyecto_final_FINAL.

Trabajo en equipo: Facilita que varios desarrolladores trabajen en paralelo sobre el mismo código sin sobrescribir el trabajo de los demás.

Trazabilidad e historial: Permite saber exactamente quién, cuándo y por qué se modificó cada línea de código.

2. Diferencias clave entre Git y GitHub

Aunque a menudo se usan juntos, no son la misma herramienta y cumplen roles completamente diferentes en el desarrollo:

Git (El sistema local): Es un software de control de versiones instalado directamente en tu computadora. Funciona de manera local y sin necesidad de internet para registrar tu historial de cambios, crear ramas y hacer commits.

GitHub (La plataforma en la nube): Es un servicio de alojamiento web basado en la nube que almacena los repositorios de Git. Su función principal es servir como punto central para que varios desarrolladores compartan código, colaboren en equipo y gestionen herramientas como Pull Requests e Issues.

En resumen: Git es la herramienta que gestiona tu historial de versiones en tu equipo, y GitHub es la plataforma en línea donde compartes y respaldas ese trabajo con el resto del mundo.

3. ¿Qué es una nube de repositorios y alternativas?
Una nube de repositorios es un servicio de alojamiento remoto diseñado para guardar y respaldar proyectos gestionados con un sistema de control de versiones (como Git). Actúa como un servidor central desde el cual se puede sincronizar, compartir y auditar el código fuente.

Alternativas en el mercado:

GitLab: Plataforma integral orientada a DevOps y CI/CD integrado.

Bitbucket: Propiedad de Atlassian, integrada nativamente con Jira y Confluence.

Azure DevOps (Azure Repos): Servicio de Microsoft para repositorios privados integrados en entornos empresariales.

4. Glosario básico de Git

Commit: Es una captura instantánea (snapshot) del estado actual de todos los archivos de tu proyecto en un momento determinado. Guarda el progreso realizado de forma permanente en el historial local de Git.

Ejemplo práctico: Al terminar de programar la interfaz de inicio de sesión, ejecutas git commit -m "feat: implementar estructura inicial del login" para congelar ese estado en el historial.

Branch (Rama): Es una línea de tiempo independiente y paralela dentro del repositorio. Permite desarrollar nuevas funciones, corregir errores o experimentar sin alterar ni desestabilizar el código de la rama principal (develop o master).

Ejemplo práctico: Creas una rama llamada feature/carrito-compras para añadir la funcionalidad de compras de forma aislada mientras la aplicación principal sigue funcionando sin modificaciones.

Merge (Fusión): Es el proceso mediante el cual Git combina el historial y los cambios de dos ramas diferentes en una sola. Integra el trabajo aislado que hiciste en una rama hacia una rama receptora (como develop).

Ejemplo práctico: Una vez probada y terminada la función en feature/carrito-compras, te posas en develop y ejecutas un merge para unir todo el código nuevo.

Pull y Push:

Push: Es la acción de enviar los commits que realizaste localmente en tu computadora hacia el repositorio remoto en la nube (por ejemplo, tu fork en GitHub).

Pull: Es la acción inversa; descarga las actualizaciones más recientes que están en el repositorio remoto y las fusiona automáticamente en tu entorno de trabajo local.

Ejemplo práctico: Ejecutas git push origin develop para subir tus últimos cambios a la nube, o git pull origin develop para traer a tu PC el código que un compañero subió recientemente.

Pull Request (PR): Es una solicitud formal realizada a través de una plataforma web (como GitHub) para avisar a los colaboradores o líderes de proyecto que has terminado cambios en una rama y pides que sean revisados e integrados (merged) en otra rama (por ejemplo, de tu rama de funciones hacia develop).

Ejemplo práctico: Creas un Pull Request en GitHub para proponer que tu rama feature/consulta se integre a la rama develop tras pasar las revisiones de código.

Clone (Clonar): Es la acción de descargar por primera vez una copia exacta de un repositorio remoto (con todo su historial de commits y ramas) desde la nube hacia el disco duro de tu computadora local.

Ejemplo práctico: Ejecutas git clone [https://github.com/usuario/proyecto.git](https://github.com/usuario/proyecto.git) para clonar el repositorio base del profesor y empezar a trabajar en él en tu ordenador.

Upstream y Origin:

Origin: Es el alias o nombre por defecto que Git le asigna a tu propio repositorio remoto personal en la nube (el fork que creaste en tu cuenta).

Upstream: Es el alias convencional que se le asigna al repositorio original o principal del cual hiciste el fork (por ejemplo, el repositorio matriz del profesor). Permite traer actualizaciones oficiales de la fuente original.

5. La importancia de las ramas (Branches)
Las ramas son uno de los pilares fundamentales del control de versiones moderno. Su propósito principal es permitir el aislamiento del flujo de trabajo, dividiendo el código en entornos independientes.

¿Por qué se deben crear ramas y qué ventajas ofrecen?

Trabajo individual seguro y limpio: Permiten experimentar, cometer errores o probar ideas experimentales sabiendo que, si algo sale mal, puedes descartar la rama sin dañar el funcionamiento principal de la aplicación.

Colaboración en equipo sin conflictos destructivos: En un equipo de 5 personas, cada desarrollador puede crear su propia rama para construir una característica distinta al mismo tiempo. Nadie sobrescribe el código de los demás directamente en el entorno estable.

Estructura de revisión organizada: Facilitan las revisiones de código (Code Reviews). Antes de que cualquier código nuevo se integre al proyecto oficial, se evalúa mediante un Pull Request aislado, garantizando que cumpla con los estándares de calidad.

6. ¿Qué es GitFlow y estructura de ramas?
GitFlow es un modelo de ramificación y estrategia de gestión de versiones para Git, ideado por Vincent Driessen. Proporciona un marco de trabajo estricto, altamente estructurado y orientado a proyectos de software que tienen ciclos de lanzamiento programados y requieren un control riguroso entre el desarrollo continuo y el entorno de producción.

Estructura de sus ramas principales y auxiliares:

master (o main): Es la rama principal de producción. Contiene únicamente código limpio, estable y listo para los usuarios finales. Cada cambio aquí representa una versión liberada oficialmente.

develop: Es la rama de integración continua. Reúne todo el código desarrollado por el equipo para las próximas actualizaciones. Es el punto base de donde nacen las nuevas funciones y hacia donde convergen.

feature/*: Son ramas temporales de desarrollo de nuevas funcionalidades. Nacen siempre a partir de develop y, una vez terminada la tarea, se fusionan de regreso a develop. Su nomenclatura suele ser feature/nombre-funcion.

release/*: Son ramas dedicadas a preparar un nuevo lanzamiento a producción. Permiten hacer pruebas finales de calidad (QA), correcciones menores de errores y actualización de versiones sin interrumpir el desarrollo de la siguiente fase en develop. Nacen de develop y se fusionan tanto a master como a develop.

hotfix/*: Son ramas de emergencia críticas. Nacen directamente de master para solucionar un fallo grave detectado en el entorno de producción en vivo. Una vez solucionado, se fusionan de urgencia tanto en master como en develop para evitar que el error persista.

¡Copia estos bloques mejorados punto por punto en tu archivo Markdown, haz tus git add . y tus commits correspondientes (git commit -m "docs: ..."), y me avisas cuando estés listo para avanzar con el push y los Pull Requests!