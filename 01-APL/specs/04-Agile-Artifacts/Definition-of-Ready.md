---
title: Definition of Ready — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 3.2, 1.2]
tags: [dor, kanban, calidad, agile]
---

# Definition of Ready (DoR)

> 🎯 **Documento de diseño** — proyecto en fase de planeación. La DoR se acuerda con Eduardo (peer Implementation Mgr) y Roberto (Telemóvil) antes del kickoff.

## Propósito

Establecer los criterios objetivos que un sitio debe cumplir **antes de entrar a la columna "Listo para Ventana"** del Kanban de Carlos. La DoR es el punto de **coordinación crítica entre los dos peers** (Carlos como NPM e Eduardo como Implementation Manager).

---

## Estructura de la DoR

La DoR del proyecto se organiza en **dos partes complementarias**:

1. **Pre-condiciones de Implementation** (responsabilidad de Eduardo y su equipo)
2. **Pre-condiciones de Integración** (responsabilidad de Carlos y su equipo)

Un sitio solo entra a "Listo para Ventana" cuando **ambas partes están cumplidas**.

---

## Parte 1 — Pre-condiciones de Implementation (owner: Eduardo)

### Hardware y materiales

- ☐ **HW recibido en bodega o sitio:** RRU, antenas, baseband, accesorios confirmados físicamente presentes
- ☐ **Inventario de HW validado** contra BOM (Bill of Materials) del sitio
- ☐ **Materiales de obra civil disponibles:** cables, soportes, herrajes según diseño

### Permisos y accesos

- ☐ **Permiso municipal vigente** para trabajo en el sitio
- ☐ **Permiso de tower company** (Telesites, American Tower) con ventana de acceso confirmada
- ☐ **Permiso de propietario del predio** firmado y vigente

### Energía e infraestructura

- ☐ **Energía eléctrica confirmada en sitio:** energización primaria de ICE/ICE completa
- ☐ **Capacidad eléctrica suficiente** para el HW adicional (validado)
- ☐ **Climatización del shelter operativa**
- ☐ **Fibra de transporte confirmada y operativa** hacia el sitio

### Cuadrilla

- ☐ **Cuadrilla asignada** con líder identificado (Luis / Javier / Ricardo)
- ☐ **Cuadrilla con materiales** y disponibilidad para la ventana

---

## Parte 2 — Pre-condiciones de Integración (owner: Carlos)

### Template y configuración

- ☐ **Template B41 aprobado** por RAN Engineering Telemóvil (Roberto)
- ☐ **Plan de RF con antigüedad ≤ 3 meses** (criterio incorporado por lección)
- ☐ **Configuración pre-cargada en ENM** lista para aplicar en la ventana
- ☐ **Plan de vecindades RF** revisado (neighbor relations preliminares)
- ☐ **Identificadores de red asignados:** Cell IDs, PCI, TAC, según plan de Telemóvil

### Equipo asignado

- ☐ **Integrador remoto asignado** según rotación + disponibilidad
- ☐ **Optimizador remoto pre-asignado** para validación post-integración
- ☐ **Plan de pruebas post-integración** disponible

### Coordinación con cliente

- ☐ **Ventana de mantenimiento confirmada** con NOC Telemóvil (Fernando — O&M) — 48h antes
- ☐ **Notificación pre-mantenimiento enviada** a NOC Telemóvil
- ☐ **Roberto (RAN Telemóvil) notificado** del sitio en agenda

### Comunicación interna

- ☐ **Documentación del sitio cargada en Confluence** (BOM, configuración, plan)
- ☐ **Coordinación con Eduardo confirmada** (peers alineados)
- ☐ **Notificación al equipo** en el daily de la víspera

---

## Quién valida cada parte

| Parte | Owner principal | Quién valida |
|-------|-----------------|--------------|
| **Parte 1 — Implementation** | Eduardo | Eduardo + líder de cuadrilla asignada |
| **Parte 2 — Integración** | Carlos | Carlos + integrador asignado + Roberto (template) |
| **Sign-off conjunto** | Carlos + Eduardo | Reunión semanal de peers (lunes) |

La revisión conjunta ocurre en la **reunión semanal de peers** los lunes (Carlos + Eduardo + opcionalmente CPM), antes de la re-priorización.

---

## Cómo se documenta el cumplimiento

Cada sitio en la columna "Backlog" tiene un sub-ticket en Jira con el checklist de DoR. Tanto Eduardo como Carlos pueden marcar items de su parte respectiva.

Cuando el sitio cumple ambas partes:
- Carlos lo mueve a "Listo para Ventana"
- Notificación automática al equipo
- Si la ventana es esta semana, queda en agenda visible

---

## Qué pasa si un sitio no cumple DoR

1. **El sitio NO entra a "Listo para Ventana"** — permanece en "Backlog"
2. **Se identifica el criterio incumplido** y el responsable de resolverlo (Eduardo o Carlos)
3. **Se asigna una fecha objetivo** para alcanzar DoR
4. **Se registra en el risk log** si el incumplimiento amenaza el cronograma

Esto previene la práctica de "empujar sitios al flujo y resolver problemas en el camino", que es la principal fuente de re-trabajos en proyectos similares.

---

## Excepciones a la DoR

Solo **Carlos + Eduardo + CPM** pueden autorizar excepciones, y solo en estos casos:

- **Riesgo controlado y aceptado por escrito** (e.g., entra al flujo con template aún en revisión final, con commitment de cierre antes de la integración)
- **Excepción documentada en el risk log** con plan de cierre
- **Comunicación explícita al equipo** de que el sitio entra con excepción

Las excepciones se discuten en la retrospectiva como oportunidad de mejorar el proceso.

---

## Métricas asociadas a la DoR

### Métrica 1 — % de sitios DoR-OK al primer intento

Mide cuántos sitios cumplen DoR sin requerir iteraciones.

**Meta:** ≥ 85% (proyectos similares suelen estar en 60-70%).

### Métrica 2 — Tiempo promedio entre identificación y DoR completa

Mide cuánto tarda un sitio en pasar de Backlog a Listo para Ventana.

**Meta:** ≤ 5 días.

### Métrica 3 — Origen de los incumplimientos

- % por Parte 1 (Implementation)
- % por Parte 2 (Integración)

Permite identificar bottlenecks específicos por peer.

---

## Lecciones esperadas durante el proyecto

Estas son hipótesis que se validarán durante el Golden Cluster:

| Hipótesis | Si se confirma, acción |
|-----------|------------------------|
| Plan de RF puede estar desactualizado | Reforzar criterio en DoR |
| Splices de fibra viejos causan atenuación | Agregar verificación específica |
| Permisos de tower company expiran sin aviso | Coordinación más temprana |

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** la DoR es la puerta de entrada que protege el flujo Kanban
- **3.2 Equipo de Alto Desempeño:** define responsabilidades compartidas entre los dos peers (Carlos + Eduardo)
- **1.2 Detección de Riesgos:** convierte preconditions implícitas en criterios explícitos y medibles

## Preguntas para Carlos

1. ¿La división en Parte 1 (Eduardo) y Parte 2 (Carlos) refleja la realidad o es artificial?
2. ¿El "Plan de RF con antigüedad ≤ 3 meses" es un criterio realista en Telemóvil Costa Rica?
3. ¿Telemóvil envía notificación pre-mantenimiento con 48h o con otro lead time?
4. ¿La meta de 85% de DoR al primer intento es ambiciosa o conservadora?
5. ¿La reunión semanal de peers (Carlos + Eduardo) los lunes es viable?

---

**Siguiente:** [[Definition-of-Done]]
**Anterior:** [[Product-Backlog]]
