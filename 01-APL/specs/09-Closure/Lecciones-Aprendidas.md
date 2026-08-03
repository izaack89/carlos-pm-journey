---
title: Lecciones Aprendidas
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [2.1, 3.2, 3.3]
tags: [lecciones, mejora-continua, cierre]
---

# Lecciones Aprendidas

> 🎯 **Simulación prospectiva** — proyecto en fase de planeación. Lecciones esperadas al cierre del proyecto.

## Propósito

Consolidar lecciones del proyecto en formato accionable y transferible a otros contextos. Diferenciar entre:
- Lecciones del **método ágil** (replicable)
- Lecciones del **dominio técnico** (B41, LTE)
- Lecciones del **equipo distribuido** (Latam + India)
- Lecciones de la **relación con cliente** (Telemóvil)
- Lecciones **personales de Carlos** como Agile Project Leader

---

## Categoría 1 — Lecciones del Método Ágil

### Lección 1.1 — El Golden Cluster es el corazón del método

**Contexto:** Hacer 5 sitios primero antes de los 20 restantes.

**Aprendizaje:** El Golden Cluster permite **encontrar problemas temprano** y aplicar mejoras al resto del proyecto. Detectamos:
- Plan de RF puede estar desactualizado (CR-014)
- Suburbanos requieren 72h validación, no 48h
- Cuadrilla 1 (Luis, Centro) tiende a sobrecargarse
- Sandeep necesita explicación cultural más rica

**Aplicable a:** cualquier proyecto de despliegue donde se puede agrupar trabajo similar.

**Action item:** documentar Golden Cluster como práctica estándar en Ericsson Latam.

### Lección 1.2 — Retrospectivas con el cliente construyen partnership

**Contexto:** Roberto (Telemóvil) fue invitado a la retrospectiva del Golden Cluster (semana 4).

**Aprendizaje:** La transparencia genera confianza más rápido que cualquier reporte. Roberto cambió de escéptico a advocate del método.

**Aplicable a:** clientes maduros, técnicamente competentes, abiertos a aprender.

**Riesgo:** clientes no preparados pueden ser disruptivos. Evaluar caso por caso.

### Lección 1.3 — WIP limits son sagrados pero pueden ajustarse

**Contexto:** WIP=3 en Integración con 4 integradores funcionó. WIP=3 en Optimización con 3 optimizadores fue ajustado en sem 5.

**Aprendizaje:** WIP limits sirven para proteger el flujo, pero deben revisarse en retrospectivas. No son dogma.

### Lección 1.4 — DoR multi-parte funciona para coordinación peer

**Contexto:** DoR dividida en Parte 1 (Eduardo/Implementation) + Parte 2 (Carlos/Integración).

**Aprendizaje:** Cuando hay dos peers, dividir DoR explícitamente reduce fricción. Cada peer es accountable de su parte.

**Aplicable a:** cualquier proyecto con handoffs entre equipos co-dependientes.

---

## Categoría 2 — Lecciones del Dominio Técnico (B41, LTE)

### Lección 2.1 — Plan de RF tiene caducidad

**Contexto:** Plan de RF de CR-014 era de 6 meses atrás, sin reflejar edificio nuevo.

**Aprendizaje:** RF planes con antigüedad > 3 meses requieren validación. Agregado a DoR.

### Lección 2.2 — Suburbanos validan KPIs en 72h, no 48h

**Contexto:** Vegetación y patrón de uso suburbano introduce variabilidad.

**Aprendizaje:** Periodo de validación debe ajustarse por tipo de sitio.

### Lección 2.3 — Automatización de pre-checks reduce 30→10 min

**Contexto:** Sandeep desarrolló scripts de validación que aplicaron a todos los sitios.

**Aprendizaje:** Invertir en automatización temprano paga dividendos. Considerar tiempo para automatización en planeación.

### Lección 2.4 — 3CA requiere validación específica

**Contexto:** CR-002 fue piloto de 3CA en la red de Telemóvil.

**Aprendizaje:** Features avanzados deben probarse en sitios controlados antes del despliegue masivo.

---

## Categoría 3 — Lecciones del Equipo Distribuido

> ℹ️ Los números X.Y de las lecciones se refieren a **Categoría.Lección** dentro de este documento, **no** a subcompetencias APL. Para evitar confusión con la **Subcompetencia 3.1 (Liderazgo Colaborativo)** definida en `Evidencia-Subcompetencias.md`, la cobertura de subcompetencias se declara en el frontmatter y en el mapa de evidencia, no aquí.

### Lección 3.1 — La inclusión es activa, no automática

**Contexto:** Sandeep en India con TZ +10.5h y barrera de idioma.

**Aprendizaje:** Sin acciones deliberadas (daily en inglés, cultural buddy, documentación), Sandeep se habría aislado. Las acciones deliberadas funcionaron — 88% participación.

**Aplicable a:** cualquier equipo geográficamente o culturalmente diverso.

### Lección 3.2 — Cultural buddies funcionan

**Contexto:** Diego como cultural buddy de Sandeep.

**Aprendizaje:** Asignar un punto de contacto reduce fricción cultural significativamente. El buddy debe ser senior y disponible.

**Action item:** formalizar el modelo en próximos proyectos.

### Lección 3.3 — TZ challenges son negociables, no inevitables

**Contexto:** Sandeep conectándose a 10:30 PM hora India.

**Aprendizaje:** Sandeep aceptó el horario pero se compensó con flexibilidad. La carga del TZ challenge no debe caer solo en quien tiene la peor hora.

### Lección 3.4 — Pre-stage del template ahorra ~1 hora por sitio

**Contexto:** Integradores hicieron pre-stage 24h antes de cada ventana.

**Aprendizaje:** 1 hora × 23 sitios = 23 horas ahorradas. Práctica replicable.

### Lección 3.5 — Junior members crecen cuando tienen mentorías informales

**Contexto:** Marco mentorizando a Patricia (junior); Diego mentorizando a Hugo y Ana.

**Aprendizaje:** Las mentorías informales son tan valiosas como las formales. Crear espacio para que ocurran.

---

## Categoría 4 — Lecciones del Cliente (Telemóvil)

### Lección 4.1 — 5 áreas Telemóvil requieren reportes diferenciados

**Contexto:** RAN, Planning, Quality, O&M, Acceptance.

**Aprendizaje:** Un reporte "para Telemóvil" no funciona. Reportes específicos por área son mejor recibidos y accionables.

### Lección 4.2 — Planning aporta valor real al ágil

**Contexto:** Marcela aportó saturación 91% en Bella Vista; re-priorización justificada.

**Aprendizaje:** El equipo de Planning del cliente es **socio de la re-priorización**, no audiencia. Invitarlo a la sesión semanal de re-priorización.

### Lección 4.3 — Quality involucrada desde el cluster previene rechazos al final

**Contexto:** Patricia Telemóvil participó desde sem 2.

**Aprendizaje:** Validación temprana con Quality previene sorpresas. 0 sitios rechazados por calidad técnica.

### Lección 4.4 — Sesión batch de aceptación es más eficiente

**Contexto:** Ricardo Mendoza acepta batch semanal vs individual.

**Aprendizaje:** Reducción de overhead de coordinación. Recomendable para todos los proyectos.

---

## Categoría 5 — Lecciones Personales de Carlos como Agile Project Leader

### Lección 5.1 — Facilitar > Controlar

**Contexto:** Primer proyecto formal como Agile Project Leader.

**Aprendizaje:** Cuando intenté tomar decisiones que correspondían al equipo (en sem 2), se notó la tensión. Cuando facilité para que el equipo decidiera (sem 3+), funcionó.

### Lección 5.2 — Métricas compartidas > separadas

**Contexto:** FTR del sitio, no de mi parte.

**Aprendizaje:** Esto cambió radicalmente la dinámica con Eduardo. Métricas compartidas crean colaboración.

### Lección 5.3 — Documentación es coaching silencioso

**Contexto:** Documentar DoR, DoD, Acuerdo de Equipo.

**Aprendizaje:** Los documentos sirven para alinear sin tener que repetir. Cuando hay duda, "está en el documento" zanja la conversación.

### Lección 5.4 — El silencio facilita más que el habla

**Contexto:** En retrospectivas, hablar menos y dejar al equipo hablar más.

**Aprendizaje:** El facilitador no es el que habla; es el que crea espacio.

### Lección 5.5 — Riesgos no son negatividad, son información

**Contexto:** Risk Register con 11 riesgos iniciales.

**Aprendizaje:** Plantear riesgos abiertamente no es pesimismo. Es preparación.

### Lección 5.6 — El cliente puede ser aliado del método

**Contexto:** Caso Roberto (Telemóvil).

**Aprendizaje:** Cuando el cliente entiende el método, deja de ser auditor y se convierte en colaborador.

---

## Anti-patrones identificados (cosas a NO hacer)

### Anti-patrón 1 — WhatsApp para decisiones operativas

Aprendizaje del acuerdo de equipo: la línea entre "emergencia" y "urgente" es ambigua. Las cuadrillas necesitaban WhatsApp para emergencias físicas reales, pero el riesgo es que se extienda a todo. Solución: definir explícitamente qué es emergencia.

### Anti-patrón 2 — Asumir que un solo correo a "Telemóvil" llega a todos

Hay 5 áreas. Cada una necesita comunicación específica.

### Anti-patrón 3 — Dejar al miembro junior solo

Hugo (junior) reportó en retrospectiva que no se atrevió a preguntar en grupo. Office hours ayudaron pero no fueron suficientes. Mentorías informales 1:1 fueron mejor solución.

### Anti-patrón 4 — Tratar al peer como subordinado

Eduardo y Carlos pudieron haber caído en fricción si Carlos hubiera asumido jerarquía. Las reglas explícitas de peer dynamics evitaron esto.

### Anti-patrón 5 — Cerrar SAD sin sign-off de O&M

Fernando (Telemóvil) pidió ser parte del handover. Sin esto, sitios "Done" generan alarmas post-aceptación.

---

## Lecciones que se transferirán

### Para próximos proyectos Ericsson Latam

| Lección | Cómo se transfiere |
|---|---|
| Golden Cluster como práctica | Documentar en playbook Latam |
| Daily en inglés inclusivo | Recomendación para equipos multinacionales |
| DoR multi-parte | Template adaptable |
| Reportes diferenciados por área cliente | Template adaptable |

### Para Telemóvil Costa Rica

| Lección | Cómo se transfiere |
|---|---|
| Modelo ágil para despliegues | Roberto interno comparte con su equipo |
| Re-priorización con Planning | Marcela como referente |

### Para Carlos personalmente

| Lección | Cómo aplica |
|---|---|
| Facilitar > Controlar | Mentalidad para próximos proyectos |
| Métricas compartidas | Práctica replicable |
| Documentar como coaching | Estilo de liderazgo |

---

## Mapeo de Subcompetencias

- **2.1 Continuous Improvement:** este documento ES la cosecha de la mejora continua
- **3.2 Equipo de Alto Desempeño:** lecciones del equipo distribuido
- **3.3 Gestión de Involucrados:** lecciones del cliente

## Preguntas para Carlos

1. ¿Hay lecciones específicas de Telemóvil que no aparecen aquí?
2. ¿Las lecciones personales reflejan tu crecimiento esperado?
3. ¿Los anti-patrones identificados son reconocibles en tu experiencia?

---

**Siguiente:** [[Resumen-Ejecutivo]]
**Anterior:** [[Retrospectiva-Final]]
