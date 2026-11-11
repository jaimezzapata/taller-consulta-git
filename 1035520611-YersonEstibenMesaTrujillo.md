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
