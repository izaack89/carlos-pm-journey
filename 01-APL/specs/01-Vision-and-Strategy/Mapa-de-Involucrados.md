---
title: Mapa de Involucrados — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [3.3, 3.2, 1.2]
tags: [agile, stakeholders, lte, ericsson, telemovil]
---

# Mapa de Involucrados

## Propósito

Identificar a todos los grupos de interés del proyecto de Expansión LTE B41, clasificarlos por nivel de influencia e interés, y definir la estrategia de comunicación e involucramiento. Este documento da soporte a la subcompetencia **3.3 Gestión de Involucrados** y establece el canal de validación semanal con el cliente.

## Tabla Resumen de Stakeholders

### Internos — Ericsson

| Stakeholder | Interés | Influencia | Estrategia de involucramiento | Preocupaciones clave |
|---|---|---|---|---|
| **Customer Project Manager (CPM)** | Alto | Alta | Reportes diarios; participación en daily Kanban; escalación de bloqueos | Cumplimiento de timeline, márgenes, riesgos comerciales |
| **Network Performance Manager (Carlos)** | Alto | Alta | Owner del Kanban y de métricas; lidera retrospectivas | FTR, validación de KPIs, propagación de errores entre sitios |
| **Integration Engineers (RAN)** | Alto | Media | Daily standup; aceptación de criterios FTR; co-creación de Definition of Done | Disponibilidad de HW, ventanas de mantenimiento, calidad de pre-checks |
| **Implementation Team / Site Engineers** | Alto | Media | Comunicación directa con cuadrillas; reporte de readiness | Permisos, energía, acceso a sitios |
| **Customer Solutions Manager (CSM)** | Medio | Alta | Sync semanal; gestión de expectativas con Telemóvil | Relación comercial, escalaciones del cliente |
| **PMO Ericsson regional** | Medio | Media | Reporte semanal de estatus y KPIs | Visibilidad de portafolio, métricas comparables entre proyectos |
| **Managed Services (si aplica)** | Bajo | Media | Notificación post-aceptación para operación continua | Estabilidad operativa post-handover |

### Externos — Cliente (Telemóvil Costa Rica)

| Stakeholder | Interés | Influencia | Estrategia de involucramiento | Preocupaciones clave |
|---|---|---|---|---|
| **RAN Engineering Telemóvil** | Alto | Alta | Validación técnica semanal; revisión de parámetros pre-integración | Calidad de configuración, alineación con templates de red |
| **Network Operations Center (NOC) Telemóvil** | Alto | Alta | Notificación pre/post integración; revisión de alarmas | Estabilidad de red durante ventanas de mantenimiento |
| **Acceptance Team Telemóvil** | Alto | Alta | Sesión formal de aceptación por sitio; reporte de KPIs | Cumplimiento de criterios contractuales |
| **Planning / Capacity Telemóvil** | Medio | Alta | Sync inicial para priorización por congestión | Cobertura de zonas más críticas primero |
| **Gerencia / Sponsors Telemóvil** | Bajo | Alta | Reporte ejecutivo bi-semanal | Avance global, ROI, riesgos altos |

### Externos — Proveedores y Terceros

| Stakeholder | Interés | Influencia | Estrategia de involucramiento | Preocupaciones clave |
|---|---|---|---|---|
| **Cuadrillas de campo subcontratadas** | Alto | Media | Daily de coordinación; check-in/check-out por sitio | Logística, materiales, seguridad |
| **Tower companies** (propietarios de torres en Costa Rica) | Medio | Media | Coordinación de accesos vía CPM | Ventanas de acceso, peso estructural, daños |
| **Operador eléctrico local (ICE, CNFL según región)** | Medio | Media | Solicitudes de energía vía equipo de implementación | Tiempos de conexión, capacidad disponible |
| **SUTEL** (regulador panameño) | Bajo | Baja | Cumplimiento de normativa por parte de Telemóvil (Ericsson como ejecutor técnico) | Cumplimiento de licencia espectral B41 |

### Externos — Usuarios Finales

| Stakeholder | Interés | Influencia | Estrategia de involucramiento | Preocupaciones clave |
|---|---|---|---|---|
| **Suscriptores móviles en zonas afectadas** | Alto | Baja | Indirecto vía Telemóvil (notificaciones de mantenimiento si aplica) | Continuidad del servicio durante integración |

## Matriz Poder / Interés

Clasificación de los stakeholders en los cuatro cuadrantes clásicos:

### Alto Poder + Alto Interés (Gestionar de cerca)

- Customer Project Manager Ericsson
- Network Performance Manager (Carlos)
- Customer Solutions Manager
- RAN Engineering Telemóvil
- Acceptance Team Telemóvil
- NOC Telemóvil

**Estrategia:** Comunicación continua, daily/weekly syncs, involucramiento en decisiones clave.

### Alto Poder + Bajo Interés (Mantener satisfechos)

- Gerencia / Sponsors Telemóvil
- PMO Ericsson regional
- Planning / Capacity Telemóvil

**Estrategia:** Reporte ejecutivo periódico; no saturar con detalle operativo; escalar solo lo relevante.

### Bajo Poder + Alto Interés (Mantener informados)

- Integration Engineers
- Implementation Team
- Cuadrillas de campo
- Suscriptores finales (vía Telemóvil)

**Estrategia:** Información transparente, tablero Kanban accesible, comunicación frecuente sobre estatus.

### Bajo Poder + Bajo Interés (Monitorear)

- Managed Services
- SUTEL
- Operador eléctrico
- Tower companies (a nivel ejecutivo)

**Estrategia:** Cumplimiento de obligaciones contractuales/regulatorias; comunicación bajo demanda.

## Narrativa de los 5 Stakeholders Críticos

### 1. RAN Engineering Telemóvil

Es el contraparte técnico directo de Carlos. Define los templates de parámetros, valida la configuración pre-integración, y aprueba las desviaciones técnicas. **Riesgo de no involucrarlo bien:** rechazo de aceptación tardía por desviaciones de template, generando re-trabajo masivo.

**Estrategia:** Reunión técnica semanal de 30 minutos, revisión conjunta de configuraciones del próximo batch de sitios antes de la integración, escalación rápida ante dudas de parametrización.

### 2. NOC Telemóvil

Es quien detecta alarmas en tiempo real durante y post-integración. **Riesgo:** ruido de alarmas no coordinadas durante ventanas de mantenimiento puede generar percepción de inestabilidad incluso si todo está bajo control.

**Estrategia:** Coordinación pre-mantenimiento (correo + llamada), ventana de monitoreo conjunta post-integración (primera hora), criterios pre-acordados sobre qué alarmas son "esperadas" durante la integración.

### 3. Customer Project Manager (Ericsson)

Es el integrador de todas las dependencias internas y externas. **Riesgo:** sin alineación con Carlos como NPM, las priorizaciones comerciales pueden contradecir la lógica de calidad técnica (e.g., empujar un sitio sin validación de KPIs por presión de cliente).

**Estrategia:** Carlos y CPM acuerdan un Definition of Done compartido donde ningún sitio se "cierra" sin validación de performance, incluso bajo presión.

### 4. Integration Engineers (Ericsson)

Son quienes ejecutan la integración técnica. **Riesgo:** sin protocolos claros de FTR, pueden marcar sitios como "completos" que aún tienen issues menores, contaminando las métricas.

**Estrategia:** Acuerdo de equipo (ver subcompetencia 3.2) donde "completo" significa FTR validado por Carlos, no solo configuración aplicada. Comunicación abierta de problemas sin penalización.

### 5. Acceptance Team Telemóvil

Da el sign-off formal de cada sitio. **Riesgo:** criterios de aceptación ambiguos generan disputas y demoras.

**Estrategia:** Criterios de aceptación documentados y firmados al inicio del proyecto, alineados con el [[Definition-of-Done]]. Aceptación semanal en batch (no sitio por sitio) para reducir fricción.

## Plan de Comunicación

| Frecuencia | Audiencia | Canal | Contenido | Responsable |
|---|---|---|---|---|
| Diario | Equipo Ericsson (integración + Carlos + CPM) | Daily Kanban (15 min) | Estatus de sitios en flujo, bloqueos, próximos pasos | CPM facilita; Carlos contribuye con KPIs |
| Semanal | RAN Engineering Telemóvil | Reunión técnica (30 min) | Revisión de batch próximo, hallazgos del batch anterior | Carlos |
| Semanal | Acceptance Team Telemóvil | Sesión de aceptación (60 min) | Aceptación formal de sitios completados en la semana | Carlos + CPM |
| Semanal | NOC Telemóvil | Coordinación de ventanas + sync de alarmas | Calendario de integraciones, criterios de alarmas | Implementation Team |
| Bi-semanal | Gerencia Telemóvil + Sponsors | Reporte ejecutivo | Avance global, FTR, riesgos, próximos hitos | CSM + Carlos |
| Continuo | Cuadrillas de campo | WhatsApp / canal directo | Check-in/check-out, materiales, blockers | Implementation Team |

## Acuerdo de Comunicación con el Cliente (Subcompetencia 3.3)

Como parte del enfoque ágil, se establece un **canal directo Carlos ↔ RAN Engineering Telemóvil** independiente del flujo formal vía CPM, para resolver dudas técnicas rápidas sin pasar por escalación comercial. Este canal:

- Reduce el lead time de resolución de dudas técnicas
- Construye confianza técnica entre las partes
- No reemplaza la gobernanza formal, pero la complementa
- Tiene reglas claras: solo asuntos técnicos, decisiones comerciales siempre vía CPM/CSM

## Acuerdo de Equipo Interno (Subcompetencia 3.2)

Carlos liderará la creación de un **acuerdo de equipo** entre Integration Engineers y cuadrillas de campo que cubrirá:

- Protocolos de comunicación durante integración (qué reportar, cuándo, a quién)
- Definición compartida de "sitio completo"
- Manejo de imprevistos en campo (decisiones autónomas vs escalación)
- Respeto a las ventanas de mantenimiento de NOC Telemóvil
- Protocolo de retrospectiva post-batch

Este acuerdo se documenta en [[Acuerdo-de-Equipo]] y se revisa después del golden cluster.

## Mapeo de Subcompetencias

- **3.3 Gestión de Involucrados:** este documento define la estrategia completa de comunicación e involucramiento con cada stakeholder, incluyendo el canal directo con Telemóvil y la cadencia de validación semanal.
- **3.2 Equipo de Alto Desempeño:** se define el acuerdo de equipo entre integración y campo como mecanismo de cohesión y comunicación.
- **1.2 Detección y Resolución de Riesgos:** la matriz Poder/Interés y la narrativa de stakeholders críticos identifican proactivamente puntos de fricción que pueden materializarse como riesgos.

## Preguntas para Carlos

1. **¿El operador eléctrico relevante es ICE, ICE o ICE?** (Depende de la región geográfica de los sitios en Costa Rica).
2. **¿Existe una tower company específica involucrada en estos 23 sitios?** (E.g., American Tower Costa Rica, otra).
3. **¿El canal directo Carlos ↔ RAN Engineering Telemóvil ya existe informalmente o hay que formalizarlo?**
4. **¿La aceptación semanal en batch es viable con el Acceptance Team de Telemóvil, o ellos prefieren aceptación sitio-por-sitio?**
5. **¿El reporte ejecutivo bi-semanal a sponsors de Telemóvil es un compromiso real o se puede ajustar?**
6. **¿Hay un sponsor ejecutivo del lado Ericsson además del CPM?** (Director de cuenta, account manager).

---

**Siguiente documento:** [[Justificacion-del-Enfoque-Agil]]
**Documento anterior:** [[Vision-del-Producto]]