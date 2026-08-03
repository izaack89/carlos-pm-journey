---
title: Topología y Alcance Técnico — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [2.2, 1.2]
tags: [tecnico, topologia, lte, b41]
---

# Topología y Alcance Técnico

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Articula el contexto técnico para audiencias no especializadas (graders del Proyecto Integrador, sponsors no técnicos).

## Propósito

Explicar **qué se hace técnicamente** en el proyecto, sin entrar en parametrización detallada confidencial.

---

## Qué es LTE Banda 41

**LTE Banda 41** es una banda de espectro radioeléctrico que opera en **2.5 GHz** con tecnología **TDD (Time Division Duplex)**. Es una banda de **capa de capacidad**, no de cobertura.

### Diferencia entre capa de capacidad y capa de cobertura

| Característica | Banda baja (ej. B28 — 700 MHz) | Banda 41 (2.5 GHz) |
|---|---|---|
| **Propagación** | Largo alcance, penetra paredes | Corto alcance, menos penetración |
| **Capacidad** | Limitada | Alta — anchos de banda mayores |
| **Uso típico** | Cobertura amplia, indoor | Capacidad en zonas densas |
| **Throughput** | Menor | Mayor (con CA puede superar 200 Mbps) |

En la red de Telemóvil Costa Rica, **B41 complementa las bandas inferiores**: los sitios ya tienen cobertura con B28, B5 u otras, y se agrega B41 para absorber la demanda de datos creciente.

---

## Alcance del proyecto en la red

### Lo que el proyecto SÍ hace

- **Activar B41 en 23 sitios** que actualmente no la tienen o la tienen subdimensionada
- **Instalar HW adicional:** RRU 2.5 GHz, antenas si requieren, capacidad de baseband (responsabilidad de Implementation, vía cuadrillas)
- **Configurar parametrización SW** alineada con el template aprobado (responsabilidad de Integradores)
- **Activar features de optimización:** ANR, MIMO 4x4 (8x8 en sitios premium si aplica), Carrier Aggregation
- **Validar y optimizar KPIs** post-integración (responsabilidad de Optimizadores)

### Lo que el proyecto NO hace

- No despliega 5G NR (aunque el diseño debe permitir migración futura)
- No modifica la red core (EPC, IMS)
- No despliega Massive MIMO en sitios donde no estaba contemplado
- No interviene en sitios fuera del scope de los 23 identificados
- No reemplaza HW existente — solo agrega capacidad

---

## Quién hace qué técnicamente

| Área técnica | Responsable | Tipo de equipo |
|---|---|---|
| **HW** (instalación física RRU, antenas, cables) | Cuadrillas locales (Luis/Javier/Ricardo) bajo Eduardo | Local presencial |
| **Energía/Fibra in-situ** | Cuadrillas locales bajo Eduardo | Local presencial |
| **Pre-stage del template** | Integradores (Diego/Ana/Sandeep/Hugo) | Remoto |
| **Aplicación del template vía ENM** | Integradores | Remoto |
| **Validación SW post-integración** | Integradores | Remoto |
| **Validación KPIs post-integración** | Optimizadores (Marco/Sofía/Patricia) | Remoto |
| **Ajustes finos de RF** | Optimizadores | Remoto |
| **Coordinación general** | Carlos (NPM) | Remoto |
| **Coordinación Implementation** | Eduardo (peer) | Local en Costa Rica |

---

## Cómo se inserta B41 en la red de Telemóvil

### Arquitectura simplificada (vista del proyecto)

```
                    ┌──────────────────────┐
                    │   Core / EPC Telemóvil │
                    └──────────┬───────────┘
                               │
                    ┌──────────┴───────────┐
                    │  Transport (Fibra)   │
                    └──────────┬───────────┘
                               │
        ┌──────────────────────┼──────────────────────┐
        │                      │                      │
   ┌────┴─────┐          ┌────┴─────┐          ┌────┴─────┐
   │ Sitio 1  │          │ Sitio 2  │   ...    │ Sitio 23 │
   │ (B28 +   │          │ (B28 +   │          │ (B28 +   │
   │  B41 ✨) │          │  B41 ✨) │          │  B41 ✨) │
   └──────────┘          └──────────┘          └──────────┘

   ✨ = layer agregado por este proyecto
```

### Capas RAN en cada sitio post-proyecto

| Capa | Banda | Propósito | Estado |
|---|---|---|---|
| **Cobertura** | B28 (700 MHz) | Penetración indoor, alcance amplio | Existente |
| **Cobertura intermedia** | B5, B2 (variable) | Capacidad media | Existente |
| **Capacidad** | **B41 (2.5 GHz)** | Absorción de demanda alta | **Activada por el proyecto** |

---

## Carrier Aggregation (CA) — el valor multiplicador

B41 no opera aislada. Mediante **Carrier Aggregation**, se combina con las bandas existentes para entregar throughput significativamente mayor al usuario final.

### Combinaciones típicas en este proyecto

| Configuración | Bandas combinadas | Throughput teórico DL (aprox.) |
|---|---|---|
| **B41 sola** | 20 MHz B41 | ~150 Mbps |
| **B41 + B28** | 20 MHz B41 + 10 MHz B28 | ~225 Mbps |
| **B41 + B28 + B5** | 3CA | ~300 Mbps |

🔶 **[VALIDAR CON CARLOS]:** Configuración exacta de CA según template de Telemóvil.

---

## TDD — Time Division Duplex

B41 usa **TDD**, no FDD. Esto significa que el uplink y downlink comparten la misma frecuencia, alternándose en el tiempo.

### Implicaciones

- **Ratio configurable** DL:UL — típicamente 7:3 u 8:2 para favorecer descarga
- **Sincronización entre sitios** requerida para evitar interferencia
- **Eficiencia espectral** mayor que FDD en escenarios asimétricos (como el patrón de uso móvil actual)

---

## Alcance específico del rol de Carlos (NPM)

Carlos como **Network Performance Manager** no diseña la arquitectura — esa es decisión corporativa de Telemóvil + Ericsson Solutions. Su rol en el proyecto:

1. **Coordinar Integración y Optimización** (sus dos equipos directos)
2. **Coordinar con Eduardo (peer Implementation Manager)** en el handoff físico/SW
3. **Validar que cada sitio post-integración** entregue los KPIs esperados según diseño (vía optimizadores)
4. **Detectar interferencias** entre sitios B41 adyacentes (vía optimizadores)
5. **Monitorear KPIs de red** durante la fase de optimización
6. **Reportar performance** semanalmente al cliente (5 áreas Telemóvil)
7. **Identificar oportunidades de mejora** vía retrospectiva del Golden Cluster

---

## Mapeo de Subcompetencias

- **2.2 Value Driven Delivery:** la topología explica dónde se materializa el valor (sitios con capacidad incremental)
- **1.2 Detección de Riesgos:** comprensión técnica permite identificar riesgos específicos (interferencia, CA mal configurada, etc.)

## Preguntas para Carlos

1. ¿La configuración de CA descrita (B41+B28, eventualmente 3CA) coincide con el template real?
2. ¿El TDD ratio es 7:3, 8:2 u otro? ¿Es configurable por sitio o uniforme?
3. ¿Hay alguna feature crítica (Massive MIMO, Beamforming) que se active en algunos sitios y no en otros?
4. ¿Los 23 sitios usan el mismo HW model o hay variantes?

---

**Ver también:** [[Vision-del-Producto]] (objetivo SMART del proyecto) · [[Product-Backlog]] (los 23 sitios priorizados) · [[Risk-Register]] (riesgos técnicos asociados)

**Siguiente:** [[Herramientas-Ericsson]]
