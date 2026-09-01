---
title: L4 — Análisis y evaluación de riesgos en los proyectos
curso: PMP
modulo: 04. Gestion de Riesgos
leccion: L4
fuente: "[[documentation/04. Gestion de Riesgos/PMP_SC1.4_versionimpresa_L4.pdf|Versión impresa L4]]"
complementos: ["[[documentation/04. Gestion de Riesgos/Información necesaria para la identificación de riesgos_.pdf|Información necesaria para la identificación de riesgos]]", "[[documentation/04. Gestion de Riesgos/Técnicas para recopilar datos e información_.pdf|Técnicas para recopilar datos e información]]", "[[documentation/04. Gestion de Riesgos/Registro de Riesgos.pdf|Registro de Riesgos]]", "[[documentation/04. Gestion de Riesgos/Análisis probabilístico de riesgos_.pdf|Análisis probabilístico de riesgos]]", "[[documentation/04. Gestion de Riesgos/Las variables más importantes en el Análisis Cuantitativo de Riesgos.pdf|Variables del Análisis Cuantitativo de Riesgos]]", "[[documentation/04. Gestion de Riesgos/Estimación de 3 puntos o de PERT_.pdf|Estimación de 3 puntos o de PERT]]", "[[documentation/04. Gestion de Riesgos/Ejercicio Análisis cuantitativo de riesgos.pdf|Ejercicio Análisis cuantitativo de riesgos]]", "[[documentation/04. Gestion de Riesgos/Registro de los resultados del análisis y evaluación de los riesgos.pdf|Registro de los resultados del análisis y evaluación de los riesgos]]"]
status: por-estudiar
tags: [pmp, riesgos]
---

# L4 — Análisis y evaluación de riesgos en los proyectos

## Resumen

Una vez planificados los procesos de gestión de riesgos e identificada la lista de riesgos del proyecto (L2-L3), corresponde **analizarlos y evaluarlos** de forma **cualitativa** y **cuantitativa** para saber cuáles son los más importantes y así asignar recursos, tiempo y costo adecuados a cada uno. El análisis **cualitativo** establece los niveles de **probabilidad**, **impacto** y **prioridad** de cada riesgo mediante la **matriz de Probabilidad vs. Impacto**. El análisis **cuantitativo** estima las cantidades de **tiempo** (reserva de contingencia de tiempo) y **costo** (reserva de contingencia de costo) necesarias para atender los riesgos, usando técnicas de estimación (análoga, paramétrica y de 3 puntos o PERT). Con esas reservas se puede además realizar un **análisis probabilístico** del proyecto (distribución Normal/Beta) para conocer el % de probabilidad de éxito del presupuesto de costo y del tiempo presupuestado. Antes de analizar los riesgos hace falta **recopilar información** suficiente (documentos de planificación, experiencia, técnicas primarias y secundarias de recopilación de datos) y volcar todo en el **Registro de Riesgos**, formato estandarizado que se va enriqueciendo en cada proceso.

## Conceptos clave (con definiciones completas)

### Variable cualitativa vs. cuantitativa
- **Variable cualitativa**: expresa **cualidades o características** de algo (ej. bajo/medio/alto). No se relaciona necesariamente con cifras, aunque se le pueden asociar números de forma convencional (1, 2, 3) para facilitar el análisis, **sin que representen magnitudes reales**.
- **Variable cuantitativa**: está ligada directamente a **cantidades o magnitudes numéricas reales** (edad, peso, costo, tiempo de retraso de un vuelo, etc.).

### Posibilidad vs. Probabilidad
- **Posibilidad**: variable **dicotómica o binaria** — dice si un evento **ES posible o NO es posible**, sin más opciones (variable cualitativa dicotómica).
- **Probabilidad**: variable **cualitativa politómica** (más de dos valores posibles) que describe **qué tan probable** es que ocurra un evento una vez establecido que sí es posible; ejemplo de niveles: Muy Bajo, Bajo, Medio, Alto, Muy Alto.

### Probabilidad Cualitativa
Para establecerla, el equipo debe usar su conocimiento, experiencia e información de proyectos similares anteriores: con qué frecuencia se ha identificado y con qué frecuencia ha ocurrido un determinado problema/riesgo en el pasado, lo que da una idea clara de la probabilidad de que ocurra en proyectos actuales y futuros. Niveles típicos: **Baja, Media, Alta**.

### Impacto Cualitativo
Con el mismo tipo de información histórica, se establece cuál(es) han sido los efectos o impactos que un riesgo ha ocasionado cada vez que ha ocurrido (¿cuánto más costó?, ¿cuánto se retrasó?). El impacto puede reflejarse en cualquier área del proyecto (alcance, recursos, calidad, comunicaciones, etc.), pero **casi siempre se refleja en las dos variables más fácilmente cuantificables: tiempo y costo**.

### Prioridad Cualitativa
Del latín *prior/prius* (primero, precedente) + sufijo *-tat* (cualidad). Es la cualidad de ser más importante que otros elementos comparables. En riesgos, la prioridad es, comúnmente, una **combinación (multiplicación) de Probabilidad e Impacto**: a mayores niveles de ambas variables, mayor prioridad; a menores niveles, menor prioridad.

### Matriz de Probabilidad vs. Impacto
Herramienta central del análisis cualitativo. Cruza los niveles de Probabilidad (filas) con los niveles de Impacto (columnas); el producto de ambos da el valor de Prioridad de cada celda. Ejemplo de escala 1-5 / 2-10 usada en el material:

| Probabilidad | Muy bajo (2) | Bajo (4) | Medio (6) | Alto (8) | Muy alto (10) |
|---|---|---|---|---|---|
| 5 Muy alta (71%-99%) | 10 | 20 | 30 | 40 | 50 |
| 4 Alta (56%-70%) | 8 | 16 | 24 | 32 | 40 |
| 3 Media (35%-55%*) | 6 | 12 | 18 | 24 | 30 |
| 2 Baja (21%-34%) | 4 | 8 | 12 | 16 | 20 |
| 1 Muy baja (1%-20%) | 2 | 4 | 6 | 8 | 10 |

(*En "Registro de los resultados…" el intervalo de probabilidad Media aparece como 35%-49%; en L4/PERT aparece 35%-55%. Usa el intervalo cualitativo asignado en el plan de gestión de riesgos de cada proyecto — el estándar admite tailoring.)

Niveles de **prioridad** resultantes (según Registro de los resultados del análisis…): 1 Muy baja (2 a 4), 2 Baja (6 a 8), 3 Media (8 a 24), 4 Alta (30 a 32), 5 Muy alta (40 a 50).

Intervalos de **impacto** en % (ejemplo del material): Muy bajo 0%-5%, Bajo 6%-10%, Medio 11%-15%, Alto 16%-20%, Muy alto >20%.

**Antes de aplicar la matriz** el equipo NO debe omitir:
1. Definir los niveles e intervalos de cada variable cualitativa (Probabilidad, Impacto, Prioridad) junto con el plan de gestión de riesgos.
2. Construir la Matriz de Probabilidad vs. Impacto con todos los datos disponibles.
3. Analizar y evaluar cada riesgo identificado con base en esa matriz.

### Reserva de contingencia
Cantidades de **dinero (sobrecostos)** o de **tiempo (tiempos de retraso)** que se **estiman y guardan** para atender los riesgos **ya identificados** en el proyecto (riesgos conocidos).

### Reserva de administración o de gestión
Cantidad de tiempo o dinero para gestionar los riesgos **no identificados o emergentes**. Como no se pueden identificar, no se puede estimar mediante técnica; la determinan los **expertos de la empresa** según la complejidad/incertidumbre del proyecto, normalmente como un **% de los costos del proyecto** (ej. 1%, 2%, 5%, según política de cada empresa), y una vez asignada al proyecto debe respetarse.

### Tiempo de retraso
Tiempo extra que dura una actividad porque se manifestó un problema/riesgo asociado. Ejemplo del material: actividad de 15 días con retraso real de 5 días → duración final real = 15 + 5 = **20 días**.

### Sobrecosto
Dinero extra que cuesta una actividad por manifestarse un riesgo asociado. Ejemplo: actividad de $10,000 con sobrecosto real de $1,550 → costo final real = $10,000 + $1,550 = **$11,550**.

### Costos totales y presupuesto del proyecto
- **Costos totales (C_T)**: acumulación de todos los costos (directos, indirectos, fijos, variables) de todas las actividades.
- **Presupuesto del proyecto (C_P)**: C_T + reserva de contingencia de costo + reserva de gestión de costo.

### Duración de la ruta crítica y tiempo presupuestado
- **Duración de la ruta crítica (T_T)**: duración total estimada del proyecto (cronograma).
- **Tiempo presupuestado (T_P)**: T_T + reserva de contingencia de tiempo + reserva de gestión de tiempo.

### Distribuciones de probabilidad aplicadas a riesgos
Para el análisis probabilístico se pueden usar distribuciones **Beta**, **Triangular** o **Normal**, según la información disponible. La distribución **Beta** es la que sustenta la técnica PERT (asimétrica); sus resultados se pueden **aproximar a la distribución Normal** (simétrica) con un error despreciable, lo cual permite usar las tablas/funciones de la Normal para calcular probabilidades de éxito.

## Desarrollo del contenido

### 1. Información necesaria para la identificación (y análisis) de riesgos
Se requiere información **real, objetiva y confiable**. Las dos fuentes más importantes: **experiencia del equipo** e **información documental histórica** de proyectos previos. Documentos de planificación del proyecto actual relevantes:
- **Plan de Administración del Proyecto**: integra estimaciones/planes de Requerimientos, Alcance, Cronograma, Costos, Calidad, Recursos, etc.
- **Project Charter**: restricciones de costo/tiempo/recursos, riesgos generales o de alto nivel identificados en factibilidad, suposiciones.
- **Registro de problemas de fases tempranas de planificación**: lecciones de lo sucedido recientemente.
- **Registro de incidentes o problemas (Issue log)**: vigilar que incidentes complejos no se conviertan en riesgos.
- **Enunciado del alcance (Project Scope Statement, PSS)**: un alcance muy ambicioso ya representa un riesgo de tiempo/presupuesto.
- **Estimaciones de costos, tiempos y recursos**: revisar cómo se hicieron para prevenir errores.
- **Registro de interesados (stakeholders)**: incluye al propio equipo; permite asignar responsabilidades de riesgo según actitud ante el riesgo.
- **Contratos y acuerdos**: con cliente, proveedores, contratistas.
- **Entorno del proyecto**: cliente, regulaciones/políticas, tecnología, lugar físico, clima, mercado, etc.

### 2. Técnicas para recopilar datos e información (identificación de riesgos)

**Técnicas primarias** (recolectan info de primera mano, dentro o fuera del equipo):
- **Lluvia de ideas (Brainstorming)**: creatividad grupal; se recomienda para grupos no muy numerosos; en proyectos: brainstorming local por área técnica → brainstorming general con líderes.
- **Grupos de discusión / Focus Groups**: grupos pequeños de la misma área generan en conjunto la lista de riesgos de su área.
- **Listas de verificación (Checklists)**: vigilan cumplimiento sistematizado; se puede generar una checklist por categorías de riesgo del plan, o por fases del proyecto.
- **Entrevistas**: encuentro uno a uno (entrevistador/entrevistado). Tipos:
  - **Estructuradas**: guion y preguntas predefinidas y concretas.
  - **Semiestructuradas**: preguntas disparadoras que guían el rumbo.
  - **No estructuradas**: conversación libre centrada solo en el tema.
  Se recomiendan cuando el equipo no tiene experiencia interna en un área o se quiere completar el análisis, con expertos internos o externos.
- **Técnica Delphi**: similar a entrevistas individuales pero consultando a **varios expertos a la vez** (a menudo sin que se enteren entre sí); un moderador analiza respuestas y retroalimenta a cada experto hasta obtener **consenso**, casi siempre sin interacción directa entre ellos. Útil cuando no hay experiencia previa ni documentación de apoyo.
- **Encuestas y cuestionarios**: para audiencias objetivo grandes, en papel o en línea (preguntas abiertas, de opción múltiple, etc.); útiles cuando el equipo es muy grande.
- **Observación directa**: la más sencilla; observar procesos, personas, interacciones y presentar un informe (regularmente lo hace el PM).

**Técnicas secundarias** (recolectan info de eventos pasados con registro documental, internas o externas):
- **Informes y documentación histórica** de proyectos similares previos: datos reales, objetivos y fidedignos — altamente recomendable basarse en ellos.
- **Registros de riesgos previos**: tablas, matrices, cálculos de proyectos similares anteriores.
- **Resúmenes ejecutivos**: presentaciones sintetizadas para directivos; revisarlos ayuda a identificar riesgos.
- **Publicaciones de la industria**: estudios y casos de asociaciones/organizaciones profesionales.
- **Libros especializados**: impresos o e-books.
- **Internet**: rápida y de bajo costo, pero hay que ser cauteloso — usar fuentes certificadas (universidades, institutos, organismos de estándares/gubernamentales).
- **Comunidades en línea / foros**: útiles pero sin ente regulador que garantice la veracidad de las respuestas — tomar con cautela.

Regla general: **a mayor información, siempre menor incertidumbre.**

### 3. Registro de Riesgos — sección de identificación
Formato estandarizado (tabla, normalmente Excel) donde se vuelca toda la información de identificación y, después, de los demás procesos de riesgos. Columnas recomendadas para identificación:

| No. | Bloque del WBS | Código WBS | Descripción del Evento de riesgo | Causa(s) del Riesgo | Categoría(s) | Descripción del Impacto(s) | Dueño del riesgo |
|---|---|---|---|---|---|---|---|

- Se recomienda identificar riesgos **desde el nivel más bajo de la EDT** (actividades) e ir subiendo a paquetes de trabajo, fases y proyecto completo.
- **Dueño del riesgo**: persona responsable de atender o supervisar la atención al riesgo; puede cambiar según el análisis y los planes de respuesta posteriores (L5).
- Es sensible al **tailoring**: cada proyecto puede ajustar/aumentar/disminuir estos campos.

Ejemplo (proyecto de instrumentación electrónica) del material:

| No. | Bloque WBS | Código | Evento de riesgo | Causa | Categoría | Impacto | Dueño |
|---|---|---|---|---|---|---|---|
| 1 | Elaboración de PCB's | 1.2.1 | Errores en ruteado final | Diseño equivocado en software | Técnico | Retrasos en construcción y sobrecosto | Ingeniero de diseño de PCB's |
| 2 | Colocación final de tarjetas | 1.4.3.4 | Espacio insuficiente | Mala interpretación de medidas en planos | Externo | Retraso en implementación final | Ingeniero de Instalaciones |
| 3 | Junta de inicio | 1.1.1.1 | Faltan stakeholders | Fallas de comunicación interna | Project Management | Retraso y sobrecosto | Project Management |
| n | Contratos con proveedores | 1. | Costos/fechas no coinciden con contrato | Compras entregó tarde requisitos | Organizacional | Sobrecostos por renegociación | PM en contacto con Gerente de Compras |

### 4. Técnicas de estimación cuantitativa (reservas de tiempo y costo)
Tres técnicas, de menor a mayor precisión/datos requeridos:

1. **Estimación análoga**: usa la **experiencia** del equipo cuando hay pocos datos históricos; se toma un **promedio aritmético simple** de los valores conocidos. Rápida pero con alta incertidumbre (±50% aprox.), por lo tanto de **baja efectividad**.
   - Ejemplo del material: un riesgo ocurrió 2 veces antes (retraso 4 y 6 días; costo $2,150 y $3,100) más la experiencia del PM (retraso 8 días, costo $2,900).
     - retraso = (4+6+8)/3 = 18/3 = **6 días**
     - sobrecosto = (2,150+3,100+2,900)/3 = 8,150/3 = **$2,716.67**
2. **Estimación paramétrica**: se aplica con **más datos** (al menos dos parámetros conocidos); es una **multiplicación** de parámetros (ej. días de retraso × costo por día).
   - Ejemplo: retraso conocido = 4 días; costo por día de retraso = $1,200 → sobrecosto = 4 × $1,200 = **$4,800**.
3. **Estimación de 3 puntos o de PERT** (*Program Evaluation and Review Technique*): desarrollada en 1958 por la Oficina de Proyectos Especiales de la Marina de EE.UU. (diseño de misiles); apoya planificación de proyectos grandes/complejos. Se basa en la distribución de probabilidad **Beta** (asimétrica), a diferencia de la Normal (simétrica). Usa tres valores para tiempo o costo, obtenidos de información histórica/experiencia:
   - **a = valor optimista** (el más pequeño; nos fue muy bien).
   - **b = valor más común** (moda; el más frecuente).
   - **c = valor pesimista** (el más grande; nos fue muy mal).
   
   **Media probabilística (PERT):**
   
   `x̄ = (a + 4b + c) / 6`
   
   (b pesa 4 veces más que los extremos por ser el valor más frecuente).
   
   **Desviación estándar (σ) y varianza (σ²):**
   
   `σ = (c - a) / 6`      `σ² = ((c - a) / 6)²`

### 5. Cálculo de la reserva a partir de la probabilidad cualitativa
Una vez obtenido el valor estimado (media PERT) de tiempo de retraso o sobrecosto, se multiplica por el **% de probabilidad** asignado al riesgo (elegido dentro del intervalo cualitativo, p. ej. Media = 35%-55%, se puede tomar 39%, 45%, 49%, etc., según el conocimiento del riesgo particular):

`Reserva = R = %Probabilidad × Impacto`

(Impacto aquí es el valor estimado de tiempo/costo, ya calculado con PERT).

**Ejemplo completo resuelto del material** (proyecto con 4 actividades, 4 riesgos, reserva de gestión = 1%):

| Riesgo | Prob. (p) | Retraso a/b/c | Retraso estimado x̄ | Reserva tiempo (p·x̄) |
|---|---|---|---|---|
| 1 | 0.33 | 9/12/33 | 15 días | 5 |
| 2 | 0.60 | 2/5/8 | 5 días | 3 |
| 3 | 0.25 | 14/19/30 | 20 días | 5 |
| 4 | 0.80 | 7/9/17 | 10 días | 8 |
| **Total** | | | | **rc_t = 21 días** |

| Riesgo | Sobrecosto a/b/c | Sobrecosto estimado x̄ | Reserva costo (p·x̄) |
|---|---|---|---|
| 1 | 1350/2200/2450 | $2,100 | $700 |
| 2 | 380/480/940 | $540 | $324 |
| 3 | 1800/2150/3160 | $2,260 | $565 |
| 4 | 800/1500/1600 | $1,400 | $1,120 |
| **Total** | | | **rc_c = $2,709** |

Reserva de gestión (1%): rg_t = 225 días × 1% = **2 días**; rg_c = $48,500 × 1% = **$485**.

**Reservas totales**: R_T = rc_t + rg_t = 21 + 2 = **23 días**; R_C = rc_c + rg_c = $2,709 + $485 = **$3,194**.

**Presupuesto**: T_P = T_T + R_T = 225 + 23 = **248 días**; C_P = C_T + R_C = $48,500 + $3,194 = **$51,694**.

**% de reserva**: %R_T = R_T/T_T × 100 = 23/225 × 100 = **10.22%**; %R_C = R_C/C_T × 100 = $3,194/$48,500 × 100 = **6.58%** (debe ser ≤ tolerancia al riesgo de la empresa).

*Nota: cuando el riesgo es específico de una actividad (fórmula de "Registro de los resultados…"), el retraso/sobrecosto estimado (Re/Se) también se calcula como p × Retraso-promedio(o Sobrecosto-promedio), y solo se suma a la reserva de contingencia de TIEMPO si la actividad **es parte de la ruta crítica** (columna Sí=1/No=0); para COSTO se suman TODAS las actividades sin importar la ruta.*

### 6. Análisis probabilístico de riesgos (distribución Normal)
La distribución **Normal** va de -∞ (0% de probabilidad) a +∞ (100%), simétrica, con la media al centro = 50%. Reglas empíricas (regla 68-95-99.7):
- Entre ±1σ ≈ **68%** del área bajo la curva.
- Entre ±2σ ≈ **95%**.
- Entre ±3σ ≈ **99.7%**.

Valores acumulados clave: -3σ=0.135%, -2σ=2.5%, -1σ=16%, media=50%, +1σ=84%, +2σ=97.5%, +3σ=99.86%.

**No es recomendable moverse hacia la izquierda** (baja la probabilidad); siempre conviene moverse hacia la **derecha** (aumenta la probabilidad de éxito), lo cual se logra **sumando las reservas** (R_T, R_C) a los valores base (T_T, C_T).

**Puntuación Z** (cuántas desviaciones estándar nos desplazamos hacia la derecha):

`Z_σT = (T_P - T_T) / σ_T = R_T / σ_T`
`Z_σC = (C_P - C_T) / σ_C = R_C / σ_C`

**Función de Excel** para obtener la probabilidad acumulada:
`=DISTR.NORM.ESTAND.N(Z, VERDADERO)` (español) / `=NORM.S.DIST(Z, TRUE)` (inglés).

**Ejemplo completo resuelto** (mismo proyecto de 4 actividades):
- Tabla de tiempos/costos de las 4 actividades con Duración/Costo Optimista, Más común, Pesimista → Duración estimada total T_T = **225 días**, σ_T = **16.5 días**; Costo total C_T = **$48,500**, σ_C = **$3,667.31**.
- Z_σT = (248-225)/16.5 = 23/16.5 = **1.39σ** → P_T = DISTR.NORM.ESTAND.N(1.39,1) = **91.77%**.
- Z_σC = (51,694-48,500)/3,667.31 = 3,194/3,667.31 = **0.87σ** → P_C = DISTR.NORM.ESTAND.N(0.87,1) = **80.78%**.
- Las mejores prácticas de los estándares internacionales recomiendan al menos **80% de probabilidad de éxito**.

**Pasos para calcular la desviación estándar de todo el proyecto** (a partir de la tabla de actividades):
1. Calcular la varianza (σ²) de cada actividad: σ² = ((c-a)/6)².
2. Para **tiempo**: sumar varianzas SOLO de las actividades de la **ruta crítica** → varianza total de tiempo (σ²_Pt).
3. Para **costo**: sumar varianzas de **TODAS** las actividades → varianza total de costo (σ²_Pc).
4. Sacar raíz cuadrada de cada varianza total para obtener σ_Pt y σ_Pc.

Razón: las actividades **no críticas** tienen holgura que (optimistamente) absorbe sus propios retrasos sin afectar la fecha fin del proyecto; si el retraso real excediera la holgura, hay que actualizar rutas/cronograma. En costo, **todas** las actividades importan porque cualquier sobrecosto afecta el presupuesto sin importar la ruta.

### 7. Registro de Riesgos — secciones de análisis cualitativo y cuantitativo
**Análisis cualitativo** — se agregan columnas a la tabla de identificación (relacionadas por el número consecutivo):

| No. | Nivel de Probabilidad Cualitativa | Nivel de Impacto Cualitativo | Nivel de Prioridad |
|---|---|---|---|
| 1 | 3 | 10 | 30 |
| 2 | 5 | 8 | 40 |
| 3 | 2 | 4 | 8 |

Se recomienda **colorear** la celda de prioridad según la matriz de Prob. vs. Impacto.

**Análisis cuantitativo de tiempo** — columnas: No. | Probabilidad (p) | Retraso Optimista (a) | Retraso Más Común (b) | Retraso Pesimista (c) | Retraso promedio (R_m, fórmula PERT) | Reserva estimada / Exposición al riesgo (Re = p × R_m) | ¿Es actividad crítica? Sí(1)/No(0) | Reserva de Contingencia de tiempo (Re × 1 o 0). La **suma total** de la última columna = rc_t.

**Análisis cuantitativo de costo** — columnas análogas: No. | Probabilidad (p, la misma que en tiempo) | Sobrecosto Optimista/Más común/Pesimista (a/b/c) | Sobrecosto promedio (S_e, fórmula PERT) | Reserva estimada (p × S_e). Aquí **se suman todas las filas sin filtrar por ruta crítica** → rc_c.

Al terminar de llenar el Registro con toda esta información, el equipo puede identificar los riesgos más prioritarios, los más impactantes en tiempo y en costo, el valor de las reservas y el % de probabilidad de éxito — insumos para diseñar las estrategias de respuesta (L5).

## Ejemplos y ejercicios del material (resueltos paso a paso)

### Ejercicio resuelto de análisis cuantitativo con diagrama de red (network diagram)
Proyecto con actividades Inicio→A→(B→D→E→G, C)→F→H→I→Final. Duraciones: A=48, B=47, C=39, D=32, E=31, F=29, G=31, H=42, I=19. Costos por actividad: A=$12,000, B=$15,000, C=$14,000, D=$23,000, E=$20,000, F=$26,000, G=$33,000, H=$28,000, I=$20,000. Tabla de riesgos con probabilidad, retraso/sobrecosto optimista-común-pesimista por actividad.

**Solución:**
a) **Ruta crítica = A-B-D-E-G-H-I**, duración total **T_T = 250 días** (C y F NO son críticas).
b) **Costo total C_T = $191,000**.
c) Reserva de contingencia de **tiempo** (solo ruta crítica, redondeado): **rc_t = 27 días**. Reserva de contingencia de **costo** (todas las actividades): **rc_c = $18,685.83**.
d) Con reserva de gestión 2%: rg_t = 250×0.02 = **5 días**; rg_c = $191,000×0.02 = **$3,820**. Reservas totales: **R_T = 27+5 = 32 días**; **R_C = $18,685.83+$3,820 = $22,505.83**.
e) **Tiempo presupuestado T_P = 250+32 = 282 días**; **Presupuesto de costo C_P = $191,000+$22,505.83 = $213,505.83**.
f) % de reserva de tiempo = 32/250×100 = **12.8%**; % de reserva de costo = $22,505.83/$191,000×100 = **11.78%**.
g) Con σ_T=25 días y σ_C=$15,000: Z_σT = 32/25 = **1.28σ** → **P_T = 89.97%**; Z_σC = 22,505.83/15,000 = **1.5σ** → **P_C = 93.32%**.

### Ejercicio 2 numérico — Estimación análoga
Riesgo ocurrido 2 veces (retraso 4 y 6 días; costo $2,150 y $3,100) + dato del PM (retraso 8 días, $2,900). Promedio: retraso = (4+6+8)/3 = **6 días**; sobrecosto = (2,150+3,100+2,900)/3 = **$2,716.67**.

### Ejercicio numérico — PERT / media probabilística (Riesgo 1 del proyecto de 4 actividades)
Retraso: a=9, b=12, c=33 → x̄ = (9+4×12+33)/6 = (9+48+33)/6 = 90/6 = **15 días**.
Sobrecosto: a=$1,350, b=$2,200, c=$2,450 → x̄ = (1,350+4×2,200+2,450)/6 = (1,350+8,800+2,450)/6 = 12,600/6 = **$2,100**.
Reserva (p=0.33): tiempo = 15×0.33 = **5 días**; costo = 2,100×0.33 = **$700**.

## Conexión con APL/PIDA

- El **Risk Register del PIDA** (`01-APL/specs/07-Risk-and-Quality/Risk-Register.md`) aplica exactamente el análisis **cualitativo** de esta lección: cada riesgo (ej. R-TEC-01 "Template B41 requiere ajustes", R-EQUIPO-01 "Aislamiento cultural de Sandeep") tiene Probabilidad (Baja/Media/Alta) × Impacto (Bajo/Medio/Alto) = **Score** de Prioridad, con la misma lógica de la matriz Probabilidad vs. Impacto de L4 (ahí Score≥6 = monitoreo activo en cada daily, equivalente a "prioridad alta" de la matriz de L4).
- **Caso real de análisis reactivo vs. formal**: R-TEC-02 "Plan de RF desactualizado (caso CR-014)" — Probabilidad Media, Impacto Medio, Score 4 🟡 — se resolvió con **ajustes en tiempo real** (mitigación reactiva) en 56h, en lugar de con una reserva de contingencia de tiempo/costo calculada formalmente con PERT como enseña L4; el PIDA no llegó a hacer análisis cuantitativo (PERT, reservas en días/dólares, análisis probabilístico con σ y Z) — su Risk Register se quedó en el nivel cualitativo, lo que es una brecha frente a las mejores prácticas de esta lección.
- El PIDA no reporta un **% de probabilidad de éxito del proyecto** (Z, DISTR.NORM.ESTAND.N) como recomienda L4; los "Indicadores de salud del Risk Register" (riesgos identificados ≥10, riesgos cerrados ≥50%) son un sustituto cualitativo de ese análisis probabilístico formal.

## Preguntas de repaso tipo quiz

1. **¿Cuál es la diferencia entre Posibilidad y Probabilidad?**
   R: Posibilidad es una variable dicotómica (ES o NO ES posible); Probabilidad es una variable cualitativa politómica que mide qué tan probable es el evento una vez que se sabe que es posible (ej. Baja/Media/Alta).

2. **¿Cómo se calcula la Prioridad de un riesgo en el análisis cualitativo?**
   R: Es la combinación (multiplicación) de los niveles de Probabilidad e Impacto en la matriz de Probabilidad vs. Impacto.

3. **¿Cuál es la fórmula de la media probabilística de PERT y por qué el valor "b" tiene coeficiente 4?**
   R: x̄ = (a + 4b + c) / 6. b (valor más común/moda) pesa 4 veces más porque es el valor que ocurre con mayor frecuencia según el comportamiento natural de los datos.

4. **¿Cuál es la fórmula de la desviación estándar en la técnica de 3 puntos?**
   R: σ = (c − a) / 6, donde c es el valor pesimista y a el valor optimista.

5. **Un riesgo tiene retraso optimista=6, más común=10, pesimista=20. ¿Cuál es el retraso estimado (PERT)?**
   R: x̄ = (6 + 4×10 + 20)/6 = (6+40+20)/6 = 66/6 = **11 días**.

6. **Si ese mismo riesgo tiene probabilidad de ocurrencia de 40%, ¿cuál es la reserva de contingencia de tiempo?**
   R: Reserva = %Probabilidad × valor estimado = 0.40 × 11 = **4.4 días**.

7. **¿Por qué al calcular la reserva de contingencia de TIEMPO de todo el proyecto solo se suman las actividades de la ruta crítica, pero para COSTO se suman todas las actividades?**
   R: Porque solo las actividades críticas, al retrasarse, modifican la fecha de terminación del proyecto (las no críticas tienen holgura); en cambio cualquier sobrecosto, sin importar la ruta, afecta el presupuesto total.

8. **¿Qué diferencia hay entre la reserva de contingencia y la reserva de administración/gestión?**
   R: La reserva de contingencia es para riesgos **identificados** (conocidos) y se calcula con técnicas de estimación; la reserva de gestión es para riesgos **no identificados/emergentes**, no se puede calcular y la asignan los expertos de la empresa como % de los costos, por política.

9. **En el análisis probabilístico, si Z_σC = 0.87σ, ¿qué función de Excel se usa para obtener el % de probabilidad de éxito y qué representa el segundo argumento?**
   R: `=DISTR.NORM.ESTAND.N(Z, Acumulado)`; el segundo argumento debe ser VERDADERO (o 1) para obtener la probabilidad acumulada desde 0% hasta el punto de análisis.

10. **Un proyecto tiene T_T = 250 días y una reserva total de tiempo R_T = 32 días. ¿Cuál es el tiempo presupuestado T_P y qué % de reserva representa?**
    R: T_P = T_T + R_T = 250 + 32 = **282 días**; % = 32/250 × 100 = **12.8%**.
