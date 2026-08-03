---
title: Herramientas Ericsson — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.5]
tags: [tecnico, herramientas, ericsson]
---

# Herramientas Ericsson en el Proyecto

> 🎯 **Documento de diseño** — proyecto en fase de planeación.

## Propósito

Describir las herramientas Ericsson que el equipo utiliza día a día. Este contexto refuerza la credibilidad técnica del proyecto.

---

## ENM (Ericsson Network Manager)

### Qué es

Plataforma centralizada de gestión de red de Ericsson. Es la herramienta principal para:
- **Configuración de nodos RAN** (eNodeB para LTE)
- **Aplicación de templates** de parametrización
- **Monitoreo de alarmas** en tiempo real
- **Software upgrade** de nodos
- **Backup y restore** de configuraciones

### Uso en el proyecto

- **Integradores remotos (Diego, Ana, Sandeep, Hugo):** aplican el template B41 vía ENM en cada uno de los 23 sitios
- **Pre-checks post-integración:** ENM reporta estado de las celdas
- **Configuración consistente:** un solo template, aplicado vía ENM, garantiza uniformidad entre sitios

### Acceso remoto

ENM es accesible vía VPN desde cualquier ubicación. Esto permite que los integradores remotos (Latam + India) trabajen sin estar en Costa Rica.

---

## EMA (Ericsson Mobility Analytics) / ENIQ

### Qué es

Plataforma de análisis de KPIs de red de Ericsson. Procesa contadores PM y los convierte en KPIs accionables.

🔶 **[VALIDAR CON CARLOS]:** Confirmar si Telemóvil usa EMA, ENIQ, u otra plataforma.

### Uso en el proyecto (Optimizadores remotos)

- **Dashboard de KPIs post-integración:** PRB Utilization, Throughput DL/UL, DCR, Handover Success Rate
- **Comparación pre/post integración:** validar que los sitios entregan el incremento de capacidad esperado
- **Detección de anomalías:** alertas si un sitio integrado tiene KPIs fuera de rango
- **Reporte semanal a Telemóvil:** Marco/Sofía/Patricia extraen métricas de EMA y arman el reporte

### Dashboard compartido con Telemóvil

Configurado por Carlos al inicio del proyecto, con acceso de visualización para:
- Roberto (RAN Engineering)
- Marcela (Planning)
- Patricia (Quality)

---

## AMOS / MOShell

### Qué es

Línea de comandos para interactuar directamente con nodos Ericsson. Acceso de bajo nivel para troubleshooting.

### Uso en el proyecto

- **Troubleshooting:** cuando un sitio tiene comportamiento inesperado, los Integradores acceden vía AMOS para diagnóstico
- **Scripts de validación:** automatizan checks repetitivos (Sandeep lidera este esfuerzo)
- **No es el primer recurso:** la mayoría del trabajo se hace en ENM

---

## MOM (Managed Object Model)

### Qué es

Modelo de datos jerárquico que describe los objetos gestionables de un nodo Ericsson. El template de configuración se expresa en términos de MOM.

### Por qué importa

- El **template B41** que se aplica a los 23 sitios es básicamente una secuencia de operaciones sobre objetos MOM
- Versiones de MOM diferentes entre nodos pueden causar incompatibilidades — uno de los riesgos a validar en pre-checks

---

## Atoll / WinFiol (legacy)

Herramientas de planeación de RF y troubleshooting. Mencionadas porque algunos equipos legacy aún las usan, pero el proyecto se basa principalmente en ENM y EMA.

---

## Jira / Confluence

Aunque no son herramientas Ericsson per se, son las plataformas donde el proyecto vive:

- **Jira:** tablero Kanban del proyecto. Cada sitio es un ticket con su estado, asignado, bloqueos, fechas
- **Confluence:** documentación del proyecto, incluyendo Site Acceptance Documents (SADs)

🔶 **[VALIDAR CON CARLOS]:** Confirmar si el proyecto usa Jira o Azure DevOps.

---

## Cómo se conectan las herramientas en el flujo de trabajo

```
┌─────────────┐    ┌──────────┐    ┌───────────┐    ┌────────┐
│   Jira      │───▶│   ENM    │───▶│   Nodo    │───▶│  EMA   │
│ (Kanban)    │    │ (Aplica  │    │  LTE      │    │ (KPIs) │
│             │    │ template)│    │ (Genera   │    │        │
└─────────────┘    └──────────┘    │ contadores)│   └────────┘
       │                            └───────────┘         │
       │                                                  │
       │           ┌──────────┐                           │
       └──────────▶│Confluence│◀──────────────────────────┘
                   │  (SAD)   │
                   └──────────┘

Quién usa qué:
- Integradores ──► ENM, AMOS, Jira
- Optimizadores ──► EMA, Jira, Confluence (SAD)
- Carlos ──► Todos (visión global)
- Eduardo ──► Jira (vista de Implementation)
- Telemóvil (Roberto, Marcela, Patricia) ──► EMA (read-only), Jira (visualización)
```

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** Jira como herramienta del tablero Kanban
- **1.5 Metrics & Reporting:** EMA como fuente única de verdad para KPIs

## Preguntas para Carlos

1. ¿Telemóvil usa EMA, ENIQ, o tiene su propia plataforma de analytics?
2. ¿La herramienta de ticketing del proyecto es Jira o Azure DevOps?
3. ¿Existen scripts de validación automatizados que el equipo use? Vale la pena documentarlos
4. ¿Hay herramientas adicionales que omití?

---

**Siguiente:** [[Template-B41-Resumen]]
**Anterior:** [[Topologia-y-Alcance]]
