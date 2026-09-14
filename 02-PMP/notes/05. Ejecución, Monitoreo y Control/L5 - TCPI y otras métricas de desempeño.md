---
title: L5 — TCPI y otras métricas de desempeño
curso: PMP
modulo: 05. Ejecución, Monitoreo y Control
leccion: L5
fuente: "[[documentation/05. Ejecución, Monitoreo y Control/PMP_SC1.5_Versión impresa_L5.pdf|Versión impresa L5]]"
complementos: ["[[documentation/05. Ejecución, Monitoreo y Control/Ejemplos de métricas para el desempeño de la ejecución de un proyecto.pdf|Ejemplos de métricas para el desempeño de la ejecución de un proyecto]]", "[[documentation/05. Ejecución, Monitoreo y Control/Earned Value y MsProject.pdf|Earned Value y MsProject]]", "[[documentation/05. Ejecución, Monitoreo y Control/Medición del desempeño del proyecto.pdf|Medición del desempeño del proyecto (caso Platinum Inc., referencia parcial)]]"]
status: por-estudiar
tags: [pmp, ejecucion-monitoreo-control]
---

# L5 — TCPI y otras métricas de desempeño

## Resumen
Además de las variaciones e índices vistos en L4 (SV, CV, SPI, CPI), existe una métrica del EVM poco conocida pero muy útil: el **TCPI (To Complete Performance Index)**, que indica la eficiencia con la que se debe gastar el presupuesto/fondos remanentes para terminar el proyecto dentro del BAC (o del EAC). Fuera del marco de Valor Ganado existen otras 8 métricas cualitativas/cuantitativas (satisfacción del cliente, productividad, tiempo de ciclo, ROI, costo de calidad, satisfacción de empleados, cumplimiento de requerimientos y alineamiento estratégico) que complementan la visión del desempeño de un proyecto, derivadas de factores reales que afectan la ejecución (scope creep, mal dinamismo de equipo, multitareas, sobrecarga, procesos ineficientes, ambiente caótico).

## Conceptos clave (con definiciones completas)

- **TCPI (To Complete Performance Index / Índice de Desempeño para Terminar)**: eficiencia a la que se debe gastar el presupuesto (o fondos) remanente para cumplir la meta de costo establecida (BAC), desde el momento de la medición hasta el final del proyecto.
- **Fondos remanentes**: pueden calcularse de dos formas — (1) BAC – AC (contra el presupuesto original), o (2) EAC – AC (contra el último pronóstico del PM).
- **Project Scope Creep**: cambios no planeados al alcance que generan problemas de tiempo/costo/riesgo/calidad; pueden originarse en el cliente, el mercado, la dirección o los recursos.
- **Poor Team Dynamics**: falta de clima de trabajo conjunto, desmotivación, conflictos, cambios de equipo.
- **Multitasking Team Members**: confusión de prioridades, falta de concentración, retrasos, errores, más riesgo.
- **Over-scheduling People's time**: sobrecarga de trabajo que hace que el personal posponga tareas por prioridades personales/familiares.
- **Inefficient Business Processes**: burocracia organizacional, exceso de papeleo por políticas obsoletas.
- **Chaotic Work Environments**: desorden que produce distracción y pérdida de tiempo buscando información.

## Desarrollo del contenido

### 1. TCPI — fórmulas

**Al considerar el BAC** (primera meta: terminar dentro del presupuesto autorizado):
```
TCPI(BAC) = Valor del trabajo remanente / Fondos remanentes = (BAC − EV) / (BAC − AC)
```

**Al considerar el EAC** (cuando ya se sabe que el BAC no se cumplirá y se usa el último pronóstico del PM):
```
TCPI(EAC) = Valor del trabajo remanente / Fondos remanentes = (BAC − EV) / (EAC − AC)
```

Interpretación: es el índice de eficiencia al que se debe **trabajar de la fecha de medición en adelante** para no exceder el presupuesto (o el pronóstico). Si el TCPI resultante es muy superior a 1.0 (y en particular mayor al CPI actual), es señal de que será muy difícil de lograr y el PM debe solicitar fondos adicionales (pronosticar un nuevo EAC y pedir autorización a la alta dirección).

### 2. Otras métricas para determinar el nivel de desempeño (fuera del EVM)

Estas métricas se derivan de factores reales de ejecución (LaBrosse, 2006, *Cheetah Project Management*) y complementan el análisis EVM con una visión 360°:

1. **Índice de satisfacción del cliente**: índice compuesto ponderado de aspectos "suaves" y "duros" que dan valor al cliente; busca detectar necesidad de acciones de mejora/correctivas.
2. **Productividad**: mide recursos utilizados sobre disponibles (humanos, materiales, instalaciones, equipo, monetarios).
   ```
   % Productividad Ganada = (1 − (horas-Recurso reales / horas-Recurso planeadas)) × 100
   ```
3. **Tiempo de ciclo**: mide el tiempo de ejecución de una actividad o proceso del ciclo de vida del proyecto, buscando disminuirlo.
4. **Retorno de la Inversión (ROI)**: cuantifica el beneficio neto sobre el total invertido (ahorros o incrementos en utilidades, contra costos de diseño/desarrollo/ejecución: mano de obra, materiales, equipo, gastos administrativos).
   ```
   ROI = ((Beneficios netos − Inversión) / Inversión) × 100
   ```
5. **Costo de calidad**: dinero perdido por pérdidas, productos/servicios defectuosos, reprocesos, inspecciones extra y atención de quejas; busca cuantificar y disminuir esa pérdida.
6. **Índice de satisfacción de los empleados**: mide moral/motivación (clima laboral, estrés, quejas, ausentismo, rotación voluntaria); se mide con encuesta periódica, igual que la satisfacción del cliente.
7. **Cumplimiento de requerimientos**: nivel de cumplimiento de características funcionales/no funcionales vs. lo establecido; se mide con checklists/listas de verificación.
8. **Nivel de alineamiento con los objetivos estratégicos del negocio**: se pregunta a los interesados si el proyecto contribuye a los objetivos estratégicos de la organización.

El conjunto total de métricas de un proyecto = las del EVM + estas 8 (cuantitativas y cualitativas), cuyas fórmulas/encuestas específicas dependen del proyecto.

## Ejemplos y ejercicios del material (resueltos paso a paso)

### A. Ejemplos de las 8 "otras métricas" (del complemento "Ejemplos de métricas...")

**1. Índice de satisfacción del cliente** — Encuesta de 5 preguntas (escala 1-5) a un cliente de construcción de casa residencial. Respuestas: 4, 3, 5, 4, 4. Con el criterio "promedio aritmético de las 5 preguntas": **índice = 4** → cliente "algo satisfecho"; se recomienda mejorar la calidad de los trabajos percibidos (pregunta 2 fue la más baja, con 3).

**2. Productividad** — Actividad de programación planeada en 380 horas-programador; se usaron realmente 355 horas.
```
% Productividad Ganada = (1 − (355/380)) × 100 = 6.6%
```
Si en cambio se hubieran usado 415 horas (más de lo planeado):
```
% Productividad Ganada = (1 − (415/380)) × 100 = −9.2% (pérdida de productividad)
```

**3. Tiempo de ciclo** — El ciclo de planeación completo dura 25 días hábiles (definición de tareas, WBS, interrelaciones, estimación de duraciones/costos). Se pide al PM comprimirlo a 10 días hábiles (dentro de un máximo de 15 días). El material plantea la pregunta abierta "¿será posible?" — sin dar una respuesta numérica cerrada; se espera un análisis cualitativo de las restricciones de compresión del cronograma (fast tracking/crashing) de esa actividad.

**4. Retorno de la Inversión (ROI)** — Inversión de $3 millones; tasa mínima esperada 10% anual.
```
ROI = ((Beneficios netos − Inversión) / Inversión) × 100
```
- **Caso a)** Beneficio neto de $3.5 millones en el año 1:
  ROI = ((3.5 − 3)/3) × 100 = **16.7% anual** → proyecto rentable (>10% mínimo esperado).
- **Caso b)** Beneficios de $2.1 millones (año 1) y $1.7 millones (año 2), traídos a valor presente con i=10%:
  ```
  Beneficios netos a valor presente = 2.1 + 1.7/(1+0.1) = $3.65 millones
  ROI = ((3.65 − 3)/3) × 100 = 21.7% anual
  ```
  → proyecto rentable.

**5. Costo de calidad** — Tabla de defectos en reportes semanales durante 9 meses (tipo de defecto, frecuencia, costo unitario de reparación). Costo total de reparación (no calidad) = **$73,850**, con ponderación por tipo de defecto:

| Tipo de defecto | Frecuencia | Costo unit. | Costo total | Ponderación |
|---|---|---|---|---|
| Errores de comunicación interna | 12 | $2,000 | $24,000 | 32.5% |
| Errores por retrasos | 25 | $800 | $20,000 | 27.1% |
| Errores de comunicación con cliente | 15 | $1,000 | $15,000 | 20.3% |
| Fallas del sistema | 3 | $3,000 | $9,000 | 12.2% |
| Errores por captura de datos | 13 | $450 | $5,850 | 7.9% |
| **Total** | | | **$73,850** | **100%** |

**6. Índice de satisfacción de los empleados** — Encuesta análoga a la del cliente (5 preguntas, escala 1-5). Respuestas: 3, 4, 4, 3, 3. Promedio = **3.4** → entre indiferente y algo satisfecho; se recomiendan medidas casi urgentes, sobre todo en motivación y remuneración (preguntas 1 y 4 fueron las más bajas).

**7. Cumplimiento de requerimientos** — Ejemplo de checklist ("Lista de verificación de la revisión de la orden de compra") con criterio de aceptación: cumplir el 100% de los puntos (si no cumple el 100%, no pasa la revisión y se contacta al solicitante).

**8. Nivel de alineamiento con objetivos estratégicos** — El PM consulta por separado a cada directivo (perspectivas financiera, operativa, tecnológica, marketing) y emite la evaluación final según la opinión de la mayoría.

### B. Ejemplo integral de EVM + TCPI vía MS Project (del complemento "Earned Value y MsProject.pdf")

Caso **Proyecto Avión**, fecha de estado 5-mayo-2023, línea base activada en MS Project. Se configuran la fecha de estado (Proyecto → Información del proyecto), se captura el avance en la "Tabla seguimiento" (%completado y Costo real), y se consultan las tablas "Valor acumulado (Earned Value)", "Valor acumulado de indicadores de costo" y "Valor acumulado de indicadores de programación".

Resultados a nivel proyecto (5-mayo-2023):

| Métrica | Valor | Interpretación |
|---|---|---|
| PV | $2,600,001 | Lo que se debió haber hecho a la fecha |
| EV | $2,453,823 | Lo que realmente se ha hecho |
| AC | $2,227,949 | Costo real erogado/comprometido |
| BAC | $8,359,000 | Presupuesto aprobado total |
| EAC | $7,589,554 | Pronóstico de costo final |
| VAC | $769,446 | BAC − EAC; positivo = ahorro esperado |
| CV | $225,874 | EV − AC; positivo = ahorro a la fecha |
| SV | −$146,178 | EV − PV; negativo = atraso |
| CV% | 9% | % de ahorro a la fecha |
| SV% | −6% | % de retraso a la fecha |
| **CPI** | **1.1** | Ahorro (mismo significado que CV%) |
| **SPI** | **0.94** | Atraso (mismo significado que SV%) |
| **TCPI** | **0.96** | Eficiencia a mantener del 5-may-23 en adelante para terminar dentro del BAC |

Umbrales de control asumidos: CPI mínimo aceptable 0.9 (90%); SPI mínimo aceptable 0.9 (90%). Conclusión del caso: el proyecto **va bien** — puede terminar dentro del presupuesto (CPI=1.1 > umbral) y, aunque va un poco retrasado (SPI=0.94), puede terminar en la fecha de la Línea base porque ambos índices superan el umbral mínimo de 0.9.

Nota: como TCPI (0.96) < CPI (1.1), terminar dentro del BAC exige trabajar solo ligeramente menos eficientemente que el desempeño promedio actual — una señal de que el objetivo de costo es alcanzable sin fondos adicionales.

### Nota sobre "Medición del desempeño del proyecto.pdf"
Igual que en L4, este caso interactivo (*Platinum Inc.*) dedica su "Misión 4" a calcular CV, SV, CPI, SPI y TCPI e interpretar resultados junto con el Control de Cambios Integrado. Es más una guía de autoevaluación/reflexión (afirmaciones tipo "sé que...", "distingo que...", "recuerdo que...") que una fuente de datos numéricos nuevos; se recomienda como **caso práctico de refuerzo** para ejercitar TCPI y el resto del EVM en MS Project.

## Conexión con APL/PIDA
- El **PIDA** no usó TCPI formalmente, pero el concepto es análogo a preguntarse "¿qué nivel de FTR/re-trabajo hay que sostener de ahora al cierre para llegar a las metas (FTR≥90%, re-trabajo −10%)?" — el corte W4 (FTR 96%, re-trabajo −11.9%) ya superaba ambas metas, equivalente a un TCPI favorable (menor exigencia futura que el desempeño ya logrado).
- Las "otras métricas" de esta lección (satisfacción del cliente, cumplimiento de requerimientos, costo de calidad) mapean directamente a métricas reales del PIDA: la **aceptación de sitios por las 5 áreas del cliente** (RAN, Planning, Quality, O&M, Acceptance) es un cumplimiento de requerimientos vía checklist; el **CR-001 (único FTR=No)** es un caso de costo de calidad (reproceso); y las **retrospectivas W3/W5/W7/W9** cumplen el mismo rol que la encuesta de satisfacción de empleados/equipo. Para el detalle de EVM aplicado a costos ver también [[L5 - Control de costos y valor ganado]] del módulo 03 de Gestión de Costos.

## Preguntas de repaso tipo quiz

1. **¿Qué mide el TCPI?** Respuesta: la eficiencia con la que se debe gastar el presupuesto/fondos remanentes de la fecha de medición en adelante para terminar el proyecto dentro del BAC (o del EAC).
2. **Escriba la fórmula del TCPI usando el BAC.** Respuesta: TCPI(BAC) = (BAC − EV) / (BAC − AC).
3. **¿Cuándo se debe usar TCPI(EAC) en lugar de TCPI(BAC)?** Respuesta: cuando ya se ha determinado que no es posible cumplir la meta original (BAC) y el PM ha generado un nuevo pronóstico (EAC) como referencia de fondos remanentes.
4. **Proyecto con BAC=$8,359,000, EV=$2,453,823, AC=$2,227,949. Calcule TCPI(BAC).**
   Respuesta: TCPI = (8,359,000 − 2,453,823) / (8,359,000 − 2,227,949) = 5,905,177 / 6,131,051 ≈ 0.963 (~0.96, coincide con el ejemplo de MS Project).
5. **En el caso "Proyecto Avión", CPI=1.1 y TCPI=0.96. ¿Qué implica que TCPI sea menor que CPI?** Respuesta: que para terminar dentro del presupuesto se requiere una eficiencia futura (0.96) menor a la ya lograda (1.1), es decir, la meta de costo es alcanzable con margen.
6. **Nombre las 8 "otras métricas" de desempeño fuera del EVM.** Respuesta: satisfacción del cliente, productividad, tiempo de ciclo, ROI, costo de calidad, satisfacción de empleados, cumplimiento de requerimientos, alineamiento con objetivos estratégicos.
7. **Se planean 380 horas-programador y se usan 400. Calcule el % de productividad ganada.**
   Respuesta: (1 − 400/380) × 100 = −5.3% (pérdida de productividad).
8. **Una inversión de $3M genera beneficios netos de $3.5M en el año 1. ¿Cuál es el ROI y es rentable si la tasa mínima esperada es 10%?**
   Respuesta: ROI = ((3.5−3)/3)×100 = 16.7% anual; sí es rentable porque supera el 10% mínimo esperado.
9. **¿Qué factor de LaBrosse describe la confusión de prioridades cuando el personal atiende varias tareas a la vez?** Respuesta: Multitasking Team Members (personal del equipo haciendo multitareas).
10. **En la métrica de costo de calidad, ¿qué representa la "ponderación"?** Respuesta: el porcentaje que cada tipo de defecto representa sobre el costo total de reparación (no calidad), permitiendo priorizar qué defectos atacar primero.
