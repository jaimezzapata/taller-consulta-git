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

