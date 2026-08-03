# 📡 Despliegue Ágil LTE B41 · Telemóvil Costa Rica

### 23 sitios · 8 semanas · First Time Right ≥ 90%

> **Proyecto Integrador del programa Agile Project Leader (APL)** — vault de diseño, simulación de ejecución y evidencia para certificación.

| | |
|---|---|
| **Participante** | Carlos Emmanuel Ramírez Castañón |
| **Rol** | Network Performance Manager (NPM), Ericsson |
| **Cliente** | Telemóvil Costa Rica |
| **Proyecto** | Optimización ágil del despliegue de Expansión para 23 sitios LTE banda 41 |
| **Programa formativo** | Agile Project Leader (APL) — 13 módulos · 9 subcompetencias seleccionadas |
| **Fase del proyecto** | Planeación → arranque de ejecución |
| **Cronograma** | 8 semanas de ejecución + 4 semanas de entregables APL · 5 hrs/semana |
| **Fecha del vault** | mayo 2026 |

📂 **Material oficial del PIDA:** [[02.DefinicionPIDA-APL]] · `specs/entregables/` (Definition, Plan de Trabajo, Defensa, entregables por semana)
🎓 **Material del curso APL:** [[Index-APL|Index-APL.md]] — 358 PDFs en `documentation/` organizados en 13 módulos

---

## 🎯 Importante: este vault es prospectivo

Todos los documentos del vault están construidos en modo **diseño + simulación prospectiva** porque el proyecto arranca pronto. Esto significa:

- **El diseño del enfoque ágil es real y aplicable** desde el día 1
- **Las simulaciones de ceremonias** (Día 1, Daily, Retrospectivas, Bloqueos) son guiones de lo que se espera vivir
- **Los datos cuantitativos** (FTR, lead times, etc.) son **proyecciones**, no resultados reales
- **Las personas y stakeholders** combinan información real con nombres sintéticos donde no hay nombre real confirmado

Cada documento abre con el marcador 🎯 indicando su naturaleza.

Una vez que el proyecto arranque, Carlos puede ir actualizando los documentos con datos reales conforme avanza.

---

## 📂 Estructura del vault

```
vault/
├── 02-Discovery/
│   └── Personas.md                              ← 16 perfiles del equipo extendido
├── 03-Contexto-Tecnico/
│   ├── Topologia-y-Alcance.md                   ← Qué hace el proyecto técnicamente
│   ├── Herramientas-Ericsson.md                 ← ENM, EMA, AMOS, Jira
│   └── Template-B41-Resumen.md                  ← Configuración a aplicar
├── 04-Agile-Artifacts/
│   ├── Product-Backlog.md                       ← Tablero Kanban + 23 sitios
│   ├── Definition-of-Ready.md                   ← DoR multi-parte (Carlos + Eduardo)
│   ├── Definition-of-Done.md                    ← DoD 3-niveles (con 5 áreas Telemóvil)
│   ├── Acuerdo-de-Equipo.md                     ← Normas del equipo distribuido
│   └── Release-Plan.md                          ← Plan de 8 semanas
├── 05-Ceremonies-Simulation/
│   ├── Dia-1-Proyecto.md                        ← Kickoff simulado
│   ├── Daily-Kanban-Sample.md                   ← Sesión típica simulada
│   ├── Bloqueo-Simulado-y-Resolucion.md         ← Caso CR-014
│   ├── Retrospectiva-Golden-Cluster.md          ← Retro con Roberto (Telemóvil) invitado
│   └── Sesion-Repriorizacion.md                 ← Re-priorización con Marcela
├── 06-Tracking-and-Metrics/
│   ├── Burndown-y-Metricas.md                   ← 11 métricas, reportes diferenciados
│   └── burndown-data.csv                        ← Datos por sitio (proyectados)
├── 07-Risk-and-Quality/
│   ├── Risk-Register.md                         ← 11 riesgos identificados
│   └── Plan-de-Calidad.md                       ← 5 dimensiones de calidad
├── 08-Governance/
│   ├── RACI-Matrix.md                           ← Roles con peer dynamics y 5 áreas Telemóvil
│   └── Plan-de-Comunicacion.md                  ← Canales y cadencias
├── 09-Closure/
│   ├── Retrospectiva-Final.md                   ← Retro final simulada
│   ├── Lecciones-Aprendidas.md                  ← 30+ lecciones en 5 categorías
│   ├── Resumen-Ejecutivo.md                     ← Para sponsors y leadership
│   └── Evidencia-Subcompetencias.md             ← Mapa de trazabilidad (clave para grader)
└── 10-Presentation/
    └── Outline-Presentacion.md                  ← Guion para certificación
```

**Nota:** este vault complementa la carpeta `01-Vision-and-Strategy` (Visión del Producto, Mapa de Involucrados, Justificación del Enfoque Ágil) que ya existe en tu vault local desde sesiones previas. La versión oficial y más reciente del PIDA (Definición y Plan de Trabajo) vive en **`specs/entregables/`** — esos archivos son la fuente de verdad; las notas del vault son material de apoyo.

---

## 🧭 Orden sugerido de lectura

Si abres el vault por primera vez:

1. **Inicio rápido:**
   - `09-Closure/Resumen-Ejecutivo.md` — visión general del proyecto en 5 minutos
   - `09-Closure/Evidencia-Subcompetencias.md` — qué documento prueba qué subcompetencia

2. **Comprensión del equipo:**
   - `02-Discovery/Personas.md` — quién es quién (16 perfiles)

3. **Comprensión técnica:**
   - `03-Contexto-Tecnico/Topologia-y-Alcance.md` — qué hace el proyecto
   - `03-Contexto-Tecnico/Template-B41-Resumen.md` — qué se configura

4. **Diseño del enfoque ágil:**
   - `04-Agile-Artifacts/Product-Backlog.md` — el tablero Kanban
   - `04-Agile-Artifacts/Definition-of-Ready.md` y `Definition-of-Done.md`
   - `04-Agile-Artifacts/Acuerdo-de-Equipo.md`
   - `04-Agile-Artifacts/Release-Plan.md`

5. **Simulaciones de ejecución:**
   - `05-Ceremonies-Simulation/Dia-1-Proyecto.md`
   - `05-Ceremonies-Simulation/Daily-Kanban-Sample.md`
   - `05-Ceremonies-Simulation/Bloqueo-Simulado-y-Resolucion.md`
   - `05-Ceremonies-Simulation/Retrospectiva-Golden-Cluster.md`
   - `05-Ceremonies-Simulation/Sesion-Repriorizacion.md`

6. **Gestión:**
   - `07-Risk-and-Quality/Risk-Register.md`
   - `07-Risk-and-Quality/Plan-de-Calidad.md`
   - `08-Governance/RACI-Matrix.md`
   - `08-Governance/Plan-de-Comunicacion.md`

7. **Cierre y aprendizajes (todo simulado / esperado):**
   - `09-Closure/Retrospectiva-Final.md`
   - `09-Closure/Lecciones-Aprendidas.md`

8. **Preparación para la defensa:**
   - `10-Presentation/Outline-Presentacion.md`

---

## 🎓 Mapeo de Subcompetencias (9 totales)

| Subcompetencia | Documentos principales |
|---|---|
| **1.1 Planeación Adaptativa** | Backlog, Release-Plan, Sesión-Repriorización, Risk-Register |
| **1.2 Detección y Resolución de Riesgos y Problemas** | Risk-Register, Bloqueo-Simulado, Daily-Kanban |
| **1.4 Lean & Kanban** | Backlog, DoR, DoD, Acuerdo-de-Equipo, Daily-Kanban |
| **1.5 Metrics & Reporting** | Burndown-y-Metricas, Plan-de-Comunicacion, Resumen-Ejecutivo |
| **2.1 Continuous Improvement** | Retro-Golden-Cluster, Retro-Final, Lecciones-Aprendidas |
| **2.2 Value Driven Delivery** | Backlog (priorización), Sesión-Repriorización |
| **3.1 Liderazgo Colaborativo** | Acuerdo-de-Equipo, Dia-1-Proyecto, Retrospectiva-Golden-Cluster, Daily-Kanban |
| **3.2 Equipo de Alto Desempeño** | Personas, Acuerdo-de-Equipo, Daily-Kanban |
| **3.3 Gestión de Involucrados** | Personas (Telemóvil), RACI-Matrix, Plan-de-Comunicacion |

**Ver `09-Closure/Evidencia-Subcompetencias.md` para el mapa detallado con secciones específicas.**

---

## 🔗 Curso APL ↔ Proyecto — Trazabilidad completa

Cada subcompetencia seleccionada del programa APL se materializa en (a) un módulo del curso bajo `documentation/`, (b) notas de diseño en este vault, y (c) entregables operativos en `specs/entregables/`. Esta es la trazabilidad de un extremo al otro:

| Subcompetencia | Módulo del curso (`documentation/`) | Diseño en el vault | Entregable operativo |
|---|---|---|---|
| **1.1 Planeación Adaptativa** | [[Index-APL#01. Planeación Adaptativa\|Módulo 01]] (32 docs) | [[Release-Plan]], [[Sesion-Repriorizacion]], [[Product-Backlog]] (re-priorización) | `semana-1/Backlog-Priorizado.xlsx` + Gantt del Plan de Trabajo |
| **1.2 Detección y Resolución de Riesgos y Problemas** | [[Index-APL#02. Detección y Resolución de Riesgos y Problemas\|Módulo 02]] (17 docs) | [[Risk-Register]], [[Bloqueo-Simulado-y-Resolucion]] | Risk-Register vivo durante ejecución |
| **1.4 Lean & Kanban** | [[Index-APL#04. Lean & Kanban\|Módulo 04]] (25 docs) | [[Product-Backlog]], [[Definition-of-Ready]], [[Definition-of-Done]], [[Daily-Kanban-Sample]] | `semana-1/Definition-of-Done.docx` + Tablero Kanban configurado en Jira/Miro |
| **1.5 Metrics & Reporting** | [[Index-APL#05. Metrics & Reporting for Agile Teams\|Módulo 05]] (33 docs) | [[Burndown-y-Metricas]], `burndown-data.csv` | Dashboards de FTR y burndown durante ejecución |
| **2.1 Continuous Improvement** | [[Index-APL#06. Continuous Improvement\|Módulo 06]] (34 docs) | [[Retrospectiva-Golden-Cluster]], [[Retrospectiva-Final]], [[Lecciones-Aprendidas]] | Plan de acciones de mejora por retrospectiva |
| **2.2 Value Driven Delivery** | [[Index-APL#07. Value Driven Delivery\|Módulo 07]] (24 docs) | [[Vision-del-Producto]], [[Justificacion-del-Enfoque-Agil]], [[Product-Backlog]] (orden por valor) | `semana-1/Backlog-Priorizado.xlsx` (orden por congestión/saturación) |
| **3.1 Liderazgo Colaborativo** | [[Index-APL#11. Liderazgo Colaborativo\|Módulo 11]] (24 docs) | [[Acuerdo-de-Equipo]], [[Dia-1-Proyecto]], [[Daily-Kanban-Sample]] | `semana-1/Acuerdo-de-Equipo.docx` (co-construido, no impuesto) |
| **3.2 Equipo de Alto Desempeño** | [[Index-APL#12. Equipo de Alto Desempeño\|Módulo 12]] (16 docs) | [[Personas]], [[Acuerdo-de-Equipo]], [[RACI-Matrix]] | `semana-1/Acuerdo-de-Equipo.docx` + métricas de adherencia |
| **3.3 Gestión de Involucrados** | [[Index-APL#13. Gestión de los Interesados\|Módulo 13]] (21 docs) | [[Mapa-de-Involucrados]], [[Plan-de-Comunicacion]] | `semana-1/Mapa-de-Stakeholders.docx`, `Matriz-Compromiso-Interesados.xlsx`, `Bitacora-de-Validacion.xlsx` |

### Cómo leer la trazabilidad

- **Verticalmente (una fila):** el módulo del curso aporta el marco conceptual; las notas del vault son el diseño aplicado al proyecto; el entregable es la materialización operativa en `specs/entregables/semana-N/`.
- **Horizontalmente entre subcompetencias:** las 9 cubren los tres dominios del programa APL (Agile PM 1.x, Conciencia del Negocio 2.x, Power Skills 3.x) — 61.5% de las 13 subcompetencias del programa, superando el umbral del 40%.

### Módulos del curso NO seleccionados (referencia)

Estos módulos del programa APL existen en `documentation/` pero **no se seleccionaron** para este PIDA. Conviene tenerlos a mano para la defensa por si surgen preguntas:

- Módulo 03 SCRUM, Módulo 08 Alineación Estratégica, Módulo 09 OCM, Módulo 10 Legal & Compliance

---

## ⚠️ Marcador para validación

A lo largo de los documentos aparece el marcador:

> 🔶 **[VALIDAR CON CARLOS]:** ...

Estos son puntos donde inventé información sintética o asumí algo que conviene confirmar con la realidad del proyecto antes de la defensa. Recomiendo revisarlos:

- **Nombres reales** del equipo (integradores, optimizadores, cuadrillas, Eduardo, Patricia Telemóvil, Fernando, Ricardo Mendoza)
- **IDs reales** de los 23 sitios y sus zonas
- **Umbrales** de KPIs específicos de Telemóvil
- **Tiempos** de ventana, validación, etc.
- **Estructura organizacional** real (si CSM existe, si el CPM es uno por proyecto, etc.)

Cada documento también termina con una sección **"Preguntas para Carlos"** con dudas específicas para validar.

---

## 🌟 Decisiones clave reflejadas en el vault

### Equipo distribuido
- **Daily Kanban en inglés** para incluir a Sandeep (India)
- **Diego como cultural buddy** de Sandeep
- Sandeep con TZ +10.5h se conecta a las 10:30 PM hora India

### Peer dynamics
- **Carlos y Eduardo son peers**, no jerarquía
- **Reunión semanal de peers** lunes 8 AM
- **Métricas compartidas** (FTR del sitio, no por parte)
- **Columna "Listo para Ventana"** como handoff explícito

### Trabajo paralelo HW/SW
- **Integradores remotos** aplican SW vía ENM durante la ventana
- **Cuadrillas locales** instalan HW en paralelo
- Coordinación durante la ventana entre ambos equipos

### Cliente con 5 áreas
- **Roberto** (RAN) ↔ Carlos + Integradores
- **Marcela** (Planning) ↔ Carlos + Optimizadores
- **Patricia Telemóvil** (Quality) ↔ Carlos + Optimizadores
- **Fernando** (O&M) ↔ Eduardo + Implementation
- **Ricardo Mendoza** (Acceptance Lead) ↔ Carlos (sign-off)

Reportes diferenciados por área. Roberto invitado a retrospectiva del Golden Cluster (decisión deliberada).

---

## 📋 Cómo usar este vault para la defensa

### Antes de la defensa
1. Lee todos los documentos al menos una vez
2. Resuelve los 🔶 [VALIDAR CON CARLOS]
3. Practica la presentación usando `10-Presentation/Outline-Presentacion.md`
4. Comparte el vault con el grader (Confluence, GitHub público, o ZIP)

### Durante la defensa
1. Sigue el outline de 23 slides
2. Sé claro: "Es proyecto en planeación, presento diseño + simulaciones"
3. Usa casos concretos:
   - **CR-014** (bloqueo simulado)
   - **Roberto (Telemóvil)** (cliente que pasa de escéptico a advocate)
   - **Sandeep India** (inclusión activa del equipo distribuido)
   - **Peer Carlos-Eduardo** (sin fricción)
   - **Bella Vista** (re-priorización por valor)
4. Conecta cada slide con subcompetencia explícita
5. Cierra con próximos pasos: el proyecto arranca, validarás las hipótesis ágiles en ejecución

### Después de la defensa
1. Mantén el vault como tu base de conocimiento personal
2. Conforme avanza el proyecto, reemplaza proyecciones con datos reales
3. Las "Preguntas para Carlos" pueden volverse decisiones documentadas
4. Comparte con tu equipo Ericsson como playbook replicable

---

## 🛠️ Convenciones del vault

### Tags Obsidian (si lo abres en Obsidian)

Cada documento tiene tags como:
- `agile`, `kanban`, `dor`, `dod`
- `equipo`, `stakeholders`, `comunicacion`
- `riesgo`, `metricas`, `lecciones`
- `simulacion`, `kickoff`, `retrospectiva`
- `evidencia`, `certificacion`

### Cross-references

Los documentos usan enlaces tipo Wiki con la sintaxis `[[NombreDelDocumento]]` (sin extensión, ejemplo). Si los abres en Obsidian, son navegables. Ejemplos reales: [[Resumen-Ejecutivo]], [[Definition-of-Done]], [[Mapa-de-Involucrados]], [[Outline-Presentacion]], [[02.DefinicionPIDA-APL]], [[Personas]].

### Frontmatter

Cada documento tiene metadata YAML con:
- proyecto, participante, rol, cliente
- fecha, status
- subcompetencias mapeadas
- tags

---

## 🎁 Qué entrega este vault

**Para el grader del Proyecto Integrador:**
- Vault auditable con 25 documentos
- 9 subcompetencias mapeadas con evidencia concreta
- Diseño riguroso + simulaciones plausibles
- Justificaciones explícitas de cada decisión

**Para Carlos:**
- Playbook listo para usar al ejecutar el proyecto
- Base de conocimiento para próximos proyectos similares
- Material para Ericsson Latam como caso piloto

**Para Ericsson y Telemóvil:**
- Diseño replicable para futuros despliegues
- Documentación que sobrevive al proyecto

---

## ✨ Cierre

> "Este vault refleja 8 semanas de planeación rigurosa antes de 8 semanas de ejecución. La hipótesis: el rigor en el diseño permite la fluidez en la ejecución. La defensa del Proyecto Integrador es el primer punto de validación; el éxito del proyecto en Telemóvil será el segundo."

— Carlos Emmanuel Ramírez Castañón, Network Performance Manager, Ericsson
