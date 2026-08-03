# Planeación adaptativa — Lección 4: MVP, priorización y reuniones

> PDF: [[documentation/01. Planeacion adaptativa/Planeación adaptativa_Lección 4_versión_impresa.pdf|Ver PDF original]]

Versión impresa de la Lección 4, que cubre la entrega temprana de valor mediante el MVP, técnicas de priorización, la técnica de las tres Cs, planificación de la ejecución del trabajo y las reuniones básicas del proyecto.

---

## Importancia del Minimum Value Product (MVP)

Estrategia popularizada por **Steve Blank y Eric Ries** (creadores de *Lean Startup*) que promueve la creación de un producto con el **mínimo de características necesarias** para dar funcionalidad y satisfacer las necesidades básicas del cliente.

La visión del MVP es entregar el **conjunto mínimo de características con funcionalidad básica** para que los *early adopters* puedan "sentir" el producto y proporcionar **retroalimentación**.

### Beneficios del MVP

1. **Ahorro de tiempo y recursos** — Prueba la viabilidad invirtiendo un mínimo de esfuerzo
2. **Retroalimentación temprana** — Comentarios valiosos para corregir problemas antes de que se agranden
3. **Enfoque en funcionalidades clave** — Evita inversión en funcionalidades que no aportan valor
4. **Mejor comprensión del mercado** — Facilita la adaptación del producto a las demandas del mercado

### Programación Extrema (XP) y el MVP

XP establece el MVP como los ***Bare bones*** ("puros huesos") — funcionalidad básica para satisfacer necesidades primarias. Puede ser un prototipo para que los usuarios finales validen la funcionalidad definitiva.

**Cinco valores de XP:**
- **Simplicidad** — Simplificar el diseño, eliminar lo innecesario, documentación sencilla
- **Comunicación** — Constante entre equipo y cliente, oportuna, abierta y honesta
- **Retroalimentación** — Ciclos cortos para obtener comentarios y mejorar procesos en tiempo real
- **Coraje** — Templanza para desechar trabajo que no cumple objetivos, asumir riesgos calculados
- **Respeto** — Para todos los miembros, generando confianza; todas las opiniones son valoradas

---

## Técnicas de priorización

El producto es como una **cebolla** a la que se añade una capa con cada liberación. La primera capa podría ser el MVP.

### 1. Método MoSCoW

| Categoría | Descripción |
|-----------|-------------|
| **Must have** | Características imprescindibles — parte crítica sin la cual el producto no funciona |
| **Should have** | Características importantes — su omisión impacta negativamente el valor |
| **Could have** | Útiles pero no esenciales — mejoran calidad/utilidad, pero el producto funciona sin ellas |
| **Won't have** | No necesarias por ahora — podrían agregar valor en el futuro |

El MVP incluye los **"M" (Must have)** para el *bare bones* y los **"S" (Should have)** para evitar retroalimentación negativa.

### 2. Técnica de valor del negocio

1. **Identificar los problemas y necesidades** del cliente
2. **Priorizar las características** por importancia y valor para el cliente
3. **Calcular el valor del negocio** — asignar valor considerando impacto (financiero, estratégico, para clientes, empleados o social)
4. **Seleccionar las características del MVP** — las de mayor calificación y esenciales para la funcionalidad
5. **Validar el MVP** — pruebas y comentarios de usuarios

### 3. Técnica de esfuerzo y complejidad

1. **Identificar funcionalidades esenciales** — críticas para objetivos del negocio
2. **Evaluar esfuerzo y complejidad** — recursos, habilidades requeridas y disponibilidad
3. **Clasificar las características** — valores "alta", "media" y "baja"
4. **Seleccionar funcionalidades del MVP** — mayor prioridad con menor esfuerzo y complejidad
5. **Validar el contenido del MVP** con los principales *stakeholders*

---

## Técnica de las tres Cs (Ron Jeffries, 2001)

Tres elementos para asegurar que la HU cumpla su objetivo:

**Card (Tarjeta):** Se escribe la HU en una tarjeta manipulable — solo texto suficiente para mantener en mente el requisito y la prioridad. No usarla como documento extenso.

**Conversation (Conversación):** El cliente comunica, aclara y revisa el entendimiento de los requisitos. Es **comunicación constante** entre cliente/PO y equipo de desarrollo a lo largo de la iteración. El equipo puede tomar notas, realizar dibujos o bocetos.

**Confirmation (Confirmación):** Prueba de funcionalidad de la HU finalizada contra los **criterios de aceptación** (checklist, pruebas de funcionalidad, aseguramiento de calidad).

Ver también: [[notes/01. Planeacion adaptativa/Técnica de las tres Cs|Técnica de las tres Cs]]

---

## Planificación de la ejecución del trabajo

- Equipos ágiles de **5 a 9 integrantes** — facilita la comunicación diaria
- Se recomienda **co-locación** para fomentar comunicación cara a cara, sentido de comunidad, compromiso y transparencia
- El equipo se **autogestiona** — no existe un líder de equipo
- Cada HU se desglosa en **tareas** (responsabilidad exclusiva del equipo de desarrollo)
- Las tareas se estiman en **horas** (máximo 16h de esfuerzo; si es mayor, descomponer más)

### Técnica SMART para tareas

- **S — Specific (Específica):** Claro lo que se quiere lograr, evitando ambigüedades
- **M — Measurable (Medible):** Criterios para medir avance y finalización
- **A — Attainable (Alcanzable):** Esfuerzo realista, ni estrecho ni holgado
- **R — Relevant (Importante):** Alineado al objetivo de la HU; no programar tareas que no aporten valor
- **T — Time boxed (Basado en tiempo):** Fecha objetivo de finalización para mantener enfoque y urgencia

### Reglas durante la iteración

- Se pueden incluir **nuevas tareas** durante la iteración
- **No adicionar HU** a las originalmente establecidas — sobrecarga al equipo e interrumpe el flujo
- HU nuevas deben **priorizarse en el backlog** e incluirse en la siguiente iteración

---

## Reuniones básicas del proyecto

### 1. Reunión de planificación de la iteración

- **Objetivo:** Revisar HU asignadas y determinar cómo se completarán
- **Timebox:** ~8h para iteración de 4-6 semanas; ~2h para iteración de 2 semanas
- **Participantes:** PO, líder ágil, equipo de desarrollo, *stakeholders* clave
- **Proceso:** PO expone objetivo y HU prioritarias → equipo hace preguntas → en conjunto determinan el **backlog de la iteración** → equipo descompone HU en tareas
- **Al final:** Acuerdo sobre el objetivo, fecha de reunión de revisión, y **Definition of Done**

### 2. Reunión diaria de seguimiento

- **Objetivo:** Sincronización y alineación al objetivo de la iteración; identificar impedimentos
- **Timebox:** Máximo 15 minutos, de pie
- **Proceso:** Cada miembro reporta qué hizo, qué hará hoy, y si tiene impedimentos
- Se mueven tarjetas en el **tablero Kanban** (To Do → In Progress → Done)

### 3. Reunión de revisión de la iteración

- **Objetivo:** Mostrar el resultado de la iteración y el incremento a la funcionalidad del producto (**"QUÉ" se hizo**)
- **Timebox:** ~2h para iteración de 4 semanas; puede llegar a 4h
- **Audiencia principal:** Product Owner y *stakeholders*
- **Proceso:** Equipo muestra trabajo realizado → PO valida criterios de aceptación → HU no finalizadas regresan al backlog del proyecto

### 4. Reunión de retrospectiva de la iteración

- **Objetivo:** Revisar **"CÓMO" se realizó** el trabajo; discutir qué salió bien y qué se puede mejorar
- **Timebox:** 1-3h para iteración de 4 semanas
- **Proceso:** Dinámica rompe-hielo → identificar aciertos y puntos débiles (análisis FODA) → **documentar acciones** de mejora → lecciones aprendidas para la siguiente iteración

> **IMPORTANTE:** No confundir **Revisión** (QUÉ se hizo) con **Retrospectiva** (CÓMO se hizo).

Ver también: [[notes/01. Planeacion adaptativa/En qué consisten las las reuniones de revisión y retrospectiva|Reuniones de revisión y retrospectiva]]

---

## Ideas para llevar

- El **MVP** es funcionalidad básica del producto o un prototipo para que usuarios iniciales lo valoren
- Varias **técnicas para determinar el MVP** — elegir la más alineada con los objetivos del proyecto
- Las HU del backlog de iteración se seleccionan por **prioridad** (responsabilidad del PO); la descomposición en tareas es del **equipo de desarrollo**
- La técnica de las **tres Cs** (Card, Conversation, Confirmation) mejora el entendimiento del incremento esperado
- **Cuatro reuniones básicas:** Planificación, Diaria, Revisión y Retrospectiva

---

## Bibliografía

- Atlassian. (2023). *Aplicación Trello*.
- Blank, S. (2020). *About Minimum Viable Product (MVP)*. Startup Istanbul.
- EUROPARC Federation. (2022). Paul Mayer — SMART goals.
- Meyer, P. (2006). *Attitude is everything*. Attitude & Motivation, Vol. 2.
- RonJeffries.com. (2001). *Essential XP: Card, Conversation, Confirmation*.
