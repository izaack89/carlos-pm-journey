---
title: Definition of Done — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.5, 3.3]
tags: [dod, calidad, ftr, agile]
---

# Definition of Done (DoD)

> 🎯 **Documento de diseño** — proyecto en fase de planeación. La DoD se acuerda con Patricia (Quality Telemóvil), Ricardo Mendoza (Acceptance Telemóvil) y Roberto (RAN Telemóvil) antes del kickoff.

## Propósito

Establecer qué significa que un sitio esté **completo**. La DoD es el criterio único compartido entre el equipo de Carlos, el equipo de Eduardo, y Telemóvil (5 áreas) para evitar disputas y re-trabajos. Se vincula directamente con la métrica **First Time Right (FTR)**.

---

## Estructura de la DoD

La DoD tiene tres niveles:

1. **DoD Técnica** — criterios objetivos de configuración y KPIs (owner: Carlos)
2. **DoD Operativa** — documentación y handover (owner: Carlos + Eduardo)
3. **DoD Cliente** — aceptación formal por Telemóvil (5 áreas distintas)

---

## Nivel 1 — DoD Técnica

### Integración (responsabilidad del Integrador)

- ☐ **Configuración aplicada exitosamente vía ENM** sin errores
- ☐ **Pre-checks post-integración OK:** cell up, software version correcta, license OK
- ☐ **Sin alarmas críticas (categoría 1-2) sostenidas** después de 1h post-integración
- ☐ **ANR operativo:** relaciones de vecinos auto-configuradas
- ☐ **Features activadas según template:** Lean Carrier, MIMO, CA si aplica

### Validación HW (responsabilidad de la Cuadrilla + Eduardo)

- ☐ **Instalación física de HW** validada (RRU, antenas, cables, conectores)
- ☐ **Fotos de evidencia** subidas al ticket
- ☐ **Mediciones de RF** dentro de tolerancia
- ☐ **Sin observaciones civiles pendientes**

### KPIs (responsabilidad del Optimizador asignado)

🔶 **[VALIDAR CON CARLOS]:** Umbrales específicos por confirmar contra estándares de Telemóvil.

- ☐ **DL Throughput** ≥ umbral de aceptación del sitio (varía por tipo)
- ☐ **UL Throughput** ≥ umbral de aceptación
- ☐ **PRB Utilization en patrón esperado:** capacidad disponible para absorber demanda
- ☐ **Drop Call Rate (DCR)** ≤ baseline pre-integración
- ☐ **Handover Success Rate** ≥ 98%
- ☐ **RSRP, RSRQ, SINR** dentro de rangos esperados en el área de cobertura
- ☐ **Sin degradación de KPIs en sitios vecinos** (validación de no causar interferencia)
- ☐ **Validación en periodo de 24-48h** para que los KPIs estabilicen

---

## Nivel 2 — DoD Operativa

### Documentación

- ☐ **Site Acceptance Document (SAD) generado** y cargado en Confluence
- ☐ **Configuración final exportada** y almacenada (snapshot post-integración)
- ☐ **Log de cambios documentado** en el ticket del sitio
- ☐ **Fotos de evidencia HW** completas (cuadrilla aporta)
- ☐ **Lecciones aprendidas del sitio** capturadas si aplica

### Handover a operación

- ☐ **NOC Telemóvil notificado** de que el sitio está en producción (vía Fernando)
- ☐ **Sitio incluido en monitoreo continuo** post-aceptación
- ☐ **Managed Services notificado** si aplica

---

## Nivel 3 — DoD Cliente (aceptación Telemóvil)

Telemóvil tiene **5 áreas con criterios distintos** que deben dar sign-off:

### Área 1 — RAN Engineering (Roberto)

- ☐ Template aplicado según diseño aprobado
- ☐ Configuración de features correcta
- ☐ Plan de vecindades validado

### Área 2 — Planning (Marcela)

- ☐ Sitio entrega capacidad esperada según diseño
- ☐ KPIs alineados con proyección de absorción de demanda

### Área 3 — Quality (Patricia)

- ☐ KPIs cumplen estándares Telemóvil
- ☐ Validación en periodo extendido OK
- ☐ Documentación de calidad completa

### Área 4 — O&M (Fernando)

- ☐ Handover formal recibido
- ☐ Sin alarmas pendientes post-aceptación
- ☐ Acceso a sitio funcional para operación

### Área 5 — Acceptance Team (Ricardo Mendoza)

- ☐ Todos los anteriores firmados
- ☐ SAD completo y consistente
- ☐ Sign-off formal en sesión semanal de aceptación

---

## First Time Right (FTR) — Definición operativa

**FTR = TRUE** si:

- El sitio cumple **todos los criterios técnicos** (Nivel 1) al primer intento
- **No hubo re-trabajos** entre integración y aceptación
- **No se requirió ajuste de configuración** post-integración para alcanzar umbrales de KPIs
- **Aceptado por las 5 áreas de Telemóvil** sin observaciones críticas

**FTR = FALSE** si:

- Cualquier criterio técnico requiere segunda intervención
- Se requiere ajuste de parámetros para alcanzar KPIs
- **Cualquiera de las 5 áreas Telemóvil rechaza** la aceptación y solicita correcciones

### Observaciones menores

Observaciones cosméticas o de documentación que no afectan operación NO bajan el FTR. Solo afectan FTR los issues que requieren intervención técnica de re-trabajo.

### Meta del proyecto

**FTR ≥ 90%** en el conjunto de los 23 sitios.

🔶 **[VALIDAR CON CARLOS]:** En proyectos similares el baseline histórico ha sido 82-88%. La meta de 90% es ambiciosa pero defendible como objetivo del enfoque ágil.

---

## Tabla resumen: DoR vs DoD

| Dimensión | DoR (Ready) | DoD (Done) |
|---|---|---|
| **Cuándo aplica** | Antes de entrar a "Listo para Ventana" | Antes de mover a "Done" |
| **Owner principal** | Carlos + Eduardo (peers) | Carlos + 5 áreas Telemóvil |
| **Foco** | Preconditions de planeación | Resultados de ejecución |
| **Naturaleza** | Lo que se necesita para empezar | Lo que se cumple para terminar |
| **Métrica asociada** | % DoR cumplido al primer intento | FTR (First Time Right) |

---

## Cómo se hace la validación de DoD

### Paso 1 — Auto-validación durante integración

Durante la ventana, el Integrador y la Cuadrilla marcan los checks técnicos respectivos en el ticket del sitio en Jira.

### Paso 2 — Validación del Optimizador

El Optimizador asignado accede a EMA, extrae los KPIs del sitio en las primeras 24-48h post-integración, y valida que estén dentro de umbrales. Si no, el sitio regresa a "Optimización" para ajustes.

### Paso 3 — Validación final de Carlos

Carlos hace check final antes de mover el sitio a "Listo para Aceptación":
- Confirma que los 3 niveles de DoD están cumplidos
- Valida que el SAD esté completo
- Coordina notificación a Fernando (O&M Telemóvil)

### Paso 4 — Sesión de aceptación con Telemóvil

En la sesión semanal de aceptación con Ricardo Mendoza (Acceptance Team) y las áreas relevantes, se revisan los sitios listos. Aprobación formal mueve el sitio a "Done".

### Paso 5 — Handover a O&M

Después de sign-off, Fernando confirma recepción y el sitio entra a monitoreo continuo.

---

## Métricas alimentadas por la DoD

| Métrica | Definición | Frecuencia de medición |
|---------|-----------|----------------------|
| **FTR (%)** | Sitios aceptados al primer intento / sitios procesados | Semanal y acumulado |
| **Cycle time** | Tiempo desde "Listo para Ventana" hasta Done | Por sitio |
| **Lead time** | Tiempo desde entrada al Backlog hasta Done | Por sitio |
| **Rechazo de Telemóvil** | Sitios rechazados / sitios presentados (por área) | Por sesión semanal |
| **Re-trabajos** | Horas-hombre invertidas en correcciones post-integración | Acumulado |

Detalle completo en `[[Burndown-y-Metricas]]`.

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** la DoD es la salida del flujo, criterio único compartido
- **1.5 Metrics & Reporting:** FTR y otras métricas derivadas de la DoD
- **3.3 Gestión de Involucrados:** la DoD se construye con las 5 áreas de Telemóvil, no impuesta

## Preguntas para Carlos

1. ¿Los criterios técnicos descritos son completos para tu workflow real?
2. ¿La meta de FTR ≥ 90% es realista o ajustar?
3. ¿Las 5 áreas de Telemóvil firman cada sitio o algunas son meramente informativas?
4. ¿El periodo de validación post-integración (24-48h) es adecuado para que los KPIs estabilicen?
5. ¿Patricia (Quality) requiere periodo extendido (>48h) o el mismo periodo aplica?

---

**Siguiente:** [[Acuerdo-de-Equipo]]
**Anterior:** [[Definition-of-Ready]]
