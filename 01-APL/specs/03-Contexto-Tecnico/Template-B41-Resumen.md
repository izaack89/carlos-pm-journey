---
title: Template B41 — Resumen
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.4, 1.2]
tags: [tecnico, template, b41, configuracion]
---

# Template B41 — Resumen de Configuración

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Template propuesto para validación con Roberto (RAN Telemóvil) en kickoff.

## Propósito

Describir a alto nivel el template de configuración que se aplicará a los 23 sitios. Este documento es **no confidencial** — describe categorías y conceptos, no valores específicos de Telemóvil.

🔶 **[VALIDAR CON CARLOS]:** Cualquier valor específico aquí debe confirmarse o reemplazarse por descripciones cualitativas si es confidencial.

---

## Estructura del template

El template B41 se organiza en bloques de configuración:

### 1. Identificación del nodo
- Cell ID (asignado por Telemóvil según plan de red)
- PCI (Physical Cell Identifier)
- TAC (Tracking Area Code)
- PLMN (Public Land Mobile Network ID — Costa Rica: 714)

### 2. Configuración de radio (RF)
- **Banda:** 41 (2.5 GHz)
- **Bandwidth:** 20 MHz (estándar B41)
- **TDD configuration:** ratio DL:UL (típicamente 7:3 u 8:2)
- **Special subframe configuration**
- **Frequency offset**

### 3. Capa física
- **Reference signal power**
- **PRACH configuration**
- **PUCCH configuration**

### 4. MIMO y antenas
- **Antenna ports:** 4 (4x4 MIMO estándar) u 8 (8x8 MIMO en sitios premium)
- **Transmission mode**
- **Beamforming:** según capacidad del HW

### 5. Carrier Aggregation
- **Combinaciones permitidas:** B41+B28, B41+B5, eventualmente 3CA
- **Carrier secundario:** B41 actúa como SCell de las bandas inferiores

### 6. Features de Ericsson

| Feature | Propósito | Default en template |
|---|---|---|
| **ANR (Automatic Neighbor Relations)** | Auto-configuración de vecinos LTE | Activado |
| **Lean Carrier** | Reducción de overhead de señalización | Activado |
| **SON (Self-Organizing Networks)** | Auto-optimización de parámetros | Activado |
| **Cell Range Boost** | Mejora de cobertura en bordes | Configurable |
| **Massive MIMO Boost** | Solo en sitios premium con HW compatible | Variable |

### 7. Parámetros de movilidad
- **Handover thresholds:** RSRP, RSRQ, A3/A5 events
- **Inter-frequency handover:** B41 ↔ B28 ↔ B5
- **Inter-RAT handover:** LTE ↔ UMTS (si aplica)

### 8. QoS y QCI
- **QCI mappings:** según servicios de Telemóvil (voz, datos, video)
- **Bearer configurations:** default y dedicados

---

## Variantes del template

El template no es 100% uniforme. Existen variantes según el **tipo de sitio**:

### Variante Urbano Denso
- TDD ratio favorable a DL (8:2)
- ANR agresivo (muchos vecinos potenciales)
- MIMO 4x4 estándar
- CA habilitada con todas las bandas disponibles

### Variante Suburbano
- TDD ratio 7:3
- ANR estándar
- MIMO 4x4
- CA con B28 prioritaria (cobertura)

### Variante Corredor Comercial
- TDD ratio asimétrico (8:2 o más agresivo)
- MIMO 8x8 si el HW lo permite
- Beamforming activado
- Cell Range Boost configurable

---

## Cómo se aplica el template

### Vía ENM (Ericsson Network Manager) — Integrador remoto

1. **Pre-stage:** el template se carga en ENM y se valida sintácticamente (T-24h)
2. **Pre-checks del sitio:** SW compatible, HW correcto, license válida (paralelo con Cuadrilla)
3. **Aplicación:** durante la ventana de mantenimiento, ENM aplica el template al nodo
4. **Post-checks automáticos:** ENM reporta éxito/fallo
5. **Validación manual:** Integrador valida con AMOS si hay observaciones

### Trabajo paralelo durante ventana

```
T-0   T+30min  T+1h    T+2h    T+3h
 │      │      │       │       │
 │  Cuadrilla local instala HW en sitio
 │      │      │       │       │
 │  Integrador remoto aplica SW vía ENM
 │      │      │       │       │
 │      └──── Coordinación si hay issue cruzado
 │                                │
 │                          Optimizador remoto inicia
 │                          validación de KPIs
```

### Tiempo típico de aplicación

🔶 **[VALIDAR CON CARLOS]:** Tiempo aproximado por sitio en ventana.

- Pre-stage: 30 min en oficina
- Aplicación + HW en sitio: 2-3h durante la ventana nocturna
- Post-validación: 30 min adicionales
- **Total: ~3-4h por sitio en la ventana**

---

## Riesgos asociados al template

| Riesgo | Probabilidad | Mitigación |
|---|---|---|
| Versión MOM incompatible | Baja | Pre-checks validan SW del nodo |
| Conflicto con configuración existente | Media | Backup pre-aplicación, plan de rollback |
| Parámetro mal definido | Media | Golden cluster valida el template antes del despliegue masivo |
| ANR mal configurado causa interferencia | Media | Optimizadores validan vecindades post-integración |
| CA no negocia correctamente | Baja | Pruebas de UE post-integración |

Estos riesgos se trasladan al `[[Risk-Register]]` en su versión completa.

---

## Mejora continua del template (Subcompetencia 2.1)

El template **no es estático**. Después del Golden Cluster (3 sitios), se realiza una retrospectiva específica sobre el template:

- ¿Hubo parámetros que requirieron ajuste manual en varios sitios?
- ¿Hubo features que no se activaron correctamente?
- ¿Hubo combinaciones de CA que fallaron consistentemente?

Si se identifican ajustes, se aplican al template antes de continuar con los 20 sitios restantes. Esto **previene la propagación de errores**.

---

## Mapeo de Subcompetencias

- **1.4 Lean & Kanban:** el template estandariza el trabajo, facilitando el flujo Kanban
- **1.2 Detección de Riesgos:** los riesgos del template son input al risk register
- **2.1 Continuous Improvement:** la retrospectiva sobre el template es mejora continua tangible

## Preguntas para Carlos

1. ¿La estructura del template descrita refleja la realidad de Telemóvil?
2. ¿Existen variantes adicionales del template que omití?
3. ¿El tiempo aproximado por sitio (3-4h) en ventana es realista?
4. ¿Hay features Ericsson activadas en este proyecto que no mencioné?

---

**Ver también:** [[Definition-of-Done]] (el template se valida vía DoD) · [[Definition-of-Ready]] (template aprobado es parte del DoR)

**Anterior:** [[Herramientas-Ericsson]]
