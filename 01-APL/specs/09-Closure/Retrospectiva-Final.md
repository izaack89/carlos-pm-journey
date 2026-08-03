---
title: Retrospectiva Final del Proyecto
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [2.1, 3.2, 1.5]
tags: [retrospectiva, cierre, lecciones]
---

# Retrospectiva Final del Proyecto

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación. Este es el guion esperado de la retrospectiva al cierre (semana 8). Carlos actualiza con datos reales después de la ejecución.

## Propósito

Capturar las lecciones consolidadas del proyecto completo. Esta retrospectiva difiere de la del Golden Cluster: el foco no es ajustar el proyecto en marcha, sino **extraer aprendizajes transferibles** para Ericsson, Telemóvil y para Carlos como Agile Project Leader.

---

## Contexto esperado

- **Fecha planeada:** miércoles 5 de agosto de 2026 (semana 8)
- **Duración:** 3 horas
- **Formato:** Híbrido (Teams + sala Telemóvil Costa Rica)
- **Asistentes:** Equipo completo (Ericsson + cuadrillas + Telemóvil áreas relevantes)
- **Idioma:** Inglés con switches a español
- **Facilitador:** Carlos

---

## Datos cuantitativos esperados al cierre

🔶 **[VALIDAR CON CARLOS]:** Estos son los resultados proyectados. Carlos los reemplaza con datos reales.

| Métrica | Meta | Resultado esperado |
|---|---|---|
| Sitios completados | 23/23 | 23/23 |
| FTR acumulado | ≥ 90% | 91% (21/23) |
| Lead time promedio | ≤ 12 días | 10.4 días |
| Cycle time promedio | ≤ 5 días | 4.1 días |
| DoR cumplido primer intento | ≥ 85% | 87% |
| Bloqueos resueltos < 72h | ≥ 80% | 85% |
| Bloqueos sorpresa (sin riesgo previo) | < 20% | 15% |
| Asistencia daily promedio | ≥ 85% | 89% |
| Sandeep participación | ≥ 80% | 88% |
| Conflictos escalados al CPM | ≤ 2 | 1 |
| Transiciones en Jira | ≥ 95% | 96% |

---

## Formato — Sailboat

Formato visual que invita reflexión más profunda que el 4L.

```
                  Viento (lo que nos impulsó)
                       ↓ ↓ ↓
                       
                      _|_
                     /   \
                    / 🚢  \
                   /_______\
                  ~~~~~~~~~~~

Anclas (lo que nos retuvo)     Rocas (riesgos que enfrentamos)
       ⬇                              ⚠️
```

---

## Narrativa esperada de la retrospectiva

### Apertura (15 min)

**Carlos:**
> "Today we close 8 weeks of work. 23 sites integrated. 91% FTR. We achieved more than the 10% efficiency improvement target. But beyond numbers, today we want to capture what helped us, what slowed us down, and what we'd do differently next time."

CSM Ericsson agradece a todos. Sponsors Telemóvil mencionan el caso como ejemplo a replicar.

### Viento (45 min) — lo que nos impulsó

Esperamos comentarios como:

**Diego (Integrador Senior):** "Pre-staging templates 24h in advance. Saved ~1 hour per integration. ~23 hours total."

**Sandeep (India):** "Daily Kanban in English. Felt included throughout the project. Cultural buddy model with Diego worked."

**Patricia (Junior optimizadora):** "Informal mentorship with Marco. I learned more in 8 weeks than in 6 months elsewhere."

**Roberto (Telemóvil RAN):** "Inviting me to the Golden Cluster retrospective. Built trust. Made me see Ericsson as partner, not vendor."

**Marcela (Telemóvil Planning):** "Bringing real saturation data to Monday's re-prioritization. Felt heard, decisions were based on facts."

**Eduardo (peer):** "Weekly peer meetings with Carlos. Zero friction this project. Compared to previous projects, night and day."

**Luis (Cuadrilla 1 leader):** "Reconocimiento semanal. Mi equipo se sintió valorado por primera vez."

**Marco:** "Sharing learning from CR-014 with Patricia (Junior). She documented it, used it for similar cases later."

**Carlos observa el patrón:** El "viento" más fuerte fue **la inclusión y la transparencia** — no la metodología en sí.

### Anclas (45 min) — lo que nos retuvo

**Hugo (Integrador Junior):** "Office hours were useful but I never had the courage to ask in front of others. Maybe more 1:1 informal?"

**Sofía:** "Timezone between Argentina and Costa Rica. Manageable but not ideal."

**Sandeep:** "Documentation was excellent, but informal channels (Teams chat) sometimes had context in Spanish. Felt I was missing things."

**Ana:** "I was assigned mostly urban dense sites. Would've grown more with variety."

**Javier (Cuadrilla 2):** "Cuando había emergencia física, el WhatsApp ayudó. Pero a veces, lo no-emergencia también fue por WhatsApp. Hay que cuidarlo."

**Fernando (Telemóvil O&M):** "Handover documentation was great but came on Friday afternoons. Hard to review with weekend coming."

**Carlos:** "Documented. Next time: handover by Wednesday."

### Rocas (45 min) — riesgos que enfrentamos

**Carlos:** "Let's review the Risk Register and discuss what was real and what surprised us."

Revisión de los 11 riesgos identificados:

| Riesgo | Materializado | Comentario |
|---|---|---|
| R-EQUIPO-01 Aislamiento Sandeep | Parcialmente | Mitigaciones funcionaron; Sandeep participación 88% |
| R-EQUIPO-02 Fricción NPM-IM | No | Peer dynamics funcionaron |
| R-TEC-01 Template ajustes | Sí | Template v2 aplicado en sem 4, como diseñado |
| R-TEC-02 RF desactualizado | Sí | Caso CR-014, freshness check agregado |
| R-FIS-01 Site readiness | Sí | CR-023 resuelto en sem 7 |
| R-FIS-02 Tower company | Sí | CR-007 diferido y resuelto |
| R-FIS-03 Cuadrilla overload | Sí | Re-balanceo en sem 5 |
| R-CLIENTE-01 Cambio prioridades | Sí | CR-004 Bella Vista subió por saturación |
| R-CLIENTE-02 Rechazo aceptación | Parcialmente | 2 sitios con observaciones menores |
| R-CLIENTE-03 NOC no disponible | No | Coordinación con Fernando preventiva |
| R-EXT-01 Clima | Parcialmente | 1 retraso de 2 días, manejable |
| R-EXT-02 Inseguridad | No | Sin incidentes |

**Surprise risk:** ninguno crítico. El 85% de bloqueos tuvieron riesgo previo.

### Acciones para el futuro (30 min)

Las acciones de esta retrospectiva no son para este proyecto (ya terminó). Son para:
1. Próximos proyectos similares en Telemóvil
2. Replicabilidad del enfoque ágil en Ericsson Latam
3. Carlos como profesional certificado

| Acción | Aplicable a | Owner |
|---|---|---|
| Documentar template v2 como standard | Ericsson Solutions Latam | Carlos + Roberto |
| Crear playbook "Agile RAN Deployments" | Ericsson | Carlos + CPM |
| Cultural buddy model formal | Ericsson HR + leaders | CPM |
| Telemóvil invite to retrospective as standard | Próximos proyectos Telemóvil | CSM |
| Capacitación de líderes de cuadrilla en Jira | Próximos proyectos | Eduardo |
| Re-priorización formal con cliente Planning | Próximos proyectos | NPM rol |

### Cierre (15 min)

**Roberto:**
> "I'm taking this approach to my team. We'd want Carlos and Eduardo to facilitate a workshop for Telemóvil RAN team if possible."

**CSM Ericsson:**
> "We're using this project as case study for Ericsson Latam's quarterly review."

**Carlos:**
> "Personally, this project gave me the confidence to facilitate ágil at scale. Thank you all."

🟢 Cierre emotivo. Equipo distribuido despide con genuino agradecimiento.

---

## Reflexión personal de Carlos (en su diario)

> "8 semanas. 23 sitios. 91% FTR. Números buenos, pero lo que me llevo no son números.
>
> Eduardo y yo no tuvimos fricción. La estructura peer + reunión semanal funcionó. Vale para siempre.
>
> Sandeep fue el caso difícil. Conectarse desde India a las 10:30 PM toda la semana es difícil. El cultural buddy con Diego funcionó. Sandeep terminó liderando automatización para todo el equipo. Lección: incluir activamente o se queda fuera.
>
> Patricia (junior optimizadora) creció mucho. Marco fue mejor mentor que algunos sénior que conozco. Lección: el alto desempeño no es por jerarquía, es por disposición.
>
> Roberto (Telemóvil) fue mi caso favorito. Empezó escéptico. Terminó queriendo aprender el método. Eso es 3.3 Gestión de Involucrados en su mejor expresión.
>
> Como Agile Project Leader, aprendí que mi rol no es controlar. Es facilitar para que el equipo entregue. Cuando los dejé brillar, brillaron. Cuando intenté tomar decisiones que correspondían al equipo, se sintieron.
>
> Tengo el resumen de lecciones para mi presentación. Estoy listo."

---

## Outputs de la retrospectiva final

| Output | Estado |
|---|---|
| Resumen de datos del proyecto | ✅ Documentado |
| Lecciones consolidadas | ✅ En documento separado |
| Acciones para futuros proyectos | ✅ 6 acciones definidas |
| Reconocimiento al equipo | ✅ Realizado |
| Caso de estudio | ✅ Aprobado por CSM |

---

## Mapeo de Subcompetencias

- **2.1 Continuous Improvement:** retrospectiva final consolida aprendizajes
- **3.2 Equipo de Alto Desempeño:** reconoce dinámicas que funcionaron
- **1.5 Metrics & Reporting:** datos cuantitativos del proyecto

## Preguntas para Carlos

1. ¿Las metas proyectadas son realistas (91% FTR)?
2. ¿La retrospectiva final con Telemóvil presente o solo equipo Ericsson?
3. ¿Las acciones para futuros proyectos resuenan con la realidad de Ericsson?

---

**Siguiente:** [[Lecciones-Aprendidas]]
