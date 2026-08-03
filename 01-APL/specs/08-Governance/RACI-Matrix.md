---
title: RACI Matrix
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [3.3, 3.2, 1.4]
tags: [raci, governance, roles]
---

# RACI Matrix

> 🎯 **Documento de diseño** — proyecto en fase de planeación.

## Propósito

Clarificar quién es Responsable, Accountable, Consultado e Informado para las actividades clave del proyecto. Es especialmente importante porque hay **dos peers (Carlos + Eduardo)** y **5 áreas distintas en Telemóvil**.

---

## Convenciones

- **R = Responsible:** quien ejecuta el trabajo
- **A = Accountable:** quien rinde cuentas finales (solo uno por fila)
- **C = Consulted:** quien aporta input
- **I = Informed:** quien debe saber el resultado

---

## Actores del proyecto

### Ericsson
| Sigla | Rol |
|---|---|
| CPM | Customer Project Manager |
| CSM | Customer Success Manager |
| **NPM** | Network Performance Manager — **Carlos** (participante) |
| **IM** | Implementation Manager — **Eduardo** (peer de Carlos) |
| Int-L | Integrador Lead (Diego) |
| Int | Integradores (Ana, Sandeep, Hugo) |
| Opt-L | Optimizador Lead (Marco) |
| Opt | Optimizadores (Sofía, Patricia Ericsson) |
| Cdrl-L | Líderes de Cuadrilla (Luis, Javier, Ricardo) |

### Telemóvil Costa Rica
| Sigla | Rol |
|---|---|
| LIB-RAN | RAN Engineering — Roberto |
| LIB-PLAN | Planning — Marcela |
| LIB-QA | Quality — Patricia |
| LIB-O&M | O&M — Fernando |
| LIB-ACC | Acceptance Team Lead — Ricardo Mendoza |
| LIB-EXEC | Sponsors ejecutivos Telemóvil |

---

## Matriz RACI por actividad

### Fase 1 — Setup del proyecto

| Actividad | CPM | CSM | NPM | IM | Int-L | Opt-L | Cdrl-L | LIB-RAN | LIB-PLAN | LIB-QA | LIB-O&M | LIB-ACC | LIB-EXEC |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Definir alcance del proyecto | A | C | R | C | C | C | I | C | C | C | C | C | C |
| Kickoff meeting | R | R | R | R | I | I | I | C | C | C | C | C | I |
| Configurar Kanban en Jira | I | I | A/R | C | I | I | I | I | I | I | I | I | - |
| Firmar Acuerdo de Equipo | I | I | R | R | R | R | R | I | I | I | I | I | - |
| Validar template B41 inicial | I | I | A | I | R | C | I | R | C | C | I | I | - |

### Fase 2 — Operación diaria del Kanban

| Actividad | CPM | CSM | NPM | IM | Int-L | Opt-L | Cdrl-L | LIB-RAN | LIB-PLAN | LIB-QA | LIB-O&M | LIB-ACC | LIB-EXEC |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Facilitar Daily Kanban | I | I | A/R | C | C | C | C | I | I | I | I | I | - |
| Pre-stage del template (por sitio) | I | I | A | I | R | I | I | I | I | I | I | I | - |
| Site readiness (HW, energía, fibra) | I | I | I | A | I | I | R | I | I | I | C | I | - |
| Aplicación del template en ventana | I | I | A | C | R | I | C | I | I | I | C | I | - |
| Trabajo físico en sitio (HW) | I | I | I | A | C | I | R | I | I | I | C | I | - |
| Validación de KPIs post-integración | I | I | A | I | I | R | I | I | I | C | I | I | - |
| Documentación SAD por sitio | I | I | A | C | C | R | I | I | I | I | I | I | - |
| Aceptación batch semanal | I | I | A/R | C | I | I | I | C | C | C | C | R | I |
| Re-priorización semanal | I | I | A/R | C | I | C | I | C | R | I | I | I | - |
| Reunión semanal peers (Carlos-Eduardo) | I | - | R | R | - | - | - | - | - | - | - | - | - |
| Reporte semanal a Telemóvil (5 áreas) | I | I | A/R | C | I | C | I | I | I | I | I | I | - |
| Reporte ejecutivo bi-semanal | I | A | R | C | I | I | I | I | I | I | I | I | I |

### Fase 3 — Gestión de riesgos y bloqueos

| Actividad | CPM | CSM | NPM | IM | Int-L | Opt-L | Cdrl-L | LIB-RAN | LIB-PLAN | LIB-QA | LIB-O&M | LIB-ACC | LIB-EXEC |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Identificación de bloqueos técnicos | I | I | A | C | R | R | I | C | I | I | I | I | - |
| Identificación de bloqueos físicos | I | I | C | A | I | I | R | I | I | I | C | I | - |
| Resolución de bloqueos cruzados HW/SW | C | I | A/R | A/R | C | C | C | I | I | I | I | I | - |
| Mantenimiento del Risk Register | I | I | A/R | C | C | C | I | C | C | C | C | C | - |
| Escalación a CPM | - | I | R | R | I | I | I | I | I | I | I | I | I |
| Escalación a CSM | I | A | R | R | I | I | I | I | I | I | I | I | I |

### Fase 4 — Calidad y aceptación

| Actividad | CPM | CSM | NPM | IM | Int-L | Opt-L | Cdrl-L | LIB-RAN | LIB-PLAN | LIB-QA | LIB-O&M | LIB-ACC | LIB-EXEC |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| DoR validación (multi-parte) | I | I | A/R | A/R | C | I | C | I | I | I | I | I | - |
| DoD nivel técnico | I | I | A | I | R | R | C | I | I | I | I | I | - |
| DoD nivel operativo (handover) | I | I | A | A | C | C | C | I | I | I | R | I | - |
| Sign-off técnico Telemóvil | I | I | R | I | C | C | I | R | I | I | I | I | - |
| Sign-off calidad Telemóvil | I | I | C | I | I | C | I | I | I | R | I | I | - |
| Sign-off planning Telemóvil | I | I | C | I | I | I | I | I | R | I | I | I | - |
| Sign-off O&M Telemóvil | I | I | C | C | I | I | I | I | I | I | R | I | - |
| Sign-off final aceptación Telemóvil | I | I | C | C | I | I | I | C | C | C | C | A/R | I |

### Fase 5 — Mejora continua

| Actividad | CPM | CSM | NPM | IM | Int-L | Opt-L | Cdrl-L | LIB-RAN | LIB-PLAN | LIB-QA | LIB-O&M | LIB-ACC | LIB-EXEC |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Retrospectiva Golden Cluster | I | I | A/R | R | R | R | R | C | C | C | I | I | - |
| Actualización del template v2 | I | I | A | I | R | C | I | R | I | I | I | I | - |
| Retrospectiva interna (cada 2 sem) | I | - | A/R | R | C | C | C | - | - | - | - | - | - |
| Retrospectiva final del proyecto | I | I | A/R | R | C | C | C | C | C | C | I | C | I |
| Lecciones aprendidas | I | I | A/R | C | C | C | C | C | C | C | I | I | - |

---

## Reglas explícitas para peer dynamics (Carlos + Eduardo)

Carlos y Eduardo aparecen como **A/R conjuntos** en varias filas. Esto significa:

1. **Ambos son accountable** del resultado, no se pueden separar
2. **Decisiones que afectan a ambos** se toman conjuntamente
3. **Reporting al CPM** lo hace cualquiera, pero ambos deben coincidir
4. **No hay "Carlos manda" o "Eduardo manda"** en estas actividades — son peers

Ejemplos de actividades con A/R conjunto:
- DoR validación
- Resolución de bloqueos cruzados HW/SW

---

## Áreas Telemóvil y su involucramiento

### Cuándo se involucra cada área

| Área Telemóvil | Cadencia de involucramiento |
|---|---|
| **RAN Engineering (Roberto)** | Diaria-semanal: template, KPIs técnicos, retrospectiva del cluster |
| **Planning (Marcela)** | Semanal: re-priorización, sign-off de planning post-aceptación |
| **Quality (Patricia)** | Por sitio: validación de KPIs, sign-off de calidad |
| **O&M (Fernando)** | Por sitio: handover post-aceptación, ventanas NOC |
| **Acceptance (Ricardo Mendoza)** | Semanal: sesión batch de aceptación |
| **Sponsors ejecutivos** | Bi-semanal: reporte ejecutivo |

### Reglas para gestionar 5 áreas

- **No se asume "Telemóvil es una sola voz"**: cada área tiene contraparte específica en Ericsson
- **Si áreas Telemóvil tienen opinión divergente**, Carlos facilita resolución (no asume su voz)
- **Sponsors ejecutivos solo se involucran** en bi-semanal o crisis
- **Comunicación cruzada entre áreas Telemóvil es responsabilidad de Telemóvil**, no de Carlos

---

## Mapeo de Subcompetencias

- **3.3 Gestión de Involucrados:** la matriz organiza explícitamente involucramientos
- **3.2 Equipo de Alto Desempeño:** clarifica responsabilidades para evitar fricción
- **1.4 Lean & Kanban:** soporta el flujo del Kanban con governance clara

## Preguntas para Carlos

1. ¿El modelo peer A/R conjunto Carlos-Eduardo refleja la realidad?
2. ¿Las 5 áreas Telemóvil tienen los involucramientos correctos o ajustar?
3. ¿Hay actividades clave que omití en la matriz?

---

**Ver también:** [[Acuerdo-de-Equipo]] (peer dynamics y compromisos por rol) · [[Mapa-de-Involucrados]] (stakeholders externos) · [[Personas]] (perfiles del equipo extendido)

**Siguiente:** [[Plan-de-Comunicacion]]
