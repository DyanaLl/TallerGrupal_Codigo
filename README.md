# 🚀 Taller Autónomo - Operación Código Legacy

**Integrantes:**

**Diana Llivipuma*

**Sumak Jami*

---

## Fase 1: Ingeniería Inversa y Documentación

### 1. ¿Qué problema resuelve esta aplicación?
Es un módulo de validación del proceso de matrícula de la carrera de Desarrollo de Software.

Su objetivo principal es determinar si un estudiante es apto o no para matricularse en la materia y el estudiante pueda acceder a **Estructuras de Datos**, verificando que cumpla con los requisitos requeridos. Esto es obligatorio, ya que debe haber cursado y aprobado la materia de **Fundamentos de Programación** con una nota mínima de **7.0**.

---

### 2. Descripción del Flujo de Datos
El sistema opera de manera secuencial mediante los siguientes pasos principales:

1. **Ingreso de Datos Iniciales:**
   - Solicitar en nombre del estudiante ('usr')
   - Preguntar si el estudiante es de reingreso o arrastre ('S/N')
2. **Evaluación de Historial Académico:**
   - **Si el estudiante es de reingreso ("S"):** El programa registra en su historial ('h_materias') la materia *Fundamentos de Programación* y solicita la nota final obtenida ('n1'), convirtiéndola a un valor numérico ('double').
   - **Si el estudiante es nuevo ("N"):** Se muestra un mensaje indicando que se registra como estudiante de Primer Semestre y no se asigna ninguna materia a su historial (`h_materias` permanece como `null`).
3. **Solicitud de Materia Destino:**
   - Muestra la materia a solicitar (*Estructuras de Datos*) y consulta si desea solicitar el cupo (`S/N`).
4. **Verificación de Prerrequisitos y Reglas de Negocio:**
   - Si el estudiante confirma ("S"), el sistema recorre el historial del estudiante para verificar si ya cursó *Fundamentos de Programación*, mediante una estructura condicional ('swith'), que valida la situación:
   - **Si cursó y aprobó el prerrequisito con nota de 10.0:** Se aprueba la matrícula y se otorga automáticamente la distinción especial con el mensaje destacado para ser *Tutor de Programación del PUCE TEC*.
     - **Si cursó el prerrequisito con nota >= 7.0 (y menor a 10):** Se aprueba exitosamente la matrícula.
     - **Si la nota es menor a 7.0:** La matrícula es rechazada por no alcanzar la nota mínima requerida.
     - **Si no cursó la materia:** La matrícula es rechazada por no contar con el prerrequisito registrado en su historial.
5. **Salida:** Imprime en la consola el resultado final del proceso de matrícula y finaliza la ejecución liberando el recurso del lector (`Scanner`).
