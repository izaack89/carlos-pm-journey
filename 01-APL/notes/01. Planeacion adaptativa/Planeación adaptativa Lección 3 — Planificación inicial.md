# Planeación adaptativa — Lección 3: ¿Cómo realizar la planificación inicial?

> PDF: [[documentation/01. Planeacion adaptativa/Planeación adaptativa_Lección 3_versión_impresa.pdf|Ver PDF original]]

Versión impresa de la Lección 3, que cubre la planificación inicial del proyecto: alcance, documentación de HU con INVEST, dimensionamiento, estimaciones y roadmap.

---

## Introducción

La planificación inicial con enfoque de planeación adaptativa consiste en **convertir los objetivos del proyecto en una lista de trabajos** (el *backlog*) que se deben realizar para cumplirlos, generar valor y satisfacer las expectativas de los *stakeholders*.

Se debe traducir los objetivos a un **plan global** tomando en cuenta las capacidades del equipo para establecer una **visión preliminar del mapa de ruta** y un conjunto de hitos.

---

## Alcance de un proyecto

**Ejemplo práctico:** El papá de Abril compra un terreno y quiere construir una casa de campo. Abril (dueña del producto) contacta a un líder ágil. Los *stakeholders* son: Abril, su mamá, su papá, su hermano y su tía.

### Historias de Usuario de los stakeholders

| Stakeholder | ¿Quién quiere qué? | Ejemplo |
|-------------|-------------------|---------|
| El papá | Sistema de seguridad con comunicación a autoridades | Para vacacionar con confianza |
| La mamá y la tía | Cocina amplia y bien equipada | Para preparar comidas para familia y amigos |
| Hermano menor | Buen sistema de sonido | Para disfrutar reuniones con amigos |
| Abril | Lugar para karaoke y piscina | Para diversión y convivencia familiar |

### Stakeholders "dummy" (Personas)

En algunos proyectos se adicionan *stakeholders* ficticios para complementar requisitos no contemplados. Cada uno se documenta como **"Persona"** con:

| Dato | Descripción |
|------|-------------|
| **Nombre o alias** | Para identificar rápidamente al personaje |
| **Datos demográficos** | Para clasificarlo en un segmento de la sociedad |
| **Descripción** | Datos generales que ayuden a conocerlo mejor |
| **Objetivos** | Necesidades del usuario que lo distinguen de los demás |

---

## Documentación del alcance de un proyecto

Para documentar el alcance se utilizan **épicas e Historias de Usuario** — evitando documentación extensa. La redacción de HU es una declaración de **¿quién quiere qué?** y **¿por qué?**

- Redactar con **lenguaje sencillo** para facilitar la comprensión
- Incluir **criterios de aceptación** para verificar que los entregables se han realizado adecuadamente

Solo documentar HU que se consideren **alcanzables y viables** (que aporten valor). Durante el ciclo de vida del proyecto, la lista se irá **priorizando** en función de capacidades, presupuesto, tiempo y cambios.

Ver también: [[notes/01. Planeacion adaptativa/Documentación del alcance de un proyecto|Documentación del alcance de un proyecto]]

---

## Método INVEST (Bill Wake, 2003)

Para asegurar la calidad de las Historias de Usuario:

- **I — Independiente:** Cada HU debe ser independiente; si hay dependencias, combinarlas en una sola
- **N — Negociable:** Mientras esté en el backlog del producto, puede ser cambiada, priorizada o eliminada
- **V — Valiosa:** Debe describir un resultado que aporte valor al negocio
- **E — Estimable:** Debe poder ser estimada por el equipo en términos de tiempo, costo y esfuerzo
- **S — Small (Pequeña):** Tamaño que permita su desarrollo en pocas semanas/persona y en una sola iteración. Si es más grande, considerarla épica y subdividirla
- **T — Testable (Comprobable):** Debe contar con criterios de validación. Si el cliente no puede definirlos, cuestionar si realmente es valiosa

### Elementos de documentación de una HU

| Elemento | Descripción |
|----------|-------------|
| **Nombre de la HU** | Para su identificación |
| **Descripción** | **Como** [rol del usuario]… **Quiero** [objetivo]… **Para poder** [beneficio] |
| **Criterios de aceptación** | Bajo qué criterio el stakeholder se dará por satisfecho |

### Campos adicionales

ID, Prioridad, Predecesora, Puntos de historia, Asignada a, Área de valor, Comentarios.

---

## Dimensionamiento del proyecto

Es necesario **involucrar a los equipos de desarrollo** para evitar omisiones e identificar necesidades no funcionales. Muchas HU quedarán como **épicas** y se irán desglosando conforme avance el proyecto.

### Pasos de la planificación

1. **Identificar las dependencias** — Qué trabajo debe realizarse antes de otro (dependencias obligatorias y las establecidas por el PO). Usar el campo **"ID" de la predecesora**
2. **Agrupar las HU** por secuencia lógica — La primera iteración será la **iteración de planeación**. Las primeras HU deben llevarse al mayor detalle posible
3. **Estimación del dimensionamiento** — En términos de **"días ideales"** (horas/días/semanas a 8h diarias). Busca una visión preliminar del esfuerzo total

Durante este proceso, considerar la **identificación de riesgos** que pueden generar HU adicionales.

---

## Técnicas para la estimación

### 1. Story Points

Unidades de medida para estimar el **esfuerzo total** de implementar un elemento del backlog:
- Se asignan puntos por **cantidad de trabajo, complejidad y riesgo**
- Con el tiempo, se convierten en la referencia para comprender cuánto trabajo puede completar el equipo
- Generan **consenso y compromiso**

### 2. Planning Poker (Serie Fibonacci)

El tamaño puede ser lineal, pero la **complejidad e incertidumbre crecen exponencialmente** → se usa la serie Fibonacci (1, 2, 3, 5, 8, 13, 21, 34…).

**Cartas especiales:** 0 (sin relevancia), ∞ (imposible determinar), ? (desconocimiento), ☕ (pausa)

**Proceso:**
1. Elegir una HU de referencia (en la media)
2. Analizar la HU en equipo (máx. 3 minutos)
3. Todos muestran su carta simultáneamente
4. Si hay consenso → registrar resultado
5. Si hay disparidad → escuchar argumentos extremos → repetir
6. Sin consenso en segundo intento → registrar promedio o estimación del experto

### 3. Estimación por tallas de camiseta

Para **épicas** que no pueden estimarse con Planning Poker (marcadas con ∞). Enfoque más **intuitivo**, evita la percepción de precisión. Valores: **S, M, L, XL, XXL**.

Ver también: [[notes/01. Planeacion adaptativa/Técnicas para la estimación de un proyecto|Técnicas para la estimación de un proyecto]]

---

## Planificación del proyecto

La planificación con enfoque adaptativo consta de **tres niveles:**
1. **Planificación de la liberación**
2. **Planificación de la iteración**
3. **Planificación diaria**

### Planificación de la liberación

En la **Iteración "0"**, el PO, líder ágil y equipo visualizan las posibles **liberaciones** y el número de iteraciones que cada una requiere. Cada liberación representa una **entrega de valor al cliente**.

**Pasos:**
1. **Agrupar HU por dependencias** — identificar obligatorias y cadenas que no pueden romperse
2. **Determinar la cadencia** (capacidad de trabajo) del equipo, usando:
   - **Juicio experto** — expertos estiman cuántos Story Points se pueden completar por semana
   - **Estimación análoga** — basada en información histórica de proyectos similares

### Iteración 0 y Time box

- El **Time box** es la duración estándar de las iteraciones → mantiene un **ritmo consistente** y genera sensación de urgencia
- **Duración:** proyectos pequeños ~2 semanas, medianos ~4, grandes ~6. No más de 6 semanas
- Cada iteración debe entregar un **producto o funcionalidad validable** por el PO

### Percepción del valor

| Tipo de valor | Descripción |
|---------------|-------------|
| **Financiero** | ROI, costo/beneficio, aumento de ingresos, reducción de costos |
| **Estratégico** | Impacto en estrategia, marca, competitividad, expansión del mercado |
| **Para empleados** | Clima laboral, ambiente de trabajo, desarrollo profesional |
| **Para clientes** | Calidad de productos, mejora en servicios, rapidez, innovación |
| **Social** | Impacto en comunidades, empleos, desarrollo sostenible |

Ver también: [[notes/01. Planeacion adaptativa/cómo el cliente percibe el valor_|¿Cómo el cliente percibe el valor?]]

---

## Estimación de lanzamientos

Un **lanzamiento** (*Release*) es la liberación de una funcionalidad **utilizable, probada y estable**, normalmente cada determinado número de iteraciones.

### Roadmap

Un **roadmap** es un elemento gráfico que muestra en una **línea de tiempo** la visión de alto nivel de la duración del proyecto y las fechas probables de liberaciones. Se genera considerando:
- Historias de Usuario y épicas
- Story Points asignados a cada HU
- Capacidad del equipo por iteración

Para **épicas**, estimar cuántas iteraciones requiere cada talla (ej: S → 1 iteración, M → 2, L → 4, XL → 6).

Ver también: [[notes/01. Planeacion adaptativa/Estimación de lanzamientos|Estimación de lanzamientos]]

---

## Ideas para llevar

- Los elementos del método **INVEST**: Independiente, Negociable, Valioso, Estimable, Pequeña y Comprobable
- Nunca dimensionar HU sin la **participación del equipo de desarrollo**
- Una buena redacción de HU evita documentación excesiva y da claridad sobre necesidades y expectativas
- Las estimaciones iniciales **no representan precisión** en horas o días de implementación
- Los lanzamientos dan a los *stakeholders* una **visión preliminar** de cuándo se liberarán funcionalidades
- El **roadmap** muestra la línea de tiempo con la duración del proyecto y fechas probables de liberaciones

---

## Bibliografía

- Altman, H. (2018). *Gestión ágil de proyectos. Guía de inicio rápido para principiantes*.
- Griffiths, M. (2023). *PMI-ACP Exam Prep*. RMC Publications. 2a edición actualizada.
- Mountain Goat Software. (2023). *Concise Tips from Mike Cohn to Help You Succeed with Agile*.
- Mulcahy's, R. (2009). *PMP. Exam Prep*. RMC Publications. 6a edición.
- Scrum Manager BoK. (2021). *INVEST*.
