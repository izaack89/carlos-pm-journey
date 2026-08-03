---
title: Día 1 del Proyecto — Kickoff (Simulación)
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 3.2, 3.3]
tags: [simulacion, kickoff, agile, dia-1]
---

# Día 1 del Proyecto — Simulación del Kickoff

> 🎯 **Documento de simulación prospectiva** — proyecto en fase de planeación. Este es el guion del kickoff que se ejecutará al inicio del proyecto.

## Propósito

Simular cómo se desarrollará el primer día del proyecto para demostrar la operación práctica del enfoque ágil con un equipo distribuido. Esta narrativa muestra al grader **cómo se ve el método en acción**, considerando el contexto remoto + peer dynamics + cuadrillas locales.

---

## Contexto

- **Fecha planeada:** lunes 1 de junio de 2026 (semana 1, día 1)
- **Hora de inicio:** 8:00 AM hora de Costa Rica
- **Formato:** Híbrido — Teams para remotos + sala presencial en oficinas Telemóvil Costa Rica
- **Asistentes (16 personas):**

### Ericsson
- **Carlos** (NPM, remoto) — anfitrión
- **Eduardo** (Implementation Manager, presencial en Costa Rica) — peer de Carlos
- **CPM Ericsson** (remoto)
- **CSM Ericsson** (presencial en Costa Rica)
- **4 Integradores:** Diego, Ana, Sandeep, Hugo (todos remotos)
- **3 Optimizadores:** Marco, Sofía, Patricia (todos remotos)

### Cuadrillas
- **3 Líderes de Cuadrilla:** Luis, Javier, Ricardo (presenciales en Costa Rica)

### Telemóvil Costa Rica (presenciales en sus oficinas)
- **Roberto** — Senior RAN Engineer
- **Marcela** — Planning Lead
- **Patricia (Telemóvil)** — Quality Lead
- **Fernando** — O&M Lead
- **Ricardo Mendoza** — Acceptance Team Lead

---

## Consideraciones especiales del kickoff distribuido

1. **Sandeep está en India (10:30 PM hora local)** — kickoff a hora razonable para él (no excede una hora extra-larga)
2. **Idioma del kickoff:** inglés para todos los presentes (incluye a Sandeep y respeta a Telemóvil bilingüe)
3. **Cuadrillas presenciales hablan español** — Carlos las introduce y Eduardo facilita su participación
4. **Mezcla presencial-remota** — videowall en sala Telemóvil para que remotos sean visibles

---

## Agenda del Kickoff (08:00 – 12:30, 4.5 horas con pausas)

| Hora | Bloque | Duración | Idioma |
|------|--------|----------|--------|
| 08:00 | Bienvenida + presentaciones | 30 min | Inglés |
| 08:30 | Visión y objetivo SMART | 20 min | Inglés |
| 08:50 | Enfoque ágil propuesto | 30 min | Inglés |
| 09:20 | Pausa | 15 min | — |
| 09:35 | Roles y peer dynamics (Carlos + Eduardo) | 25 min | Inglés |
| 10:00 | DoR y DoD | 30 min | Inglés |
| 10:30 | Pausa | 10 min | — |
| 10:40 | Acuerdo de Equipo — discusión y firmas | 60 min | Inglés + español para cuadrillas |
| 11:40 | Tablero Kanban (demo en Jira) | 20 min | Inglés |
| 12:00 | Cronograma + golden cluster | 20 min | Inglés |
| 12:20 | Q&A y siguientes pasos | 10 min | Inglés |

---

## Narrativa del kickoff

### 08:00 — Apertura

**CPM** abre la sesión, presenta brevemente la importancia del proyecto para Telemóvil y para Ericsson.

**Carlos** se conecta vía Teams y aparece en el videowall. Saluda en inglés:

> "Good morning, everyone. For those of you joining remotely — Sandeep from India, Diego from Costa Rica, Ana from Colombia, Hugo from Mexico, and our optimization team — welcome. For those in the room in Panama City — Roberto, Marcela, Patricia, Fernando, Ricardo, Eduardo, Luis, Javier, and Ricardo from Cuadrilla 3 — welcome too."

Roberto, desde Telemóvil Costa Rica:
> "We've seen previous deployments with headaches at the end. I hope this time will be different."

Carlos toma nota mental: Roberto está abierto pero escéptico. Es el momento de demostrar valor temprano.

### 08:30 — Visión y objetivo SMART

Carlos presenta el objetivo:

> "Achieve 100% integration and service activation of 23 LTE Band 41 sites in Panama, increasing operational efficiency by 10% through technical rework reduction, in an 8-week implementation cycle."

Enfatiza:
- **First Time Right (FTR)** como métrica compartida con Telemóvil
- **No solo lo técnico**: este proyecto también es un piloto de método ágil para futuros despliegues

### 08:50 — Enfoque ágil

Carlos presenta el rationale:

- **Por qué Kanban** en lugar de Scrum puro
- **Golden Cluster** como mecanismo de validación temprana
- **Retrospectivas** como motor de mejora continua
- **Peer dynamics** Carlos + Eduardo (no jerarquía)
- **Equipo distribuido** + cuadrillas locales

Roberto pregunta:
> "How do we from Telemóvil know about progress? I don't want to wait until the end."

Carlos responde mostrando el tablero Kanban:
> "You'll all have view access to the board. Each Monday there's a technical meeting with your team. Fridays are batch acceptance sessions. If you have any technical doubt, there's a direct channel with me."

Roberto asiente. Pequeño momento de construcción de confianza.

### 09:35 — Roles y peer dynamics

Carlos y Eduardo presentan el modelo peer dynamics conjuntamente.

**Carlos:** "Eduardo and I report to the same CPM. We are peers. He owns Implementation; I own Integration and Optimization. The hand-off between us is the 'Ready for Window' column."

**Eduardo:** "Right. My team — the three cuadrillas with Luis, Javier, and Ricardo — handles physical work. Carlos's team — four integrators and three optimizers — handles software. We coordinate every Monday morning."

Roberto interviene:
> "Will I see who is responsible if there's an issue?"

**Carlos:** "Yes. Every site card in Jira has clear ownership. And we don't blame across teams — we have shared metrics."

### 10:00 — DoR y DoD

Se revisa la Definition of Ready con sus dos partes (Implementation + Integration).

Patricia (Telemóvil Quality) observa:
> "I want to add to the DoD the requirement for extended KPI validation, not just 24 hours."

**Marco (Optimizador Senior):** "I agree completely. 24-48 hours minimum, and we can extend for premium sites."

Esta colaboración temprana entre el equipo de optimización y Patricia Telemóvil es buena señal.

### 10:40 — Acuerdo de Equipo

Este es el bloque más rico del kickoff.

CPM facilita discusión abierta. **Carlos cambia parcialmente al español** para que las cuadrillas puedan participar plenamente:

> "Luis, Javier, Ricardo — quiero escuchar de ustedes. ¿Qué les frustró en proyectos pasados?"

**Luis:** "Cambios de último minuto. Llegamos al sitio y resulta que la integración no estaba lista."

**Javier:** "Que se decide algo en una llamada en español y luego se reporta en inglés a Ericsson y se pierde contexto."

**Ricardo (Cuadrilla):** "Falta de retroalimentación. Solo escuchamos quejas, no reconocimiento."

**Carlos (en inglés para que todos entiendan):** "These are the friction points we want to solve. The Team Agreement addresses each: Jira as single source of truth, weekly recognition, and explicit communication protocols."

**Diego (Integrador):** "Carlos, can I add a commitment to the integrators? We commit to coordinating directly with cuadrillas during windows — not through email chains."

**Carlos:** "Documented in the agreement."

**Sandeep desde India (vía Teams):** "I want to acknowledge the timezone challenge. I commit to flexible scheduling and asynchronous documentation. Please let me know if I'm missing anything cultural."

**Carlos:** "Sandeep, thank you. Diego will be your cultural buddy."

Después de 50 minutos de discusión, **todos firman el acuerdo** (digital + presencial).

🌟 **Momento clave del kickoff.**

### 11:40 — Demo del Kanban

Carlos hace demo en vivo del tablero. Muestra:
- Las 7 columnas y WIP limits
- El formato de tarjeta
- La columna "Listo para Ventana" como hand-off
- Cómo se marcan los blockers

Roberto, Marcela, Patricia, Fernando y Ricardo Mendoza piden acceso de visualización. Carlos configura los accesos ahí mismo.

### 12:00 — Cronograma

Se revisa el Release Plan:
- Semana 1: Setup
- Semanas 2-4: Golden Cluster
- Semana 4: **Retrospectiva clave** — Roberto invitado especialmente
- Semanas 5-7: Despliegue masivo
- Semana 8: Cierre

Roberto:
> "Inviting me to the retrospective is unusual. I accept."

### 12:20 — Q&A

Pregunta clave de Patricia (Telemóvil Quality):
> "What if Telemóvil rejects a site?"

**Carlos:** "It returns to Optimization. We identify what failed. If it's a template issue, we apply the learning to remaining sites. If it's site-specific, we resolve it there. We document. It's not a drama, it's information."

### 12:30 — Cierre

CPM cierra con próximos pasos:

1. Carlos + Eduardo: validar DoR de los primeros 3 sitios (esta semana)
2. Roberto: validar y aprobar el template B41 antes del miércoles
3. Eduardo: confirmar disponibilidad de las 3 cuadrillas para semana 2
4. Diego (lead integrators): pre-stage del primer sitio en ENM antes del viernes
5. Marco (lead optimizadores): configurar dashboards de KPIs en EMA
6. Carlos: configurar permisos de visualización en Jira para Telemóvil

**Primer daily Kanban:** martes a las 9:00 AM (en inglés).

---

## Reflexión de Carlos (en su diario personal)

> "Buen kickoff. Roberto se mostró abierto, aunque escéptico al inicio. El momento clave fue cuando le mostré el canal directo y el acceso al Kanban.
>
> Lo que me preocupa: las cuadrillas firmaron el acuerdo, pero falta ver si lo respetan en práctica. La primera semana es prueba de fuego.
>
> Sandeep se conectó a las 10:30 PM hora India sin queja. Eso me dice que está comprometido. Tengo que cuidar que no se sienta aislado.
>
> Eduardo y yo nos coordinamos bien en la presentación. Cero fricción visible. Espero que se mantenga en operación.
>
> Próxima acción crítica: validar el template con Roberto antes del miércoles. Si eso se atrasa, todo el cronograma se mueve."

---

## Outputs del Día 1

| Output | Estado |
|--------|--------|
| Acta de kickoff | ✅ Generada |
| Acuerdo de Equipo firmado | ✅ Firmado por todos |
| Tablero Kanban configurado | ✅ Operativo |
| Acceso de Telemóvil al tablero (5 personas) | ✅ Configurado |
| Próximos pasos asignados | ✅ Documentados |
| Daily agendado | ✅ Para martes 9:00 (inglés) |
| Reunión semanal de peers agendada | ✅ Lunes 8:00 |

---

## Patrones observables en el kickoff

### Lo que funcionó

1. **Híbrido bien gestionado** — videowall + voz clara para remotos
2. **Idioma flexible** — inglés default, español en momentos clave para cuadrillas
3. **Sandeep incluido** — su comentario sobre TZ challenge fue acogido
4. **Carlos + Eduardo presentaron juntos** — peer dynamics visible
5. **Roberto aceptó retrospectiva** — momento poderoso

### Pequeñas fricciones

- El comentario de Javier (cuadrilla) sobre español/inglés mostró tensión real — se acordó traducciones explícitas
- Hora india tarde para Sandeep — no se puede evitar siempre, pero hubo conciencia

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** se establece el tablero y las reglas operativas
- **3.2 Equipo de Alto Desempeño:** se firma el acuerdo de equipo, incluye consideraciones culturales/idiomáticas
- **3.3 Gestión de Involucrados:** se establecen canales explícitos con 5 áreas de Telemóvil
- **1.1 Planeación Adaptativa:** se presenta el plan adaptable

---

**Siguiente:** [[Daily-Kanban-Sample]]
