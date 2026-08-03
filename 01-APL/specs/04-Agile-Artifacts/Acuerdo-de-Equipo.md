---
title: Acuerdo de Equipo — Expansión LTE Banda 41 Costa Rica
proyecto: Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41
participante: Carlos Emmanuel Ramírez Castañón
rol: Network Performance Manager — Ericsson
cliente: Telemóvil (Costa Rica)
fecha: 2026-05-10
status: draft
subcompetencias: [3.2, 3.3, 1.4]
tags: [acuerdo, equipo, cuadrillas, integracion, optimizacion]
---

# Acuerdo de Equipo — Equipo Distribuido + Peer Dynamics

> 🎯 **Documento de diseño** — proyecto en fase de planeación. Este acuerdo se firma en el kickoff (semana 1) y se revisa en cada retrospectiva.

## Propósito

Establecer normas explícitas de colaboración para un equipo **geográficamente distribuido** (Latam + India + Costa Rica presencial) trabajando bajo un modelo de **peers coordinados** (Carlos + Eduardo). Este documento es clave para la subcompetencia **3.2 Equipo de Alto Desempeño**.

---

## Contexto especial de este proyecto

El equipo es atípico en varios sentidos:

1. **Carlos (NPM) es remoto** facilitando equipos también remotos
2. **Eduardo (Implementation Manager) es peer**, no subordinado de Carlos
3. **Integradores y optimizadores remotos** desde 4-5 países
4. **Un integrador en India** (Sandeep) — TZ +10.5h y diferencia cultural significativa
5. **Cuadrillas locales** (3 cuadrillas distintas, líderes independientes) presenciales en Costa Rica

Esto genera retos específicos:
- Comunicación cross-cultural (especialmente con Sandeep)
- Coordinación de peers Carlos ↔ Eduardo sin jerarquía
- Inclusión de cuadrillas locales en un flujo dominado por remotos
- Idioma del proyecto

---

## Decisión #1 — Idioma del proyecto

**Idioma oficial:** **inglés** para reuniones síncronas con todo el equipo (incluyendo daily).

**Razón:** garantizar que **Sandeep (integrador en India)** pueda participar plenamente. La diversidad lingüística no debe excluir a nadie del trabajo central.

### Excepciones permitidas

- **Coordinaciones bilaterales** entre dos hispanohablantes pueden ser en español
- **Documentación técnica formal** se mantiene en inglés (estándar Ericsson)
- **Documentación del Proyecto Integrador** se mantiene en español (es para certificación Carlos)
- **Comunicación con cuadrillas locales** en español por practicidad
- **Comunicación con Telemóvil** en español (cliente local)

### Reglas

- Cuando hay alguien que no domina el idioma local, **se cambia al inglés** para incluirlo
- **Documentos clave (DoR, DoD, template)** se traducen al inglés para que Sandeep los entienda
- **Carlos asigna un "buddy cultural"** a Sandeep (Diego) para reducir aislamiento

---

## Decisión #2 — Modelo de coordinación de peers (Carlos ↔ Eduardo)

### Principios

- Ninguno es jefe del otro
- Ambos reportan al mismo CPM
- Decisiones que afectan a ambos equipos se toman conjuntamente
- Conflictos se escalan al CPM solo si no se resuelven entre peers

### Mecanismos

- **Reunión semanal de peers** (Carlos + Eduardo), lunes 8:00 AM, 45 minutos
  - Revisión de avance de la semana
  - Validación conjunta de DoR de sitios próximos
  - Identificación temprana de issues cruzados
  - Coordinación de ventanas
- **Eduardo participa en dailies de Carlos** (5 min con su update de cuadrillas)
- **Carlos participa en dailies de Eduardo** opcional, cuando hay sitios próximos

### Reglas explícitas anti-fricción

- **Métricas compartidas, no separadas:** FTR es del sitio, no de "su parte"
- **Comunicación de bloqueos en tiempo real:** ambos notifican al otro inmediatamente
- **Decisiones que afectan al otro se consultan, no se imponen**
- **Conflictos públicos prohibidos:** si discrepan, se hablan en privado primero

---

## Compromisos del Equipo de Integradores (remotos)

### Antes de la ventana

- ✅ Pre-stage del template en ENM con 24h de anticipación
- ✅ Validar pre-checks de SW
- ✅ Confirmar disponibilidad para la ventana
- ✅ Coordinar con cuadrilla asignada vía Eduardo

### Durante la ventana

- ✅ Estar disponibles durante el horario de la ventana (típicamente nocturna en Costa Rica)
- ✅ Aplicar el template tal cual aprobado
- ✅ Comunicación continua con cuadrilla y Eduardo si surge issue cruzado
- ✅ Reportar progreso cada 30-60 min en Jira

### Al cerrar la integración

- ✅ Marcar checks técnicos en Jira con evidencia (logs, snapshots)
- ✅ Notificar al optimizador asignado
- ✅ NO mover el sitio sin validación del Optimizador

### Compromiso especial para Sandeep

- ✅ Documentar exhaustivamente (compensar barrera de comunicación oral)
- ✅ Compartir aprendizajes con el equipo en daily
- ✅ Buddy: Diego para apoyo cultural/contextual

---

## Compromisos del Equipo de Optimizadores (remotos)

### Antes de la integración

- ✅ Revisar configuración del template y umbrales esperados de KPIs
- ✅ Preparar dashboards en EMA del sitio
- ✅ Confirmar acceso a herramientas necesarias

### Durante la integración

- ✅ Disponible (on-call) durante la ventana por si surge tema de RF
- ✅ NO interrumpe trabajo del integrador salvo emergencia

### Post-integración

- ✅ Validación de KPIs en periodo de 24-48h
- ✅ Coordinación con Patricia (Quality Telemóvil) si requiere validación extendida
- ✅ Sin "validar y pasar" — la optimización es real, no firma
- ✅ Documentación de KPIs en el SAD

### Apoyo mutuo entre optimizadores

- ✅ Aunque cada uno tiene sitios asignados, **apoyan a quien tenga carga alta**
- ✅ Comparten patrones que descubren en daily
- ✅ Patricia (junior) tiene mentoría informal de Marco (senior)

---

## Compromisos de las Cuadrillas Locales (vía Eduardo)

### Antes del trabajo en sitio (T-48h)

- ✅ Confirmar asignación de cuadrilla
- ✅ Validar material disponible en bodega
- ✅ Reportar blockers conocidos en Jira (vía Eduardo)
- ✅ Coordinar logística (transporte, equipo)

### Durante el trabajo en sitio

- ✅ Check-in en el ticket al arribar (foto + timestamp)
- ✅ Reporte de progreso al menos 2 veces durante la jornada
- ✅ Coordinación directa con Integrador remoto cuando se requiera
- ✅ Documentar desviaciones del diseño

### Al cerrar el sitio físicamente

- ✅ Validación final con checklist (energía, fibra, conexión RRU, antenas)
- ✅ Fotos de evidencia subidas al ticket
- ✅ Notificación al Integrador asignado vía Jira (no WhatsApp)

### Comportamientos esperados

- ✅ Comunicación profesional, respetuosa
- ✅ Cumplir protocolos de seguridad sin excepción
- ✅ Reportar problemas temprano

---

## Compromisos compartidos por todo el equipo

### Sobre el tablero Kanban (Jira)

- 📌 **Jira es la realidad del proyecto.** Si no está en Jira, no existe.
- 📌 Todos los cambios de estado se registran en Jira, no en WhatsApp
- 📌 Los blockers se marcan explícitamente y se discuten en el daily
- 📌 Nadie cierra un ticket por otro sin coordinación

### Sobre el daily Kanban

- 📌 **9:00 AM Panamá** (10:30 PM en India — Sandeep se conecta a esa hora difícil; equipo le compensa con flexibilidad)
- 📌 **Duración estricta de 15 minutos**
- 📌 **Idioma: inglés**
- 📌 Asistencia de al menos un representante de cada equipo
- 📌 Foco en: ¿qué se cerró ayer?, ¿qué se cerrará hoy?, ¿qué bloquea?
- 📌 Bloqueos se discuten fuera del daily

### Sobre la comunicación general

- 📌 **Canal principal:** Jira (comentarios en el ticket)
- 📌 **Canal urgente:** chat de Teams/Slack del proyecto
- 📌 **Solo emergencias:** llamada telefónica directa
- 📌 **NO WhatsApp para decisiones operativas**

### Sobre los conflictos

- 📌 Si hay desacuerdo, se escala primero a Carlos (si es interno al equipo de Carlos) o a Carlos+Eduardo (si es cruzado)
- 📌 NO se exponen problemas internos frente a stakeholders de Telemóvil
- 📌 Las retrospectivas son el espacio para feedback estructurado
- 📌 Todos los conflictos se documentan brevemente para aprendizaje

### Compromiso con la inclusión

- 📌 **Sandeep no se queda fuera por idioma o TZ**
- 📌 **Cuadrillas no se ven como "ejecutoras"**, su voz aporta
- 📌 **Junior members tienen espacio** en retrospectivas
- 📌 **Nadie es invisible** — Patricia (Junior optimizadora) y Hugo (Junior integrador) participan activamente

---

## Decisión #3 — Reconocimiento al equipo

### Cadencia

**Semanal** en el reporte del viernes:
- Mención específica a quien aportó algo destacable esa semana
- Reconocimiento a cuadrillas cuando tienen FTR positivo
- Reconocimiento a integrador/optimizador con cero issues

### Quién facilita

Carlos lo lidera, pero **cualquier miembro del equipo puede proponer reconocimientos** durante el daily del viernes.

---

## Roles y responsabilidades clave

| Rol | Empresa | Reporta a | Responsabilidad principal |
|---|---|---|---|
| **Customer Project Manager (CPM)** | Ericsson | — | Owner contractual, escalación de conflictos cruzados |
| **Customer Success Manager (CSM)** | Ericsson | — | Relación comercial con Telemóvil |
| **Carlos (NPM)** | Ericsson | CPM | Owner del Kanban + facilitador ágil + lidera Integración y Optimización |
| **Eduardo (Implementation Manager)** | Ericsson | CPM (mismo que Carlos) | Owner de Implementation, peer de Carlos, lidera cuadrillas |
| **Integradores (4)** | Ericsson | Carlos | Calidad técnica de integración |
| **Optimizadores (3)** | Ericsson | Carlos | Calidad técnica de optimización |
| **Líderes de Cuadrilla (3)** | Contratistas externos | Eduardo | Ejecución física, seguridad en sitio |

---

## Revisiones y ajustes del acuerdo

### Cuándo se revisa

- **Después del Golden Cluster (Semana 4):** primera retrospectiva conjunta
- **Mitad del proyecto (Semana 6):** mini-retrospectiva, validación de adherencia
- **Cierre del proyecto (Semana 8):** consolidación de lecciones

### Cómo se ajusta

Cualquier miembro del equipo puede proponer un cambio al acuerdo. El cambio se discute en la retrospectiva más cercana y, si hay consenso, se documenta en una nueva versión.

---

## Firmas (al inicio del proyecto)

🔶 **[VALIDAR CON CARLOS]:** Confirmar nombres reales de los firmantes.

| Rol | Nombre | Fecha de firma |
|---|---|---|
| Customer Project Manager | [Por definir] | Semana 1 |
| Customer Success Manager | [Por definir] | Semana 1 |
| Network Performance Manager | Carlos Emmanuel Ramírez Castañón | Semana 1 |
| Implementation Manager | Eduardo [apellido] | Semana 1 |
| Integradores Lead (Diego) | Diego [apellido] | Semana 1 |
| Optimizadores Lead (Marco) | Marco [apellido] | Semana 1 |
| Integrador remoto (Sandeep — India) | Sandeep [apellido] | Semana 1 (vía Teams) |
| Líder de Cuadrilla #1 | Luis [apellido] | Semana 1 |
| Líder de Cuadrilla #2 | Javier [apellido] | Semana 1 |
| Líder de Cuadrilla #3 | Ricardo [apellido] | Semana 1 |

---

## Métricas de adherencia al acuerdo

| Métrica | Cómo se mide | Meta |
|---|---|---|
| **% de transiciones de estado en Jira (no en WhatsApp)** | Conteo manual semanal | ≥ 95% |
| **Participación de Sandeep en dailies** | Asistencia | ≥ 80% |
| **Asistencia general a dailies** | Conteo de representación por equipo | ≥ 85% |
| **Conflictos escalados al CPM** | Conteo absoluto | Tendencia decreciente |
| **Reconocimientos públicos a cuadrillas** | Conteo semanal | ≥ 1 por semana |

Estas métricas alimentan las retrospectivas.

---

## Mapeo de Subcompetencias

- **3.2 Equipo de Alto Desempeño:** este documento ES la materialización de esta subcompetencia
- **3.3 Gestión de Involucrados:** define cómo se gestionan internamente los equipos del proyecto + cuadrillas externas
- **1.4 Lean & Kanban:** establece Jira como única fuente de verdad del flujo

## Preguntas para Carlos

1. ¿La decisión de **inglés como idioma de daily** es viable o crea fricción?
2. ¿La reunión semanal de peers (Carlos + Eduardo) ya existe en proyectos similares o es nueva?
3. ¿Sandeep realmente está dispuesto a conectar a las 10:30 PM hora India para el daily? ¿O hay otra solución?
4. ¿Eduardo tiene apellido conocido? Mismo para integradores/optimizadores/cuadrillas.
5. ¿La meta de 95% de transiciones en Jira es realista al inicio?

---

**Ver también:** [[Personas]] (perfiles detallados de las 16 personas del equipo extendido) · [[Mapa-de-Involucrados]] (stakeholders externos)

**Siguiente:** [[Release-Plan]]
**Anterior:** [[Definition-of-Done]]
