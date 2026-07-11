# PUCEFundamentos01
## 🚀 Taller Autónomo - Operación Código Legacy

Bienvenidos a su primer reto de mantenimiento de software. En el mundo real, rara vez crearán sistemas desde cero; la mayor parte del tiempo heredarán código escrito por otras personas, a menudo sin documentación, con nombres confusos y errores ocultos.

Hoy asumen el rol de **Analistas de Desarrollo**. El departamento de TI del PUCE TEC les ha entregado el módulo beta de validación de matrículas escrito en Java 25. El programador anterior fue reasignado y dejó el trabajo a medias.

El sistema compila, pero tiene fallos estructurales graves. Su objetivo es entenderlo, arreglarlo y mejorarlo.

---

### Misión de la Semana (Trabajo en Grupos)

### Fase 1: Ingeniería Inversa
* **Clonen** este repositorio y creen una rama (`branch`) con el nombre de su grupo.
* **Lean** el código línea por línea. Usen herramientas de IA si lo necesitan, pero *solo para entender*, no para reescribir.
* **Expliquen** en el archivo `README.md` de forma clara y objetiva qué problema resuelve esta aplicación y describan el flujo de datos.

### Fase 2: Refactorización y Debugging
* **Nombres vagos:** El código está lleno de variables como `usr`, `m1`, `n1`, `p1`. Renómbrenlas usando las buenas prácticas de la industria para que el código sea legible.
* **El Bug Oculto:** Si ejecutan el programa y registran a un estudiante nuevo (que no es de reingreso), el sistema colapsa abruptamente al evaluar la materia destino. Encuentren la línea exacta que causa la excepción, entiendan por qué ocurre lógicamente y apliquen la solución en el código.

### Fase 3: Nueva Funcionalidad (Requerimiento del Cliente)
Dirección Académica ha solicitado un cambio urgente en la regla de negocio:

> Si un estudiante aprueba el prerrequisito con una calificación perfecta de **10.0**, el sistema no solo debe aprobar la matrícula, sino imprimir el siguiente mensaje destacado: *"¡Felicidades! Ha sido seleccionado como Tutor de Programación del PUCE TEC para este semestre."*

---

### Entregables Finales
* **Pull Request:** Suban sus cambios a GitHub y abran un *Pull Request* hacia el repositorio original. Se evaluará el historial de commits para validar el trabajo en equipo.
* **Video de Defensa Técnica (Máximo 3 minutos):** Incluyan el enlace al video en la descripción de su Pull Request. En la grabación deben demostrar la aplicación funcionando sin errores en la terminal, explicar dónde estaba el error oculto y cómo lo solucionaron, y mostrar el código refactorizado con la nueva funcionalidad implementada.
