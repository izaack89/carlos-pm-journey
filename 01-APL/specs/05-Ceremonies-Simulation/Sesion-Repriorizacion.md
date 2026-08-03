---
title: Sesión de Re-priorización (Semana 5)
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.1, 2.2, 3.3]
tags: [simulacion, repriorizacion, valor]
---

# Sesión de Re-priorización — Semana 5

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación.

## Propósito

Mostrar cómo el equipo re-prioriza el backlog basándose en aprendizajes del Golden Cluster + nuevas inputs de Telemóvil Planning. Materializa subcompetencia **1.1 Planeación Adaptativa** y **2.2 Value Driven Delivery**.

---

## Contexto

- **Fecha planeada:** lunes 29 de junio de 2026 (semana 5, primer día)
- **Hora:** 10:00 AM Costa Rica (después del peer meeting Carlos-Eduardo de las 8 AM)
- **Duración:** 60 minutos
- **Formato:** Híbrido (remotos por Teams, presenciales en Telemóvil)
- **Idioma:** Inglés
- **Asistentes:** Carlos, Eduardo (peer), Roberto (RAN Telemóvil), Marcela (Planning Telemóvil), Marco (Optimizadores Lead)

---

## Inputs para la sesión

### 1. Aprendizajes del Golden Cluster

- Template v2 ya aprobado
- KPIs suburbanos requieren 72h validación (no 48h)
- RF plan freshness check ahora en DoR
- Sandeep's automation reduce pre-checks de 30 a 10 min → libera capacidad

### 2. Marcela (Planning Telemóvil) — nueva data de demanda

Marcela trae datos de saturación de los últimos 30 días:

| Zona | Saturación actual | Crecimiento mensual |
|------|-------------------|---------------------|
| Costa del Este (CR-002) | 87% | +4% |
| Bella Vista (CR-004) | 91% 🔴 | +6% |
| Punta Pacífica (CR-007) | 83% | +5% |
| Tocumen (CR-015) | 65% | +2% |
| Arraiján (CR-021) | 58% | +1% |

**Hallazgo de Marcela:** Bella Vista (CR-004) está al 91%, más urgente de lo originalmente estimado.

### 3. Roberto (RAN Telemóvil) — observaciones técnicas

Después de validar template v2 con los 5 sitios del cluster, Roberto sugiere:
- Sitios con MIMO 8x8 deben tener un día adicional de validación
- Carrier Aggregation 3CA debe probarse en uno de los próximos sitios

### 4. Eduardo (peer) — estado de readiness físico

Eduardo aporta el estado de site readiness:

| Sitio | Estado de readiness |
|-------|---------------------|
| CR-002 Costa del Este | ✅ Listo |
| CR-004 Bella Vista | ✅ Listo |
| CR-006 Obarrio | ✅ Listo |
| CR-007 Punta Pacífica | ⚠️ Tower company issue, ETA viernes |
| CR-008 Vía Brasil | ✅ Listo |
| CR-009 Calidonia | ✅ Listo |

---

## Narrativa de la sesión

### 10:00 — Apertura

**Carlos:** "We're 5 sites done. 18 to go. Today we revisit priorities based on what we learned, new data from Marcela, and Eduardo's pipeline."

### 10:05 — Marcela presenta datos de demanda

**Marcela:** "Bella Vista is at 91% saturation. Customers are noticing slowness. If we delay much more, we may lose market share to Tigo."

**Carlos:** "Originally CR-004 was 7th in priority. Are we moving it up?"

**Marcela:** "Yes, please. Top of the next batch."

### 10:10 — Roberto comments técnicos

**Roberto:** "Two things. First, 3CA hasn't been tested in our network yet. The first site with 3CA would be valuable to validate proactively. Second, MIMO 8x8 needs an extra day."

**Carlos:** "CR-002 Costa del Este is a candidate for 3CA. Marco, opinion?"

**Marco:** "Yes, it's a good site for that test. I'd take it myself. But it means an extra day."

**Carlos:** "OK, CR-002 in next batch as 3CA test."

### 10:15 — Eduardo aporta readiness

**Eduardo:** "CR-007 Punta Pacífica has a tower company issue. Probability of resolution this week: 60%. I propose we don't include it in this batch and move it to week 6."

**Carlos:** "Agreed. CR-007 deferred."

### 10:20 — Re-priorización

Carlos pinta el nuevo orden de la semana 5 en el tablero:

| Orden anterior | Sitio | Orden nuevo | Razón del cambio |
|---|---|---|---|
| 6 | CR-002 Costa del Este | 1 (sem 5) | Test de 3CA + readiness OK |
| 7 | CR-004 Bella Vista | 2 (sem 5) | Saturación 91% — urgencia comercial |
| 8 | CR-006 Obarrio | 3 (sem 5) | Readiness OK, plan original |
| 9 | CR-007 Punta Pacífica | Diferido a sem 6 | Tower company pendiente |
| 10 | CR-008 Vía Brasil | 4 (sem 5) | Readiness OK |
| 11 | CR-009 Calidonia | 5 (sem 5) | Readiness OK |

### 10:30 — Marco confirma asignaciones

**Marco:**
- CR-002 (3CA test) — Marco mismo
- CR-004 (Bella Vista urgente) — Sofía
- CR-006 — Patricia (Junior, con apoyo de Sofía)
- CR-008 — Marco
- CR-009 — Sofía

Sandeep va a integrar CR-008 (donde su automatización se prueba en escala).

### 10:40 — Eduardo confirma cuadrillas

| Sitio | Cuadrilla |
|---|---|
| CR-002 | Luis (Cuadrilla 1, Centro) |
| CR-004 | Luis |
| CR-006 | Luis |
| CR-008 | Luis |
| CR-009 | Luis |

🤔 **Eduardo observa:** "All sites this week are Centro. Luis's team is overloaded. I'll redistribute by switching CR-009 to Javier (Cuadrilla 2)."

**Carlos:** "Good catch. Updated."

### 10:50 — Validación con Marcela y Roberto

**Marcela:** "OK with the new order. Thank you for moving CR-004 up."

**Roberto:** "OK. Will validate CR-002 3CA results carefully."

### 10:55 — Cierre

**Carlos:** "Decisions logged. Updating Jira and notifying full team in today's daily. Same time next Monday."

---

## Decisiones documentadas

| # | Decisión | Aprobado por |
|---|----------|--------------|
| 1 | CR-002 sube a primera posición sem 5, prueba 3CA | Carlos + Roberto + Marcela + Marco |
| 2 | CR-004 sube a segunda posición sem 5 (saturación 91%) | Carlos + Marcela |
| 3 | CR-007 diferido a sem 6 (tower company pendiente) | Carlos + Eduardo |
| 4 | MIMO 8x8 sitios requieren día adicional validación | Roberto + Marco |
| 5 | Sandeep toma CR-008 para piloto de automatización | Carlos |
| 6 | Cuadrilla 2 (Javier) toma CR-009 para balancear carga | Eduardo |

---

## Indicadores de la sesión

- **Decisiones tomadas:** 6
- **Stakeholders Telemóvil involucrados:** 2 (Roberto, Marcela)
- **Tiempo invertido:** 60 minutos
- **Conflictos escalados:** 0
- **Cambios al backlog:** 4 sitios re-priorizados

---

## Patrones observables

### Lo que funcionó

1. **Marcela aportó data real** (no opinión) — saturación 91%
2. **Roberto fue proactivo** — sugirió 3CA test antes del despliegue masivo
3. **Eduardo identificó cuello de botella** de cuadrilla y propuso solución
4. **Carlos facilitó sin imponer** — escuchó, sintetizó, decidió en consenso
5. **Sandeep apareció en discusión** — su automatización integrada al plan

### Por qué esto es Planeación Adaptativa real

El plan se ajusta basado en:
- Aprendizajes (cluster)
- Nueva información (saturación Marcela)
- Restricciones físicas (tower company CR-007)
- Capacidad del equipo (cuadrilla Luis sobrecargada)
- Oportunidades técnicas (3CA test)

**No es replanificación caprichosa. Es respuesta a información real.**

---

## Mapeo de Subcompetencias

- **1.1 Planeación Adaptativa:** caso concreto de adaptar el plan con razones objetivas
- **2.2 Value Driven Delivery:** prioridad por valor de negocio (Bella Vista urgente)
- **3.3 Gestión de Involucrados:** Marcela y Roberto integrados en la decisión

---

**Anterior:** [[Retrospectiva-Golden-Cluster]]
