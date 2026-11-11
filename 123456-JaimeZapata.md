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