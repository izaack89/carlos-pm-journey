---
title: Risk Register
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.2, 3.3, 1.5]
tags: [riesgos, calidad, mitigacion]
---

# Risk Register

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Risk Register inicial. Se actualiza en cada reunión semanal de pipeline.

## Propósito

Identificar, categorizar y planear la mitigación de los riesgos del proyecto. Materializa subcompetencia **1.2 Detección y Resolución de Riesgos y Problemas**.

---

## Estructura de cada riesgo

Cada riesgo tiene:
- **ID:** R-XXX-NN (categoría + número)
- **Descripción:** qué puede salir mal
- **Probabilidad:** Baja / Media / Alta
- **Impacto:** Bajo / Medio / Alto
- **Prioridad:** P × I = score
- **Owner:** quién monitorea
- **Mitigación:** acción preventiva
- **Plan de contingencia:** qué hacer si ocurre

---

## Matriz de prioridad

```
                  Impacto
              Bajo   Medio   Alto
Probabilidad
    Alta      P=3    P=6     P=9 🔴
    Media     P=2    P=4 🟡  P=6
    Baja      P=1    P=2     P=3
```

Score ≥ 6: monitoreo activo en cada daily.
Score 4-5: revisión semanal.
Score ≤ 3: monitoreo background.

---

## Categorías de riesgos

### Riesgos técnicos (R-TEC)
### Riesgos físicos / Implementation (R-FIS)
### Riesgos de equipo (R-EQUIPO)
### Riesgos cliente / Stakeholders (R-CLIENTE)
### Riesgos externos (R-EXT)

---

## Riesgos identificados (al inicio del proyecto)

### R-EQUIPO-01 — Aislamiento cultural y de TZ del integrador en India 🔴

**Categoría:** Equipo
**Descripción:** Sandeep (integrador remoto basado en India) tiene TZ +10.5h respecto a Costa Rica. Adicionalmente, no habla español (idioma informal del resto del equipo Latam). Riesgo de aislamiento, pérdida de información en handoffs, y fricción cultural.
**Probabilidad:** Alta (es contexto real, no especulación)
**Impacto:** Medio (afecta colaboración pero no detiene el flujo si se gestiona)
**Score:** 6 🔴

**Owner:** Carlos

**Mitigación:**
- Daily Kanban en **inglés** (decisión documentada en Acuerdo de Equipo)
- **Diego asignado como buddy cultural** de Sandeep
- Documentos clave traducidos al inglés
- Sandeep asignado a sitios donde su expertise (automatización) genera mayor valor
- Sandeep no se le asigna sitios que requieran coordinación intensa con cuadrillas locales en español
- Knowledge sharing sessions formales para que Sandeep exhiba su trabajo (refuerza pertenencia)

**Plan de contingencia:**
- Si participación de Sandeep en dailies cae < 70%, Carlos hace 1:1 individual
- Si emerge fricción cultural, Diego facilita conversación
- Como último recurso: ajustar asignaciones para minimizar coordinación síncrona

---

### R-EQUIPO-02 — Fricción histórica NPM ↔ Implementation Manager 🟡

**Categoría:** Equipo
**Descripción:** Históricamente en proyectos Ericsson, NPM e Implementation Manager tienen tensiones (separación de blame en bloqueos cruzados, métricas separadas). Carlos y Eduardo son peers en este proyecto.
**Probabilidad:** Media
**Impacto:** Alto (fricción peer puede paralizar handoffs)
**Score:** 6 🔴

**Owner:** Carlos + Eduardo + CPM

**Mitigación:**
- **Reunión semanal de peers** Carlos + Eduardo (lunes 8 AM)
- **Métricas compartidas** (FTR del sitio, no por parte)
- **Columna "Listo para Ventana"** como punto explícito de coordinación
- **Eduardo asiste a dailies** de Carlos (5 min update)
- **Acuerdo de Equipo** documenta peer dynamics
- Reportan al mismo CPM

**Plan de contingencia:**
- Si emerge tensión, conversación 1:1 entre Carlos y Eduardo (no en daily)
- Si no se resuelve, escalación al CPM
- Retrospectiva interna sin Telemóvil para discutir dinámicas

---

### R-TEC-01 — Template B41 requiere ajustes significativos post-cluster

**Categoría:** Técnico
**Descripción:** Hallazgos en los primeros 3 sitios pueden requerir ajustes mayores al template, retrasando despliegue masivo.
**Probabilidad:** Media
**Impacto:** Alto
**Score:** 6 🔴

**Owner:** Carlos + Diego (Integrador Senior)

**Mitigación:**
- Golden Cluster diseñado **específicamente** para detectar estos ajustes
- 5 sitios diversos (corredor + urbano + suburbano) para validación amplia
- Retrospectiva del cluster con Roberto (Telemóvil) para co-construir template v2

**Plan de contingencia:**
- Si template requiere cambios mayores: pausa de 3-5 días en sem 4 para implementar
- Si imposible aplicar v2 a todos los sitios: documentar variantes por tipo

---

### R-TEC-02 — Plan de RF desactualizado (caso CR-014) 🟡

**Categoría:** Técnico
**Descripción:** Planes de RF en sistemas Telemóvil pueden tener antigüedad > 3 meses, sin reflejar cambios urbanos (edificios nuevos, vegetación).
**Probabilidad:** Media
**Impacto:** Medio (causa re-trabajo de optimización)
**Score:** 4 🟡

**Owner:** Marco (Optimizadores Lead) + Roberto (Telemóvil)

**Mitigación:**
- **Freshness check** de plan de RF agregado a DoR (acción de retrospectiva del cluster)
- Plan con antigüedad > 3 meses requiere validación de campo o ajuste

**Plan de contingencia:**
- Si se detecta durante optimización: ajustes en tiempo real (tilt eléctrico, potencia)
- Caso documentado: CR-014 resuelto en 56h

---

### R-FIS-01 — Site readiness pendiente al inicio del proyecto

**Categoría:** Físico / Implementation
**Descripción:** Algunos sitios (CR-023 Vista Alegre identificado) pueden tener readiness pendiente al inicio.
**Probabilidad:** Alta (identificado al inicio)
**Impacto:** Medio
**Score:** 6 🔴

**Owner:** Eduardo (peer Implementation Manager)

**Mitigación:**
- Sitios pendientes diferidos a semana 7-8 en plan original
- Eduardo monitorea progreso semanalmente
- Comunicación temprana a Carlos sobre cambios de status

**Plan de contingencia:**
- Si readiness no se resuelve por semana 6: escalación a CPM
- Si sitio no se puede integrar en cronograma: re-priorizar con Marcela

---

### R-FIS-02 — Tower company causa retrasos imprevistos 🟡

**Categoría:** Físico / Implementation
**Descripción:** Permisos de tower companies (Telesites, American Tower) pueden tener delays inesperados.
**Probabilidad:** Media
**Impacto:** Medio
**Score:** 4 🟡

**Owner:** Eduardo + CPM

**Mitigación:**
- Validación de permisos en DoR
- Lead time de 2 semanas para nuevos permisos
- Caso CR-007 identificado en sem 5

**Plan de contingencia:**
- Sitio se difiere y se sustituye con otro listo

---

### R-FIS-03 — Cuadrilla con disponibilidad limitada 🟡

**Categoría:** Físico
**Descripción:** Las 3 cuadrillas tienen capacidad finita. Si se concentran muchos sitios en una zona (e.g., Centro = Luis), hay sobrecarga.
**Probabilidad:** Media
**Impacto:** Medio
**Score:** 4 🟡

**Owner:** Eduardo

**Mitigación:**
- Balanceo de carga en re-priorización semanal
- Caso visible en sem 5 (Eduardo re-balanceó CR-009 a Javier)
- Las 3 cuadrillas pueden cubrir zonas adyacentes en emergencia

**Plan de contingencia:**
- Si una cuadrilla tiene > 2 sitios/semana, redistribuir
- Capacitación cruzada de cuadrillas en LTE B41 para mayor flexibilidad

---

### R-CLIENTE-01 — Telemóvil cambia prioridades durante el proyecto 🟡

**Categoría:** Cliente
**Descripción:** Marcela puede solicitar cambiar el orden de sitios por urgencia comercial (caso: Bella Vista 91% saturación).
**Probabilidad:** Alta
**Impacto:** Bajo a Medio (el enfoque ágil acomoda esto)
**Score:** 4 🟡

**Owner:** Carlos

**Mitigación:**
- Re-priorización formal cada lunes con Marcela presente
- Backlog ordenable, sitios intercambiables
- Comunicación explícita de impacto en cronograma

**Plan de contingencia:**
- Si cambio significa diferir sitios críticos: discutir con CPM y CSM

---

### R-CLIENTE-02 — Una de las 5 áreas Telemóvil rechaza aceptación

**Categoría:** Cliente
**Descripción:** Acceptance Team (Ricardo Mendoza), Quality (Patricia), RAN (Roberto), Planning (Marcela), u O&M (Fernando) pueden rechazar un sitio.
**Probabilidad:** Media
**Impacto:** Medio
**Score:** 4 🟡

**Owner:** Carlos

**Mitigación:**
- DoD multi-nivel co-construida con las 5 áreas
- Sign-off temprano de las áreas durante el flujo
- Patricia (Quality) invitada a retrospectiva del cluster

**Plan de contingencia:**
- Sitio regresa a Optimización
- Identificar patrón si rechazos se repiten

---

### R-CLIENTE-03 — NOC Telemóvil (Fernando) no disponible para ventana

**Categoría:** Cliente
**Descripción:** Para integrar un sitio, se requiere ventana coordinada con NOC. Fernando puede no tener slots disponibles.
**Probabilidad:** Baja a Media
**Impacto:** Medio
**Score:** 3

**Owner:** Carlos + Eduardo

**Mitigación:**
- Solicitud de ventana con 48h de anticipación
- Coordinación mensual con Fernando para calendarizar

**Plan de contingencia:**
- Si no hay slot esta semana, sitio se difiere al menor impacto
- Negociar slots premium para sitios críticos

---

### R-EXT-01 — Clima adverso en Costa Rica interrumpe trabajos en sitio

**Categoría:** Externo
**Descripción:** Lluvias intensas (Costa Rica tiene 9 meses de lluvias) pueden impedir trabajo de cuadrillas.
**Probabilidad:** Media
**Impacto:** Bajo (retraso típico 1-2 días)
**Score:** 2

**Owner:** Eduardo

**Mitigación:**
- Cronograma con buffer de contingencia
- Trabajo SW (integradores) no afectado por clima

**Plan de contingencia:**
- Reagendar ventana cuando el clima permita
- Aprovechar para trabajo remoto (pre-staging, optimización de otros sitios)

---

### R-EXT-02 — Inseguridad en zonas específicas

**Categoría:** Externo
**Descripción:** Algunas zonas (Curundú, partes de Tocumen) tienen niveles de inseguridad que pueden afectar trabajo en sitio.
**Probabilidad:** Baja a Media
**Impacto:** Alto (seguridad de equipo)
**Score:** 4 🟡

**Owner:** Eduardo + líderes de cuadrilla

**Mitigación:**
- Coordinación con seguridad privada de Telemóvil
- Trabajo de día cuando sea posible
- Equipo en pares, nunca solo

**Plan de contingencia:**
- Cancelar ventana si hay incidentes activos
- Coordinación con autoridades locales

---

## Heatmap visual

```
                Impacto
            Bajo    Medio   Alto
   Alta     -       FIS-01  -
            -       EQUIPO-01 -
            -       CLIENTE-01 -
   Media    -       FIS-02   TEC-01
            -       TEC-02   EQUIPO-02
            -       FIS-03   -
            -       CLIENTE-02 -
            -       EXT-02   -
   Baja     -       CLIENTE-03 -
            EXT-01  -       -
```

---

## Indicadores de salud del Risk Register

| Indicador | Meta |
|-----------|------|
| Riesgos identificados al inicio | ≥ 10 |
| Riesgos nuevos por retrospectiva | 2-4 esperados |
| Riesgos cerrados durante el proyecto | ≥ 50% al final |
| Bloqueos sorpresa (sin riesgo previo) | < 20% del total |

---

## Mapeo de Subcompetencias

- **1.2 Detección y Resolución de Riesgos y Problemas:** este documento ES la materialización principal
- **3.3 Gestión de Involucrados:** riesgos de cliente y cuadrillas con owners específicos
- **1.5 Metrics & Reporting:** indicadores de salud del registry

## Preguntas para Carlos

1. ¿Los riesgos identificados son completos o falta alguno crítico de tu experiencia?
2. ¿La probabilidad/impacto asignados son razonables?
3. ¿Hay algún riesgo regulatorio o de licencias específico de Telemóvil?
4. ¿R-EQUIPO-02 (fricción NPM-Implementation) es real en tu contexto o exagerada?

---

**Siguiente:** [[Plan-de-Calidad]]
