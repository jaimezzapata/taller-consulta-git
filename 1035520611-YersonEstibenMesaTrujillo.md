Respuesta pregunta 1: 
Git es un **sistema de control de versiones distribuido** creado por Linus Torvalds en 2005. Su función principal es registrar y gestionar todos los cambios realizados en el código fuente de un proyecto a lo largo del tiempo.

El problema fundamental que resuelve es el **caos en la colaboración y el historial de desarrollo**. Antes de sistemas como Git, los desarrolladores solían trabajar copiando carpetas enteras (con nombres como `proyecto_final_v1`, `proyecto_final_definitivo`, `proyecto_copia_juan`), lo que provocaba:

* **Pérdida de código:** Sobrescribir por accidente el trabajo de un compañero.
* **Falta de historial:** No saber quién modificó qué línea, cuándo y por qué motivo.
* **Bloqueos en equipo:** No poder trabajar varias personas en la misma funcionalidad simultáneamente sin pisarse los cambios.
* **Dificultad para experimentar:** Probar una nueva idea implicaba arriesgar el funcionamiento de la versión estable del software.

### ¿Cómo lo soluciona?

1. **Historial completo y local:** Cada desarrollador tiene una copia exacta del repositorio con todo su historial en su máquina, permitiendo trabajar sin conexión.
2. **Ramas (*Branches*):** Permiten crear entornos de trabajo aislados para desarrollar nuevas características o corregir errores sin afectar la versión principal.
3. **Fusión (*Merge*):** Facilita la integración segura del código desarrollado por diferentes personas, detectando y ayudando a resolver conflictos automáticamente cuando dos cambios se contraponen.

---

Respuesta pregunta 2:
**Git** es la herramienta fundamental: un sistema de control de versiones distribuido que se instala y funciona de forma local en tu ordenador. Su objetivo principal es resolver el caos en el desarrollo de software (como la pérdida de cambios, las versiones duplicadas o los conflictos al colaborar) registrando cada modificación realizada en el código y permitiendo trabajar en ramas independientes sin riesgo. Por su parte, **GitHub** es una plataforma web en la nube que utiliza el motor de Git para alojar repositorios en internet, ofreciendo una interfaz visual e herramientas de colaboración en equipo como Pull Requests, gestión de tareas y revisión de código. **Git es el motor de seguimiento que trabaja en tu equipo sin necesidad de internet, mientras que GitHub es el servicio en la nube donde compartes y sincronizas ese trabajo con otros desarrolladores.**

---

Respuesta pregunta 3: 
Una **nube de repositorios** (o servicio de alojamiento de código en la nube) es una plataforma web que almacena y centraliza repositorios de control de versiones (principalmente Git) en servidores remotos.

Su función principal es actuar como un punto de encuentro centralizado donde los desarrolladores pueden respaldar su código, colaborar de forma síncrona o asíncrona, revisar cambios mediante herramientas de revisión (*pull/merge requests*), gestionar tareas (*issues*) y automatizar flujos de trabajo de pruebas y despliegue (CI/CD).

---

### Principales alternativas en el mercado

Además de GitHub, existen otras plataformas muy potentes y ampliamente utilizadas en la industria del desarrollo de software:

1. **GitLab**
* **Características:** Es una de las alternativas más robustas. Destaca por ofrecer una plataforma de DevOps todo en uno muy integrada, destacando especialmente por sus potentes herramientas nativas de **Integración y Despliegue Continuo (CI/CD)**. Ofrece tanto planes en la nube como la opción de alojarlo en servidores propios (*self-hosted*).


2. **Bitbucket**
* **Características:** Desarrollado por **Atlassian**, es una plataforma muy popular en entornos empresariales porque se integra a la perfección con otras herramientas de la misma familia, como **Jira** (para gestión de proyectos ágiles) y Confluence.


3. **Azure DevOps**
* **Características:** La plataforma de Microsoft enfocada en el desarrollo de software empresarial. Ofrece repositorios Git privados gratuitos, tableros Kanban, gestión de pipelines de despliegue avanzados y una integración muy profunda con el ecosistema de herramientas de Microsoft y Visual Studio.

---

Respuesta pregunta 4: 

### 1. *Commit*

* **Definición:** Es la unidad básica de almacenamiento en Git. Funciona como una "fotografía" o un punto de control (*checkpoint*) que guarda de forma permanente el estado actual de tus archivos en el historial del repositorio. Cada commit incluye un mensaje descriptivo de lo que cambiaste.
* **Ejemplo práctico:** Modificas el archivo `index.html` para cambiar el título de tu página web y ejecutas `git commit -m "feat: actualizar titulo principal del sitio"`. Has creado un commit que sella ese cambio en el historial.

### 2. *Branch* (Rama)

* **Definición:** Es una línea de desarrollo independiente que te permite trabajar en una nueva funcionalidad, corrección o experimento sin alterar ni poner en riesgo el código principal (*main* o *master*).
* **Ejemplo práctico:** Estás creando una tienda online y quieres añadir una pasarela de pagos. En lugar de hacerlo directamente en la versión oficial, creas una rama llamada `feature/pasarela-pagos` para programarlo de forma aislada.

### 3. *Merge* (Fusión)

* **Definición:** Es el proceso de integrar los cambios de una rama en otra (por ejemplo, unir una rama de trabajo con la rama principal), combinando el historial y el código nuevo de forma automática o resolviendo posibles conflictos.
* **Ejemplo práctico:** Terminaste de programar la pasarela de pagos en tu rama `feature/pasarela-pagos`, te cambias a la rama `main` y ejecutas el comando de fusión (`git merge feature/pasarela-pagos`) para que la tienda oficial ahora incluya la nueva función.

### 4. *Pull* y *Push*

* **Definición:** Son los comandos para sincronizar tu repositorio local con uno remoto (como GitHub):
* ***Push* (Empujar):** Sube tus commits locales hacia el servidor remoto para compartirlos.
* ***Pull* (Jalar):** Descarga los últimos cambios del servidor remoto e inmediatamente los fusiona en tu repositorio local.


* **Ejemplo práctico:**
* Haces `git push origin main` para enviar los commits que hiciste en tu computadora a tu repositorio en GitHub.
* Un compañero subió cambios nuevos a GitHub; tú ejecutas `git pull origin main` para traer esos cambios a tu computadora y ponerte al día.


### 5. *Pull Request (PR)*

* **Definición:** Es una solicitud formal (muy común en plataformas como GitHub o GitLab) donde avisas al equipo que has terminado una rama y pides que revisen tu código antes de fusionarlo (*merge*) en la rama principal. Permite hacer comentarios, sugerencias y auditorías de calidad.
* **Ejemplo práctico:** Subes tu rama a GitHub y abres un Pull Request titulado *"Añadir carrito de compras"*. Tus compañeros de equipo revisan el código, aprueban los cambios en la interfaz web y finalmente se hace clic en "Merge" para integrarlo.

### 6. *Clone* (Clonar)

* **Definición:** Es la acción de descargar una copia completa y exacta de un repositorio remoto (con todo su historial, ramas y archivos) desde una plataforma en la nube hacia tu ordenador local por primera vez.
* **Ejemplo práctico:** Un amigo te comparte el enlace de un proyecto en GitHub. Abres tu terminal y escribes `git clone <url-del-repositorio>` para descargar todo el proyecto en tu computadora y empezar a trabajar en él inmediatamente.

### 7. *Upstream* vs. *Origin*

* **Definición:** Son nombres que se le dan a los repositorios remotos para identificarlos:
* ***Origin*:** Es el nombre predeterminado que le da Git al repositorio remoto personal desde el cual clonaste o al que subes tu propio código (tu copia en la nube).
* ***Upstream*:** Es el término que se suele usar para referirse al repositorio original o principal (generalmente el proyecto de otra persona u organización) del cual tú hiciste un *fork* o copia.


* **Ejemplo práctico:**
* Contribuyes a un proyecto de código abierto de una empresa. Tu propia copia en GitHub es `origin`. El repositorio oficial de la empresa donde descargas las actualizaciones generales es `upstream`.

---

Respuesta pregunta 5: 

Las **ramas (*branches*)** son una de las características más potentes y fundamentales de Git. Su propósito principal es permitirte trabajar en diferentes versiones de un proyecto de forma simultánea e independiente, sin alterar ni poner en riesgo la línea de desarrollo principal (generalmente llamada `main` o `master`).

### ¿Para qué sirven?

Sirven para aislar los cambios que realizas en el código. Imagina que la rama principal es como la estructura de una casa ya construida y habitable; crear una rama es como levantar una habitación en un plano separado para remodelarla o probar materiales nuevos antes de decidir si se integra definitivamente a la casa.

---

### Ventajas en el trabajo individual

* **Experimentación sin miedo:** Puedes probar librerías nuevas, refactorizar código o implementar lógica compleja sabiendo que, si algo sale mal o rompes la aplicación, puedes simplemente descartar la rama y tu versión estable seguirá intacta.
* **Organización por tareas:** Te permite mantener tu enfoque dividido por objetivos específicos (por ejemplo, una rama para el diseño estético de la página de inicio, otra para la conexión con la base de datos y otra para un arreglo rápido).

### Ventajas en el trabajo en equipo

* **Desarrollo simultáneo y sin bloqueos:** Varios desarrolladores pueden trabajar en el mismo proyecto al mismo tiempo sin pisarse el código ni sobrescribir el trabajo de los demás, ya que cada uno opera en su propia burbuja temporal (*rama*).
* **Protección de la rama principal (`main`):** Se establece la regla de oro de que `main` siempre debe contener código limpio, estable y listo para producción. Nadie programa directamente en ella.
* **Revisiones de calidad más seguras:** Al trabajar en ramas separadas, se facilita la creación de *Pull Requests* para que otros compañeros revisen, prueben y validen el código antes de fusionarlo (*merge*) con el proyecto oficial.

---