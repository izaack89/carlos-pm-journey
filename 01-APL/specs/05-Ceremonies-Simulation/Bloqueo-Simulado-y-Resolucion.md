---
title: Bloqueo Simulado y Resolución
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.2, 1.1, 3.2]
tags: [simulacion, bloqueo, riesgo, resolucion]
---

# Bloqueo Simulado y Resolución

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación. Escenario plausible esperado durante el Golden Cluster.

## Propósito

Mostrar cómo el equipo manejará un bloqueo real durante la ejecución, aplicando subcompetencia **1.2 Detección y Resolución de Riesgos y Problemas**. Esta narrativa retrata un caso concreto con cronología, decisiones y aprendizajes.

---

## El bloqueo simulado — Caso CR-014 San Miguelito

### Día 1 del bloqueo — Martes 16 de junio (sem 3)

**Contexto:** Sitio CR-014 (San Miguelito, suburbano) integrado durante la noche del lunes 15.
- **Cuadrilla en sitio:** Cuadrilla 3 (Ricardo) bajo coordinación de Eduardo
- **Integrador remoto:** Ana
- **Optimizadora asignada:** Marco (a pesar de ser senior, este sitio le toca por rotación)

Marco corre la validación inicial el martes en la mañana desde Mexico (remoto).

**Hallazgo:** Throughput DL del sector beta (orientación norte) está consistentemente 8% por debajo del umbral esperado. Otros KPIs (PRB utilization, handover success) están dentro de rango.

**Marco reporta en Jira:**
> "CR-014 — Beta sector with DL throughput = 92 Mbps. Expected threshold: ≥100 Mbps. Other KPIs OK. No critical alarms. Suspect RF propagation factor."

**Marcado como bloqueado.**

### Día 1 — Daily Kanban

(Ver `[[Daily-Kanban-Sample]]` para la transcripción completa)

Carlos asigna a Sofía (otra optimizadora con experiencia en RF) para apoyar a Marco. Deadline: jueves EOD.

### Día 2 — Miércoles 17

**Mañana:** Sofía (desde Argentina) revisa el plan de RF original del sitio vs el escenario actual.

**Hallazgo de Sofía:** El plan de RF es de hace 6 meses. Desde entonces se construyó un edificio nuevo de 12 pisos a ~200m al norte del sitio, causando reflexión y posible interferencia.

**Sofía en Jira:**
> "Confirmed Marco's hypothesis. New building not contemplated. Options: (a) adjust electrical tilt of north antenna from -2° to -4°, (b) reduce beta sector power by 1 dB to mitigate interference, (c) both."

### Día 2 — Tarde

Sofía y Marco discuten vía Teams:

**Marco:** "Option A or C?"

**Sofía:** "Try A first. Adjusting tilt is reversible via ENM in 5 min. If it doesn't resolve, add option B."

**Acción:** Marco notifica a Diego (integrador disponible) para hacer el ajuste vía ENM. Diego confirma a Eduardo (peer) y al NOC Telemóvil que harán un cambio no disruptivo de configuración.

**Resultado preliminar:** Tilt ajustado a las 16:00. Esperan 4 horas para que los KPIs estabilicen.

### Día 2 — Noche

A las 20:00, Marco revisa los KPIs en EMA.

**Throughput DL sector beta:** 96 Mbps. Mejora pero aún por debajo del umbral.

**Decisión:** Aplicar también la opción B (reducción de 1 dB). Diego ejecuta el cambio. Notificación al NOC.

### Día 3 — Jueves 18

**Mañana:** Marco revisa los KPIs nuevamente.

**Throughput DL sector beta:** 103 Mbps. ✅ Sobre el umbral.

**Validación adicional:** Marco verifica que no haya degradación en sitios vecinos. Confirma: ningún vecino afectado.

**Validación de Patricia (Telemóvil Quality):** Patricia revisa también desde su dashboard. Aprueba.

**Marco marca el bloqueo como resuelto.**

### Día 3 — Daily Kanban

**Marco en daily:** "CR-014 resolved. KPIs in green. Moving to 'Ready for Acceptance'."

**Carlos:** "Excellent. FTR positive or negative?"

**Marco:** "Technically, FTR negative. Required 2 post-integration adjustments."

**Carlos:** "OK. Logging FTR=False. Learning?"

**Marco:** "RF plan is 6 months old. Worth a freshness check before integration. That should go to pre-checks template."

**Patricia (Junior optimizadora):** "Carlos, I followed Marco's process step by step. Documented for the lessons learned."

**Carlos:** "Excellent contribution Patricia. Goes to cluster retrospective."

🟢 **Bloqueo resuelto en ~56 horas (3 días). Aprendizaje capturado.**

---

## Anatomía del manejo del bloqueo

### Lo que se hizo bien

1. **Detección temprana** — Marco identificó el issue 24h post-integración
2. **Asignación rápida de apoyo** — Sofía entró al caso el mismo día via daily
3. **Deadline explícito** — Carlos puso jueves EOD como límite
4. **Colaboración remota efectiva** — Marco (México), Sofía (Argentina), Diego (Costa Rica) coordinándose vía Jira + Teams
5. **Patricia Telemóvil involucrada** — validación cruzada antes de cerrar
6. **Eduardo (peer) informado** — no se necesitó cuadrilla pero estaba en stand-by
7. **Aprendizaje capturado** — Patricia (Junior) documentó el proceso

### Lo que se pudo mejorar

1. **El plan de RF desactualizado** debió detectarse en pre-checks (input para mejorar la DoR)
2. **El umbral de "esperado"** no estaba completamente claro al inicio — input para refinar la DoD

### Indicadores cuantitativos del caso

| Indicador | Valor |
|-----------|-------|
| Tiempo entre integración y detección | 12h |
| Tiempo entre detección y asignación de apoyo | 2h (siguiente daily) |
| Tiempo entre asignación y diagnóstico | 24h |
| Tiempo entre diagnóstico y aplicación de fix | 4h |
| Tiempo entre fix y validación final | 14h |
| **Lead time total del bloqueo** | **~56h (2.3 días)** |
| FTR del sitio | False |
| Personas involucradas | 5 (Marco, Sofía, Diego, Eduardo, Patricia Telemóvil) |
| Ubicaciones involucradas | 4 (México, Argentina, Costa Rica, Costa Rica) |

---

## Comparativa: ¿qué hubiera pasado en modelo tradicional?

| Dimensión | Tradicional | Ágil (Kanban distribuido) |
|-----------|-------------|---------------------------|
| **Cuándo se hubiera detectado** | En aceptación final del proyecto (semana 8) | 24h post-integración (semana 3) |
| **Quién lo hubiera resuelto** | Equipo de optimización post-deployment | Marco + Sofía + Diego en flujo |
| **Costo de re-trabajo** | Alto (regresar al sitio, escalación con cliente) | Bajo (ajuste vía ENM, sin re-visita) |
| **Aprendizaje** | Probablemente perdido en el ruido del cierre | Capturado por Junior optimizadora, aplicado a próximos sitios |
| **Visibilidad para Telemóvil** | Sorpresa en aceptación | Reportado proactivamente a Patricia |
| **Coordinación con peer (Implementation)** | No aplicable o reactiva | Eduardo informado, en stand-by |

**Valor del enfoque ágil en este caso:** detección temprana + resolución estructurada + aprendizaje sistemático + coordinación distribuida fluida.

---

## Otros tipos de bloqueos típicos esperados

Estos son los bloqueos más comunes que el proyecto puede enfrentar:

### Bloqueos físicos (mayoritariamente owner: Eduardo)

| Bloqueo | Owner principal | Tiempo típico esperado |
|---------|-----------------|------------------------|
| Energía no conectada | Eduardo | 24-72h (depende de ICE) |
| Permiso municipal pendiente | CPM + Eduardo | Variable |
| Acceso a torre denegado | Eduardo | 24-48h |
| HW faltante en sitio | Eduardo | 24-48h |
| Materiales civiles incompletos | Líder de cuadrilla | Mismo día |

### Bloqueos técnicos (mayoritariamente owner: Carlos)

| Bloqueo | Owner principal | Tiempo típico esperado |
|---------|-----------------|------------------------|
| Template requiere ajustes | Carlos + Integradores + Roberto | 24-72h |
| Alarmas críticas persistentes | Integrador asignado | 12-48h |
| KPIs bajo umbral | Optimizador + Patricia Telemóvil | 24-72h (como CR-014) |
| Interferencia con sitios vecinos | Optimizadores + Roberto (Telemóvil) | 48-96h |
| Software incompatible | Integrador | 48-96h |

### Bloqueos de coordinación cruzada

| Bloqueo | Owner | Tiempo típico esperado |
|---------|-------|------------------------|
| Issue cruzado HW/SW durante ventana | Carlos + Eduardo (peers) | Mismo día |
| Cuadrilla y Integrador con diferentes interpretaciones | Carlos + Eduardo | 24h |
| Disponibilidad de Sandeep (India) en TZ Costa Rica | Carlos | Coordinación previa |

### Bloqueos con cliente (5 áreas Telemóvil)

| Bloqueo | Owner | Tiempo típico esperado |
|---------|-------|------------------------|
| Ventana de NOC no disponible (Fernando) | Carlos | 24-48h |
| Cambio de prioridades (Marcela) | Carlos + Marcela | Inmediato |
| Quality rechaza sitio (Patricia) | Carlos + Marco | 24-72h |
| Acceptance rechaza sitio (Ricardo Mendoza) | Carlos | 24-72h |
| RAN observa (Roberto) | Carlos + Integradores | 24-48h |

---

## Protocolo de escalación

| Tiempo del bloqueo | Acción |
|--------------------|--------|
| 0-24h | Visible en tablero, asignado en daily |
| 24-48h | Mencionado en daily como riesgo activo |
| 48-72h | Escalación formal al CPM |
| 72+h | Escalación al CSM, comunicación al cliente |
| 7+ días | Riesgo crítico, comité ad-hoc con sponsors |

### Escalación entre peers

Si Carlos detecta un bloqueo que depende de Eduardo (o viceversa):
1. Comunicación inmediata entre peers (Teams o llamada)
2. Si no se resuelve en 4 horas, se escala al CPM
3. Decisiones que afectan a ambos equipos se toman conjuntamente

---

## Métricas de gestión de bloqueos

Para alimentar el `[[Burndown-y-Metricas]]`:

| Métrica | Definición | Meta |
|---------|-----------|------|
| **Tiempo promedio de resolución** | Tiempo entre detección y resolución | <72h |
| **% de bloqueos resueltos en <48h** | Indicador de agilidad | ≥80% |
| **Bloqueos recurrentes** | Mismos patrones que se repiten | Tendencia a 0 |
| **Bloqueos escalados al CPM** | Cuántos requirieron escalación | <20% |
| **Bloqueos cruzados (Carlos↔Eduardo)** | Coordinación peer | Resueltos sin escalación |

---

## Mapeo de Subcompetencias

- **1.2 Detección y Resolución de Riesgos y Problemas:** este documento ES la demostración práctica
- **1.1 Planeación Adaptativa:** el bloqueo causa ajuste en el plan sin descarrilar el proyecto
- **3.2 Equipo de Alto Desempeño:** el equipo distribuido colabora eficientemente

---

**Siguiente:** [[Retrospectiva-Golden-Cluster]]
**Anterior:** [[Daily-Kanban-Sample]]
