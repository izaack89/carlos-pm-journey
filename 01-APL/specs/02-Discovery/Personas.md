---
title: Personas del Proyecto — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [3.2, 3.3]
tags: [personas, equipo, stakeholders]
---

# Personas del Proyecto

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Las personas representan perfiles reales del equipo que arranca el proyecto. Nombres y detalles personales pueden ser sintéticos.

## Propósito

Mapear las personas clave del proyecto con suficiente profundidad para entender sus motivaciones, retos y formas preferidas de trabajar. Esta comprensión informa el Acuerdo de Equipo, el Plan de Comunicación y la dinámica de las ceremonias.

---

## Estructura del equipo extendido

```
                            ┌─────────────────────────────────┐
                            │  Carlos (NPM) — Ericsson remoto │
                            │  Owner del Kanban + facilitador │
                            └────────┬────────────────────────┘
                                     │
              ┌──────────────────────┼──────────────────────┐
              │                                             │
   ┌──────────┴──────────┐                       ┌─────────┴────────┐
   │ 4 Integradores      │                       │ 3 Optimizadores  │
   │ (remotos, Ericsson) │                       │ (remotos,        │
   │                     │                       │  Ericsson)       │
   │ Diego, Ana, Sandeep,│                       │ Marco, Sofía,    │
   │ Hugo                │                       │ Patricia         │
   └─────────────────────┘                       └──────────────────┘

   ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ Coordinación entre peers ─ ─ ─ ─ ─ ─ ─ ─ ─ ─

   ┌─────────────────────────────────────────────────────────────┐
   │ Eduardo (Implementation Manager) — Ericsson, peer de Carlos │
   │                                                              │
   │   ┌───────────────────────────────────────────────────────┐ │
   │   │ 3 Cuadrillas locales (externos en Costa Rica)             │ │
   │   │ - Cuadrilla 1: Líder Luis                              │ │
   │   │ - Cuadrilla 2: Líder Javier                            │ │
   │   │ - Cuadrilla 3: Líder Ricardo                           │ │
   │   └───────────────────────────────────────────────────────┘ │
   └─────────────────────────────────────────────────────────────┘

   ─ ─ ─ ─ ─ ─ ─ ─ ─ ─ Cliente Telemóvil Costa Rica ─ ─ ─ ─ ─ ─ ─ ─ ─ ─

   Roberto (RAN Engineering) ── Marcela (Planning) ── Patricia (Quality)
   Fernando (O&M) ──── Ricardo (Acceptance Team Lead)
```

🔶 **[VALIDAR CON CARLOS]:** Reemplazar nombres sintéticos con nombres reales del equipo cuando sea posible.

---

## Equipo de Carlos (Ericsson)

### Persona 1 — Diego (Integrador Senior remoto)

**Datos:**
- **Rol:** Integration Engineer Senior
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Costa Rica (remoto, mismo TZ que Costa Rica)
- **Experiencia:** 8 años en RAN Ericsson, especialista ENM/AMOS
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Crecer técnicamente en proyectos retadores
- Reconocimiento por calidad técnica
- Reducir trabajo nocturno (las ventanas son nocturnas)

**Frustraciones:**
- Sitios marcados como "listos" que no lo estaban (frustración histórica)
- Falta de visibilidad de status de HW cuando integra SW
- Cambios de último minuto al template

**Cómo prefiere trabajar:**
- Tareas claras vía Jira, no WhatsApp
- Coordinación temprana con cuadrillas (24-48h antes)
- Documentación clara del template

**Qué necesita Carlos de él:**
- Calidad técnica de la integración del template
- Reportar bloqueos temprano, no ocultarlos
- Coordinar con cuadrillas y Eduardo durante la ventana

---

### Persona 2 — Ana (Integradora Mid-level remota)

**Datos:**
- **Rol:** Integration Engineer Mid-level
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Colombia (remoto, mismo TZ que Costa Rica)
- **Experiencia:** 4 años en RAN Ericsson, expertise en RF
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Aprender de Integradores Senior como Diego
- Especializarse en RF y troubleshooting avanzado
- Crecer a nivel Senior en 1-2 años

**Frustraciones:**
- Que su voz se ignore por ser más junior
- Documentación incompleta de proyectos anteriores que no le permite aprender

**Cómo prefiere trabajar:**
- Mentoría informal de Diego y Carlos
- Espacio para hacer preguntas sin miedo
- Tareas con suficiente challenge pero no abrumadoras

**Qué necesita Carlos de ella:**
- Apoyo en troubleshooting de RF (su fortaleza emergente)
- Documentar lo que aprende para futuras integradoras
- Participar activamente en retrospectivas

---

### Persona 3 — Sandeep (Integrador Senior remoto — India) ⚠️

**Datos:**
- **Rol:** Integration Engineer Senior
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Bangalore, India (remoto, TZ +10.5h vs Costa Rica)
- **Experiencia:** 10 años en RAN Ericsson, expertise en automatización ENM
- **Idioma:** Inglés profesional, hindi nativo; no habla español

**Motivaciones:**
- Aportar expertise técnico de proyectos en Asia
- Conocer una región nueva (Latam)
- Apoyar despliegues internacionales

**Frustraciones:**
- Aislamiento por timezone (cuando hace daily a las 9 AM Costa Rica, son 7:30 PM en India)
- Barrera de idioma (mucha comunicación informal del equipo es en español)
- Falta de contexto cultural (referencias locales en Costa Rica que no entiende)

**Cómo prefiere trabajar:**
- Documentación escrita exhaustiva (más confiable que conversación oral)
- Reuniones programadas con anticipación
- Tareas con scope claro, ejecutables independientemente

**Cómo lo incluye el equipo:**
- **Daily en inglés** (decisión del equipo) para que pueda participar
- Documentos clave traducidos al inglés
- Buddy de cultura: Diego es su punto de contacto principal
- Si requiere apoyo nocturno (ventana en Costa Rica = madrugada en India), se compensa con tiempo

**Qué necesita Carlos de él:**
- Expertise técnico en casos complejos
- Apoyo en automatización (scripts de pre-checks)
- Documentación detallada para otros integradores

**🚨 Riesgos asociados (van al Risk Register):**
- Aislamiento cultural/lingüístico afecta integración al equipo
- TZ +10.5h limita disponibilidad para reuniones síncronas
- Confusión por diferencias culturales en comunicación (más directo en India vs más indirecto en Latam)

---

### Persona 4 — Hugo (Integrador Junior remoto)

**Datos:**
- **Rol:** Integration Engineer Junior
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** México (remoto, TZ -1h vs Panamá; mismo TZ working hours)
- **Experiencia:** 2 años en RAN Ericsson, primer proyecto B41
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Ser parte de un proyecto piloto ágil
- Aprender de Diego, Ana y Sandeep
- Crecer a Mid-level

**Frustraciones:**
- Sentirse junior cuando habla en reuniones
- Falta de retroalimentación estructurada

**Cómo prefiere trabajar:**
- Pair programming con un Integrador Senior
- Feedback explícito sobre su trabajo
- Tareas con scope acotado al inicio del proyecto

**Qué necesita Carlos de él:**
- Compromiso y disposición a aprender
- Apoyo en sitios con baja complejidad (para construir confianza)
- Voz en retrospectivas (la perspectiva de junior aporta valor)

---

### Persona 5 — Marco (Optimizador Senior remoto)

**Datos:**
- **Rol:** Optimization Engineer Senior
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** México (remoto, TZ -1h vs Costa Rica)
- **Experiencia:** 9 años en optimización RAN, expertise en EMA y RF tuning
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Lograr KPIs óptimos en cada sitio
- Establecer mejores prácticas de optimización
- Liderar técnicamente entre optimizadores

**Frustraciones:**
- Tiempo insuficiente para optimizar correctamente (presión por cerrar sitios)
- Sitios pasados a aceptación con KPIs justo en el umbral, no óptimos

**Cómo prefiere trabajar:**
- 48h mínimo de validación de KPIs antes de mover a aceptación
- Datos completos de EMA antes de tomar decisiones
- Acceso directo a Roberto (RAN Telemóvil) para validar criterios

**Qué necesita Carlos de él:**
- Liderazgo técnico entre optimizadores
- Mantener estándares altos de validación
- Identificar patrones que requieran ajuste al template

---

### Persona 6 — Sofía (Optimizadora Mid-level remota)

**Datos:**
- **Rol:** Optimization Engineer Mid-level
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Argentina (remoto, TZ +2h vs Costa Rica)
- **Experiencia:** 5 años en optimización RAN, expertise en carrier aggregation
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Especializarse en CA y MIMO avanzado
- Trabajar en proyectos de alta visibilidad
- Crecer a Senior

**Frustraciones:**
- Diferencia horaria (cuando llega al daily a las 11 AM ARG, ya pasaron 1h tras inicio de Costa Rica)
- Documentación de templates incompleta

**Cómo prefiere trabajar:**
- Acceso temprano a EMA cada mañana
- Coordinación clara de qué sitio toma cada optimizador
- Sesiones técnicas semanales con Marco

**Qué necesita Carlos de ella:**
- Validación rigurosa de CA en cada sitio
- Documentar patrones que descubra
- Compartir aprendizajes con Patricia (optimizadora junior)

---

### Persona 7 — Patricia (Optimizadora Junior remota)

**Datos:**
- **Rol:** Optimization Engineer Junior
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Perú (remoto, mismo TZ que Costa Rica)
- **Experiencia:** 1.5 años en optimización RAN, primer proyecto LTE B41 grande
- **Idioma:** Español nativo, inglés intermedio

**Motivaciones:**
- Aprender de Marco y Sofía
- Construir reputación técnica
- Crecer a Mid-level

**Frustraciones:**
- Sentir que su contribución es marginal por ser junior
- Documentación técnica densa, difícil de procesar al inicio

**Cómo prefiere trabajar:**
- Tareas acotadas al inicio, ampliando con el tiempo
- Mentoría con Marco (semanal)
- Espacio para preguntar sin presión

**Qué necesita Carlos de ella:**
- Compromiso con calidad técnica
- Reportar cuando algo no entienda (es información, no fracaso)
- Crecer en autonomía durante el proyecto

---

## Peer de Carlos: Implementation Manager

### Persona 8 — Eduardo (Implementation Manager — Ericsson, peer de Carlos)

**Datos:**
- **Rol:** Implementation Manager
- **Empresa:** Ericsson (contratación directa)
- **Ubicación:** Costa Rica (presencial, no remoto)
- **Experiencia:** 12 años en despliegues de campo, coordinación de contratistas
- **Idioma:** Español nativo, inglés profesional

**Motivaciones:**
- Cumplir cronograma de implementación física
- Mantener buena relación con cuadrillas y proveedores
- Que su parte del proyecto no sea cuello de botella

**Frustraciones:**
- Que Integration culpe a Implementation cuando hay issues (fricción histórica)
- Falta de visibilidad de cuándo Integration está listo para empezar la ventana
- Cuadrillas a veces sub-rendimiento, requiere micromanagement

**Cómo prefiere trabajar:**
- Coordinación clara con Carlos como peer
- Información temprana del status de Integration
- Autonomía sobre cómo gestiona sus cuadrillas

**Cómo coordina con Carlos:**
- **Reunión semanal de peers** Carlos + Eduardo (45 min) para alinear backlog y plan
- Eduardo asiste a dailies de Carlos como observador/participante
- **Coordinación durante ventana:** ambos en stand-by, Eduardo coordina cuadrillas, Carlos coordina integradores; ambos hablan si hay issue cruzado
- Reportan al mismo CPM por encima

**Riesgo histórico de fricción:**
La relación NPM ↔ Implementation Manager ha sido fuente de fricción en proyectos anteriores de Ericsson. Este proyecto **identifica esa fricción como riesgo** y la maneja con:
- Acuerdo de Equipo explícito sobre coordinación de peers
- Reunión semanal de alineación
- Métricas compartidas (no "FTR de integración" y "FTR de implementation" separados, sino FTR de sitio único)

**Qué necesita Carlos de Eduardo:**
- Sitios físicamente listos (HW + energía + fibra) según calendario
- Comunicación temprana de retrasos en site readiness
- Disponibilidad durante ventanas para resolver issues cruzados HW/SW

---

## Cuadrillas locales (bajo Eduardo, pero relevantes para el equipo extendido)

### Persona 9 — Luis (Líder Cuadrilla 1 — local, externo)

**Datos:**
- **Rol:** Líder de Cuadrilla
- **Empresa:** Contratista externo (no Ericsson directo)
- **Ubicación:** San José Centro
- **Experiencia:** 15 años en obra civil RAN, ex-Ericsson

**Motivaciones:**
- Mantener su contrato con Ericsson largo plazo
- Ser percibido como cuadrilla de alto rendimiento
- Cuidar la seguridad de su equipo

**Frustraciones:**
- Cambios de programación de último minuto
- Sentir que su voz no se considera en decisiones técnicas
- Tiempos extra no compensados

**Cómo coordina:**
- Reporta a Eduardo (Implementation Manager)
- Coordina con integradores remotos (especialmente Diego/Ana) durante ventanas
- Participa en dailies del equipo extendido

---

### Persona 10 — Javier (Líder Cuadrilla 2 — local, externo)

**Datos:**
- **Rol:** Líder de Cuadrilla
- **Empresa:** Contratista externo (diferente a Luis)
- **Ubicación:** San José Oeste (cubre Arraiján, La Chorrera)
- **Experiencia:** 10 años en obra civil RAN

**Motivaciones:**
- Crecer su empresa contratista
- Construir reputación con Ericsson
- Capacitar a su equipo en LTE B41

**Frustraciones:**
- Distancia a San José Centro (logística)
- Comunicación a veces inconsistente con Ericsson Integration

**Cómo coordina:**
- Reporta a Eduardo
- Coordina con integradores en ventanas

---

### Persona 11 — Ricardo (Líder Cuadrilla 3 — local, externo)

**Datos:**
- **Rol:** Líder de Cuadrilla
- **Empresa:** Contratista externo (diferente a Luis y Javier)
- **Ubicación:** San José Este (cubre Tocumen, Don Bosco)
- **Experiencia:** 8 años en obra civil RAN

**Motivaciones:**
- Asegurar trabajo continuo
- Aprender el flujo ágil (nuevo para él)
- Mantener seguridad e impecabilidad de su trabajo

**Frustraciones:**
- Sentirse "el nuevo" entre las tres cuadrillas
- Necesita más capacitación en Jira

**Cómo coordina:**
- Reporta a Eduardo
- Coordina con integradores en ventanas

---

## Stakeholders del Cliente — Telemóvil Costa Rica

### Persona 12 — Roberto (Senior RAN Engineer Telemóvil)

**Datos:**
- **Rol:** Senior RAN Engineer
- **Empresa:** Telemóvil Costa Rica
- **Ubicación:** San José
- **Experiencia:** 12 años en RAN, ha trabajado con Ericsson, Nokia, Huawei
- **Idioma:** Español, inglés profesional

**Motivaciones:**
- Que la red entregue lo prometido en diseño
- Mantener su reputación interna en Telemóvil
- Aprender enfoques nuevos (abierto al ágil)

**Frustraciones:**
- Reportes incompletos o tardíos de Ericsson en proyectos pasados
- Sorpresas en aceptación (problemas descubiertos al final)
- Falta de visibilidad granular

**Cómo coordina con Ericsson:**
- **Contraparte técnica diaria de Carlos** y los integradores
- Valida y aprueba el template B41 antes del Golden Cluster
- Recibe reportes semanales de KPIs
- Participa en sesión semanal de re-priorización
- 🌟 **Invitado a la retrospectiva del Golden Cluster** (movimiento clave)

**Qué espera del proyecto:**
- Visibilidad continua al status
- Voz técnica considerada
- Problemas reportados temprano, no ocultados

---

### Persona 13 — Marcela (Planning Lead Telemóvil)

**Datos:**
- **Rol:** Planning Lead (planificación de red y capacidad)
- **Empresa:** Telemóvil Costa Rica
- **Ubicación:** San José
- **Experiencia:** 8 años en planificación de redes móviles
- **Idioma:** Español, inglés profesional

**Motivaciones:**
- Que la expansión absorba la demanda real
- Justificar inversiones con datos de uso
- Anticiparse a competencia (Tigo en zonas comerciales)

**Frustraciones:**
- Que las decisiones de priorización se tomen sin input de planning
- Datos de uso post-implementation lleguen tarde

**Cómo coordina con Ericsson:**
- **Contraparte de Carlos y optimizadores** (especialmente Marco y Sofía)
- Aporta datos de saturación para re-priorización semanal
- Recibe reportes de KPIs post-aceptación
- Participa en la sesión semanal de re-priorización

**Qué espera del proyecto:**
- Sitios priorizados por valor de negocio
- KPIs post-implementation que validen el diseño
- Comunicación temprana de cualquier desviación

---

### Persona 14 — Patricia (Quality Lead Telemóvil)

🔶 **Nuevo perfil — confirmar nombre real con Carlos.**

**Datos:**
- **Rol:** Quality Lead (aseguramiento de calidad de red)
- **Empresa:** Telemóvil Costa Rica
- **Ubicación:** San José
- **Experiencia:** 7 años en QA de red, ex-Ericsson en otra región
- **Idioma:** Español, inglés profesional

**Motivaciones:**
- Que cada sitio cumpla estándares de calidad de Telemóvil
- Defender la calidad frente a presión de cronograma
- Construir métricas de calidad replicables

**Frustraciones:**
- Sitios entregados con calidad mínima aceptable, no óptima
- Presión de Acceptance para aprobar antes de tiempo

**Cómo coordina con Ericsson:**
- **Contraparte de los optimizadores** (Marco, Sofía, Patricia Ericsson)
- Valida que los KPIs entregados cumplan estándares Telemóvil
- Su sign-off es parte de aceptación formal

**Qué espera del proyecto:**
- KPIs validados en periodo extendido (no solo 24h)
- Documentación de calidad completa
- Patrones de mejora identificados durante el proyecto

---

### Persona 15 — Fernando (O&M Lead Telemóvil)

🔶 **Nuevo perfil — confirmar nombre real con Carlos.**

**Datos:**
- **Rol:** Operations & Maintenance Lead
- **Empresa:** Telemóvil Costa Rica
- **Ubicación:** San José
- **Experiencia:** 15 años en operaciones de red móvil
- **Idioma:** Español, inglés profesional

**Motivaciones:**
- Recibir sitios listos para operación, sin issues colgados
- Minimizar trabajo de troubleshooting post-aceptación
- Mantener KPIs estables en producción

**Frustraciones:**
- Sitios "aceptados" que generan alarmas post-aceptación
- Falta de handover formal a O&M

**Cómo coordina con Ericsson:**
- **Contraparte de Eduardo (Implementation Manager)** principalmente
- También recibe handover de Carlos en cada sitio aceptado
- Coordina ventanas de mantenimiento con NOC Telemóvil

**Qué espera del proyecto:**
- Handover formal documentado por sitio
- Estabilidad de KPIs en primer mes post-aceptación
- Comunicación oportuna de configuración aplicada

---

### Persona 16 — Ricardo Mendoza (Acceptance Team Lead Telemóvil)

🔶 **Nuevo perfil — confirmar nombre real con Carlos. (Nota: hay dos Ricardos en el proyecto — Cuadrilla 3 y Telemóvil Acceptance. Distinguir en Jira.)**

**Datos:**
- **Rol:** Acceptance Team Lead
- **Empresa:** Telemóvil Costa Rica
- **Ubicación:** San José
- **Experiencia:** 10 años en validación y aceptación de despliegues
- **Idioma:** Español, inglés profesional

**Motivaciones:**
- Aceptar solo sitios que cumplan 100% de criterios
- Mantener estándares Telemóvil consistentes
- Que el proceso sea predecible para su equipo

**Frustraciones:**
- Sitios presentados con observaciones que requieren re-trabajo
- Documentación incompleta de SAD

**Cómo coordina con Ericsson:**
- **Contraparte de Carlos** para sign-off semanal
- Su equipo recibe los SADs en sesión de aceptación batch (viernes)
- Decisión final de aceptar/rechazar es suya

**Qué espera del proyecto:**
- Aceptación batch semanal funcional (formato nuevo)
- SADs completos y consistentes
- Cero sorpresas en sesión de aceptación

---

## Mapeo de coordinación Ericsson ↔ Telemóvil

Esta tabla materializa lo discutido sobre el mapeo:

| Equipo Telemóvil | Contraparte principal en Ericsson | Cadencia de coordinación |
|----------------|----------------------------------|--------------------------|
| **O&M (Fernando)** | Implementation Manager (Eduardo) | Coordinación continua + handover por sitio |
| **RAN Engineering (Roberto)** | Carlos + Integradores | Diaria durante ventanas + semanal técnica |
| **Planning (Marcela)** | Carlos + Optimizadores | Semanal (re-priorización) |
| **Quality (Patricia)** | Carlos + Optimizadores | Por sitio + sign-off de calidad |
| **Acceptance (Ricardo Mendoza)** | Carlos | Semanal (sesión de aceptación batch) |

---

## Persona implícita — Carlos (el participante)

### Datos:
- **Rol:** Network Performance Manager (NPM)
- **Empresa:** Ericsson
- **Ubicación:** Remoto (zona TZ Costa Rica / similar)
- **Experiencia:** Sólida en NPM; primer proyecto formal como Agile Project Leader

### Motivaciones:
- Lograr certificación Agile Project Leader con un proyecto real
- Aplicar metodología ágil a despliegue tradicionalmente cascada
- Construir su perfil profesional combinando técnico + liderazgo

### Retos personales en el proyecto:
- Es su primera vez facilitando dailies, retrospectivas, re-priorización formal
- Equipo distribuido geográficamente (Latam + India)
- Manejar peer dynamics con Eduardo (Implementation Mgr) sin generar fricción
- Validar el modelo ágil frente a un cliente acostumbrado al modelo tradicional

### Apoyo externo:
- Coach técnico/ágil (su hermano Germán, detrás de escena)
- Documentación del Proyecto Integrador
- Estructura de certificación Agile Project Leader

---

## Mapeo de Subcompetencias

- **3.2 Equipo de Alto Desempeño:** comprensión profunda de cada miembro es base para construir el equipo
- **3.3 Gestión de Involucrados:** mapeo completo de stakeholders Ericsson y Telemóvil con sus motivaciones

## Preguntas para Carlos

1. ¿Los perfiles de cada integrador/optimizador reflejan la realidad o ajustar (ubicación, experiencia, idioma)?
2. ¿Los nombres sintéticos te sirven o los reemplazas con nombres reales?
3. ¿Eduardo (Implementation Mgr) tiene nombre real conocido?
4. ¿La fricción histórica NPM ↔ Implementation Manager es real en tu experiencia o exagerada?
5. ¿Los 5 stakeholders de Telemóvil están todos identificados por nombre o algunos son aún sin contacto definido?
6. ¿La descripción de Sandeep (India) refleja un perfil real o ajustar (experiencia, idioma)?

---

**Siguiente:** [[Mapa-de-Involucrados]]
