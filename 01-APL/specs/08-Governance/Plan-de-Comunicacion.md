---
title: Plan de Comunicación
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [3.3, 1.5, 3.2]
tags: [comunicacion, stakeholders, reporting]
---

# Plan de Comunicación

> 🎯 **Documento de diseño** — proyecto en fase de planeación.

## Propósito

Definir qué se comunica, a quién, con qué frecuencia y por qué canal. El proyecto tiene un equipo distribuido (Latam + India + Costa Rica) y 5 áreas distintas en Telemóvil, lo que requiere un plan explícito.

---

## Principios

### Pocos canales, claros y consistentes

- **Jira:** fuente única de verdad operativa (estado de sitios, asignaciones, bloqueos)
- **Confluence:** documentación formal (SADs, plan, retrospectivas)
- **Teams/Slack:** comunicación síncrona del equipo (no decisional)
- **Email:** reportes formales a Telemóvil
- **WhatsApp:** solo emergencias físicas (canal owned por Eduardo)
- **NUNCA WhatsApp para decisiones operativas**

### Audiencias específicas

Cada comunicación tiene una audiencia clara. **No se hace "comunicación masiva"** — los reportes a Telemóvil se diferencian por área.

### Idiomas explícitos

- **Inglés:** comunicación interna síncrona del equipo (incluye Sandeep)
- **Español:** comunicación con cuadrillas locales, con Telemóvil
- **Documentación dual:** los docs clave (DoR, DoD, template) en español + inglés

---

## Matriz de comunicación

### Comunicación interna del equipo Ericsson

| # | Comunicación | Audiencia | Frecuencia | Canal | Owner | Idioma |
|---|---|---|---|---|---|---|
| 1 | Daily Kanban | Equipo Ericsson + cuadrillas | Diaria 9:00 AM PA | Teams | Carlos | Inglés |
| 2 | Reunión peers Carlos-Eduardo | Carlos + Eduardo | Semanal lunes 8 AM | Teams o presencial | Ambos | Español |
| 3 | Retrospectiva interna | Equipo Ericsson sin Telemóvil | Cada 2 semanas | Teams | Carlos | Inglés |
| 4 | Knowledge sharing | Equipo Ericsson | Mensual | Teams | Voluntario | Inglés |
| 5 | Office hours Carlos | Quien lo requiera | Martes y jueves 2-3 PM | Teams | Carlos | Bilingüe |
| 6 | 1:1 Carlos-miembro equipo | Carlos + 1 | Quincenal | Teams | Carlos | Idioma del miembro |
| 7 | Coordinación durante ventana | Integrador + cuadrilla + Eduardo | Durante ventana | Teams + Jira | Integrador asignado | Bilingüe |
| 8 | Alerta de bloqueo | Equipo | Inmediata | Jira + Teams | Quien identifica | Inglés |
| 9 | WhatsApp emergencia física | Eduardo + cuadrilla afectada | Emergencias | WhatsApp | Eduardo | Español |

### Comunicación con Telemóvil Costa Rica (5 áreas)

| # | Comunicación | Audiencia Telemóvil | Frecuencia | Canal | Owner Ericsson | Idioma |
|---|---|---|---|---|---|---|
| 10 | Reporte semanal técnico | Roberto (RAN) | Lunes EOD | Email + dashboard | Carlos + Marco | Español |
| 11 | Reporte semanal planning | Marcela (Planning) | Lunes EOD | Email + dashboard | Carlos | Español |
| 12 | Reporte semanal calidad | Patricia (Quality) | Lunes EOD | Email | Marco + Carlos | Español |
| 13 | Coordinación O&M | Fernando (O&M) | Continua + handover por sitio | Email + Teams | Eduardo + Carlos | Español |
| 14 | Reunión técnica semanal | Roberto + Carlos + Marco | Semanal | Teams | Carlos | Español |
| 15 | Reunión de re-priorización | Marcela + Carlos + Eduardo | Semanal lunes | Teams | Carlos | Español |
| 16 | Sesión de aceptación batch | Ricardo Mendoza + Carlos | Semanal viernes | Presencial o Teams | Carlos | Español |
| 17 | Notificación pre-ventana | Fernando + Roberto | T-48h por sitio | Email | Carlos | Español |
| 18 | Reporte ejecutivo bi-semanal | Sponsors Telemóvil + áreas líderes | Bi-semanal | Email + presentación | CSM + Carlos | Español |
| 19 | Reporte mensual ejecutivo | Sponsors Telemóvil | Mensual | Email + presentación | CSM | Español |

### Comunicación con cuadrillas locales

| # | Comunicación | Audiencia | Frecuencia | Canal | Owner | Idioma |
|---|---|---|---|---|---|---|
| 20 | Asignación de sitio | Líder de cuadrilla | T-48h | Jira + Email | Eduardo | Español |
| 21 | Briefing pre-ventana | Cuadrilla asignada | T-24h | Teams | Eduardo + Integrador | Español |
| 22 | Coordinación durante ventana | Cuadrilla + Integrador | Durante ventana | Teams + Jira | Integrador asignado | Bilingüe |
| 23 | Reconocimiento semanal | Cuadrilla | Semanal viernes | Email + daily | Eduardo + Carlos | Español |
| 24 | Retrospectiva con cuadrillas | Líderes de cuadrilla | Cada 2 semanas | Teams o presencial | Eduardo | Español |

### Comunicación con sponsors y leadership

| # | Comunicación | Audiencia | Frecuencia | Canal | Owner | Idioma |
|---|---|---|---|---|---|---|
| 25 | Reporte ejecutivo Telemóvil | Sponsors Telemóvil | Bi-semanal | Email + presentación | CSM + Carlos | Español |
| 26 | Reporte ejecutivo Ericsson | Leadership Ericsson | Mensual | Email | CPM | Inglés |
| 27 | Escalación urgente | CPM + CSM | Cuando aplique | Llamada + email | Carlos o Eduardo | Bilingüe |

---

## Reportes diferenciados a Telemóvil — contenido por área

### A Roberto (RAN Engineering) — semanal lunes EOD

**Contenido:**
- Sitios completados esta semana con detalle técnico
- KPIs por sitio (tabla)
- Observaciones sobre el template
- Bloqueos técnicos activos
- Próximos sitios en agenda (semana entrante)

**Formato:** Email + acceso a dashboard de KPIs en EMA

**Quién lee:** Roberto + su equipo

### A Marcela (Planning) — semanal lunes EOD

**Contenido:**
- Sitios completados esta semana
- Capacidad agregada acumulada
- Saturación reducida por zona (donde aplique)
- Sitios próximos en agenda
- Solicitudes de re-priorización si las hay

**Formato:** Email + tabla de planning

**Quién lee:** Marcela + su equipo

### A Patricia (Quality) — semanal lunes EOD

**Contenido:**
- Sitios completados con calidad de KPIs
- Sitios pendientes de validación extendida
- Patrones de calidad observados
- Bloqueos relacionados a calidad

**Formato:** Email + dashboard

### A Fernando (O&M) — continua + por sitio

**Contenido por sitio aceptado:**
- Configuración final aplicada
- KPIs en momento de handover
- Alarmas pendientes (debería ser 0)
- Equipo de contacto del proyecto si surge issue
- Documentación de O&M

**Formato:** Email + Confluence link

### A Ricardo Mendoza (Acceptance) — semanal viernes

**Contenido:**
- Lista de sitios listos para aceptación esta semana
- SADs adjuntos
- Resumen de validaciones de las áreas
- Próximos sitios en agenda

**Formato:** Sesión presencial o Teams + email pre-sesión

---

## Comunicación de bloqueos

### Bloqueo identificado (cualquiera lo identifica)

**Acción inmediata:**
1. Marcar en Jira con tag "blocked" + descripción
2. Mencionar en próximo daily Kanban
3. Asignar owner de resolución

### Bloqueo de < 24h

**Comunicación:** Solo en Jira y daily

### Bloqueo de 24-48h

**Comunicación:**
- Carlos menciona en reporte semanal a Telemóvil (área relevante)
- Si afecta a Eduardo, comunicación directa entre peers

### Bloqueo de 48-72h

**Comunicación:**
- Escalación a CPM
- Comunicación formal a área Telemóvil afectada

### Bloqueo de > 72h

**Comunicación:**
- Escalación a CSM
- Comunicación a sponsors Telemóvil
- Comité ad-hoc para resolución

---

## Reconocimiento al equipo

### Reconocimiento semanal

- **Cuándo:** viernes en reporte interno + email a líderes de cuadrilla
- **Contenido:** mención específica a logros de la semana
- **Quién:** Carlos (lo lidera), pero cualquier miembro puede proponer

### Reconocimiento por hito

- **Cuándo:** al cierre del Golden Cluster, mitad del proyecto, cierre
- **Contenido:** reconocimiento ampliado, agradecimientos visibles
- **Quién:** CSM + Carlos

---

## Plantillas de comunicación

### Plantilla 1 — Reporte semanal a área Telemóvil

```
Asunto: Status semanal Proyecto B41 — [Área] — Semana N

Hola [Nombre área Telemóvil],

Resumen de la semana N:

▼ Sitios completados: X
[Lista con detalle relevante para tu área]

▼ Sitios próximos:
[Agenda de la siguiente semana]

▼ Métricas clave para tu área:
[Tabla específica]

▼ Bloqueos o riesgos relevantes:
[Si los hay]

▼ Próximos pasos / decisiones requeridas:
[Si las hay]

Si requieres más detalle, podemos agendar 30 min esta semana.

Saludos,
Carlos
```

### Plantilla 2 — Notificación pre-ventana

```
Asunto: Pre-ventana de mantenimiento sitio PA-XXX — fecha hora

Hola Fernando (O&M) y Roberto (RAN),

Notificamos la próxima ventana de mantenimiento:

▼ Sitio: PA-XXX [Zona]
▼ Fecha: [día]
▼ Hora: [start] – [end]
▼ Tipo: Integración B41 + activación de capacidad
▼ Cuadrilla: [Líder]
▼ Integrador remoto: [Nombre]
▼ Impacto: [Sin servicio momentáneo / Reducción / Ninguno según el caso]

Plan de rollback disponible si surge issue.

Confirmar disponibilidad del NOC para esta ventana.

Saludos,
Carlos
```

---

## Métricas de comunicación

| Métrica | Cómo se mide | Meta |
|---|---|---|
| Adherencia al canal correcto (Jira vs WhatsApp) | Auditoría semanal | ≥ 95% |
| Reportes semanales enviados a tiempo | Conteo | 100% |
| Respuesta a stakeholders Telemóvil en < 24h | Tiempo de respuesta | ≥ 90% |
| Asistencia a dailies | Conteo | ≥ 85% |
| Sandeep participación | Conteo específico | ≥ 80% |

---

## Mapeo de Subcompetencias

- **3.3 Gestión de Involucrados:** el plan ES la materialización de esta subcompetencia
- **1.5 Metrics & Reporting:** cadencia y formato de reportes definidos
- **3.2 Equipo de Alto Desempeño:** comunicación interna del equipo distribuido

## Preguntas para Carlos

1. ¿Reportar separadamente a 5 áreas de Telemóvil es viable o consolidar en menos?
2. ¿Los canales propuestos coinciden con la realidad de Ericsson y Telemóvil?
3. ¿El idioma bilingüe planteado funciona o ajustar?

---

**Ver también:** [[Mapa-de-Involucrados]] (estrategia por stakeholder) · [[Burndown-y-Metricas]] (cadencia de reportes) · [[Acuerdo-de-Equipo]] (canales internos del equipo)

**Anterior:** [[RACI-Matrix]]
