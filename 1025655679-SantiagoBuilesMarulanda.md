# Guia de Actividad: Dominando Git, Github y GitFlow

**Pregunta 1 respuesta**

## Git es un sistema de control de versiones distribuido, gratuito y de código abierto, Su propósito fundamental es registrar los cambios realizados en el código fuente de un proyecto a lo largo del tiempo, permitiendo que múltiples desarrolladores trabajen de forma ordenada, eficiente y simultánea.

* Git resuelve problemas como: *

## Elimina carpetas duplicadas tipo proyecto_v2_final.

## Evita que varios desarrolladores se borren trabajo al editar juntos.

## Permite probar funciones en ramas sin romper el código funcional.

## Permite regresar a cualquier versión anterior si algo falla.

## Registra quién hizo cada cambio, cuándo y por qué para tener trazabilidad total.

## Evita perder información al permitir trabajar y guardar cambios sin conexión a internet.

**Pregunta 2 respuesta**

# Diferencias Clave entre Git y GitHub

Aunque a menudo se mencionan juntos, **Git** y **GitHub** son herramientas completamente distintas que se complementan en el desarrollo de software.

* **Git** es la herramienta que rastrea y gestiona los cambios en tu código local.
* **GitHub** es la plataforma en la nube donde almacenas y compartes tus repositorios.

---

## 📊 Tabla Comparativa

| Característica | 🛠️ Git | ☁️ GitHub |
| :--- | :--- | :--- |
| **Naturaleza** | Sistema de control de versiones (software local). | Servicio de alojamiento en la nube (plataforma web). |
| **Ubicación** | Se ejecuta en tu computadora. | Se aloja en servidores remotos en internet. |
| **Interfaz** | Línea de comandos (terminal) o GUIs locales. | Interfaz web gráfica accesible desde el navegador. |
| **Conexión** | **No requiere internet** para trabajar offline. | **Requiere internet** para sincronizar y colaborar. |
| **Propósito** | Gestionar historiales, commits y ramas locales. | Centralizar código, colaborar, hacer *Pull Requests* e *Issues*. |

**Pregunta 3 respuesta**

## ☁️ ¿Qué es una Nube de Repositorios?

Una **nube de repositorios** es un servicio en línea que permite almacenar, respaldar y gestionar código fuente de manera remota mediante sistemas de control de versiones como Git. Funciona como un centro de operaciones donde los desarrolladores pueden respaldar sus proyectos, colaborar en equipo y gestionar tareas sin sobrescribir el trabajo de los demás.

### Alternativas a GitHub en el Mercado

1. **GitLab**
   * **Destacado:** Integra herramientas potentes de **CI/CD** (Integración y Despliegue Continuo) de forma nativa para automatizar pruebas y despliegues. Ofrece opciones tanto en la nube como para instalación en servidores propios (*self-hosted*).
2. **Bitbucket**
   * **Destacado:** Desarrollado por Atlassian, ofrece una **integración fluida con Jira y Trello**, lo que facilita la gestión de tareas en entornos corporativos.
3. **Azure DevOps**
   * **Destacado:** La solución de Microsoft orientada a empresas. Incluye tableros Kanban, pipelines avanzados y conexión directa con la nube de Azure.

**Pregunta 4 respuesta**

**Glosario Básico**

### 1. Commit
* **Definición:** Es como tomar una "fotografía" o un punto de control del estado actual de tu código. Guarda los cambios que has hecho con un mensaje descriptivo para que puedas volver a ese punto en el futuro si algo sale mal.
* **Ejemplo práctico:** Modificas el archivo `index.html` para agregar el título de tu página web y ejecutas `git commit -m "Añadir título principal a la página"`. Ese paquete de cambios queda guardado permanentemente en el historial de Git.

### 2. Branch (Rama)
* **Definición:** Es una línea de desarrollo independiente. Te permite trabajar en una nueva funcionalidad o corregir un error sin alterar el código principal (`main` o `master`). 
* **Ejemplo práctico:** Estás creando una tienda online que ya funciona bien en la rama `main`. Creas una rama llamada `rama-carrito-compras` (ej. `git checkout -b carrito`) para programar el botón de pago sin miedo a romper la página que ya está funcionando.

### 3. Merge (Fusión)
* **Definición:** Es el proceso de unir el trabajo de dos ramas diferentes. Por lo general, tomas los avances que hiciste en una rama secundaria y los integras en la rama principal.
* **Ejemplo práctico:** Terminaste de programar el carrito de compras en tu rama y todo funciona correctamente. Te cambias a la rama `main` y haces un `git merge carrito` para fusionar todo ese código nuevo con la versión oficial del proyecto.

### 4. Pull y Push
* **Definición:** Son los comandos para sincronizar tu computadora con el repositorio remoto en la nube (como GitHub).
    * **Push:** Envía tus *commits* locales hacia el servidor remoto para compartirlos o respaldarlos.
    * **Pull:** Descarga y fusiona automáticamente los cambios más recientes que otros desarrolladores hayan subido al servidor remoto hacia tu computadora.
* **Ejemplo práctico:** 
    * Terminas una función en tu laptop y escribes `git push origin main` para subirla a GitHub. 
    * Un compañero agregó cambios al repositorio en la nube, así que escribes `git pull` en tu terminal para traer esos cambios a tu computadora y actualizar tu código.

### 5. Pull Request (PR)
* **Definición:** Es una solicitud formal en una plataforma de alojamiento (como GitHub) para avisar al equipo que has terminado una rama y deseas fusionarla con la rama principal. Permite que otros revisen tu código antes de aceptarlo.
* **Ejemplo práctico:** Subiste tu rama con el sistema de inicio de sesión a GitHub. Como trabajas en equipo, abres un *Pull Request* para que tus compañeros puedan leer el código, dejar comentarios o aprobar los cambios antes de que pasen oficialmente al proyecto principal.

### 6. Clone (Clonar)
* **Definición:** Es la acción de descargar una copia completa y exacta de un repositorio remoto existente (con todo su historial de commits y ramas) por primera vez en tu computadora.
* **Ejemplo práctico:** Encuentras un proyecto interesante en GitHub y quieres probarlo o modificarlo localmente. Copias su enlace web y ejecutas `git clone <url-del-repositorio>` en tu terminal para descargarlo por completo en tu equipo.

### 7. Upstream vs. Origin
* **Definición:** Son nombres que se le asignan a los repositorios remotos para identificarlos:
    * **Origin:** Es el nombre predeterminado que le da Git al repositorio remoto **original de tu propiedad** (o tu propia copia bifurcada / *fork*) desde el cual clonaste o al que subes tus cambios directamente.
    * **Upstream:** Se suele utilizar para referirse al repositorio **original o principal** del proyecto (el de los creadores o dueños legítimos), especialmente cuando has hecho un *fork* y necesitas mantenerte sincronizado con sus actualizaciones oficiales.
* **Ejemplo práctico:** 
    * Haces un *fork* de una librería famosa de código abierto en tu propio GitHub; ese repositorio personal en tu cuenta se convierte en tu `origin`.
    * Configuras el repositorio oficial del creador original como `upstream` (ej. `git remote add upstream <url-original>`) para poder descargar las actualizaciones que ellos vayan lanzando y mantener tu proyecto al día.