---
title: Plan de Calidad
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.5, 2.1, 3.3]
tags: [calidad, dod, ftr, validacion]
---

# Plan de Calidad del Proyecto

> 🎯 **Documento de diseño** — proyecto en fase de planeación.

## Propósito

Definir el sistema de aseguramiento de calidad del proyecto. La calidad no es un evento al final, sino una práctica continua incorporada al flujo Kanban.

---

## Filosofía de calidad

### Build quality in, don't inspect it at the end

La calidad se construye sitio por sitio, no se verifica al final del proyecto. Esto se traduce en:
- DoD multi-nivel por sitio (técnica, operativa, cliente)
- Validación 24-72h post-integración por Optimizadores
- Sign-off batch semanal con Telemóvil (no acumulación al final)
- Quality (Patricia Telemóvil) involucrada desde el cluster

### First Time Right como métrica central

FTR es el indicador líder de calidad. Meta del proyecto: **≥ 90% FTR**.

---

## Dimensiones de calidad

### Dimensión 1 — Calidad técnica de integración

**Owner:** Carlos + Diego (Integradores Lead)

**Aplicación del template:**
- Template aprobado por Roberto (Telemóvil) antes de aplicar
- Pre-stage en ENM 24h antes de la ventana
- Post-aplicación: pre-checks automáticos exitosos
- Sin alarmas críticas sostenidas

**Configuración:**
- Variantes del template documentadas por tipo de sitio
- Cualquier desviación del template documentada en el ticket

### Dimensión 2 — Calidad de KPIs (optimización)

**Owner:** Marco (Optimizadores Lead) + Patricia Telemóvil

**Validación post-integración:**
- Periodo de 24-48h en sitios urbanos
- Periodo de 72h en sitios suburbanos (ajustado tras retrospectiva del cluster)
- KPIs dentro de umbrales definidos por Telemóvil
- Sin degradación de KPIs en vecinos

**Documentación:**
- Snapshot de KPIs antes y después en el SAD
- Comparación pre/post integración

### Dimensión 3 — Calidad de implementation física

**Owner:** Eduardo (peer) + Líderes de cuadrilla

**HW instalado:**
- Instalación según diseño
- Fotos de evidencia subidas al ticket
- Mediciones de RF dentro de tolerancia
- Conexiones validadas (RRU, antenas, fibra)

**Seguridad:**
- Protocolos de seguridad cumplidos
- Sin incidentes durante el trabajo
- Equipo certificado para trabajo en altura

### Dimensión 4 — Calidad de aceptación cliente

**Owner:** Carlos + Ricardo Mendoza (Acceptance Telemóvil)

**Sign-off de las 5 áreas Telemóvil:**
- RAN Engineering (Roberto) — configuración correcta
- Planning (Marcela) — capacidad entregada
- Quality (Patricia) — KPIs validados
- O&M (Fernando) — handover recibido
- Acceptance Team (Ricardo Mendoza) — sign-off formal

### Dimensión 5 — Calidad de documentación

**Owner:** Carlos + Optimizadores asignados

**Site Acceptance Document (SAD):**
- Configuración aplicada
- KPIs pre/post integración
- Observaciones del sitio
- Lecciones específicas si aplica

**Confluence del proyecto:**
- Template versionado (v1, v2)
- Risk register actualizado
- Retrospectivas documentadas
- Decisiones de re-priorización registradas

---

## Procesos de aseguramiento de calidad

### Proceso 1 — Validación de DoR

**Cuándo:** Antes de mover sitio a "Listo para Ventana"

**Quién:** Carlos + Eduardo en reunión semanal de peers

**Qué se valida:** Las dos partes de la DoR (ver `[[Definition-of-Ready]]`)

**Output:** Sitio pasa o se identifica gap específico

### Proceso 2 — Validación durante integración

**Cuándo:** Durante la ventana de mantenimiento

**Quién:** Integrador remoto + Líder de cuadrilla local

**Qué se valida:**
- SW aplicado correctamente vía ENM
- HW instalado físicamente (cuadrilla aporta evidencia)
- Sin alarmas críticas

**Output:** Sitio listo para optimización

### Proceso 3 — Validación post-integración (24-72h)

**Cuándo:** En las 24-72h posteriores a la ventana

**Quién:** Optimizador asignado

**Qué se valida:**
- KPIs dentro de umbrales
- Sin degradación de vecinos
- Estabilidad de la configuración

**Output:** Sitio listo para aceptación o regresa a optimización

### Proceso 4 — Sesión de aceptación batch semanal

**Cuándo:** Viernes de cada semana

**Quién:** Carlos + Ricardo Mendoza (Acceptance) + áreas relevantes Telemóvil

**Qué se valida:** Sitios "Listos para Aceptación" cumplen DoD multi-nivel

**Output:** Sign-off formal o regreso a corrección

### Proceso 5 — Retrospectivas de calidad

**Cuándo:** Semana 4 (cluster) + semana 8 (final) + mensual interno

**Quién:** Equipo completo + Telemóvil selectivamente

**Qué se revisa:** Patrones de calidad, FTR, áreas de mejora

**Output:** Acciones de mejora aplicadas

---

## Indicadores de calidad

| Indicador | Definición | Frecuencia | Meta |
|---|---|---|---|
| **FTR (%)** | Sitios aceptados al primer intento | Semanal acumulado | ≥ 90% |
| **Sitios rechazados** | Por área Telemóvil | Por sesión aceptación | ≤ 1 por sesión |
| **Re-trabajos** | Horas-hombre en correcciones | Acumulado | Tendencia decreciente |
| **Alarmas post-aceptación** | Alarmas en 7 días post-Done | Por sitio | 0 |
| **Cumplimiento DoR primer intento** | Sitios DoR sin iteración | Semanal | ≥ 85% |

---

## Roles y responsabilidades de calidad

| Rol | Responsabilidad de calidad |
|---|---|
| **Carlos (NPM)** | Owner global de calidad del flujo Carlos |
| **Eduardo (peer)** | Owner de calidad del flujo Implementation |
| **Integradores** | Calidad técnica de aplicación del template |
| **Optimizadores** | Calidad de KPIs y validación post-integración |
| **Líderes de cuadrilla** | Calidad de instalación física |
| **Patricia (Telemóvil Quality)** | Validación cruzada de calidad de KPIs |
| **Ricardo Mendoza (Telemóvil Acceptance)** | Sign-off formal por sitio |

---

## Manejo de no-conformidades

### Clasificación

| Tipo | Severidad | Acción |
|---|---|---|
| **Crítica** | Sitio en producción con falla mayor | Rollback inmediato, escalación |
| **Mayor** | Sitio no cumple umbral de KPI | Regresa a Optimización |
| **Menor** | Observación cosmética, documentación | Se corrige sin retrasar acceptance |

### Documentación

Cada no-conformidad se documenta con:
- Sitio afectado
- Tipo y descripción
- Acción correctiva
- Lección aprendida (si aplica)

---

## Mejora continua del Plan de Calidad

Este plan no es estático. Se ajusta:
- Después del Golden Cluster (sem 4): ajustes basados en retrospectiva
- A mitad del proyecto (sem 6): mini-revisión
- Al cierre (sem 8): lecciones consolidadas

---

## Mapeo de Subcompetencias

- **1.5 Metrics & Reporting:** indicadores de calidad
- **2.1 Continuous Improvement:** mejora continua del plan
- **3.3 Gestión de Involucrados:** Patricia (Quality) y Ricardo Mendoza (Acceptance) integrados

## Preguntas para Carlos

1. ¿La meta FTR ≥ 90% es alcanzable?
2. ¿Las 5 dimensiones cubren todo o falta alguna?
3. ¿Patricia Telemóvil realmente está dispuesta a involucrarse desde el cluster?

---

**Anterior:** [[Risk-Register]]
