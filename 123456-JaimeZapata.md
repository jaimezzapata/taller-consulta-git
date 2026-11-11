1: 
Git es un sistema de control de versiones distribuido diseñado para registrar los cambios en los archivos de un proyecto a lo largo del tiempo.

En el desarrollo de software, resuelve problemas fundamentales relacionados con la coordinación y el mantenimiento del código:

Trabajo colaborativo simultáneo: Permite que múltiples desarrolladores trabajen en el mismo proyecto o incluso en el mismo archivo al mismo tiempo. Git gestiona la fusión de estas aportaciones y, si dos personas modifican la misma línea, alerta sobre el conflicto para que se resuelva manualmente, evitando que el trabajo de uno sobrescriba el del otro.

Trazabilidad y auditoría: Mantiene un historial exacto de cada modificación. Permite saber quién cambió el código, qué líneas específicas se alteraron, cuándo se hizo y cuál fue el motivo (a través del mensaje del commit).

Experimentación aislada (Ramas): Mediante el uso de branches, permite crear copias de trabajo independientes. Se puede desarrollar una nueva funcionalidad o corregir un error crítico sin riesgo de romper el código de la rama principal (producción). Una vez que el código nuevo es estable, se integra.

Recuperación ante errores: Si un nuevo despliegue falla o se introduce un bug, Git permite revertir el proyecto a un estado anterior completamente funcional de manera rápida y segura.

En la práctica, elimina la gestión manual de archivos (como proyecto_v1, proyecto_final, proyecto_final_ahora_si) y estructura el caos del trabajo en equipo en un flujo organizado.


Punto 2:

Git es el sistema de control de versiones que instalas en tu computadora para registrar y gestionar el historial de cambios en tu código de forma local. GitHub, en cambio, es un servicio web que sirve para alojar, compartir y colaborar en los repositorios que previamente creaste con Git. La diferencia fundamental radica en que Git es el motor subyacente que rastrea las modificaciones mediante comandos, mientras que GitHub es una plataforma en internet que añade una interfaz gráfica y funciones sociales o de equipo, como pull requests, gestión de incidencias e integraciones. Puedes usar Git sin GitHub, pero no puedes usar GitHub sin Git.

Una nube de repositorios es una infraestructura remota diseñada para centralizar los proyectos de software, permitiendo que múltiples desarrolladores sincronicen su código local en un servidor compartido. Funciona como un punto de encuentro y de respaldo que evita la pérdida de código, y proporciona herramientas adicionales para revisar los aportes de otros, automatizar pruebas y gestionar los pases a producción.

Además de GitHub, existen otras alternativas destacadas para alojar repositorios:

GitLab: Destaca por incluir herramientas de integración y despliegue continuo (CI/CD) muy potentes desde su versión base, permitiendo gestionar todo el ciclo de vida del software en un solo lugar.

Bitbucket: Desarrollada por Atlassian, su mayor atractivo es la integración nativa y profunda con herramientas de gestión de proyectos ágiles como Jira y Trello.

Azure DevOps (Azure Repos): La solución corporativa de Microsoft, muy orientada a empresas que buscan repositorios privados ilimitados y una conexión directa con la infraestructura de la nube de Azure.

Punto tres

Commit: Es como tomarle una foto o guardar un punto de control al estado actual de tus archivos. Registra los cambios específicos que hiciste para que queden guardados en el historial del proyecto de forma permanente.

Ejemplo práctico: Terminaste de armar la estructura HTML del menú de navegación y funciona bien. Haces un commit con el mensaje "Agrega estructura del menú principal" para asegurar ese avance antes de empezar a modificar los estilos CSS, sabiendo que siempre puedes volver a ese punto si rompes algo.

Branch (Rama): Es una línea de tiempo paralela de tu proyecto. Te permite trabajar en nuevas funcionalidades, hacer pruebas o corregir errores sin afectar el código principal o estable (que suele estar en la rama main).

Ejemplo práctico: Tienes una aplicación en producción, pero quieres probar un nuevo diseño para el inicio de sesión. Creas una rama llamada nuevo-login. Si el código falla mientras experimentas, la aplicación original sigue intacta.

Merge (Fusión): Es el proceso de unir el historial y los cambios que hiciste en una rama separada hacia otra rama, generalmente para integrar un trabajo nuevo a la línea principal del proyecto.

Ejemplo práctico: Ya terminaste, probaste y validaste el nuevo diseño en la rama nuevo-login. Ejecutas un merge para pasar esos cambios a la rama main y que la nueva vista pase a ser la oficial.

Pull y Push: Son los comandos utilizados para sincronizar tu entorno local con la nube (como GitHub). Push (empujar) envía tus commits locales al repositorio remoto. Pull (tirar) descarga los cambios que están en la nube y actualiza automáticamente los archivos en tu computadora.

Ejemplo práctico: Un compañero arregló un error anoche; al iniciar tu día, haces un pull para traer su arreglo a tu PC. Luego, terminas una nueva función de la base de datos y haces un push para subirla a la nube y que él pueda descargarla.

Pull Request (PR): Es una petición formal en plataformas web para que otros revisen tu código antes de hacer un merge. Permite discutir los cambios, ver exactamente qué líneas se agregaron o borraron, y aprobar el código antes de integrarlo a la rama principal.

Ejemplo práctico: Desarrollaste la integración de una pasarela de pagos en tu propia rama. Antes de unirla a main, abres un Pull Request. El líder técnico revisa el código, te sugiere cambiar una variable por seguridad, haces la corrección y, una vez aprobado, se fusiona.

Clone (Clonar): Es descargar una copia exacta y completa de un repositorio remoto a tu computadora por primera vez. Esto trae todos los archivos, el historial de commits y las ramas existentes.

Ejemplo práctico: Entras a trabajar a una nueva empresa y te dan acceso al proyecto del sistema de facturación en GitHub. Haces un clone de esa URL para tener la carpeta del proyecto en tu máquina local y empezar a programar.

Upstream (y su diferencia con Origin): Ambos son identificadores para repositorios remotos, pero se usan para diferenciar fuentes cuando trabajas con copias (forks). Origin es el repositorio remoto que te pertenece (tu copia en la nube), mientras que Upstream es el repositorio original del proyecto principal del cual sacaste tu copia.

Ejemplo práctico: Quieres aportar a una librería pública de React (Upstream). Como no tienes permisos para editarla directamente, haces una copia hacia tu propia cuenta de GitHub (Origin). Clonas tu Origin a tu PC, haces los cambios, los subes de vuelta a tu Origin (con un push), y desde ahí abres un PR hacia el Upstream pidiendo que acepten tu mejora.