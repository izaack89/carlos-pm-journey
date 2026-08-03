---
title: Retrospectiva del Golden Cluster
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [2.1, 3.2, 1.5]
tags: [simulacion, retrospectiva, mejora-continua]
---

# Retrospectiva del Golden Cluster (Semana 4)

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación. Esta es la retrospectiva planeada después de los primeros 3 sitios. Es el **punto de inflexión** del proyecto.

## Propósito

Capturar lecciones, ajustar template y proceso, refrescar el plan para los 20 sitios restantes. Esta ceremonia es la materialización principal de la subcompetencia **2.1 Continuous Improvement**.

---

## Contexto

- **Fecha planeada:** martes 23 de junio de 2026 (semana 4)
- **Duración:** 2 horas
- **Formato:** Híbrido (Teams + sala presencial Telemóvil)
- **Idioma:** Inglés (con switches a español cuando sea necesario)
- **Asistentes (17 personas):**

### Ericsson
- Carlos (facilitador)
- Eduardo (peer Implementation Manager)
- CPM Ericsson
- 4 Integradores: Diego, Ana, Sandeep, Hugo
- 3 Optimizadores: Marco, Sofía, Patricia
- 3 Líderes de Cuadrilla: Luis, Javier, Ricardo

### Telemóvil (invitados clave)
- 🌟 **Roberto** (RAN Engineering) — invitado especial
- 🌟 **Patricia (Telemóvil Quality)** — invitada para perspectiva de calidad
- Marcela (Planning) — opcional

---

## Por qué invitar a Roberto y Patricia Telemóvil

En retrospectivas tradicionales, el cliente no participa. En este proyecto, Carlos toma la decisión deliberada de invitarlos al Golden Cluster por varias razones:

1. **Confianza:** Roberto fue escéptico al inicio. Verlo participar en una retrospectiva real construye confianza
2. **Información directa:** sus observaciones técnicas son input valioso
3. **Co-ownership del template v2:** las mejoras del template requieren su validación; mejor que sea co-construida
4. **Demostración del enfoque ágil:** Roberto puede llevar la experiencia a Telemóvil como caso interno

🔶 **[VALIDAR CON CARLOS]:** Esta decisión es ambiciosa. Confirmar si culturalmente Telemóvil acepta esta apertura.

---

## Formato: 4L (Liked / Learned / Lacked / Longed for)

Formato simple, traducible, funcional con grupos diversos.

### Setup

Tablero (Miro o Mural compartido en pantalla):

```
┌─────────────────┬─────────────────┐
│     LIKED       │     LEARNED     │
│  (lo que       │  (lo que        │
│   funcionó)     │   aprendimos)   │
├─────────────────┼─────────────────┤
│     LACKED      │  LONGED FOR     │
│  (lo que       │  (lo que        │
│   faltó)        │   quisiéramos)  │
└─────────────────┴─────────────────┘
```

Cada persona escribe sticky notes durante 15 min en silencio, luego se comparten.

---

## Datos cuantitativos esperados del Golden Cluster

🔶 **[VALIDAR CON CARLOS]:** Estos son los datos hipotéticos esperados. Carlos los actualiza con datos reales después de la ejecución.

| Métrica | Resultado esperado |
|---------|-------------------|
| **Sitios completados** | 5 (CR-001, CR-003, CR-005, CR-014, CR-019) |
| **FTR (First Time Right)** | 4/5 = 80% (CR-014 requirió ajuste) |
| **Tiempo promedio por sitio** | 6-7 días desde "Listo para Ventana" hasta "Done" |
| **Bloqueos identificados** | 2-3 (incluyendo CR-014 RF) |
| **Tiempo promedio resolución** | <48h |
| **Cumplimiento DoR primer intento** | 80-85% |
| **Participación de Sandeep en dailies** | 90%+ |
| **Conflictos peer Carlos-Eduardo** | Tendencia a 0 |
| **Reportes a Telemóvil** | 4 (uno por semana, por área) |

---

## Narrativa esperada de la retrospectiva

### Apertura (10 min)

**Carlos:** "Welcome everyone. Today we look at what we did in the first 5 sites and decide what to keep, what to change, and what to try."

**Roberto (Telemóvil RAN):** "I'm here to learn the format. I appreciate the invitation."

### Sticky notes (15 min en silencio)

Todos los participantes escriben en silencio. Se proyecta el tablero y se observa cómo se va llenando.

### Compartir — LIKED (15 min)

Patrones esperados:

**Sandeep (India):** "Daily in English. I felt included for the first time in a Latam project."

**Luis (Cuadrilla 1):** "Que se nos avisara con 48h. Eso me permitió organizar mi equipo."

**Patricia (Optimizadora Junior):** "Marco was an excellent informal mentor. I learned more in 3 weeks than in 3 months at another project."

**Diego (Integrador Senior):** "Pre-staging the template 24h in advance saved at least 1 hour per integration."

**Roberto (Telemóvil RAN):** "Transparency. I could see CR-014 issue almost in real time. That doesn't happen in traditional projects."

**Eduardo (peer):** "Weekly peer meeting with Carlos every Monday. Zero friction this cluster."

**Carlos** observa: el comentario de Roberto es **el más valioso**. Transparencia generó confianza temprana.

### Compartir — LEARNED (15 min)

**Marco:** "RF plan in the system was 6 months old in CR-014. New building wasn't documented. Should be a freshness check pre-integration."

**Ana:** "Suburban sites take 20% longer to validate KPIs because vegetation introduces variability."

**Sandeep:** "Automation scripts can reduce pre-checks from 30 to 10 minutes. I'll share the code."

**Ricardo (Cuadrilla 3):** "Tres cuadrillas con diferentes empresas tienen diferentes formatos de reporte. Sería bueno unificar."

**Patricia (Telemóvil Quality):** "Validating KPIs in 48h is enough for urban sites, but suburban sites should be 72h."

### Compartir — LACKED (20 min)

Aquí emerge la información más rica.

**Hugo (Integrador Junior):** "Sometimes I didn't know who to ask. Diego is senior but is in Costa Rica; Carlos is busy. Maybe formalize office hours?"

**Javier (Cuadrilla 2):** "Falta de WhatsApp para emergencias. Sé que el acuerdo dice solo Jira, pero a veces no hay tiempo."

🤔 Esta es información incómoda. El acuerdo prohibía WhatsApp para decisiones operativas, pero Javier reporta que en práctica hace falta para emergencias.

**Carlos** decide:
> "Let's discuss. The agreement is to keep decisions in Jira. But for real emergencies — physical safety in site, immediate cancellation — we add a WhatsApp channel only for emergencies. Eduardo, do you agree?"

**Eduardo:** "Yes, I propose Eduardo as channel owner — he creates it and monitors."

Acción acordada: agregar al Acuerdo de Equipo un párrafo sobre "WhatsApp solo para emergencias físicas, definidas explícitamente".

**Sofía:** "Distance Argentina-Panama makes 9 AM Panama feel rushed. I lose 30 min adjusting from my morning. Could daily be 9:30 AM Panama?"

**Sandeep:** "9:30 Panama would be 11 PM India for me. Even later."

**Carlos:** "Let's keep 9 AM. Sofía, would it work to push your start to 8 AM ARG instead?"

**Sofía:** "Yes, manageable."

**Roberto (Telemóvil RAN):** "Tuesday weekly reports come at end of day. By the time we read them, it's almost Wednesday. Could they come Tuesday morning?"

**Carlos:** "Marco, can we move weekly reports to Monday at end of day?"

**Marco:** "Yes."

### Compartir — LONGED FOR (15 min)

**Patricia (Junior Optimizadora):** "More formal knowledge sharing sessions. Sandeep's automation session was a great example."

**Diego:** "A team retrospective without Telemóvil present so we can be more candid about internal frictions."

🤔 Carlos nota esto. Pequeña fricción visible que Diego no quiere airear con Telemóvil presente. Carlos acuerda:
> "Yes, we'll have internal retrospectives every 2 weeks, no Telemóvil present. This is the joint retrospective for cluster lessons; the internal one is for team dynamics."

**Eduardo:** "More visibility into the Implementation Manager queue would help Carlos plan. I'll share my pipeline more proactively."

**Marcela (Telemóvil Planning):** "I would love to be involved in re-prioritization more visibly. I have data on user demand that could inform Carlos's decisions."

**Carlos:** "Marcela, let's formalize the Monday re-prioritization meeting and include you."

---

## Acciones acordadas

| # | Acción | Owner | Deadline | Subcomp. |
|---|--------|-------|----------|----------|
| 1 | Agregar "freshness check" del plan de RF a la DoR | Carlos + Roberto | Antes de sem 5 | 1.4 |
| 2 | Extender validación de KPIs a 72h en sitios suburbanos | Patricia Telemóvil + Marco | Antes de sem 5 | 1.5 |
| 3 | Implementar automatización de pre-checks de Sandeep | Sandeep + todos los Integradores | Sem 5 | 2.1 |
| 4 | Unificar formato de reporte de cuadrillas | Eduardo + 3 líderes | Sem 5 | 3.2 |
| 5 | Agregar canal WhatsApp solo para emergencias físicas | Eduardo | Sem 5 | 3.2 |
| 6 | Mover reportes semanales a Telemóvil al lunes EOD | Marco | Sem 5 | 1.5 |
| 7 | Formalizar reunión de re-priorización lunes con Marcela | Carlos | Sem 5 | 1.1 |
| 8 | Retrospectivas internas cada 2 semanas (sin Telemóvil) | Carlos | Recurrente | 3.2 |
| 9 | Office hours de Carlos: martes y jueves 2-3 PM | Carlos | Recurrente | 3.2 |
| 10 | Template v2 con ajustes del Golden Cluster | Diego + Roberto | Sem 5 | 2.1 |

---

## Compromiso de seguimiento

- Las acciones se revisan en la mini-retrospectiva de la semana 6
- Si alguna acción no se ejecuta, se discute por qué y se ajusta
- El nuevo template v2 se documenta y se versiona

---

## Cierre del retrospectivo

**Carlos:**
> "Thank you everyone. Roberto, your participation today changes this retrospective. Patricia, your input on Quality is invaluable. Eduardo, we continue as peers without friction. Sandeep, thank you for the automation contribution. The cuadrillas, thank you for the honest feedback on WhatsApp.
> 
> The Golden Cluster did its job — we found things to improve, and we have time to apply them. Let's make the remaining 18 sites better."

**Roberto:**
> "I am taking this format to my team at Telemóvil. I hadn't seen agile work at this level in a Latam telco project."

🟢 Momento clave. Roberto, originalmente escéptico, ahora es **advocate del enfoque**.

---

## Comparativa: aprendizaje en este modelo vs tradicional

| Dimensión | Tradicional | Ágil (este proyecto) |
|---|---|---|
| **Cuándo se aprende** | Al final, en post-mortem | Cada 4 sitios (golden cluster) |
| **Quién participa** | Solo equipo Ericsson interno | Equipo + cliente + cuadrillas |
| **Acciones aplicadas** | Al próximo proyecto (si hay) | Al mismo proyecto, en marcha |
| **Documentación** | Variable, baja | Estructurada, accionable |
| **Cliente como advocate** | Raro | Posible (caso Roberto) |

---

## Mapeo de Subcompetencias

- **2.1 Continuous Improvement:** este documento ES la materialización principal
- **3.2 Equipo de Alto Desempeño:** retrospectiva revela y mejora dinámicas del equipo
- **1.5 Metrics & Reporting:** datos del cluster informan decisiones

## Preguntas para Carlos

1. ¿Invitar a Roberto a la retrospectiva es viable culturalmente en Telemóvil?
2. ¿El formato 4L es adecuado o prefieres otro (sailboat, mad/sad/glad)?
3. ¿La ausencia de fricción entre tú y Eduardo en el cluster es realista o esperar tensión?
4. ¿Las 10 acciones acordadas son demasiadas o adecuadas?

---

**Siguiente:** [[Sesion-Repriorizacion]]
**Anterior:** [[Bloqueo-Simulado-y-Resolucion]]
