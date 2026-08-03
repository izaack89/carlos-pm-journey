# Práctica — Una planeación adaptativa y exitosa en Secufin

> PDF: [[documentation/01. Planeacion adaptativa/Práctica.pdf|Ver PDF original]]

Manual de ejercicios interactivo donde se aplica lo aprendido sobre Planeación adaptativa a través de 4 misiones con el caso de *Secufin*, una startup que desarrolla una aplicación móvil de finanzas personales.

---

## Contexto del caso

**Claudia**, líder ágil especializada en planificación adaptativa, ayuda a **Secufin** — una startup con presupuesto limitado que quiere lanzar una app de finanzas personales dirigida a clase media. El equipo incluye a **Esteban** (socio experto en finanzas), **Bertha** (*Product Owner*) y un equipo de programadores.

---

## Misión 1 — Determinando los objetivos del proyecto, las iteraciones y los lanzamientos

**Propósito:** Dimensionamiento del proyecto y estimación inicial de iteraciones y lanzamientos.

### Ejercicio 1: Objetivos y requerimientos del proyecto
Identificar los aspectos necesarios para determinar los objetivos iniciales:

| Aspecto | ¿Necesario? |
|---------|:-----------:|
| Conocer con el mayor detalle posible los intereses de los stakeholders | No |
| Identificar a los clientes y obtener su visión del proyecto | **Sí** |
| Identificar la funcionalidad que el producto requiere para ser considerado completo | **Sí** |
| Estimar las tareas que se deben realizar para finalizar el producto | No |
| Tomar en cuenta a los stakeholders clave para determinar los objetivos | **Sí** |
| Tener una visión holística de los requisitos iniciales | **Sí** |
| Asignar el cumplimiento de cada objetivo a un miembro del equipo | No |
| Documentar los objetivos con la mayor claridad posible | **Sí** |

### Ejercicio 2: Épicas vs. Historias de Usuario

| Característica | Pertenece a |
|---------------|-------------|
| Criterio INVEST | Historia de usuario |
| Funcionalidades de alto nivel con amplio conjunto de requisitos | Épica |
| Redactadas en lenguaje sencillo desde el punto de vista del usuario | Ambas |
| Descompuestas en actividades por el equipo | Historia de usuario |
| Planificación a largo plazo | Épica |
| Priorizadas en el backlog del producto | Ambas |
| Seleccionadas para el backlog de la iteración | Historia de usuario |
| Descripción de funcionalidad específica | Historia de usuario |
| Dimensionadas con Story points / Planning Poker | Historia de usuario |
| Dimensionadas con talla de camiseta | Épica |

### Ejercicio 3: Estimación de iteraciones y lanzamientos

- **Incorrecto:** Las estimaciones deben ser exactas.
- **Correcto:** Los story points expresan estimación de esfuerzo, no duración.
- **Correcto:** Story points para HU, tallas de camiseta para épicas.
- **Incorrecto:** El Planning Poker se usa para estimar épicas (realmente es para HU).
- **Correcto:** Al planificar una iteración, los story points se dividen en actividades.
- **Correcto:** En Planning Poker sin consenso, escuchar argumentos extremos.
- **Correcto:** Tallas de camiseta evitan percepción de precisión.
- **Incorrecto:** Una épica estimada debe desagregarse inmediatamente en actividades.
- **Incorrecto:** El PO es el principal responsable de estimar (es el equipo de desarrollo).
- **Correcto:** La estimación no representa tiempo de desarrollo.

---

## Misión 2 — Establecer el MVP, identificar tareas y reuniones

**Propósito:** Establecer el MVP, identificar tareas y realizar reuniones de revisión y retrospectiva.

### Ejercicio 1: Importancia del MVP (MoSCoW)

| Categoría | Historias de usuario |
|-----------|---------------------|
| **Must have** | Registro seguro, Registrar/categorizar ingresos y gastos, Reporte mensual categorizado, Metas de ahorro |
| **Should have** | Presupuesto personalizado, Sincronizar tarjetas/cuentas, Notificaciones de vencimiento de pagos |
| **Could have** | Herramientas de análisis financiero, Exportar información, Informes de rendimiento de inversiones |
| **Won't have** | Crear y gestionar varios perfiles |

El MVP incluye las HU clasificadas como **Must have**.

### Ejercicio 2: Técnica SMART para tareas

| Planteamiento | Elemento SMART |
|--------------|----------------|
| Alineado al objetivo de la HU, no programar tareas sin valor | **Relevant** |
| Establecer fecha objetivo de finalización | **Time boxed** |
| Claro lo que se quiere lograr, evitar ambigüedades | **Specific** |
| Esfuerzo realista, ni estrecho ni holgado | **Attainable** |
| Criterios para medir avance y finalización | **Measurable** |

### Ejercicio 3: Tipos de reunión

| Actividad | Tipo de reunión |
|-----------|----------------|
| Evaluar si se alcanzaron los objetivos de la iteración | Revisión |
| Analizar problemas y obstáculos de la iteración | Retrospectiva |
| Determinar las tareas de la iteración | Planificación |
| Reportar avances e impedimentos | Diaria de seguimiento |
| Analizar qué se hizo bien/mal y mejoras | Retrospectiva |
| Analizar objetivos de HU para la siguiente iteración | Planificación |
| De pie, máximo 15 minutos | Diaria de seguimiento |
| Mostrar funcionalidades al cliente | Revisión |

---

## Misión 3 — Control de la realización del trabajo

**Propósito:** Seguimiento al trabajo, validación de valor y uso de artefactos de control.

### Ejercicio 1: Validación de objetivos

| Planteamiento | ¿Aporta valor? |
|--------------|:--------------:|
| PO y stakeholders satisfechos con la funcionalidad | **Sí** |
| Equipo dedicó más horas de las estimadas | No |
| Iteración completada antes sin validación del cliente | No |
| Requisitos de cada HU completados | **Sí** |
| Métricas/KPIs cumplidos y HU aceptadas por PO | **Sí** |

### Cumulative Flow Diagram

| Concepto | Significado |
|----------|-------------|
| **Cycle time** | Tiempo desde inicio hasta finalización de una tarea |
| **Done** | Trabajo ya realizado en un momento dado |
| **To do** | Trabajo pendiente por realizar |
| **WIP** | Cantidad de trabajo en desarrollo |

### Ejercicio 2: Análisis de riesgos

| Situación | ¿Es riesgo? |
|-----------|:-----------:|
| Ataques cibernéticos que afecten finanzas de usuarios | **Sí** |
| No atender solicitudes de adecuación de usuarios | No |
| Cambios en regulaciones financieras por entorno VUCA | **Sí** |
| Equipo no entienda funcionalidad de las HU | No |
| Errores en cálculos que afecten información al usuario | **Sí** |

### Ejercicio 3: Comunicación con stakeholders

| Objetivo | Habilidad |
|----------|-----------|
| Generar confianza, evitar sensación de insinceridad | Mirar directamente a los ojos |
| Enfatizar aspectos importantes del mensaje | Cuidar el tono de voz |
| Gestos y movimientos refuerzan los mensajes | Utilizar lenguaje corporal |
| Parafrasear y confirmar para comprender mejor | Escucha activa |
| Generar clima positivo y confianza | Empatía |
| Frases de aprobación para mejorar confianza | Utilizar cumplidos |
| No interrumpir a media frase | Respetar los turnos |

---

## Misión 4 — Ajuste del backlog y determinación del MVI

**Propósito:** Ajustar prioridades del backlog integrando riesgos, sugerencias de usuarios y nuevas HU.

### Ejercicio 1: Proceso de ajuste del backlog

1. **Realizar análisis del backlog actual** — Identificar la razón del ajuste y qué se pretende lograr
2. **Identificar HU a ajustar** — Basándose en información recopilada y objetivos
3. **Priorizar las HU** — Usando técnicas como MoSCoW
4. **Revisar el feedback de los usuarios** — Comentarios y retroalimentación
5. **Estimar el esfuerzo requerido** — Story points o tallas de camiseta
6. **Actualizar el backlog** — Modificar, agregar o eliminar HU con estimación y criterios de aceptación

### Ejercicio 2: Determinación del MVI con Modelo Kano

| Requerimiento | Categoría Kano | ¿Incluir en MVI? |
|--------------|----------------|:-----------------:|
| Educación financiera | Indiferente | No |
| Notificaciones inteligentes | Excitador | **Sí** |
| Metas y seguimiento de ahorros | Desempeño | **Sí** |

### Ejercicio 3: Lecciones aprendidas

| Planteamiento | ¿Es beneficio? |
|--------------|:--------------:|
| Cultura de colaboración y aprendizaje | **Sí** |
| Evitar que ocurran riesgos en futuros proyectos | No |
| Evitar cometer errores en futuros proyectos | **Sí** |
| Mejorar la eficiencia en el desempeño del equipo | **Sí** |
| Asegurar mejor actitud de los stakeholders | No |
| Fomentar el aprendizaje organizacional | **Sí** |
| Evitar planificación detallada en futuros proyectos | No |
| Identificar buenas prácticas para proyectos posteriores | **Sí** |
