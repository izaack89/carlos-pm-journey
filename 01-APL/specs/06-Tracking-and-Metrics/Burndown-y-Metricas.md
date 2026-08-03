---
title: Burndown y Métricas
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.5, 1.4, 1.1]
tags: [metricas, burndown, ftr, kpis]
---

# Burndown y Métricas del Proyecto

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Las métricas son **proyecciones esperadas**, no resultados reales. Se actualizan semanalmente durante la ejecución.

## Propósito

Definir el sistema de métricas del proyecto: qué se mide, cómo se mide, con qué frecuencia, y cómo se comunica a los stakeholders. Materializa la subcompetencia **1.5 Metrics & Reporting**.

---

## Filosofía de métricas

### Pocas, claras, accionables

El proyecto monitoriza un set acotado de métricas. La regla: **si una métrica no genera decisión, no se reporta**.

### Compartidas, no separadas

Las métricas son del proyecto, no de "el equipo de Carlos" vs "el equipo de Eduardo". El FTR es del sitio, no de su parte respectiva.

### Visibles para todos

Las métricas se publican en un dashboard accesible para todo el equipo y Telemóvil.

---

## Métricas principales

### M1 — Sitios completados (Burndown)

**Definición:** Sitios en estado "Done" del Kanban.

**Cómo se mide:** Conteo simple en Jira al final de cada semana.

**Meta:** 23 sitios en 8 semanas (~3 sitios/semana en promedio, con pico en sem 5-6).

**Proyección esperada:**

| Semana | Sitios planeados acumulados | Hitos |
|--------|------------------------------|-------|
| 1 | 0 | Setup |
| 2 | 2-3 | Golden Cluster iniciando |
| 3 | 5 | Golden Cluster completo |
| 4 | 5 | Retrospectiva, pausa de ejecución |
| 5 | 11 | Despliegue masivo iniciando |
| 6 | 17 | 50%+ del proyecto |
| 7 | 22 | Cierre del masivo |
| 8 | 23 | Proyecto completo |

### M2 — First Time Right (FTR)

**Definición:** Sitios aceptados al primer intento / sitios procesados.

**Cómo se mide:** Cada sitio tiene FTR = TRUE o FALSE basado en criterios de `[[Definition-of-Done]]`.

**Meta:** ≥ 90% (baseline histórico 82-88%).

**Proyección esperada (acumulada):**

| Semana | FTR acumulado esperado |
|--------|------------------------|
| 2 | 100% (cluster inicial) |
| 3 | 80% (CR-014 baja FTR) |
| 4 | 80% |
| 5 | 91% (5 nuevos OK) |
| 6 | 88% (CR-010 baja con restricciones) |
| 7 | 90% |
| 8 | 91% (objetivo cumplido) |

### M3 — Lead Time por sitio

**Definición:** Tiempo desde entrada al Backlog hasta Done.

**Cómo se mide:** Diferencia de timestamps en Jira.

**Meta:** Promedio ≤ 12 días.

**Proyección esperada:**

| Tipo de sitio | Lead time esperado |
|---|---|
| Corredor / Urbano simple | 7-9 días |
| Urbano denso | 10-12 días |
| Suburbano | 9-11 días |
| Casos con bloqueo | 14-18 días |

### M4 — Cycle Time

**Definición:** Tiempo desde "Listo para Ventana" hasta Done.

**Meta:** ≤ 5 días promedio.

**Proyección:** 3-5 días en sitios sin bloqueo, hasta 7 con bloqueo.

### M5 — Cumplimiento de DoR al primer intento

**Definición:** % de sitios que cumplen DoR sin requerir iteraciones.

**Cómo se mide:** Validación de Carlos + Eduardo en reunión semanal de peers.

**Meta:** ≥ 85%.

### M6 — Bloqueos activos

**Definición:** Sitios bloqueados en cualquier momento del proyecto.

**Cómo se mide:** Reporte en Jira con tag "blocked".

**Meta:** ≤ 2 bloqueos activos simultáneos en promedio.

### M7 — Tiempo de resolución de bloqueos

**Definición:** Tiempo entre marcar bloqueado y marcar resuelto.

**Meta:** ≤ 72h en el 80% de los casos.

---

## Métricas de equipo (Subcompetencia 3.2)

### M8 — Participación en dailies

**Definición:** Asistencia a daily Kanban.

**Cómo se mide:** Carlos registra asistencia silenciosamente.

**Meta general:** ≥ 85% por miembro.

**Meta específica para Sandeep (India):** ≥ 80% considerando TZ adversa.

### M9 — Transiciones en Jira vs WhatsApp

**Definición:** % de cambios de estado que ocurren en Jira (no por chat).

**Meta:** ≥ 95%.

### M10 — Conflictos escalados al CPM

**Definición:** Conteo absoluto de issues escalados por encima de Carlos o Eduardo.

**Meta:** Tendencia decreciente, ideal ≤ 2 en todo el proyecto.

### M11 — Reconocimientos públicos

**Definición:** Menciones explícitas a cuadrillas, integradores u optimizadores en reportes semanales.

**Meta:** ≥ 1 por semana.

---

## Métricas técnicas (de KPIs de red)

Estas métricas se miden post-integración en EMA por sitio:

| KPI | Umbral aceptación | Quién mide |
|---|---|---|
| **DL Throughput (Mbps)** | Varía por tipo | Marco / Sofía / Patricia |
| **UL Throughput (Mbps)** | Varía por tipo | Optimizador |
| **PRB Utilization** | Patrón esperado | Optimizador |
| **DCR (Drop Call Rate)** | ≤ baseline | Optimizador |
| **HO Success Rate** | ≥ 98% | Optimizador |
| **Alarmas críticas** | 0 sostenidas | Integrador + NOC |

---

## Cadencia de reporting

### Diario — Daily Kanban (15 min)

- Estado del tablero
- Bloqueos
- Decisiones

**Audiencia:** Equipo completo (Ericsson + cuadrillas)

### Semanal — Reporte a Telemóvil (lunes EOD)

Lo más importante: **reportes diferenciados por área de Telemóvil**:

| Audiencia Telemóvil | Contenido del reporte |
|---|---|
| **Roberto (RAN)** | KPIs técnicos por sitio, observaciones de template |
| **Marcela (Planning)** | Sitios completados, capacidad agregada, saturación reducida |
| **Patricia (Quality)** | KPIs validados, calidad de aceptación |
| **Fernando (O&M)** | Sitios entregados a operación, alarmas, handover status |
| **Ricardo Mendoza (Acceptance)** | Sitios pendientes de aceptación, agenda batch semanal |

### Bi-semanal — Reporte ejecutivo a sponsors

- Avance global (X/23 sitios)
- FTR acumulado
- Top 3 riesgos
- Decisiones de re-priorización significativas

**Audiencia:** Sponsors de Telemóvil (CTO, COO) y leadership Ericsson

### Mensual — Reporte interno Ericsson

- Salud del equipo
- Métricas de equipo (M8-M11)
- Lecciones aprendidas en curso

---

## Cómo se visualiza el burndown

```
Sitios pendientes (decremento ideal)

23 ●
   |\\
22 | ●
   |  \
20 |   ●
   |    \
17 |     ●
   |      \
12 |       ●
   |        \
 6 |         ●
   |          \
 1 |           ●
 0 +────────────●─────► Semanas
   1  2  3  4  5  6  7  8

Línea ideal: pendiente uniforme
Línea real (proyectada): paso desigual, mayor descenso en sem 5-6 (despliegue masivo)
```

🔶 **[VALIDAR CON CARLOS]:** Carlos puede usar este formato en su presentación, llenando con datos reales conforme avance el proyecto.

---

## Indicadores de adherencia al Acuerdo de Equipo

| Indicador | Cómo se mide | Meta |
|---|---|---|
| Decisiones en Jira | Auditoría semanal | ≥ 95% |
| Asistencia daily | Conteo Carlos | ≥ 85% |
| Sandeep participación | Conteo específico | ≥ 80% |
| Reconocimientos a cuadrillas | Conteo en reportes | ≥ 1/sem |
| Conflictos escalados | Conteo absoluto | ≤ 2 total |

---

## Mapeo de Subcompetencias

- **1.5 Metrics & Reporting:** este documento ES la columna vertebral
- **1.4 Lean & Kanban:** métricas alimentadas por el flujo Kanban
- **1.1 Planeación Adaptativa:** las métricas son input al refresh de plan

## Preguntas para Carlos

1. ¿Las metas (FTR 90%, lead time 12 días) son ambiciosas y realistas o ajustar?
2. ¿Los reportes diferenciados por área Telemóvil son viables o demasiado granulares?
3. ¿Hay alguna métrica técnica de KPIs específica de Telemóvil que omití?

---

**Siguiente:** [[Risk-Register]]
