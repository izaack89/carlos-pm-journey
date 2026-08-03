---
title: Release Plan — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.1, 2.1, 1.5]
tags: [release-plan, roadmap, cronograma]
---

# Release Plan — 8 Semanas

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Plan de 8 semanas con mecanismos explícitos de adaptación.

## Propósito

Definir el plan de entrega a lo largo de las 8 semanas del proyecto, organizando los 23 sitios en hitos clave y dejando explícito el punto de inflexión del **Golden Cluster** en la semana 4. Soporta la subcompetencia **1.1 Planeación Adaptativa** mostrando un plan adaptable, no rígido.

---

## Vista general — Roadmap del proyecto

```
Sem 1     Sem 2     Sem 3     Sem 4     Sem 5     Sem 6     Sem 7     Sem 8
│         │         │         │         │         │         │         │
│ Setup   │ Golden  │ Golden  │ RETRO   │ Despl   │ Despl   │ Despl   │ Cierre
│ &       │ Cluster │ Cluster │ + Plan  │ Masivo  │ Masivo  │ Masivo  │ &
│ Kickoff │ (1-3)   │ (4-5)   │ Refresh │ (6-12)  │ (13-18) │ (19-23) │ Hand-
│         │         │         │         │         │         │         │ over
│         │         │         │  ▲      │         │         │         │
│         │         │         │ Punto   │         │         │         │
│         │         │         │ inflex. │         │         │         │
└─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────
```

---

## Hitos clave

| Hito | Semana | Descripción | Criterio de cumplimiento |
|------|--------|-------------|--------------------------|
| **H1 — Kickoff** | Sem 1 | Proyecto arrancado, equipo alineado, tablero operativo | Acuerdo de equipo firmado + Kanban configurado |
| **H2 — Golden Cluster Done** | Sem 4 | 5 sitios integrados y aceptados | 5/5 sitios en "Done" + FTR validado |
| **H3 — Retrospectiva del Cluster** | Sem 4 | Lecciones aplicadas al template y proceso | Documento de mejoras incorporado |
| **H4 — 50% del proyecto** | Sem 6 | ~12 sitios completados | 12/23 sitios en "Done" |
| **H5 — Despliegue masivo completo** | Sem 7 | Sitios urbanos y suburbanos cerrados | 20/23 en "Done" |
| **H6 — Cierre del proyecto** | Sem 8 | Todos los sitios aceptados + handover | 23/23 + retrospectiva final |

---

## Detalle por semana

### Semana 1 — Setup y Kickoff

**Objetivo:** dejar el proyecto listo para arrancar el flujo.

| Día | Actividad | Responsable | Output |
|-----|-----------|-------------|--------|
| L | Kickoff con Telemóvil + Ericsson | CPM + Carlos | Acta de inicio |
| L | Primera reunión de peers (Carlos + Eduardo) | Ambos | Calendario semanal alineado |
| M | Configuración del tablero Kanban en Jira | Carlos | Tablero operativo |
| M | Firma del Acuerdo de Equipo | Todos los líderes | Acuerdo firmado |
| X | Validación de DoR de los primeros 8-10 sitios | Carlos + Eduardo | Sitios listos |
| J | Revisión técnica del template B41 con Roberto (Telemóvil) | Carlos + Integradores | Template aprobado |
| J | Primera reunión con Patricia (Quality), Marcela (Planning), Fernando (O&M) | Carlos | Stakeholders alineados |
| V | Daily Kanban arranca formalmente | Todo el equipo | Rutina establecida |

**Sitios procesados:** 0
**Sitios en flujo al cierre:** 2-3 (en "Listo para Ventana")

---

### Semana 2 — Golden Cluster (sitios 1-3)

**Objetivo:** integrar los 3 primeros sitios del Golden Cluster para validar el template.

**Sitios objetivo:**
- 🎯 CR-001 Vía España (corredor comercial) — Cuadrilla Luis + Integrador Diego + Optimizador Marco
- 🎯 CR-003 El Cangrejo (urbano denso) — Cuadrilla Luis + Integradora Ana + Optimizadora Sofía
- 🎯 CR-005 San Francisco (urbano denso) — Cuadrilla Luis + Integrador Diego + Optimizadora Sofía

**Actividades clave:**
- Integración técnica de los 3 sitios en ventanas de mantenimiento
- Validación de KPIs por Optimizadores 24-48h post-integración
- Primer reporte semanal a Telemóvil (5 áreas)
- Daily Kanban con foco en bloqueos del cluster

**Riesgos a monitorear:**
- Template requiere ajustes en el primer sitio (esperado, no debe ser sorpresa)
- Cuadrillas aún se están acoplando al nuevo flujo
- Sandeep aún se está acoplando culturalmente

**Métricas al cierre:**
- 3 sitios en "Aceptación" o "Done"
- FTR del cluster parcial: medida y reportada

---

### Semana 3 — Golden Cluster (sitios 4-5) + Estabilización

**Objetivo:** completar el Golden Cluster.

**Sitios objetivo:**
- 🎯 CR-014 San Miguelito (suburbano) — Cuadrilla Ricardo + Integradora Ana + Optimizador Marco
- 🎯 CR-019 Juan Díaz (suburbano) — Cuadrilla Ricardo + Integrador Hugo + Optimizadora Patricia

**Actividades clave:**
- Integración de los 2 sitios suburbanos
- Comparación de KPIs urbanos vs suburbanos
- Sesión semanal de aceptación con Acceptance Team Telemóvil (primer batch importante)
- Preparación de DoR para los siguientes 6-8 sitios

**Riesgos a monitorear:**
- Diferencias significativas de KPIs entre tipos de sitio
- Fatiga del equipo si las ventanas nocturnas no se gestionan bien

**Métricas al cierre:**
- 5 sitios del Golden Cluster en "Done"
- FTR completo del cluster: medida final

---

### Semana 4 — Retrospectiva del Golden Cluster + Refresh del plan

**🎯 Punto de inflexión del proyecto.**

**Objetivo:** capturar lecciones del cluster, ajustar template y proceso, refrescar el plan para los 20 sitios restantes.

**Actividades clave:**

| Día | Actividad | Quiénes | Output |
|-----|-----------|---------|--------|
| L | Compilación de datos del cluster | Carlos + optimizadores | Reporte del cluster |
| L | Reunión peers Carlos + Eduardo | Ambos | Alineamiento previo a retro |
| M | **Sesión de retrospectiva (formato 4L)** | Equipo completo + Roberto invitado | Documento de mejoras |
| X | Revisión y ajuste del template | Carlos + Roberto + Diego/Ana | Template v2 |
| J | Refresh del Release Plan para sem 5-8 | Carlos + Eduardo + CPM | Plan actualizado |
| V | Comunicación a Telemóvil | CSM + Carlos | Reporte ejecutivo |

**Subcompetencia central:** **2.1 Continuous Improvement** se materializa esta semana.

**Métricas al cierre:**
- Retrospectiva documentada con N acciones de mejora
- Template v2 aprobado
- Plan refrescado para los 20 sitios restantes

---

### Semana 5 — Inicio del Despliegue Masivo (sitios 6-12)

**Objetivo:** arrancar el despliegue masivo aprovechando las mejoras del Golden Cluster.

**Sitios objetivo:** 7 sitios urbanos densos
- CR-002 Costa del Este
- CR-004 Bella Vista
- CR-006 Obarrio
- CR-007 Punta Pacífica
- CR-008 Vía Brasil
- CR-009 Calidonia
- CR-011 Curundú

**Cadencia objetivo:** ~3-4 sitios completados por semana

**Asignaciones:** rotación de integradores y optimizadores según disponibilidad. Sandeep toma 1-2 sitios con foco en automatización de pre-checks.

**Riesgos a monitorear:**
- WIP limits del tablero (no sobrecargar integración)
- Disponibilidad de ventanas con NOC Telemóvil
- Cualquier regresión del template v2

---

### Semana 6 — Despliegue Masivo continuado (sitios 13-18)

**Objetivo:** alcanzar el ~50% del proyecto al cierre de la semana.

**Sitios objetivo:** 6 sitios mixtos (urbano + suburbano)
- CR-012 Río Abajo
- CR-013 Parque Lefevre
- CR-010 Santa Ana
- CR-015 Tocumen
- CR-018 Don Bosco
- CR-021 Arraiján

**Hito intermedio:** **H4 — 50% del proyecto** al cierre de la semana.

**Actividades especiales:**
- Mini-retrospectiva intermedia (1h, foco en flujo) con equipo completo
- Reporte ejecutivo a sponsors de Telemóvil
- Validación de cumplimiento del Acuerdo de Equipo

---

### Semana 7 — Cierre del Despliegue Masivo (sitios 19-23)

**Objetivo:** cerrar los sitios restantes incluyendo aquellos con readiness pendiente.

**Sitios objetivo:** 5 sitios finales
- CR-022 La Chorrera
- CR-016 Las Cumbres
- CR-017 Pedregal
- CR-020 Las Acacias
- CR-023 Vista Alegre (validar readiness)

**Riesgos a monitorear:**
- Sitios con readiness "Pendiente" al inicio del proyecto
- Acumulación de aceptaciones pendientes con Telemóvil

**Métricas al cierre:**
- 22-23 sitios en "Done"

---

### Semana 8 — Cierre y Handover

**Objetivo:** completar el último sitio si quedó pendiente, cerrar formalmente el proyecto.

**Actividades:**

| Día | Actividad | Output |
|-----|-----------|--------|
| L | Cierre del último sitio si pendiente | 23/23 |
| M | Sesión final de aceptación con Acceptance Team Telemóvil | Sign-off completo |
| X | Retrospectiva final del proyecto | Documento de lecciones aprendidas |
| J | Handover a O&M Telemóvil (Fernando) | Documentación entregada |
| V | Reunión de cierre con sponsors Telemóvil | Resumen ejecutivo presentado |

**Métricas finales del proyecto:**
- 23/23 sitios integrados y aceptados
- FTR final acumulado
- Lead time promedio por sitio
- % de DoR cumplido al primer intento
- Adherencia al Acuerdo de Equipo
- Participación de Sandeep (métrica de inclusión)

---

## Adaptabilidad del plan (Subcompetencia 1.1)

Este plan **NO es rígido**. Cada lunes, en la reunión semanal de pipeline:

1. Se revisa el avance vs plan
2. Se identifican desviaciones
3. Se re-prioriza el backlog si es necesario
4. Se ajusta el plan de la semana en curso si hay bloqueos

### Triggers de re-planeación

- Sitio bloqueado >72h afecta el cronograma
- Cambio de prioridades de Telemóvil (Marcela aporta input)
- Hallazgos técnicos significativos del Golden Cluster
- Disponibilidad alterada del equipo (vacaciones, otros proyectos)
- Eventos climáticos en Costa Rica (lluvias extremas)
- Issue cruzado entre Carlos y Eduardo (escalación de coordinación)

### Documentación de cambios

Cualquier cambio significativo al plan se registra en una bitácora de cambios (ver casos de re-priorización en [[Sesion-Repriorizacion]]; durante la ejecución cada cambio queda como entrada con fecha, razón y aprobación en esa nota o en `specs/entregables/semana-N/`).

---

## Vista de capacidad — Equipos vs Carga

| Semana | Sitios en flujo (de Carlos) | Sitios en integración | Carga estimada |
|--------|-----------------------------|------------------------|-----------------|
| 1 | 2-3 | 0-1 | Baja (setup) |
| 2 | 4-5 | 2-3 | Media |
| 3 | 5-6 | 2 | Media |
| 4 | 3-4 | 1 | Baja (retro) |
| 5 | 7-8 | 3 | Alta |
| 6 | 7-8 | 3 | Alta |
| 7 | 5-6 | 2-3 | Media-Alta |
| 8 | 2-3 | 0-1 | Baja (cierre) |

**Capacidad del equipo:**
- 4 integradores en paralelo (WIP=3 en columna Integración deja margen)
- 3 optimizadores en paralelo (WIP=3 en Optimización)
- 3 cuadrillas para 23 sitios — Eduardo equilibra carga

🔶 **[VALIDAR CON CARLOS]:** Validar capacidad real considerando disponibilidad parcial del equipo.

---

## Reporting alineado al plan

### Semanal — A Telemóvil (Operativo)

- A cada una de las 5 áreas, contenido específico:
  - **RAN (Roberto):** detalle técnico de configuración + KPIs preliminares
  - **Planning (Marcela):** sitios completados + capacidad agregada
  - **Quality (Patricia):** KPIs validados + observaciones de calidad
  - **O&M (Fernando):** sitios entregados a operación + alarmas
  - **Acceptance (Ricardo Mendoza):** sitios listos para sign-off

### Bi-semanal — A Sponsors (Ejecutivo)

- Avance vs plan global (% completado)
- FTR acumulado
- Riesgos top 3
- Hitos próximos

---

## Mapeo de Subcompetencias

- **1.1 Planeación Adaptativa:** el plan tiene mecanismos explícitos de adaptación
- **2.1 Continuous Improvement:** la retrospectiva en semana 4 es el corazón de la mejora continua
- **1.5 Metrics & Reporting:** las métricas semanales y bi-semanales soportan la trazabilidad del plan

## Preguntas para Carlos

1. ¿8 semanas reales o hay buffer de contingencia?
2. ¿La cadencia de 3-4 sitios/semana en despliegue masivo es realista?
3. ¿Roberto realmente acepta ser invitado a la retrospectiva del Golden Cluster en sem 4?
4. ¿El reporting a 5 áreas Telemóvil es viable o se consolida en menos?

---

**Anterior:** [[Acuerdo-de-Equipo]]
**Siguiente paso:** Step 6 — Simulación de Ejecución
