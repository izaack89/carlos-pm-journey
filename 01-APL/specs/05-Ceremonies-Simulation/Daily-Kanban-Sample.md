---
title: Daily Kanban — Simulación de Sesión Típica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.2, 3.2]
tags: [simulacion, daily, kanban, ceremonia]
---

# Daily Kanban — Sesión Típica de la Semana 3 (Simulación)

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación. Esta es una sesión típica esperada del daily Kanban durante la fase de Golden Cluster.

## Propósito

Mostrar cómo se ejecutará una ceremonia diaria con equipo distribuido (Latam + India + Costa Rica local). La simulación retrata una **sesión realista esperada**, con bloqueos, dudas y decisiones tomadas en tiempo real.

---

## Contexto

- **Fecha simulada:** miércoles 17 de junio de 2026 (Semana 3, Día 3)
- **Hora:** 9:00 AM Costa Rica (10:30 PM India — Sandeep se conecta)
- **Duración:** 15 minutos estrictos
- **Idioma:** **Inglés**
- **Formato:** 100% remoto vía Teams; cuadrillas locales se conectan desde campo o oficina con audio
- **Asistentes (12 personas):**

### Ericsson (remotos)
- **Carlos** (NPM, facilitador)
- **Diego, Ana, Sandeep, Hugo** (Integradores)
- **Marco, Sofía, Patricia** (Optimizadores)
- **Eduardo** (Implementation Manager, presencial en Costa Rica pero se conecta vía Teams)

### Cuadrillas locales
- **Luis, Javier, Ricardo** (vía Teams desde campo o oficina)

---

## Estado del tablero al inicio del daily

```
| Backlog | Listo Ventana | Integración | Optimización | Listo Acept. | Aceptación | Done |
|---------|---------------|-------------|--------------|--------------|------------|------|
| CR-006  | CR-014        | CR-019      |              | CR-003       | CR-001     | -    |
| CR-007  | CR-021        |             |              |              |            |      |
| CR-002  |               |             | CR-014 🚫    |              |            |      |
| ...     |               |             | CR-005 🆕    |              |            |      |
```

**Sitios activos:** 5
**Bloqueados:** 1 (CR-014)

---

## Transcripción de la sesión

> Nota: Diálogo en inglés (traducido al español entre paréntesis cuando aporta).

### 09:00 — Apertura

**Carlos:** "Good morning, team. Sandeep, good evening to you. 15 minutes as always. We'll go column by column, right to left. Let's start with Acceptance."

(Buenos días equipo. Sandeep, buenas noches para ti. 15 min como siempre. Vamos columna por columna, derecha a izquierda. Empezamos con Aceptación.)

### 09:01 — Columna Aceptación

**Carlos:** "CR-001 Vía España. Diego?"

**Diego:** "Ready. KPIs validated by Marco yesterday. SAD uploaded to Confluence. Presenting at Friday's session with Acceptance Team."

**Carlos:** "Excellent. FTR?"

**Diego:** "Positive. No observations."

**Carlos:** "Great. One more in 'Done' soon."

### 09:02 — Columna Listo para Aceptación

**Carlos:** "CR-003 El Cangrejo. Marco?"

**Marco:** "Optimization complete. KPIs solid for 48 hours. Patricia Telemóvil validated this morning. Ready for Friday's batch."

**Carlos:** "Perfect."

### 09:03 — Columna Optimización

**Carlos:** "CR-014 San Miguelito. Red flag — what's happening?"

**Marco:** "Integration finished last night. Configuration OK, but DL throughput on the north sector is consistently 8% below expected threshold."

**Carlos:** "Probable cause?"

**Marco:** "I suspect RF reflection from a new building. Not in the original RF plan, which is 6 months old."

**Carlos:** "Critical for acceptance?"

**Marco:** "Not critical, but below minimum threshold. I need 24-48 hours more to optimize the electrical tilt of the antenna."

**Carlos:** "OK. Marking block as active. Sofía, can you support Marco with the RF analysis? You have experience with similar cases."

**Sofía:** "Sí, lo veo hoy en la tarde." (Switches to English) "Yes, I can look at it this afternoon."

**Carlos:** "Perfect. If not resolved by Friday EOD, we elevate it to the template — could be a pattern for other sites."

**Eduardo (peer):** "Carlos, quick note — the cuadrilla left the site at 6 AM after physical installation. If we need them back for additional measurements, I need to know by tomorrow."

**Carlos:** "Good point Eduardo. Marco, coordinate with Eduardo if you need physical re-visit."

**Marco:** "Will do, probably not needed."

🔴 **Decisión clave:** mantener CR-014 bloqueado, asignar apoyo Sofía, deadline jueves EOD.

**Carlos:** "CR-005 San Francisco. Sofía?"

**Sofía:** "Just moved from Integration. Sandeep applied the template last night. I'm starting KPI validation now. No surprises so far."

**Carlos:** "Sandeep, anything to note on CR-005?"

**Sandeep (vía Teams from India):** "All template features applied successfully. Some automation logs I'd like to share with team — I'll post in the Jira ticket. Good site for the validation script I'm working on."

**Carlos:** "Thanks Sandeep. Looking forward to that automation."

### 09:06 — Columna Integración

**Carlos:** "Nothing in Integration today. Empty column means good flow."

### 09:07 — Columna Listo para Ventana

**Carlos:** "CR-019 Juan Díaz. Ana?"

**Ana:** "Window tonight, 23:00 to 03:00. Template pre-staged. Hugo will support remotely. Ricardo's cuadrilla on site."

**Ricardo (Cuadrilla):** "Confirmado. Mi equipo llega al sitio a las 21:00 para preparación."

**Ana (en inglés):** "Ricardo confirms his team arrives at 21:00 for setup."

**Carlos:** "Good. Eduardo, on standby tonight?"

**Eduardo:** "Yes, both Ricardo and I will be available."

**Carlos:** "CR-021 Arraiján. Hugo?"

**Hugo:** "Window day after tomorrow. Pre-staging today. Javier's cuadrilla."

**Javier:** "Listo de mi lado." (English) "Ready on my side."

### 09:09 — Columna Backlog

**Carlos:** "CR-006 Obarrio, CR-007 Punta Pacífica, CR-002 Costa del Este. Next to enter."

**Eduardo:** "I'm validating site readiness for CR-006 today. CR-007 has a tower company issue I'm escalating with the CPM. CR-002 ready, enters next week."

**Carlos:** "CR-007 worries me. Probability of delay?"

**Eduardo:** "Medium. If not resolved by Monday, I'll formally register it as a risk."

### 09:11 — Bloqueos generales

**Carlos:** "Active blockers summary:
- CR-014: support assigned to Marco/Sofía, deadline Friday EOD
- CR-007: tower company issue, escalated to CPM by Eduardo"

**Carlos:** "Anyone has any blocker not visible on the board?"

**Diego:** "A question — has Telemóvil confirmed if they want daily or weekly KPI reports for the cluster?"

**Carlos:** "Weekly batch — we agreed at kickoff. But I'll confirm with Roberto in Monday's technical meeting."

**Patricia (Optimizadora Junior):** "Carlos, quick note. I'm learning a lot from Marco's case on CR-014. Would it be possible to document the troubleshooting steps?"

**Carlos:** "Yes — Marco, can you write a brief note after resolution for the lessons learned?"

**Marco:** "Will do."

### 09:13 — Decisiones del daily

**Carlos:** "Today's decisions:

1. CR-001 to Acceptance Friday — Diego
2. CR-014 with support from Marco/Sofía — deadline Friday EOD, possible RF physical re-visit if Marco confirms
3. CR-005 in Optimization, Sofía leads validation
4. CR-019 integration tonight — Ana + Hugo + Ricardo cuadrilla, Eduardo on standby
5. CR-021 pre-staging today, integration in 2 days — Hugo + Javier cuadrilla
6. Marco documents CR-014 troubleshooting for Patricia (Junior) — input to lessons learned

Anything else?"

**Sandeep:** "I'd like to suggest a 15-minute knowledge sharing this Friday — I want to demo the automation scripts I've built."

**Carlos:** "Excellent. Diego, can you organize that? Friday 4 PM Panama time."

**Sandeep:** "Thanks. I'll keep it brief and recorded for those who can't attend."

**Carlos:** "Great daily, everyone. Same time tomorrow."

### 09:15 — Cierre

Daily termina a tiempo. Total: 15 minutos exactos.

---

## Estado del tablero post-daily

```
| Backlog | Listo Ventana | Integración | Optimización | Listo Acept.   | Aceptación | Done |
|---------|---------------|-------------|--------------|----------------|------------|------|
| CR-002  | CR-019 ⚡     | (vacío)     | CR-005 🆕    | CR-003 ✅      | CR-001 ✅  | -    |
| CR-006  | CR-021        |             | CR-014 🚫    |                |            |      |
| CR-007 ⚠️|              |             |              |                |            |      |
```

Leyenda:
- ⚡ Integración esta noche
- 🆕 Recién pasado a Optimización
- 🚫 Bloqueado, con apoyo asignado
- ✅ Listo para aceptación / aceptado
- ⚠️ Riesgo identificado

---

## Patrones observables del daily

### Lo que funcionó bien

1. **Foco estricto en 15 minutos** — todos respetaron el tiempo
2. **Inglés inclusivo** — Sandeep participó plenamente, hubo traducciones puntuales para cuadrillas
3. **Carlos como facilitador, no controlador** — pregunta, escucha, decide
4. **Eduardo aportó como peer** — comentó sobre cuadrilla sin imponer
5. **Sandeep iniciativa** — propuso knowledge sharing
6. **Patricia (Junior) participó** — su voz tuvo espacio
7. **Captura de aprendizajes en vivo** — documentación de CR-014

### Pequeñas fricciones

- Ricardo (Cuadrilla) habló en español primero antes de cambiar al inglés — pequeño momento de fricción lingüística, manejado bien
- El tema de los reportes a Telemóvil quedó "para confirmar el lunes" — podría haberse resuelto antes

### Indicadores de salud del equipo

- Todos los presentes hablaron al menos una vez
- Hubo respeto entre Carlos y Eduardo como peers
- Sandeep participó activamente a pesar de TZ
- Junior members (Hugo, Patricia) participaron
- Cuadrillas se comunicaron en su idioma con apoyo de Integradores

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** el daily ES la ceremonia central del Kanban
- **1.2 Detección de Riesgos:** bloqueos identificados y atendidos en tiempo real
- **3.2 Equipo de Alto Desempeño:** dinámica colaborativa, distribuida, inclusiva

---

**Siguiente:** [[Bloqueo-Simulado-y-Resolucion]]
**Anterior:** [[Dia-1-Proyecto]]
