---
title: L3 — Estimación de costos
curso: PMP
modulo: 03. Gestion de costos
leccion: L3
fuente: "[[documentation/03. Gestion de costos/Resumen. Estimación de costos.pdf|Resumen. Estimación de costos]]"
complementos: [Estimado por analogía.pdf, Estimado de tres puntos.pdf, Ejemplo práctico construcción de una casa.pdf]
status: por-estudiar
tags: [pmp, costos, estimacion]
---

# L3 — Estimación de costos

## Resumen

La **estimación de costos** consiste en desarrollar una aproximación precisa de cuánto costarán los recursos asignados a cada actividad o paquete de trabajo del proyecto: mano de obra, materiales, equipos, servicios, instalaciones, contingencias para riesgos, consideraciones inflacionarias, etc. Es crítica porque los costos al finalizar un proyecto a menudo exceden el presupuesto inicial — **solo un 62 % de los proyectos logra mantenerse dentro del presupuesto original**, y una causa significativa y frecuente es la falta de aplicación formal de técnicas de estimación.

La estimación se dificulta por el entorno **VUCA** (*Volatility, Uncertainty, Complexity & Ambiguity*):
- **Volatilidad** → cambios inmediatos.
- **Incertidumbre** → falta de conocimiento acerca del futuro.
- **Complejidad** → influencia de múltiples variables o factores simultáneos.
- **Ambigüedad** → falta de claridad.

La lección cubre 4 técnicas: **analogía (top-down)**, **paramétrica**, **ascendente (bottom-up / definitiva)** y **tres puntos (PERT)**, más los elementos y documentos de entrada necesarios para estimar.

## Conceptos clave (con definiciones completas)

**Elementos que se recomienda tener definidos antes de estimar:**

- **Plan de gestión del proyecto (con foco en el plan de gestión de costos)**: documento formal que describe cómo se planificará, ejecutará, monitoreará, controlará y cerrará un proyecto. Guía detallada de enfoques, procesos, recursos y responsabilidades. El plan de gestión del costo establece los procedimientos para estimar y presupuestar, y define las plantillas/formatos para documentar la información de costos. Estructura típica: **Portada** (nombre, fecha, versión) · **Índice** · **Introducción** (descripción, propósito y alcance del plan) · **Objetivos** (objetivos de costos específicos y presupuesto total) · **EDT** (desglose de costos por fase y categorías) · **Método de estimación de costos** (metodología, fuente de datos, suposiciones y factores) · **Presupuesto** (costos por fases y/o categorías) · **Control de costos** (registro de costos reales y desviaciones vs. presupuesto original) · **Proceso de aprobación de cambios** · **Riesgos relacionados con los costos** · **Seguimiento y reporte** · **Anexos** (hojas de cálculo, gráficos, tablas de recursos).
- **Plan de calidad**: documento formal que establece estándares, procesos, procedimientos y recursos para garantizar que el proyecto cumpla los requisitos de calidad; contiene las métricas de calidad que deben cumplir los entregables (p. ej. en una casa: cimientos, estructura, instalaciones, acabados interiores y exteriores, paisajismo).
- **Línea base del alcance**: comprende el **enunciado del alcance + EDT + diccionario de la EDT**. Define qué incluye y qué excluye el proyecto, con asunciones y restricciones (incluyendo el presupuesto máximo). Es el punto de referencia para evaluar y controlar cambios de alcance.

**Documentos adicionales de entrada:**

- **Registro de lecciones aprendidas**: capitaliza el conocimiento de proyectos previos similares (p. ej. una definición detallada del alcance facilita estimaciones más precisas; un registro actualizado de precios de materiales mitiga impactos financieros imprevistos).
- **Registro de riesgos**: identifica riesgos potenciales que podrían aumentar los costos (fluctuaciones de precios de materiales por factores económicos, cambios en requisitos del cliente durante la ejecución, problemas de mano de obra o calidad de materiales ante condiciones ambientales imprevistas).
- **Cronograma del proyecto**: fases, paquetes de trabajo y actividades con fechas y duraciones; esencial para estimar costos sobre elementos de trabajo específicos.
- **Lista de requerimientos de recursos**: recursos humanos, materiales, equipos, financiamiento, tiempo y recursos externos (proveedores, subcontratistas, trámites de permisos).
- **Factores ambientales**: influencias externas — condiciones del mercado, inflación, competencia, demanda, cambios regulatorios/normativos, clima extremo, fluctuación de precios de materiales, avances tecnológicos.
- **Activos organizacionales**: políticas y procedimientos de la organización — procesos financieros, políticas de compras/adquisición, metodología y método(s) de estimación definidos, plantillas de estimación.

**Otros conceptos:**
- **Paquete de trabajo**: unidad discreta que compone un proyecto más grande; tarea o actividad específica que debe realizarse para lograr los objetivos (p. ej. en una casa: diseño de planos, excavación y preparación del sitio, cimientos, estructura, instalación eléctrica, fontanería, acabados interiores, paisajismo, inspecciones y permisos, mano de obra).
- **Umbrales de control**: los niveles de precisión de la estimación definitiva (−5 %/+10 %) se convierten posteriormente en umbrales de control para seguimiento y control del proyecto.

## Técnicas de estimación

### 1. Estimado por analogía (descendente / Top-Down Estimating)

- **Qué es**: se usa en las **primeras fases** del proyecto; toma como referencia los costos de **proyectos anteriores y similares**. No requiere mucha información — es una **primera aproximación**. La realizan normalmente directivos o expertos.
- **Cómo funciona**: es "descendente" porque parte de la EDT: el costo inicial del entregable principal se estima por analogía con otro proyecto, y luego se **desciende** nivel por nivel de la EDT asignando (repartiendo proporcionalmente) el costo a fases y paquetes de trabajo hasta el nivel más bajo. La suma de cada nivel debe corresponder al total del nivel superior.
- **Precisión**: **no es muy preciso** (falta de información inicial o información limitada). El PDF no da rango numérico.
- **Ventajas**: rapidez para generar una primera estimación; útil con información muy limitada y urgencia.
- **Desventajas**: baja precisión; depende de que exista un proyecto similar comparable.
- **Ejemplo genérico (Figura 1)**: Producto Final $1,000 → Diseño $100 (1.1) + Construcción $800 (1.2) + Entrega $100 (1.3); Construcción se desglosa en C1 $200 + C2 $300 + C3 $300.
- **Ejemplo viaje a Cancún**: un amigo viajó 7 días, 4 personas, temporada alta, gasto total $150,000.
  - Costo diario: $150,000 / 7 días = **$21,429/día**.
  - Costo por persona y día: $21,429 / 4 = **$5,357/día-persona**.
  - Tu viaje (2 personas, 4 días): Costo estimado = $5,357 × 2 personas × 4 días = **$42,856**.
  - Asignación descendente (Figura 2): Vacaciones $42,856 → Hospedaje $20,500 + Transportación $18,300 + Alimentación $4,056; Transportación → terrestre origen $1,000 + aéreo $14,000 + aeropuerto-hotel-aeropuerto $3,300 (suman $18,300).

### 2. Estimado paramétrico

- **Qué es**: requiere tener disponible **la mayoría de la información** (plan de costo, plan de calidad, plan de alcance, cronograma, registro de riesgos, lecciones aprendidas, recursos). Usa **relaciones matemáticas y datos históricos** (costos por unidad de medida: $/hora, $/m², etc.) para calcular el costo de **cada actividad o paquete de trabajo**.
- **Fórmula tipo**: Costo = cantidad de recursos × unidades de uso × tasa unitaria.
- **Cuándo usarla**: ya avanzada la planificación, cuando hay información puntual (tasas autorizadas, duraciones, cantidades).
- **Precisión**: **−10 % a +25 %**.
- **Ventajas**: mucho más específico y puntual → mayor exactitud que la analogía; automatizable con herramientas de gestión de proyectos.
- **Desventajas**: exige investigar información puntual de cada elemento; requiere que haya pasado tiempo de planificación.
- **Ejemplo (mano de obra)**: 3 ingenieros de diseño × 8 hrs/día × 5 días × $100/hora = **$12,000**.
- **Ejemplo Cancún (nivel 3 de la EDT)**: se investiga el dato puntual de cada paquete (aerolínea, tarifa, equipaje, seguros, impuestos…): transportación aérea = **$15,870** · transportación en el lugar de origen = **$1,320** · aeropuerto-hotel-aeropuerto = **$4,550**.

### 3. Estimado ascendente (Bottom-Up / estimado definitivo)

- **Qué es**: comienza por las **actividades** (lista de actividades/cronograma) o por los **paquetes de trabajo de los niveles inferiores de la EDT**, calcula su costo (paramétricamente) y va **sumando hacia arriba**: $PT = ΣCostos → $Fase = Σ$PT → Proyecto = Σ$Fases, hasta llegar al entregable/producto final.
- **Requisitos**: mucha información — enunciado del alcance, EDT, lista de actividades, cronograma, lista de requerimientos de recursos, tasas de costo de cada recurso, registro de riesgos y registro de lecciones aprendidas.
- **Precisión**: es el método de **mayor precisión**: **−5 % a +10 %**. Por eso se le llama **estimado definitivo**; esos niveles de precisión se convierten después en umbrales de control del proyecto.
- **Ventajas**: máxima precisión y trazabilidad por paquete.
- **Desventajas**: requiere la mayor cantidad de información y esfuerzo; solo posible en fases avanzadas de planificación.
- **Ejemplo genérico (Figura 3)**: C1 $300 + C2 $400 + C3 $400 → Construcción $1,000; Diseño $300 + Construcción $1,000 + Entrega $200 → Producto Final **$1,600**.
- **Ejemplo Cancún (Figura 4)**: nivel 3 (paramétricos): terrestre origen $1,320 + aéreo $15,870 + aeropuerto-hotel-aeropuerto $4,550 → **Transportación $21,740**. Nivel 2: Hospedaje $24,550 + Transportación $21,740 + Alimentación $3,850 → **Vacaciones $50,140**. Compárese con el estimado análogo de $42,856: el ascendente es muy diferente y mucho más preciso.

### 4. Estimado de tres puntos (PERT)

- **Qué es**: se aplica en ambientes de **mucha incertidumbre** (nueva tecnología, I+D, innovación). Define **tres escenarios de costo** para cada elemento de la EDT o del cronograma, por consenso/opinión de un grupo de expertos:
  - **Optimista "a"**: la opinión más favorable del grupo.
  - **Más probable "m"**: la opinión más común.
  - **Pesimista "b"**: la estimación más alta según los expertos.
- Se asume que los tres escenarios siguen una **distribución beta o PERT** (distribución **no simétrica**).
- **Fórmulas** (notación exacta del PDF):
  - Costo esperado: **Ce = (a + 4m + b) / 6**
  - Desviación estándar: **σ = (b − a) / 6**
- **Cuándo usarla**: alta incertidumbre de costos; permite además **análisis de riesgo**: si se aplica a todos los paquetes y fases (misma situación de incertidumbre), el costo total del proyecto se aproxima a una **distribución normal**, y con áreas bajo la curva normal (o Excel) se calculan probabilidades de terminar dentro de un costo dado.
- **Ventajas**: incorpora la incertidumbre y cuantifica el riesgo (probabilidades).
- **Desventajas**: depende del juicio de expertos; requiere más cálculo.
- **Ejemplo (diseño de componente de nueva tecnología)**: a = $5,000, m = $12,000, b = $30,000.
  - Ce = (5,000 + 4×12,000 + 30,000)/6 = **$13,833.33**
  - σ = (30,000 − 5,000)/6 = **$4,166.67**
- **Ejemplo de análisis de riesgo 1**: proyecto con costo promedio total $750,000 y σ = $10,500 (obtenidos combinando tres puntos + ascendente). Probabilidad de gastar hasta $760,000: área bajo la curva = **83 %**; riesgo de exceder $760,000 = **17 %** (riesgo significativo).
- **Ejemplo de análisis de riesgo 2 (Cancún)**: costo total esperado $55,800, σ = $6,500, presupuesto máximo $60,000. El texto concluye **74 % de probabilidad de cumplir** el presupuesto y **26 % de excederlo** → situación de **alto riesgo**; sugerencia: tener preparada una cantidad mayor a $60,000. ⚠️ Nota: la figura del PDF rotula el área como "64 %", pero el texto dice 74 % — con z = (60,000 − 55,800)/6,500 ≈ 0.646 el área real es ≈74 %, así que el 64 % de la figura es errata del material.

> Comparativa rápida de precisión (según los PDFs): Analogía = baja, sin rango numérico · Paramétrica = **−10 %/+25 %** · Ascendente/definitiva = **−5 %/+10 %** (la mayor) · Tres puntos = da Ce ± σ y probabilidades, no un rango fijo.

## Ejemplo práctico completo (la casa, paso a paso)

El PDF de la casa no calcula cifras: recorre **qué información se necesita** para estimar con precisión en un entorno VUCA. Elementos aplicados al proyecto "construcción de una casa":

1. **Línea base del alcance**: enunciado del alcance + EDT + diccionario EDT. Del enunciado se define qué se incluye/excluye: tipo de vivienda, número de habitaciones, baños, garaje, acabados, servicios, suposiciones y restricciones (incluido el **presupuesto máximo**). La EDT muestra gráficamente las fases desde el diseño de planos hasta inspecciones y permisos.
2. **Plan de gestión del costo**: procedimientos para estimar y presupuestar la construcción + plantillas/formatos. Estructura completa: Portada, Índice, Introducción, Objetivos, EDT, Método de estimación de costos, Presupuesto, Control de costos, Proceso de aprobación de cambios, Riesgos relacionados con los costos, Seguimiento y reporte, Anexos (ver Conceptos clave).
3. **Plan de calidad**: métricas para evaluar si la construcción cumple expectativas del cliente, estándares y normativas locales — cimientos, estructura, instalaciones, acabados interiores/exteriores, paisajismo.
4. **Registro de lecciones aprendidas**: p. ej. alcance detallado → estimaciones más precisas; registro actualizado de precios de materiales → mitiga impactos financieros imprevistos.
5. **Registro de riesgos**: fluctuación de precios de materiales por factores económicos, cambios en requisitos del cliente durante la construcción, problemas de mano de obra/calidad de materiales ante condiciones ambientales imprevistas.
6. **Cronograma del proyecto** — descomposición ejemplo:
   - **6 fases**: Planificación y diseño → Preparación del sitio → Construcción principal → Acabados → Inspección y entrega → Cierre del proyecto.
   - Fase "Planificación y diseño" → **2 paquetes de trabajo**: planificación inicial y diseño arquitectónico.
   - Paquete "Diseño arquitectónico" → **4 actividades**: contratación de un arquitecto, desarrollo de los planos arquitectónicos, diseño de interiores y selección de materiales.
7. **Lista de requerimientos de recursos**: humanos (equipo del proyecto, trabajadores de construcción y acabados), materiales (materiales de construcción, equipamiento, sistema eléctrico y fontanería, mobiliario), financieros, de tiempo (plazos de entrega, tiempo de inspección y pruebas), externos (proveedores, subcontratistas, trámites de permisos).
8. **Factores ambientales**: mercado inmobiliario, competitividad de precios en la zona, cambios regulatorios/normativos locales, lluvias torrenciales/sequías/clima extremo, fluctuación de precios de materiales, avances tecnológicos en construcción.
9. **Activos organizacionales**: metodología y método(s) de estimación definidos, plantillas de estimación.

**Conclusión del caso**: la estimación requiere una base sólida de información, considerar diversos factores, mantenerse actualizado y aprender de experiencias anteriores para mejorar la precisión y ejecutar dentro del presupuesto.

*(El ejemplo numérico paso a paso del módulo — analogía $42,856 → paramétrico por paquete → ascendente $50,140 → tres puntos con probabilidades — es el del viaje a Cancún, desarrollado en las secciones de técnicas.)*

## Conexión con APL/PIDA

- En el PIDA, Carlos estimó el **re-trabajo en horas-hombre** partiendo de un baseline FTR de 82-88 %: es en esencia una estimación **paramétrica** (horas-hombre × tasa) alimentada por **lecciones aprendidas** (bitácora FTR) y **registro de riesgos**, exactamente los insumos que pide esta lección.
- La **estimación de tres puntos/PERT** con (O+4M+P)/6 ya apareció aplicada a duraciones en [[L4 - Cálculo de la ruta crítica|M01-L4]]; aquí la misma fórmula se aplica a **costos** (Ce y σ) y se extiende al análisis probabilístico con la curva normal.

## Preguntas de repaso tipo quiz

**P1. ¿Qué comprende la línea base del alcance y por qué es insumo de la estimación de costos?**
R: Enunciado del alcance + EDT + diccionario de la EDT. Define qué incluye/excluye el proyecto, con asunciones y restricciones (incluido el presupuesto máximo); sin ella no se sabe qué trabajo hay que costear.

**P2. ¿Qué porcentaje de proyectos logra mantenerse dentro del presupuesto original y cuál es una causa frecuente de los excesos?**
R: Solo el 62 %. Una causa significativa y frecuente es la falta de aplicación formal de técnicas de estimación de costos.

**P3. ¿Por qué la estimación por analogía se llama "descendente" y quién suele realizarla?**
R: Porque parte del costo del entregable principal (por analogía con un proyecto anterior/similar) y desciende por la EDT asignando costos a fases y paquetes hasta el nivel más bajo. La realizan directivos o expertos, en fases tempranas, con poca información.

**P4. Ordena las técnicas de menor a mayor precisión y da los rangos que aparecen en el material.**
R: Analogía (baja, sin rango numérico) < Paramétrica (−10 % a +25 %) < Ascendente o definitiva (−5 % a +10 %, la mayor precisión; sus niveles se vuelven umbrales de control).

**P5. ¿En qué distribución se basa el estimado de tres puntos, qué significan a, m, b, y cuáles son sus fórmulas?**
R: Distribución beta o PERT (no simétrica). a = optimista (opinión más favorable), m = más probable (opinión más común), b = pesimista (estimación más alta). Ce = (a + 4m + b)/6; σ = (b − a)/6.

**P6. ¿Por qué al ascendente se le llama "estimado definitivo" y qué información requiere?**
R: Porque proporciona la mayor precisión (−5 %/+10 %). Requiere enunciado del alcance, EDT, lista de actividades, cronograma, requerimientos de recursos, tasas de costo por recurso, registro de riesgos y lecciones aprendidas.

**P7. [Ejercicio numérico — analogía] Tu amigo gastó $150,000 en 7 días con 4 personas. ¿Cuánto estimas para tu viaje de 2 personas y 4 días?**
R paso a paso: (1) $150,000 / 7 = $21,429/día. (2) $21,429 / 4 = $5,357 por persona-día. (3) $5,357 × 2 × 4 = **$42,856**.

**P8. [Ejercicio numérico — paramétrico] 3 ingenieros de diseño trabajan 8 hrs/día durante 5 días; la tasa de costo directo autorizada es $100/hora. ¿Estimado paramétrico de mano de obra?**
R: 3 × 8 × 5 × $100 = **$12,000** (3 ingenieros × 40 hrs c/u = 120 hrs × $100).

**P9. [Ejercicio numérico — tres puntos] Para el diseño de un componente los expertos dan a = $5,000, m = $12,000, b = $30,000. Calcula Ce y σ.**
R paso a paso: Ce = (5,000 + 4×12,000 + 30,000)/6 = (5,000 + 48,000 + 30,000)/6 = 83,000/6 = **$13,833.33**. σ = (30,000 − 5,000)/6 = 25,000/6 = **$4,166.67**.

**P10. [Ejercicio — análisis de riesgo] Un proyecto tiene costo esperado total $750,000 y σ = $10,500. ¿Qué probabilidad hay de terminar con $760,000 o menos, y cuál es el riesgo de excederlo? ¿Y en el caso Cancún ($55,800, σ = $6,500, tope $60,000)?**
R: Con el área bajo la curva normal: 83 % de terminar en ≤$760,000, 17 % de excederlo (riesgo significativo). En Cancún: 74 % de cumplir el tope de $60,000 y 26 % de excederlo → alto riesgo; se sugiere tener preparada una cantidad mayor a $60,000.

**P11. [Ejercicio — ascendente] Con los paramétricos del nivel 3 de Cancún (terrestre origen $1,320, aéreo $15,870, aeropuerto-hotel-aeropuerto $4,550) y con Hospedaje $24,550 y Alimentación $3,850, calcula el costo total ascendente y compáralo con el análogo.**
R: Transportación = 1,320 + 15,870 + 4,550 = $21,740. Total = 24,550 + 21,740 + 3,850 = **$50,140**, vs. $42,856 del método análogo: el ascendente da un resultado muy diferente y más preciso.

**P12. Menciona 4 factores ambientales y 2 activos organizacionales que influyen en la estimación de la casa.**
R: Ambientales: mercado inmobiliario, competitividad de precios de la zona, cambios en regulaciones/normativas locales, clima extremo (lluvias/sequías), fluctuación de precios de materiales, avances tecnológicos. Activos: método(s) de estimación definidos y plantillas de estimación (también procesos financieros y políticas de compras).
