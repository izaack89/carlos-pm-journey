---
title: Product Backlog — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.1, 2.2]
tags: [backlog, kanban, agile, sitios]
---

# Product Backlog

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Tablero Kanban y backlog definidos antes del kickoff.

## Propósito

Estructurar el trabajo del proyecto en épicas y tarjetas de sitio gestionables vía Kanban. El backlog refleja el flujo **bajo responsabilidad directa de Carlos como NPM** (Integración + Optimización), con puntos de coordinación claros con el flujo de Implementation Manager (su peer).

---

## Estructura del Backlog

### Épicas

| Épica | Descripción | Sitios | Semanas |
|---|---|---|---|
| **E1 — Golden Cluster** | Despliegue piloto de 3 sitios para validar template y proceso | 5 | 2-4 |
| **E2 — Despliegue Masivo Urbano** | 10 sitios urbanos densos de San José | 10 | 5-7 |
| **E3 — Despliegue Suburbano** | 5 sitios suburbanos en San José Oeste y zonas periféricas | 5 | 5-7 |
| **E4 — Sitios de Cierre** | 3 sitios con readiness pendiente al inicio | 3 | 7-8 |
| **E5 — Setup y Cierre** | Setup del proyecto, retrospectivas, documentación final | — | 1 y 8 |

🔶 **[VALIDAR CON CARLOS]:** Distribución exacta de sitios por épica una vez confirme la lista real.

---

## Alcance del Kanban de Carlos (vs flujo de Implementation)

### Lo que está EN el Kanban de Carlos

- **Integración** (aplicación del template SW vía ENM)
- **Optimización** (validación y ajuste de KPIs)
- **Aceptación** (presentación a Telemóvil)

### Lo que está FUERA del Kanban de Carlos (responsabilidad de Eduardo, peer)

- Construcción / site readiness físico
- HW logistics (RRU, antenas en sitio)
- Energía, fibra, permisos
- Cuadrillas locales

### Punto de coordinación crítico

La columna **"Listo para Ventana"** es el handoff explícito entre los dos peers (Carlos + Eduardo). Cuando un sitio está aquí, ambos confirman que:
- Site readiness OK (Eduardo confirma)
- Template aprobado y pre-staged (Carlos confirma)
- Ventana NOC agendada (coordinada entre ambos)
- Cuadrilla asignada (Eduardo) e Integrador asignado (Carlos)

---

## Columnas del tablero Kanban

| # | Columna | WIP Limit | Owner | Criterio de entrada | Criterio de salida |
|---|---------|-----------|-------|---------------------|--------------------|
| 1 | **Backlog** | — | Carlos prioriza | Sitio asignado por Telemóvil al proyecto | Plan de site readiness en curso (handoff a Eduardo) |
| 2 | **Listo para Ventana** | 5 | Carlos + Eduardo (peers) | DoR completa: site ready + template aprobado + ventana NOC | Día de ventana inicia |
| 3 | **Integración** ⚡ | 3 | Integrador remoto + Cuadrilla local (paralelo) | Ventana activa | SW aplicado OK + HW validado OK (ambos firman) |
| 4 | **Optimización** | 3 | Optimizador remoto asignado | Integración técnica OK | KPIs dentro de umbral, validados 24-48h, no impacto vecinos |
| 5 | **Listo para Aceptación** | 5 | Carlos (validación final) | Optimización completa | SAD listo, presentable a Telemóvil |
| 6 | **Aceptación Telemóvil** | 5 | Ricardo Mendoza (Telemóvil) | SAD entregado | Sign-off formal Telemóvil |
| 7 | **Done** | — | — | Sign-off completo | — |

### Reglas explícitas

- **WIP limits son sagrados:** si una columna está llena, no se empuja, se ayuda a desbloquear
- **Columna transversal "Bloqueado":** cualquier sitio bloqueado se marca y se discute en el daily
- **Trabajo paralelo en "Integración":** Integrador remoto (SW) y Cuadrilla local (HW) trabajan simultáneamente durante la ventana
- **Sitios bloqueados >24h se escalan al CPM**
- **Sitios bloqueados >72h se escalan al CSM y se comunica a Telemóvil**

---

## Formato de Tarjeta de Sitio

```
┌──────────────────────────────────────────────────┐
│ ID: PA-XXX                                       │
│ Zona: [Nombre de colonia/distrito]               │
│ Tipo: [Urbano denso / Suburbano / Corredor]      │
│ Épica: E1 / E2 / E3 / E4                         │
├──────────────────────────────────────────────────┤
│ Estado Kanban: [Backlog → ... → Done]            │
│ Asignaciones:                                    │
│   Integrador: [Diego/Ana/Sandeep/Hugo]           │
│   Optimizador: [Marco/Sofía/Patricia]            │
│   Cuadrilla: [Luis/Javier/Ricardo] (vía Eduardo) │
├──────────────────────────────────────────────────┤
│ DoR cumplido:                                    │
│  ☐ Site Ready (Eduardo)                          │
│  ☐ Template aprobado (Carlos + Roberto)          │
│  ☐ Ventana NOC agendada                          │
│  ☐ Integrador asignado                           │
│  ☐ Cuadrilla asignada                            │
├──────────────────────────────────────────────────┤
│ Fechas:                                          │
│  Entrada al flujo:                               │
│  Listo para ventana:                             │
│  Inicio integración (ventana):                   │
│  Fin integración:                                │
│  Optimización iniciada:                          │
│  Optimización completa:                          │
│  Aceptación Telemóvil:                             │
├──────────────────────────────────────────────────┤
│ KPIs post-integración (Optimizador valida):      │
│  PRB Utilization: ____                           │
│  DL Throughput: ____                             │
│  UL Throughput: ____                             │
│  DCR: ____                                       │
│  Handover Success Rate: ____                     │
│  Alarmas críticas: ____                          │
│  FTR: ☐ Sí  ☐ No                                 │
├──────────────────────────────────────────────────┤
│ Bloqueos / Notas:                                │
│                                                  │
└──────────────────────────────────────────────────┘
```

---

## Backlog ordenado — Estado inicial del proyecto

🔶 **[VALIDAR CON CARLOS]:** Los IDs y zonas son sintéticos. Carlos reemplaza con identificadores reales de Telemóvil.

### Semanas 1-4 — Golden Cluster (E1)

| Orden | ID | Zona | Tipo | Justificación |
|---|---|---|---|---|
| 1 | CR-001 | Vía España | Corredor comercial | Hotspot oficinas — alta visibilidad |
| 2 | CR-003 | El Cangrejo | Urbano denso | Caso típico urbano denso |
| 3 | CR-005 | San Francisco | Urbano denso | Variante urbano con complejidad media |
| 4 | CR-014 | San Miguelito | Suburbano | Suburbano típico |
| 5 | CR-019 | Juan Díaz | Suburbano | Segundo suburbano para confirmar consistencia |

### Semanas 5-7 — Despliegue Masivo Urbano (E2)

| Orden | ID | Zona | Tipo | Prioridad |
|---|---|---|---|---|
| 6 | CR-002 | Costa del Este | Corredor comercial | Alta — zona corporativa |
| 7 | CR-004 | Bella Vista | Urbano denso | Alta — alta densidad poblacional |
| 8 | CR-006 | Obarrio | Urbano denso | Alta — densidad media |
| 9 | CR-007 | Punta Pacífica | Urbano denso | Alta — zona en crecimiento |
| 10 | CR-008 | Vía Brasil | Urbano denso | Media — congestión confirmada |
| 11 | CR-009 | Calidonia | Urbano denso | Media — zona comercial densa |
| 12 | CR-011 | Curundú | Urbano denso | Media |
| 13 | CR-012 | Río Abajo | Urbano denso | Media |
| 14 | CR-013 | Parque Lefevre | Urbano denso | Media — acceso fácil |
| 15 | CR-010 | Santa Ana | Urbano denso | Media — restricciones de acceso |

### Semanas 5-7 — Despliegue Suburbano (E3)

| Orden | ID | Zona | Tipo |
|---|---|---|---|
| 16 | CR-015 | Tocumen | Suburbano |
| 17 | CR-018 | Don Bosco | Suburbano |
| 18 | CR-021 | Arraiján | San José Oeste |
| 19 | CR-022 | La Chorrera | San José Oeste |
| 20 | CR-016 | Las Cumbres | Suburbano |

### Semanas 7-8 — Sitios de Cierre (E4)

| Orden | ID | Zona | Tipo | Razón de orden |
|---|---|---|---|---|
| 21 | CR-017 | Pedregal | Suburbano | Baja prioridad |
| 22 | CR-020 | Las Acacias | Suburbano | Baja prioridad |
| 23 | CR-023 | Vista Alegre | San José Oeste | Pendiente de readiness |

---

## Asignación de equipo a sitios (estrategia inicial)

### Integradores (Carlos asigna)

| Tipo de sitio | Integrador preferido | Justificación |
|---|---|---|
| Corredor comercial (alta visibilidad) | Diego (Senior) | Experiencia en sitios críticos |
| Urbano denso | Diego, Ana, Hugo (rotación) | Mix de seniority |
| Suburbano | Ana, Hugo | Complejidad media adecuada para crecimiento |
| Casos especiales / automatización | Sandeep (India) | Su expertise en automatización ENM |

### Optimizadores (Carlos asigna)

| Tipo de sitio | Optimizador preferido | Justificación |
|---|---|---|
| Corredor comercial | Marco (Senior) | Patrones de tráfico complejos |
| Urbano denso | Marco, Sofía | Carrier aggregation crítica |
| Suburbano | Sofía, Patricia | Crecimiento de Patricia (Junior) |

**Regla:** los 3 optimizadores se asignan por sitio, pero **pueden apoyarse entre ellos** cuando hay carga desbalanceada.

### Cuadrillas (Eduardo asigna, Carlos coordina)

| Zona | Cuadrilla |
|---|---|
| San José Centro (Vía España, El Cangrejo, etc.) | Luis (Cuadrilla 1) |
| San José Oeste (Arraiján, La Chorrera) | Javier (Cuadrilla 2) |
| San José Este (Tocumen, Don Bosco) | Ricardo (Cuadrilla 3) |

---

## Re-priorización adaptativa (Subcompetencia 1.1)

El backlog se revisa **cada lunes** en la reunión semanal con Telemóvil (RAN Engineering + Planning).

### Disparadores de re-priorización

1. **Hallazgos del Golden Cluster** que indiquen que un tipo de sitio requiere más atención
2. **Cambio en site readiness** (sitio pendiente que se libera, o sitio listo que se bloquea) — input de Eduardo
3. **Solicitud de Telemóvil** por urgencia comercial o competitiva (input de Marcela)
4. **Capacidad real del equipo** según semana (vacaciones, otros proyectos)
5. **Hallazgos del equipo de optimización** sobre patrones de KPIs

### Documentación del cambio

Cada re-priorización se documenta con:
- Fecha
- Sitios afectados
- Razón del cambio
- Decisión final
- Aprobado por (Carlos + Eduardo + Roberto + Marcela)

Se mantiene un log de re-priorizaciones (ver casos concretos en [[Sesion-Repriorizacion]]; durante la ejecución, las decisiones se registran como entradas en esa nota o en `specs/entregables/semana-N/` según corresponda).

---

## Coordinación con flujo de Implementation

```
Flujo de Eduardo (Implementation):       Flujo de Carlos (NPM):
Site selection                            ↓
↓                                         Backlog (priorización)
Site survey                               ↓
↓                                         Listo para Ventana ←── HANDOFF AQUÍ
HW logistics                              ↓
↓                                         Integración (SW vía remoto)
Energía / Fibra                           [PARALELO: Cuadrilla aporta HW in-situ]
↓                                         ↓
Cuadrilla en sitio                        Optimización
↓                                         ↓
HW instalado (durante ventana) ───────────► Listo para Aceptación
                                          ↓
                                          Aceptación Telemóvil
                                          ↓
                                          Done
```

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** estructura del tablero, WIP limits, formato de tarjetas
- **1.1 Planeación Adaptativa:** mecanismo de re-priorización semanal
- **2.2 Value Driven Delivery:** orden del backlog por congestión y prioridad estratégica

## Preguntas para Carlos

1. ¿La columna "Listo para Ventana" como punto de sincronización con Eduardo es viable o ajustar?
2. ¿Los WIP limits propuestos son realistas? (WIP=3 en integración con 4 integradores; WIP=3 en optimización con 3 optimizadores)
3. ¿La estrategia de asignación por seniority es realista?
4. ¿Sandeep (India) realmente toma sitios complejos o se especializa en automatización exclusivamente?

---

**Siguiente:** [[Definition-of-Ready]]
