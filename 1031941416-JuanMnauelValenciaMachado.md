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