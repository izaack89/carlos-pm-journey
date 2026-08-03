---
title: Justificación del Enfoque Ágil — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.1, 2.1, 1.5, 1.2]
tags: [agile, kanban, lean, framework, justificacion, ericsson]
---

# Justificación del Enfoque Ágil

## Propósito

Justificar la elección de **Lean & Kanban como framework principal** complementado con prácticas ágiles selectivas, para el proyecto de Expansión de Capacidad LTE B41 (23 sitios — Telemóvil Costa Rica). Este documento aborda directamente las subcompetencias **1.4 Lean & Kanban** y **1.1 Planeación Adaptativa**.

---

## 1. Punto de partida — Gestión tradicional

Históricamente, los despliegues de capacidad LTE en Ericsson se han ejecutado bajo un modelo de **gestión tradicional en cascada**:

### Características del modelo tradicional

- **Secuencia fija** de sitios establecida en planeación, sin re-priorización en ejecución
- **Hitos rígidos** alineados a fechas de entrega contractuales
- **Aceptación al final del ciclo**, con todos los sitios entregados en bloque
- **Documentación extensiva** previa a ejecución (planes detallados, runbooks por sitio)
- **Roles especializados** trabajando en silos: planeación → implementación → integración → optimización
- **Reportes de estatus** semanales o quincenales con poca visibilidad operativa día a día

### Limitaciones observadas

| Limitación | Impacto | Frecuencia |
|---|---|---|
| **Re-trabajos técnicos** detectados tarde | Sobreesfuerzo en últimas semanas del proyecto | Recurrente |
| **Bloqueos ocultos** en sitios individuales | Demoras propagadas al cronograma global | Alta |
| **Falta de visibilidad** del flujo end-to-end | El cliente y los equipos no saben dónde está cada sitio | Constante |
| **Propagación de errores** de configuración entre sitios | Un error de template aplicado a múltiples sitios antes de ser detectado | Crítica |
| **Capacidad de respuesta lenta** ante cambios de prioridad del cliente | Pérdida de oportunidad de entregar valor primero donde más se necesita | Alta |
| **Aceptación bottleneck** al final del ciclo | Disputas, re-trabajos y demoras concentrados en últimas semanas | Crítica |

Estas limitaciones son particularmente costosas en proyectos de capacidad como este, donde **el valor de negocio se materializa con cada sitio puesto en servicio** (no al final del proyecto). Cada semana que un sitio congestionado espera por la finalización completa del batch es una semana de mala experiencia para los suscriptores de Telemóvil.

---

## 2. Por qué Kanban como framework principal

### La naturaleza del trabajo encaja con Kanban, no con sprints

El proyecto consiste en **flujo continuo de sitios** atravesando una secuencia de etapas: