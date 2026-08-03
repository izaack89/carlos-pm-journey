# Planeación adaptativa — Lección 5: Monitoreo y evaluación

> PDF: [[documentation/01. Planeacion adaptativa/Planeación adaptativa_Lección 5_versión_impresa.pdf|Ver PDF original]]

Versión impresa de la Lección 5, que cubre el monitoreo y evaluación del proyecto: seguimiento del avance, artefactos, análisis de riesgos, riesgos del equipo, comunicación efectiva y beneficios del trabajo en equipo.

---

## Introducción

La problemática principal en el seguimiento de un proyecto radica en:

- Existe resistencia a realizar una planificación y estimación del esfuerzo requerido
- El porcentaje de avance basado en tiempo **no refleja la realidad** y no considera el valor generado
- El concepto de la línea base se percibe rígido y no se utiliza
- Los proyectos tienen muchas incidencias → el control de cambios resulta complicado y burocrático
- Se pierde la visibilidad de las incidencias cuando se documentan en minutas
- Difícilmente se da seguimiento a los riesgos

El paradigma de que un **proyecto exitoso** es el que completa su alcance dentro del tiempo y presupuesto ha quedado en el pasado. El principal propósito actual es **generar valor a la organización**.

El monitoreo y control debe enfocarse en asegurar que se están cumpliendo los **objetivos establecidos** y que se está obteniendo un **beneficio cuantificable**, mediante la **inspección y comparación del progreso** para establecer y adaptar la cadencia con base en la experiencia y la retroalimentación.

---

## Importancia del seguimiento del avance de un proyecto

En **prácticas ágiles**, solamente las historias de usuario que están **completamente terminadas** se consideran como parte del avance de la iteración. Hasta que una HU es totalmente finalizada y **aceptada por el Product Owner**, es cuando realmente agrega valor al proyecto.

Mientras las HU se encuentren en las columnas "Por hacer" o "En progreso" del **tablero Kanban**, realmente no han agregado valor.

### Definición de hecho

Cuando la HU se finaliza, el equipo de desarrollo en conjunto con el PO verifica la **"Definición de hecho"** (*Definition of Done*) — los **criterios de aceptación** han sido totalmente satisfechos y el objetivo fue cumplido. Si no es así, el resultado será rechazado y el equipo deberá realizar los ajustes correspondientes o regresar la HU al backlog para otra iteración.

En proyectos ágiles se utilizan diferentes **artefactos para medir el avance del trabajo**, mantener visibilidad de los acuerdos y pendientes, y ajustar constantemente el plan de desarrollo.

Ver también: [[notes/01. Planeacion adaptativa/Artefactos para el seguimiento del avance de un proyecto|Artefactos para el seguimiento del avance de un proyecto]]

---

## Análisis de riesgos

Un **riesgo** es un evento que puede o no suceder, pero que si sucede, tendrá un **impacto negativo o positivo** en el proyecto.

- Cuando existe la **certeza** de que algo pasará → es un **problema**, no un riesgo
- Existen **riesgos negativos** (amenazas) y **riesgos positivos** (oportunidades)
- Los riesgos **no deben usarse como excusas** para justificar una mala gestión

### Proceso de gestión de riesgos

El proceso se realiza de manera **constante** durante todo el ciclo de vida del proyecto:

#### 1. Identificación de riesgos

Participan todos los roles involucrados. El líder ágil debe mantener un **registro y seguimiento** de cada riesgo.

**Redacción de riesgos** — tres elementos para asegurar que efectivamente se trata de un riesgo:

- **Debido a…** (causa)
- **Es posible que…** (el riesgo)
- **Ocasionando…** (impacto)

**Ejemplo:** *"Debido a que la existencia de tóner está disminuyendo, las impresoras pueden dejar de funcionar ocasionando disgustos en los usuarios"* → causa muy ambigua. Mejor: *"Debido a que el proveedor está fallando en las entregas oportunas, es posible que el abasto de tóner se vea afectado ocasionando que no se puedan cubrir la necesidad de todas las impresoras"* → ahora se puede pensar en acciones (buscar otro proveedor).

#### 2. Evaluación de riesgos

Para cada riesgo se establece:
- Un **valor numérico de impacto** (escala del 2 al 8: Bajo, Medio, Alto, Muy alto)
- Un **porcentaje de probabilidad** de ocurrencia (10% a 90%)
- **Calificación** = Impacto × Probabilidad

| | Bajo (2) | Medio (4) | Alto (6) | Muy alto (8) |
|---|---|---|---|---|
| **90%** | 1.8 | 3.6 | 5.4 | 7.2 |
| **70%** | 1.4 | 2.8 | 4.2 | 5.6 |
| **50%** | 1 | 2 | 3 | 4 |
| **30%** | 0.6 | 1.2 | 1.8 | 2.4 |
| **10%** | 0.2 | 0.4 | 0.6 | 0.8 |

- Riesgos en **zonas oscuras** (calificación alta) → determinar un **plan de respuesta**
- Riesgos en **zona clara** → solo **monitorear**

#### 3. Definición de un plan de respuesta a riesgos

Para riesgos con impacto significativo: definir un **plan de acción** para evitar, transferir o reducir la probabilidad o consecuencias de una amenaza, o aprovechar, intensificar o compartir una oportunidad.

- El plan de respuesta se convierte en una **historia de usuario** que se adiciona al **backlog**, normalmente con **prioridad alta**
- **Ventaja de la planificación adaptativa:** los planes de respuesta a riesgos se integran al backlog mediante el refinamiento y se manejan de manera constante entre iteraciones

---

## Riesgos que amenazan el cumplimiento del compromiso del equipo

Estos riesgos amenazan la capacidad del equipo de alcanzar logros de manera temprana y mantener una **cadencia de desempeño estable**.

### 1. Multitasking

Trabajar al mismo tiempo en varias tareas → **baja en la productividad**.

**Solución:** **Limitar el WIP** en el tablero Kanban — establecer un máximo de elementos en la columna "En progreso". Mientras no salga una tarea, no puede ingresar otra.

### 2. Ley de Parkinson

El trabajo se expande hasta llenar el **tiempo disponible** para realizarlo. Más tiempo disponible → menor esfuerzo → mayor propensión a perder el tiempo.

**Solución:** Mantener el **sentido de urgencia** en las reuniones diarias, motivar a terminar tareas lo antes posible para iniciar otras o **apoyar a compañeros**.

### 3. Procrastinación

Hábito de **postergar tareas** y dedicarse a actividades más agradables pero menos relevantes. Causas: falta de motivación, carencia de habilidades o falta de interés.

**Estrategias:**
- **Establecer metas realistas** — estimaciones adecuadas que motiven
- **Solicitar ayuda** — apoyarse en compañeros con mayor experiencia
- **Tomar descansos regulares** — 10-15 min cada 2 horas para mantener energía
- **Lidiar con ansiedad y estrés** — dar tiempo para atender situaciones personales

### Autoselección de tareas

En lugar de asignar tareas, permitir que cada miembro **seleccione del backlog de la iteración** las tareas que realizará (por habilidad o experiencia). También es válido el trabajo en parejas (**Pair programming** de XP).

---

## La comunicación en los equipos de trabajo

La **comunicación** debe fluir de manera **constante y efectiva** entre todos los *stakeholders* (incluyendo el equipo de desarrollo).

### Características de la comunicación

- **Comunicación constante** — No esperar a una junta periódica; resolver necesidades y obstáculos lo antes posible
- **Comunicación abierta** — Todos deben sentirse cómodos de exponer puntos de vista, preocupaciones y opiniones sin temor a críticas
- **Comunicación clara** — Ayudar a los miembros del equipo a aclarar ideas antes de exponerlas

La **mejor forma de comunicación es cara a cara** — la asistencia de *stakeholders* clave a las reuniones de revisión es fundamental.

El cliente o PO deben estar **informados sobre el progreso** en todo momento y **mantenerse involucrados** durante todo el ciclo de vida para la toma de decisiones.

### Reuniones extraordinarias

No abstenerse de solicitar reuniones adicionales cuando exista necesidad de aclarar HU en desarrollo o proponer maneras diferentes de realizar el trabajo.

### Documentación y control de acuerdos

Para evitar que acuerdos y pendientes se olviden, documentarlos en un **archivo de seguimiento** (Excel) con las columnas:

| Campo | Descripción |
|-------|-------------|
| **ID** | Consecutivo para identificar el acuerdo/pendiente/problema |
| **Descripción** | Descripción clara del tema |
| **Tipo** | Acuerdo, pendiente o problema |
| **Fecha** | Fecha en que se identifica |
| **Solicitado por** | Persona que solicita o autoriza |
| **Asignado a** | Persona responsable de resolverlo |
| **Fecha compromiso** | Fecha esperada de resolución |
| **Fecha de cierre** | Fecha real de cumplimiento |
| **Estatus** | Para filtros e información relevante |
| **Comentarios** | Seguimiento con fechas de actualización |

El archivo debe estar disponible en un **repositorio accesible** para todo el equipo.

---

## Técnicas de comunicación efectiva

La comunicación efectiva consiste en **transmitir mensajes de manera clara y entendible** para el receptor. Cada persona interpreta diferente debido a su cultura, desarrollo y personalidad.

### 7 técnicas

1. **Practica la empatía** — Entender que todos tienen diferentes reacciones; genera un clima positivo para el entendimiento y la confianza
2. **Mira directamente a los ojos** — El contacto visual genera confianza; evitarlo se interpreta como falta de seguridad o sinceridad
3. **Utiliza lenguaje corporal** — Gestos y movimientos son herramientas para reforzar los mensajes
4. **Ocasionalmente utiliza cumplidos** — Frases de aprobación mejoran la empatía y confianza
5. **Emplea el lenguaje de acuerdo con el contexto** — Adaptar el lenguaje a la audiencia (director, equipo, cliente)
6. **Cuida el tono de voz** — Crea el ambiente adecuado, enfatiza lo importante, haz pausas para asimilar
7. **Escucha de manera activa** — Parafrasear y hacer preguntas de confirmación para comprender mejor el mensaje
8. **Respeta los turnos** — No interrumpir a media frase; hablar uno a la vez

Ver también: [[notes/01. Planeacion adaptativa/Técnicas de comunicación efectiva|Técnicas de comunicación efectiva]]

---

## Beneficios del trabajo en equipo

El trabajo en equipo es parte fundamental del desarrollo de un proyecto ágil. Mejora el **rendimiento, las actitudes** y genera **lealtad al proyecto**. A nivel individual, genera **seguridad, autoestima** y **sentido de pertenencia**.

| Beneficio | Descripción |
|-----------|-------------|
| **Colaboración** | Resolver problemas entre dos o más personas mejora fortalezas individuales y conduce a soluciones creativas e innovadoras |
| **Comunicación** | La comunicación se vuelve clara y efectiva entre integrantes; alineados con los objetivos, la posibilidad de éxito se intensifica |
| **Flexibilidad** | Retroalimentación y puntos de vista diversos permiten respuesta más rápida a los cambios |
| **Responsabilidad** | Compartir la responsabilidad y el compromiso genera mayor motivación e iniciativa |
| **Eficiencia** | Tareas se pueden dividir y trabajar en paralelo para completar más trabajo en menos tiempo |
| **Calidad** | Compartir conocimientos y habilidades fomenta buenas prácticas y mejora la calidad del producto final |

Se requieren **verdaderos equipos de trabajo** con alta integración — **equipos de alto rendimiento**.

Ver también: [[notes/01. Planeacion adaptativa/Beneficios del trabajo en equipo|Beneficios del trabajo en equipo]]

---

## Ideas para llevar

- En un proyecto ágil no se reporta porcentaje de avance — las HU **finalizadas y aceptadas por el PO** son las que aportan valor
- El **tablero Kanban** muestra el estado de las HU/tareas (por hacer, en proceso, terminado); conviene **limitar el WIP**
- Los **riesgos** están siempre presentes (amenazas y oportunidades); no deben usarse como pretexto
- Los **planes de respuesta** a riesgos se convierten en HU con prioridad alta en el backlog
- Riesgos del equipo: **multitasking, Ley de Parkinson y procrastinación**
- Desarrollar **técnicas de comunicación efectiva**: escucha activa, contacto visual, cumplidos, respetar turnos

---

## Bibliografía

- Atlassian. (2023). *App Trello*.
- Buchtik, L. (2012). *Secretos para Dominar la Gestión de Riesgos en Proyectos*. Editorial Buchtik global.
- Gillis, A. (2021). *What is pair programming?* TechTarget.
- La información. (2019). *Este es el tiempo que gastas buscando las cosas que "pierdes" en tu propia casa*.
- Mulcahy, R. (2019). *Risk Management. Tricks of the Trade® for Project Managers*. 3a edición. RMC Publications.
- Project Management Institute. (2022). *PMI Risk Management Professional (PMI-RMP)®*.
- Romanukha, A. (2021). *Stop Starting, Start Finishing with Agile*. Readwrite.
