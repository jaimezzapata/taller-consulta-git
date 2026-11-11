*1*
**Git** es un sistema de control de versiones distribuido, gratuito y de código abierto, diseñado por Linus Torvalds en 2005 para gestionar el código fuente del núcleo Linux. Su función principal es **registrar todos los cambios realizados en un proyecto a lo largo del tiempo**, permitiendo a los desarrolladores volver a versiones anteriores, comparar estados y trabajar en equipo de manera eficiente.

### ¿Qué problema resuelve en el desarrollo de software?

Antes de sistemas como Git, el desarrollo colaborativo era un proceso caótico y propenso a errores. Git soluciona problemas fundamentales como:

1. **El fin del caos de archivos duplicados:**
* **El problema antiguo:** Guardar copias como `proyecto_final.zip`, `proyecto_final_v2.zip`, `proyecto_final_revisado_por_juan.zip` dificultaba saber cuál era la versión correcta.
* **La solución de Git:** Mantiene un único directorio de proyecto conectado a una base de datos interna (el repositorio) que almacena el historial completo de forma limpia y organizada.


2. **La colaboración sin pisar el trabajo de otros:**
* **El problema antiguo:** Si dos personas editaban el mismo archivo al mismo tiempo, uno sobrescribía el trabajo del otro y se perdía información.
* **La solución de Git:** Gracias a las **ramas** (*branches*), los desarrolladores pueden trabajar en funciones o correcciones de forma aislada y segura (`feature/login`, `bugfix/header`), para luego fusionarlas (*merge*) de manera controlada. Git ayuda a detectar automáticamente conflictos si dos personas modifican exactamente la misma línea de código.


3. **La red de seguridad (historial y reversión):**
* **El problema antiguo:** Un cambio experimental rompía todo el sistema y obligaba a reescribir código desde cero o intentar recordar qué se modificó.
* **La solución de Git:** Cada cambio (*commit*) es un punto de restauración. Si algo falla, se puede **viajar en el tiempo** para inspeccionar versiones anteriores, revertir errores específicos de forma instantánea o auditar quién escribió cada línea de código y por qué.


4. **El trabajo desconectado y distribuido:**
* Al ser *distribuido*, cada desarrollador tiene una copia local completa del repositorio con todo su historial. Esto permite trabajar sin conexión a internet y sincronizar los cambios con servidores remotos (como GitHub, GitLab o Bitbucket) cuando sea necesario.

*2.*
### Diferencias clave entre Git y GitHub.

* A menudo se confunden o se usan como si fueran sinónimos, pero Git y GitHub no son lo mismo. La diferencia fundamental radica en que uno es la herramienta tecnológica y el otro es el servicio de alojamiento (hosting) en la nube. *

* Naturaleza y función: *

* Git es un software de control de versiones local e independiente. Se instala en tu computadora y se ejecuta desde la terminal para rastrear los cambios en tu código fuente y gestionar ramas de trabajo de forma offline. *

* GitHub es una plataforma web y un servicio en la nube (propiedad de Microsoft) diseñado para alojar repositorios Git, facilitando la colaboración en equipo, la revisión de código (pull requests), la gestión de tareas (issues) y la automatización (GitHub Actions). *

* Dependencia: *

* Puedes usar Git perfectamente en tu ordenador sin necesidad de tener internet ni una cuenta en GitHub. *

* GitHub depende completamente de Git para funcionar; de hecho, utiliza Git como motor principal para gestionar las versiones del código que los usuarios suben a sus servidores. *

* Infraestructura: *

* Git opera de manera distribuida; cada desarrollador tiene una copia completa del historial en su máquina local. *

* GitHub actúa como un servidor centralizado remoto donde los equipos sincronizan sus repositorios locales para centralizar el trabajo compartido. *

*3*
### ¿Qué es una nube de repositorios?
* Una nube de repositorios (o servicio de alojamiento de código en la nube) es una plataforma basada en web que permite almacenar, gestionar y sincronizar repositorios de Git de forma remota. *

* Mientras que Git funciona de manera local en tu computadora, la "nube" actúa como un servidor centralizado al que múltiples desarrolladores pueden conectarse. Esto facilita la colaboración en equipo, la copia de seguridad (backup) del código fuente, la revisión de cambios (pull/merge requests), la gestión de tareas (issues) y la automatización de procesos de integración y despliegue continuo (CI/CD). *

* Alternativas en el mercado (Plataformas de alojamiento Git)
* Además de GitHub, existen otras plataformas líderes en la industria que ofrecen servicios similares con diferentes enfoques y características: *

*GitLab*

* Características principales: Es una plataforma completa que destaca por integrar de forma nativa potentes herramientas de CI/CD (Integración y Despliegue Continuo), gestión de proyectos, escaneo de seguridad y control de calidad de código directamente en su interfaz. *

* Modelo: Ofrece versión gratuita en la nube, planes de pago empresariales y la opción de autoalojamiento (self-hosted) en servidores propios. *

*Bitbucket*

* Características principales: Desarrollado por Atlassian, está optimizado para integrarse de manera fluida con otras herramientas del mismo ecosistema corporativo, como Jira (para gestión de proyectos ágiles) y Confluence. *

* Modelo: Muy popular en entornos empresariales y corporativos que ya utilizan productos de Atlassian. Ofrece repositorios privados gratuitos para equipos pequeños. * 

*Gitea (o Forgejo)*

* Características principales: Es una solución de código abierto (open-source) de peso ligero, diseñada para ser autohospedada. Es sumamente rápida, consume pocos recursos de hardware y ofrece una experiencia muy similar a GitHub pero bajo control total del usuario o la empresa. *

* Modelo: Gratuito y de código abierto para quienes prefieren alojar sus propios servidores de Git en lugar de depender de grandes nubes comerciales.*

*4*
### Glosario básico de Git

*Commit*

* Definición: Es una instantánea o punto de control (checkpoint) que guarda el estado actual de los archivos en el repositorio local. Cada commit incluye un identificador único, un mensaje descriptivo y registra exactamente qué cambios se hicieron.

* Ejemplo práctico: Después de escribir la estructura inicial de una página de inicio (index.html), ejecutas git commit -m "feat: agregar estructura HTML inicial" para congelar y guardar ese progreso de forma permanente en el historial.*

*Branch (Rama)*

* Definición: Es una línea de desarrollo independiente que te permite trabajar en nuevas funcionalidades, correcciones o experimentos sin alterar el código principal o estable del proyecto (que suele llamarse main o master).

* Ejemplo práctico: Para desarrollar un módulo de inicio de sesión sin romper la aplicación actual que ya funciona, creas y te cambias a una nueva rama ejecutando git checkout -b feature/login.*

*Merge (Fusión)*

* Definición: Es el proceso de combinar el historial y los cambios realizados en una rama (por ejemplo, una rama de características) con otra rama principal (como main), integrando todo el trabajo nuevo.

* Ejemplo práctico: Una vez que terminaste y probaste el módulo de inicio de sesión en tu rama feature/login, te pasas a main y ejecutas git merge feature/login para incorporar todo ese código nuevo al proyecto principal.*

*Pull y Push*

* Definición: Son los comandos fundamentales para sincronizar tu repositorio local con un repositorio remoto en la nube (como GitHub):*

* Push: Envía tus commits locales hacia el servidor remoto para compartirlos o respaldarlos.

* Pull: Descarga y fusiona automáticamente los últimos cambios del servidor remoto hacia tu computadora.

* Ejemplo práctico: Al terminar tu jornada laboral, ejecutas git push origin main para subir tus avances a GitHub. Al día siguiente, antes de empezar a programar de nuevo, ejecutas git pull origin main para asegurarte de tener la versión más actualizada que subieron tus compañeros.*

*Pull Request (PR)*

* Definición: Es una solicitud formal en una plataforma web (como GitHub) para avisar al equipo que has terminado una rama de trabajo y que propones fusionarla (merge) en la rama principal. Permite revisar el código, hacer comentarios y discutir cambios antes de integrarlos.

* Ejemplo práctico: Subes tu rama de la pasarela de pagos a GitHub y abres un Pull Request titulado "Añadir pasarela de pagos" para que el líder del equipo o tus compañeros revisen las líneas de código antes de autorizar su pase a producción.*

*Clone (Clonar)*

* Definición: Es la acción de descargar una copia completa y exacta de un repositorio remoto existente (con todo su historial de versiones y ramas) desde la nube hacia tu computadora por primera vez.

* Ejemplo práctico: Cuando un compañero te comparte el enlace de un proyecto nuevo en GitHub, abres tu terminal y escribes git clone [https://github.com/usuario/proyecto.git](https://github.com/usuario/proyecto.git) para descargarlo y empezar a trabajar inmediatamente en tu máquina.*

*Upstream (y su diferencia con Origin)*

* Definición:

* Origin: Es el alias predeterminado que Git le asigna al repositorio remoto original del cual clonaste tu proyecto.

* Upstream: Es el alias que comúnmente se le asigna al repositorio remoto principal u oficial (el de la organización o autor original) cuando estás colaborando en proyectos ajenos mediante un fork, sirviendo como referencia para sincronizar las actualizaciones globales.

* Ejemplo práctico: Si haces un fork del repositorio de una empresa, tu repositorio personal en GitHub se convierte en origin, mientras que el repositorio oficial de la empresa de donde sacaste la copia se configura como upstream para poder jalar (pull) las actualizaciones generales que vayan lanzando.*

*5*
# La importancia de las ramas (*Branches*)

En Git, una **rama** (*branch*) es esencialmente un apuntador móvil hacia un *commit* específico. Representa una línea de desarrollo independiente dentro de un repositorio. En lugar de trabajar directamente sobre la versión principal y estable del código, las ramas permiten aislar cambios, experimentar y desarrollar nuevas funcionalidades de forma segura.

---

### ¿Para qué sirven las ramas?

Las ramas sirven para fragmentar el flujo de trabajo en partes manejables y seguras. Sus aplicaciones principales incluyen:

* **Aislamiento de código:** Permiten escribir código nuevo, probar soluciones o realizar experimentos sin alterar el funcionamiento del sistema actual.
* **Desarrollo en paralelo:** Hacen posible que múltiples características, mejoras o correcciones se programen simultáneamente en el mismo proyecto sin que interfieran entre sí.
* **Gestión de versiones y estabilidad:** Permiten mantener una versión de producción limpia y estable mientras el equipo implementa cambios profundos en entornos separados.

---

### Ventajas en el trabajo individual y en equipo

El uso de ramas ofrece beneficios clave tanto si se programa en solitario como en un equipo de desarrollo:

#### 1. En el trabajo individual

* **Experimentación sin miedo:** Si una solución experimental o un bloque de código falla por completo, puedes simplemente descartar la rama sin dañar el progreso anterior que ya funcionaba.
* **Organización por tareas:** Permite estructurar el desarrollo enfocando cada rama en un objetivo específico (por ejemplo, una rama para la interfaz, otra para la conexión a la base de datos).

#### 2. En el trabajo en equipo

* **Colaboración sin sobreescrituras:** Cada miembro del equipo puede trabajar en su propia rama (*feature branches*) de manera independiente, evitando alterar o romper el trabajo de sus compañeros.
* **Revisiones de código estructuradas (*Pull Requests*):** Facilita que el equipo revise, discuta y pruebe el código de una rama antes de fusionarlo (*merge*) al repositorio principal, garantizando altos estándares de calidad.

*6*
# ¿Qué es GitFlow?

**GitFlow** es un modelo de flujo de trabajo (*workflow*) para Git, propuesto por Vincent Driessen en 2010. Define una estructura estricta de ramificación diseñada alrededor del ciclo de liberación (*release*) del software. Su objetivo principal es organizar y estructurar proyectos que tienen un ciclo de lanzamiento programado, separando claramente el código en desarrollo del código que ya está en producción.

### Estructura de sus ramas principales

El modelo se basa en dos ramas principales de larga duración y tres ramas auxiliares de vida corta:

1. **`master` (o `main`)**
* **Función:** Contiene el código oficial que está listo para producción. Cada cambio en esta rama representa una versión o lanzamiento oficial estable que ya está disponible para los usuarios finales.


2. **`develop`**
* **Función:** Es la rama de integración principal. Contiene todo el código nuevo que se ha completado para la próxima versión y sirve como base para construir las nuevas funcionalidades.


3. **`feature` (Ramas de características)**
* **Función:** Se crean a partir de `develop` para desarrollar nuevas funcionalidades de manera aislada (por ejemplo, `feature/login` o `feature/carrito`). Una vez terminadas, se fusionan (*merge*) nuevamente en `develop`.


4. **`release` (Ramas de lanzamiento)**
* **Función:** Permiten preparar una nueva versión para producción. Se ramifican desde `develop` cuando este ya incluye todas las características del nuevo lanzamiento. En esta fase se realizan correcciones de errores menores y ajustes de última hora antes de pasar a producción. Al finalizar, se fusionan tanto en `master` como en `develop`.


5. **`hotfix` (Ramas de corrección urgente)**
* **Función:** Se utilizan para solucionar errores críticos descubiertos en producción (*master*) de forma inmediata. Se ramifican directamente desde `master` y, una vez solucionado el problema, se fusionan tanto en `master` como en `develop` para asegurar que el error quede resuelto en todo el ciclo.