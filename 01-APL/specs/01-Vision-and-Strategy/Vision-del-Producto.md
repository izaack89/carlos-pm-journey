---
title: Visión del Producto — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [1.1, 2.2, 1.5]
tags: [agile, kanban, lte, vision, ericsson, telemovil]
---

# Visión del Producto

## Contexto

Telemóvil, operador móvil en Costa Rica, enfrenta un incremento sostenido en el consumo de datos móviles en zonas urbanas y suburbanas. La saturación de la capa de capacidad LTE en banda 41 (2.5 GHz TDD) está afectando la experiencia de usuario, con degradación en throughput descendente y aumento en la utilización de PRB (Physical Resource Blocks) por encima del 70% en las horas pico.

Ericsson, como socio de despliegue, ha sido seleccionado para ejecutar la expansión de capacidad en 23 sitios LTE estratégicos. Este proyecto representa una oportunidad para transicionar de un modelo de gestión tradicional hacia **Agile Project Management**, aplicando **Lean & Kanban** como framework principal (ver [[Justificacion-del-Enfoque-Agil]]).

## Declaración de Visión

> **PARA** Telemóvil Costa Rica y sus suscriptores móviles en zonas de alta demanda de datos,
> **QUIENES** experimentan congestión de red, degradación de throughput y deterioro en la calidad de servicio LTE,
> **EL** proyecto de Expansión de Capacidad LTE Banda 41 **ES UNA** iniciativa de despliegue ágil de 23 sitios,
> **QUE** entrega capacidad adicional de red de forma incremental, con validación continua de performance y detección temprana de riesgos,
> **A DIFERENCIA DEL** modelo tradicional en cascada que entrega todos los sitios al final del ciclo con re-trabajos costosos,
> **NUESTRA SOLUCIÓN** aplica un flujo Kanban con **First Time Right** (definido operativamente en [[Definition-of-Done]]) como criterio de aceptación, retrospectivas tempranas en un golden cluster, y métricas de desempeño visibles para todos los involucrados.

## Objetivo SMART

> Lograr la integración y puesta en servicio al **100% de los 23 sitios LTE banda 41** en Costa Rica, incrementando la eficiencia operativa en un **10%** mediante la reducción de re-trabajos técnicos, en un ciclo de implementación de **8 semanas**.

### Desglose SMART

- **Específico:** Expansión de capacidad LTE B41 en 23 sitios identificados por Telemóvil Costa Rica.
- **Medible:** 23/23 sitios integrados; FTR ≥ 90%; reducción del 10% en horas-hombre de re-trabajo.
- **Alcanzable:** Cadencia promedio de ~3 sitios/semana con equipo de integración Ericsson y cuadrillas de campo locales.
- **Realista:** Basado en capacidad histórica de despliegue de Ericsson en la región y disponibilidad confirmada de HW.
- **De duración limitada:** 8 semanas, con hito intermedio de golden cluster (3 sitios) al final de la semana 4.

## Beneficios Esperados

### Para Telemóvil (cliente)

- **Capacidad adicional** en 23 celdas, reduciendo la utilización promedio de PRB en horas pico.
- **Mejora en experiencia de usuario:** incremento esperado en throughput descendente y reducción en latencia percibida.
- **Visibilidad continua del avance** vía tablero Kanban compartido y reportes semanales de aceptación.
- **Detección temprana de problemas** que en el modelo tradicional aparecerían en fase final de aceptación.

### Para Ericsson (entregador)

- **Reducción de re-trabajos técnicos** en un 10%, liberando capacidad del equipo de integración para otros proyectos.
- **Validación temprana de configuraciones** vía golden cluster, evitando propagar errores de parametrización a los 20 sitios restantes.
- **Mejora en la relación con el cliente** gracias a la cadencia de validación semanal.

### Para los suscriptores finales

- Mejora tangible en velocidad y estabilidad del servicio móvil en zonas afectadas por congestión.

## Métricas de Éxito

### Métricas de entrega (ownership: Ericsson — Carlos como NPM)

| Métrica | Definición | Meta |
|---|---|---|
| **First Time Right (FTR)** | % de sitios integrados al primer intento sin alarmas críticas ni desviaciones de KPI | ≥ 90% |
| **Cycle time por sitio** | Tiempo desde llegada de HW al sitio hasta aceptación de Telemóvil | ≤ 5 días hábiles |
| **Lead time del proyecto** | Tiempo total de los 23 sitios | ≤ 8 semanas |
| **Re-trabajos técnicos** | Horas-hombre invertidas en corregir errores post-integración | -10% vs baseline |
| **Cumplimiento de aceptación semanal** | Sitios aceptados por Telemóvil cada semana | Según plan adaptativo |

### Métricas de red (ownership: Telemóvil, validadas por Carlos como NPM)

| Métrica | Definición | Comportamiento esperado |
|---|---|---|
| **PRB Utilization** | Utilización de Physical Resource Blocks en horas pico | Reducción significativa post-expansión |
| **DL Throughput** | Throughput descendente promedio por celda | Incremento medible |
| **RSRP / RSRQ** | Calidad de señal recibida | Estable o mejorada en el área |
| **Alarmas críticas** | Conteo de alarmas categoría 1-2 post-integración | 0 alarmas críticas sostenidas |
| **Drop Call Rate (DCR)** | Tasa de llamadas caídas en el cluster | Estable o reducida |

## Segmento de Usuarios Afectados

- **Suscriptores móviles** en las zonas geográficas de los 23 sitios seleccionados.
- **Operaciones de red de Telemóvil:** NOC, ingeniería RAN, planeación.
- **Equipos de Ericsson:** PMO, integración RAN, performance management, implementación.
- **Cuadrillas de campo subcontratadas** para instalación física en sitio.

## Por qué Banda 41

LTE banda 41 (2.5 GHz, TDD) ofrece:

- **Mayor capacidad** comparada con bandas de cobertura (B28, B5) debido a anchos de banda mayores (típicamente 20 MHz o más con CA).
- **TDD asimétrico** configurable para favorecer tráfico descendente, alineado con el patrón de consumo móvil actual (streaming, descarga).
- **Reutilización de infraestructura** existente — la mayoría de los sitios ya cuentan con sectores en bandas inferiores y la expansión añade B41 como capa de capacidad sin reemplazar la cobertura.
- **Espectro disponible** ya licenciado a Telemóvil por SUTEL (Autoridad Nacional de los Servicios Públicos de Costa Rica).

## Restricciones y Supuestos

### Supuestos

- HW (RRUs, antenas, baseband) ya procurado o con fechas de entrega confirmadas.
- Permisos municipales y de propietarios de sitio resueltos antes del inicio del proyecto.
- Disponibilidad de ventanas de mantenimiento nocturnas para integración.
- Equipo de cuadrillas de campo con capacidad para 3 sitios/semana en cadencia sostenida.

### Restricciones

- Ventana de 8 semanas para entrega completa (compromiso comercial con Telemóvil).
- Equipo Ericsson de integración con bandwidth compartido entre este proyecto y otros despliegues activos.
- Dependencia de energía ICE local (operador eléctrico de Costa Rica) para sitios sin infraestructura redundante.

## Mapeo de Subcompetencias

Este documento toca las siguientes subcompetencias del Proyecto Integrador:

- **2.2 Value Driven Delivery:** la visión prioriza explícitamente la entrega de valor incremental a Telemóvil (sitios entregados semanalmente) y a los suscriptores (mejora de experiencia). La priorización por congestión actual se aborda en [[Sesion-Repriorizacion]].
- **1.5 Metrics & Reporting:** la sección de métricas de éxito define tanto métricas de entrega como de red, base para el [[Burndown-y-Metricas]] y el dashboard de KPIs.
- **1.1 Planeación Adaptativa:** el cronograma de 8 semanas con golden cluster intermedio permite re-secuenciar sitios según hallazgos del cluster.

## Preguntas para Carlos

> Validar antes de finalizar este documento:

1. **¿La zona geográfica exacta de los 23 sitios es la San José, otra región o nacional?** (Esto afecta detalles del Mapa de Involucrados — tower companies, autoridades municipales).
2. **¿El KPI baseline de PRB Utilization es público o se puede mencionar?** (Si sí, lo podemos cuantificar; si no, lo dejamos cualitativo).
3. **¿La cadencia real de Ericsson es ~3 sitios/semana o difiere?** Ajustar si es otro número.
4. **¿Existe un nombre interno del proyecto en Ericsson o Telemóvil que debamos usar?** (E.g., "Project Capacity Expansion PA-2026" o similar).
5. **¿La meta de FTR ≥ 90% es realista para Carlos o debería ser otro umbral (85%, 95%)?**
6. **¿La duración real del proyecto es exactamente 8 semanas o tiene buffer/contingencia?**

---

**Siguiente documento:** [[Mapa-de-Involucrados]]