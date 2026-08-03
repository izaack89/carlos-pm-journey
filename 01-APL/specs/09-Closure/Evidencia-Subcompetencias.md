---
title: Evidencia de Subcompetencias
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
tags: [evidencia, subcompetencias, certificacion]
---

# Evidencia de Subcompetencias — Mapa de Trazabilidad

> 🎯 **Documento clave para el grader del Proyecto Integrador.** Mapea cada subcompetencia con los documentos y evidencias específicas que la demuestran.

## Propósito

Demostrar al grader que cada subcompetencia requerida está respaldada por evidencia concreta en el vault del proyecto.

---

## Subcompetencia 1.1 — Planeación Adaptativa

### Definición
Capacidad de planear con flexibilidad, integrar nueva información, y ajustar el plan sin perder dirección estratégica.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Vision-del-Producto.md` | Sección "Restricciones y Supuestos" + Objetivo SMART | Mecanismos de revisión del objetivo |
| `Product-Backlog.md` | Sección "Re-priorización adaptativa" | Disparadores y proceso de re-priorización |
| `Release-Plan.md` | Sección "Adaptabilidad del plan" | Triggers explícitos de re-planeación |
| `Sesion-Repriorizacion.md` | Documento completo | Caso concreto de re-priorización con datos |
| `Risk-Register.md` | Riesgos identificados | Anticipación de incertidumbres |

### Caso ejemplar
**`Sesion-Repriorizacion.md`** muestra cómo en semana 5 se re-priorizó el backlog basado en:
- Saturación 91% en Bella Vista (input de Marcela Telemóvil)
- Tower company pendiente en CR-007 (input de Eduardo)
- Oportunidad de probar 3CA (input de Roberto (Telemóvil))
- Cuadrilla 1 sobrecargada (input de Eduardo)

Decisiones tomadas con razones objetivas, no caprichosas.

---

## Subcompetencia 1.2 — Detección y Resolución de Riesgos y Problemas

### Definición
Anticipar riesgos, identificar problemas temprano, y aplicar resolución estructurada.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Risk-Register.md` | Documento completo | 11 riesgos identificados con probabilidad, impacto, mitigación |
| `Bloqueo-Simulado-y-Resolucion.md` | Caso CR-014 | Resolución estructurada en 56h con 5 personas, 4 ubicaciones |
| `Definition-of-Ready.md` | Sección de criterios | Criterios objetivos previenen problemas |
| `Daily-Kanban-Sample.md` | Discusión CR-014 | Detección y asignación de apoyo en daily |

### Caso ejemplar
**`Bloqueo-Simulado-y-Resolucion.md`** documenta el manejo del bloqueo CR-014:
- Detección 12h post-integración
- Asignación de apoyo en próximo daily
- Diagnóstico en 24h, fix en 4h, validación en 14h
- Coordinación remota: Marco (México) + Sofía (Argentina) + Diego (Costa Rica)
- Aprendizaje capturado por Patricia (Junior) para próximos sitios

---

## Subcompetencia 1.4 — Lean & Kanban

### Definición
Aplicar principios Lean y Kanban: flujo continuo, WIP limits, eliminación de desperdicio.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Product-Backlog.md` | Sección "Columnas del tablero" | Tablero Kanban con 7 columnas + WIP limits |
| `Definition-of-Ready.md` | Documento completo | Criterios objetivos de entrada |
| `Definition-of-Done.md` | Documento completo | Criterios objetivos de salida |
| `Daily-Kanban-Sample.md` | Transcripción de daily | Ceremonia Kanban en acción |
| `Acuerdo-de-Equipo.md` | Sección "Sobre el Kanban" | Reglas explícitas |

### Caso ejemplar
**`Daily-Kanban-Sample.md`** muestra una sesión típica donde:
- Se respeta el límite de 15 minutos
- Se revisan columnas de derecha a izquierda (pull)
- Se identifican bloqueos (WIP gestionado)
- Se toman decisiones operativas inmediatas

---

## Subcompetencia 1.5 — Metrics & Reporting

### Definición
Diseñar, medir y reportar métricas que informan decisiones.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Burndown-y-Metricas.md` | Documento completo | 11 métricas definidas con metas y proyección |
| `burndown-data.csv` | Archivo de datos | Datos por sitio (proyección esperada) |
| `Plan-de-Comunicacion.md` | Cadencias de reporting | Frecuencia, audiencia, contenido |
| `Resumen-Ejecutivo.md` | Sección "Indicadores cuantitativos" | Resultados consolidados |

### Caso ejemplar
**`Burndown-y-Metricas.md`** define las métricas principales:
- 11 métricas con definición operativa
- Cadencia: diaria, semanal, bi-semanal, mensual
- Reporting diferenciado por audiencia (5 áreas Telemóvil + sponsors)

---

## Subcompetencia 2.1 — Continuous Improvement

### Definición
Capacidad de extraer aprendizajes y aplicar mejoras de forma sistemática.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Retrospectiva-Golden-Cluster.md` | Documento completo | Retro estructurada con formato 4L, 10 acciones acordadas |
| `Retrospectiva-Final.md` | Documento completo | Retro final con formato Sailboat |
| `Lecciones-Aprendidas.md` | Documento completo | 30+ lecciones consolidadas en 5 categorías |
| `Plan-de-Calidad.md` | Sección "Mejora continua" | Cadencia de mejora del plan |

### Caso ejemplar
**`Retrospectiva-Golden-Cluster.md`** demuestra:
- Formato estructurado (4L)
- Cliente invitado (Roberto (Telemóvil))
- 10 acciones de mejora documentadas
- Template v2 aprobado para los siguientes 20 sitios
- Caso donde se reconoció abiertamente que WhatsApp es necesario para emergencias (ajuste al acuerdo)

---

## Subcompetencia 2.2 — Value Driven Delivery

### Definición
Priorizar entrega de valor por encima de cumplimiento ciego.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Vision-del-Producto.md` | Sección "Beneficios Esperados" + Objetivo SMART | Valor explícito por audiencia |
| `Justificacion-del-Enfoque-Agil.md` | Trade-offs ágil vs cascada | Decisiones de diseño por valor |
| `Product-Backlog.md` | Orden del backlog | Priorización por valor |
| `Sesion-Repriorizacion.md` | Caso Bella Vista | CR-004 sube por saturación 91% |
| `Topologia-y-Alcance.md` | Sección "valor multiplicador" | CA como multiplicador de valor |

### Caso ejemplar
**`Sesion-Repriorizacion.md`** muestra cómo CR-004 Bella Vista subió de posición 7 a posición 2 porque Marcela aportó datos: saturación 91% con crecimiento mensual del 6%. La decisión priorizó valor de negocio sobre orden inicial.

---

## Subcompetencia 3.1 — Liderazgo Colaborativo

### Definición
Facilitar reuniones ágiles como espacios colaborativos, remover cuellos de botella y empoderar al equipo distribuido para que tome decisiones donde ocurre el trabajo.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Acuerdo-de-Equipo.md` | Documento completo | Carlos facilita la co-construcción del acuerdo en lugar de imponerlo |
| `Dia-1-Proyecto.md` | Bloque de kickoff | Carlos facilita el kickoff dando voz a remotos (Sandeep, Diego, Ana, Hugo) antes que a presenciales |
| `Daily-Kanban-Sample.md` | Transcripción completa | Carlos no asigna trabajo; pregunta y empodera al equipo a decidir |
| `Retrospectiva-Golden-Cluster.md` | Apertura + facilitación 4L | Carlos como facilitador, no dueño de soluciones; Roberto (Telemóvil) invitado como par |
| `Sesion-Repriorizacion.md` | Decisión de CR-004 | Carlos integra inputs de Marcela, Eduardo y Roberto sin sobreponer su criterio |
| `RACI-Matrix.md` | Peer dynamics Carlos↔Eduardo | Liderazgo compartido NPM e Implementation Manager |

### Caso ejemplar
**`Retrospectiva-Golden-Cluster.md`** demuestra liderazgo colaborativo en acción:
- Carlos abre el espacio sin agenda cerrada (formato 4L)
- Invita explícitamente a Roberto (Telemóvil) (cliente) y a Patricia (junior optimizadora) — el espacio es para todos, no solo Ericsson senior
- Cuando surge el conflicto WhatsApp vs Jira, Carlos no decide unilateralmente; facilita acuerdo del equipo (WhatsApp solo emergencias)
- El template v2 emerge de la discusión, no de un mandato de Carlos

Complementado por **`Daily-Kanban-Sample.md`**, donde Carlos hace preguntas ("¿Hugo, qué necesitas?") en lugar de asignar tareas, y deja que el equipo proponga apoyos entre pares.

---

## Subcompetencia 3.2 — Equipo de Alto Desempeño

### Definición
Construir y gestionar equipos efectivos, diversos, comprometidos.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Personas.md` | 16 perfiles | Comprensión profunda del equipo distribuido |
| `Acuerdo-de-Equipo.md` | Documento completo | Normas explícitas para equipo distribuido |
| `Dia-1-Proyecto.md` | Bloque del acuerdo | Construcción participativa |
| `Daily-Kanban-Sample.md` | Sandeep, Patricia (Junior) participación | Inclusión activa |
| `Bloqueo-Simulado-y-Resolucion.md` | Colaboración Marco + Sofía + Diego | Equipo distribuido funcional |
| `Lecciones-Aprendidas.md` | Categoría 3 | Lecciones del equipo |

### Caso ejemplar
**`Acuerdo-de-Equipo.md`** muestra:
- Decisión de daily en **inglés** para incluir a Sandeep
- **Cultural buddy** Diego ↔ Sandeep
- **Peer dynamics** Carlos ↔ Eduardo formalizado
- **Reconocimiento semanal** sistemático
- **Inclusión** de cuadrillas locales con espacio para su voz

---

## Subcompetencia 3.3 — Gestión de Involucrados

### Definición
Identificar, mapear y gestionar relaciones con stakeholders diversos.

### Documentos y secciones de evidencia

| Documento | Sección clave | Evidencia |
|---|---|---|
| `Mapa-de-Involucrados.md` | Documento completo | Mapa de poder/interés |
| `Personas.md` | 5 perfiles Telemóvil | Stakeholders profundizados |
| `RACI-Matrix.md` | Documento completo | Roles y responsabilidades explícitos |
| `Plan-de-Comunicacion.md` | Matrices de comunicación | 5 áreas Telemóvil con reportes diferenciados |
| `Retrospectiva-Golden-Cluster.md` | Invitación a Roberto y Patricia | Cliente como socio |
| `Sesion-Repriorizacion.md` | Marcela aportando datos | Cliente involucrado en decisiones |

### Caso ejemplar
**`Plan-de-Comunicacion.md`** demuestra gestión de 5 áreas Telemóvil con:
- Contraparte específica en Ericsson
- Cadencia diferenciada
- Contenido específico por área
- Idioma adecuado al contexto
- Canal apropiado por tipo de mensaje

Y **`Retrospectiva-Golden-Cluster.md`** muestra el caso de Roberto (Telemóvil) pasando de escéptico a advocate por la transparencia del enfoque.

---

## Resumen visual de evidencia

```
Subcompetencia               | Documentos principales
─────────────────────────────|──────────────────────────────────
1.1 Planeación Adaptativa    | Vision-del-Producto, Backlog, Release Plan,
                              | Sesión-Repriorización, Risk-Register
─────────────────────────────|──────────────────────────────────
1.2 Detección de Riesgos     | Risk-Register, Bloqueo-Simulado,
                              | Daily-Kanban (CR-014)
─────────────────────────────|──────────────────────────────────
1.4 Lean & Kanban            | Backlog, DoR, DoD, Daily, Acuerdo
─────────────────────────────|──────────────────────────────────
1.5 Metrics & Reporting      | Burndown-y-Métricas, Plan-Comunicación,
                              | Resumen-Ejecutivo
─────────────────────────────|──────────────────────────────────
2.1 Continuous Improvement   | Retro-Golden, Retro-Final,
                              | Lecciones-Aprendidas
─────────────────────────────|──────────────────────────────────
2.2 Value Driven Delivery    | Vision-del-Producto, Justificación-Ágil,
                              | Backlog, Sesión-Repriorización
─────────────────────────────|──────────────────────────────────
3.1 Liderazgo Colaborativo   | Acuerdo, Dia-1, Daily, Retro-Golden,
                              | Sesión-Repriorización, RACI
─────────────────────────────|──────────────────────────────────
3.2 Equipo Alto Desempeño    | Personas, Acuerdo, Dia-1, Daily,
                              | Lecciones (cat 3)
─────────────────────────────|──────────────────────────────────
3.3 Gestión Involucrados     | Mapa-de-Involucrados, Personas (Telemóvil),
                              | RACI, Plan-Comunicación, Retro-Golden
```

---

## Tabla cruzada — documentos clave

Cada documento del vault mapeado contra las subcompetencias que evidencia:

| Documento | 1.1 | 1.2 | 1.4 | 1.5 | 2.1 | 2.2 | 3.1 | 3.2 | 3.3 |
|---|---|---|---|---|---|---|---|---|---|
| Vision-del-Producto | ✓ | | | | | ✓ | | | |
| Justificacion-del-Enfoque-Agil | ✓ | ✓ | | | | ✓ | | | |
| Mapa-de-Involucrados | | | | | | | | | ✓ |
| Personas | | | | | | | | ✓ | ✓ |
| Topologia-y-Alcance | | ✓ | | | | ✓ | | | |
| Product-Backlog | ✓ | | ✓ | | | ✓ | | | |
| Definition-of-Ready | | ✓ | ✓ | | | | | ✓ | |
| Definition-of-Done | | | ✓ | ✓ | | | | | ✓ |
| Acuerdo-de-Equipo | | | ✓ | | | | ✓ | ✓ | ✓ |
| Release-Plan | ✓ | | | ✓ | ✓ | | | | |
| Dia-1-Proyecto | | | ✓ | | | | ✓ | ✓ | ✓ |
| Daily-Kanban-Sample | | ✓ | ✓ | | | | ✓ | ✓ | |
| Bloqueo-Simulado | | ✓ | | | | | | ✓ | |
| Retro-Golden-Cluster | | | | ✓ | ✓ | | ✓ | ✓ | ✓ |
| Sesion-Repriorizacion | ✓ | | | | | ✓ | ✓ | | ✓ |
| Burndown-y-Metricas | ✓ | | ✓ | ✓ | | | | | |
| Risk-Register | | ✓ | | ✓ | | | | | ✓ |
| Plan-de-Calidad | | | | ✓ | ✓ | | | | ✓ |
| RACI-Matrix | | | ✓ | | | | ✓ | ✓ | ✓ |
| Plan-de-Comunicacion | | | | ✓ | | | | ✓ | ✓ |
| Retro-Final | | | | ✓ | ✓ | | | ✓ | |
| Lecciones-Aprendidas | | | | | ✓ | | | ✓ | ✓ |
| Resumen-Ejecutivo | ✓ | | | ✓ | | ✓ | | | ✓ |

---

## Cómo el grader puede verificar la evidencia

1. **Lee el documento referenciado**
2. **Busca la sección clave** mencionada
3. **Verifica que la evidencia sea concreta** (no abstracta)
4. **Valida que los datos sean coherentes** entre documentos
5. **Las preguntas para Carlos** en cada documento son inputs adicionales

---

**Anterior:** [[Resumen-Ejecutivo]]
**Siguiente paso:** Preparación de la presentación final
