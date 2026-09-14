---
title: L4 — Earned Value Method (EVM)
curso: PMP
modulo: 05. Ejecución, Monitoreo y Control
leccion: L4
fuente: "[[documentation/05. Ejecución, Monitoreo y Control/PMP_SC1.5_Versión impresa_L4.pdf|Versión impresa L4]]"
complementos: ["[[documentation/05. Ejecución, Monitoreo y Control/Ejemplos de casos para determinar el costo final.pdf|Ejemplos de casos para determinar el costo final]]", "[[documentation/05. Ejecución, Monitoreo y Control/Medición del desempeño del proyecto.pdf|Medición del desempeño del proyecto (caso Platinum Inc., referencia parcial)]]"]
status: por-estudiar
tags: [pmp, ejecucion-monitoreo-control]
---

# L4 — Earned Value Method (EVM)

## Resumen
Medir el desempeño de la gestión de un proyecto es comparar los datos reales de ejecución contra lo planeado (Línea base) a una fecha determinada. El método más usado para esto es el **Earned Value Method (EVM)**, que integra mediciones de alcance, costo y tiempo en valores numéricos objetivos. Esta lección define las tres variables base del EVM (PV, EV, AC), las variaciones (SV, CV), los índices de eficiencia (SPI, CPI) y los pronósticos de costo final (BAC, EAC, ETC, VAC) bajo tres escenarios de riesgo.

## Conceptos clave (con definiciones completas)

- **Controlar un proyecto**: ejecutarlo según la Línea base, tanto en tiempo como en costo, logrando el alcance esperado.
- **Valor Planeado (VP) / Planned Value (PV)**: presupuesto autorizado y asignado al trabajo programado a una fecha específica (fecha de revisión del estado del proyecto). El PV total del proyecto se llama **Budget at Completion (BAC)**.
- **Valor Ganado (VG) / Earned Value (EV)**: valor del trabajo realmente realizado, expresado en términos del presupuesto autorizado, a la misma fecha de revisión. No puede ser mayor que el presupuesto autorizado de una actividad. Se deriva del % completado.
- **Costo Real (CR) / Actual Cost (AC)**: costo gastado a la fecha de revisión; no tiene límite hacia arriba; debe corresponder a lo presupuestado en el PV y medido con el EV.
- **Línea base**: el plan aprobado (alcance + costo + cronograma) contra el cual se comparan los datos reales.

## Desarrollo del contenido

### 1. Las tres dimensiones del EVM
Para cada actividad o paquete de trabajo el EVM considera **PV, EV y AC** a una fecha de estado (status date) determinada. Estas tres cifras son la base de todo el análisis de variaciones e índices.

### 2. Análisis de variaciones

**Variación del avance / Schedule Variance (SV)**
```
SV = EV – PV
```
- SV > 0 → el proyecto va adelantado.
- SV < 0 → el proyecto va atrasado.
- SV = 0 → cumple exactamente la Línea base.

**Variación del costo / Cost Variance (CV)**
```
CV = EV – AC
```
- CV > 0 → se está gastando menos de lo planeado (ahorro).
- CV < 0 → se está gastando de más (sobrecosto).
- CV = 0 → cumple exactamente la Línea base.
- El CV es crítico porque relaciona el desempeño físico (trabajo hecho) con los costos incurridos.

### 3. Índices de eficiencia (desempeño)

**Índice de desempeño del avance / Schedule Performance Index (SPI)**
```
SPI = EV / PV
```
- SPI < 1.0 → menos trabajo realizado del planeado (atrasado).
- SPI > 1.0 → más trabajo realizado del planeado (adelantado).
- SPI = 1.0 → caso ideal (a tiempo).

**Índice de desempeño del costo (CPI)**
```
CPI = EV / AC
```
- CPI < 1.0 → sobregasto a la fecha.
- CPI > 1.0 → ahorro a la fecha.
- CPI = 1.0 → caso ideal; es **la métrica más crítica del EVM**.

### 4. Pronóstico de costo final para mejorar el desempeño

Un pronóstico es una estimación de las condiciones futuras del proyecto, basada en la información y el desempeño conocidos hasta el momento. Sirve para decidir si se deben emprender acciones correctivas, preventivas o de mejora.

Variables adicionales del pronóstico:

- **Presupuesto a la Terminación (Budget At Completion – BAC)**: presupuesto aprobado total del proyecto.
  ```
  BAC = Σ PV (de todas las actividades del proyecto)
  ```
- **Estimado del Costo Final (Estimate At Completion – EAC)**: costo final estimado del proyecto, considerando el gasto actual y lo que falta por hacer, bajo distintos escenarios.
- **Estimado del Costo para Terminar (Estimate to Complete – ETC)**: costo estimado para terminar el trabajo remanente (bajo distintos escenarios).
- **Variación del Costo en la Terminación (Variance at Completion – VAC)**: diferencia entre el costo final estimado y el presupuesto/pronóstico, considerando lo que falta por hacer.
  ```
  VAC = BAC – EAC
  ```

Los EAC se basan en el costo real del trabajo realizado más un ETC del trabajo remanente. El enfoque más común es el agregado "abajo hacia arriba" (bottom-up, en el contexto de la EDT/WBS):
```
EAC = AC + bottom-up ETC
```

**Los tres escenarios de riesgo para el EAC:**

1. **Escenario optimista / riesgo bajo** (estabilidad; asume que el resto del proyecto se ejecutará según lo planeado, a tasa normal):
   ```
   EAC = AC + (BAC – EV)
   ```
2. **Escenario más probable / riesgo medio** (usa el BAC y el CPI actual; es el enfoque más común):
   ```
   EAC = BAC / CPI
   ```
3. **Escenario pesimista / riesgo alto** (poca estabilidad; ajusta el ETC restante por el CPI y el SPI combinados — asume que tanto el costo como el avance seguirán con el desempeño actual):
   ```
   EAC = AC + (BAC – EV) / (CPI × SPI)
   ```

También existe un pronóstico de la **duración final** con el SPI:
```
EAC_T = Duración Planeada (PD) / SPI
```

## Ejemplos y ejercicios del material (resueltos paso a paso)

Estos ejercicios provienen del complemento **"Ejemplos de casos para determinar el costo final.pdf"**, que se integró íntegramente a esta lección por ser aplicación directa de BAC/EAC/ETC/VAC.

### Ejemplo 1 — Pronóstico de duración (EAC_T)
Proyecto planeado a 15 meses. A los 3 meses, SPI = 0.9.
```
EAC_T = PD / SPI = 15 / 0.9 = 16.7 meses
```

### Ejemplo 2 — Caso de consultoría (informe EVM completo a la 4ª semana)
9 actividades con predecesoras, duración y costo (PV) definidos; a la 4ª semana se reporta %Avance y Costo real (AC) de las 3 primeras actividades (las demás siguen en 0%).

Datos totales del proyecto a la 4ª semana:
- AC = $50,800; PV = $51,200; EV = $47,160
- **SV = EV – PV = 47,160 – 51,200 = –$4,040** (atrasado)
- **CV = EV – AC = 47,160 – 50,800 = –$3,640** (sobrecosto)
- **CPI = EV/AC = 0.928**; **SPI = EV/PV = 0.921**
- BAC = $223,200
- **EAC₁ (optimista) = AC + (BAC – EV) = 50,800 + (223,200 – 47,160) = $226,840**
- **EAC₂ (más probable) = BAC / CPI = 223,200 / 0.928 = $240,427**
- **EAC₃ (pesimista) = AC + (BAC – EV)/(CPI × SPI) = $256,672**
- VAC₁ = BAC – EAC₁ = –$3,640; VAC₂ = –$17,227; VAC₃ = –$33,472
- **EAC_T = PD / SPI = 22.8** (unidades de la duración total planeada)

Conclusión del material: como CPI y SPI están por encima del umbral de tolerancia (0.9) y los pronósticos son solo ligeramente superiores al BAC, **no es necesario aplicar acciones correctivas/preventivas** ni cambiar la Línea base; basta con ajustes menores en las actividades subsecuentes.

### Ejemplo 3 — EAC escenario más probable (opción múltiple)
Tres tareas A, B, C con valor planeado, %avance y costo real; BAC = $3,000.
- EV = 400 + 337.5 + 540 = **1,277.5**
- AC = 500 + 402 + 550 = **1,452**
- CPI = EV/AC = 1,277.5/1,452 = **0.88**
- **EAC = BAC/CPI = 3,000/0.88 = $3,370.8 ≈ $3,371** (respuesta correcta: b)

### Ejemplo 4 — EAC escenario pesimista
Tres actividades A, B, C con PV total, PV a la fecha, %avance y AC; BAC = $1,000.
- EV = 200 + 67.5 + 150 = **417.5**
- AC = 200 + 120 + 175 = **495**
- PV (a la fecha) = 200 + 65 + 180 = **445**
- CPI = EV/AC = 417.5/495 = **0.84**
- SPI = EV/PV = 417.5/445 = **0.94**
- **EAC = AC + (BAC – EV)/(CPI × SPI) = 495 + (1,000 – 417.5)/(0.84 × 0.94) ≈ $1,241**
  (el material redondea el producto CPI×SPI a 0.84×0.93 y obtiene $1,240.6 ≈ $1,241; con 0.84×0.94 el resultado es prácticamente el mismo)

### Nota sobre "Medición del desempeño del proyecto.pdf"
Este complemento es un **caso interactivo completo** (empresa ficticia *Platinum Inc.*, personajes Enrique/Cleo/Carmen) que recorre 4 "misiones": (1) establecer características de la Línea base, (2) preparar el archivo en MS Project (fecha de estado, tabla de seguimiento, línea de progreso), (3) calcular PV/EV/AC con Valor Ganado, y (4) calcular CV/SV/CPI/SPI/TCPI e interpretar resultados con Control de Cambios Integrado. Es mayormente una guía de reflexión y autoevaluación (preguntas tipo checklist) más que una tabla numérica resuelta; se recomienda usarlo como **caso práctico de refuerzo** para aplicar manualmente las fórmulas de esta lección y de L5, más que como fuente de datos para el quiz.

## Conexión con APL/PIDA
- El **PIDA (Telemóvil Costa Rica)** usó como métricas de desempeño el **FTR (First Time Right) ≥90%** y el **re-trabajo (−10%)** en lugar de EVM puro — son métricas de calidad/eficiencia de ejecución análogas al CPI/SPI, pero orientadas a aceptación técnica de sitios en vez de costo/cronograma monetario. El corte de semana 4 del PIDA (FTR 96%, re-trabajo −11.9%) es conceptualmente equivalente a revisar CPI/SPI en una fecha de estado: ambos permiten decidir si se requieren acciones correctivas.
- El seguimiento semanal de aceptación de sitios (7/23 en W4) funciona como un "avance físico" (~EV) que se puede comparar contra el cronograma planeado (~PV) para estimar un "SPI informal" del proyecto PIDA — aunque el PIDA no usó EAC/BAC formalmente, el desfase estructural integración→aceptación que retrasó el cierre a W9 es análogo a un SV negativo sostenido.

## Preguntas de repaso tipo quiz

1. **¿Qué significa un SV = –$5,000?** Respuesta: el proyecto va atrasado; se ha ganado $5,000 menos de valor del que se planeó tener a la fecha.
2. **¿Qué significa un CPI = 1.15?** Respuesta: hay ahorro; por cada dólar gastado se obtuvo $1.15 de valor (eficiencia de costo favorable).
3. **Un proyecto tiene BAC = $500,000, EV = $200,000, AC = $250,000. Calcule CV y CPI.**
   Respuesta: CV = EV – AC = 200,000 – 250,000 = –$50,000 (sobrecosto); CPI = 200,000/250,000 = 0.8.
4. **Con los datos de la pregunta anterior, calcule el EAC bajo el escenario más probable.**
   Respuesta: EAC = BAC/CPI = 500,000/0.8 = $625,000.
5. **¿Cuál es la diferencia conceptual entre EAC y ETC?** Respuesta: EAC es el costo final total estimado del proyecto completo; ETC es solo el costo estimado de lo que falta por hacer desde ahora hasta el final.
6. **¿Cuál escenario de EAC usa simultáneamente el CPI y el SPI?** Respuesta: el escenario pesimista (riesgo alto): EAC = AC + (BAC – EV)/(CPI × SPI).
7. **Proyecto planeado a 12 meses; a los 4 meses SPI = 0.8. ¿Cuál es el pronóstico de duración final (EAC_T)?**
   Respuesta: EAC_T = PD/SPI = 12/0.8 = 15 meses.
8. **En el Ejemplo 3 (Actividades A, B, C; BAC=$3,000), ¿por qué el EAC resultante ($3,371) es mayor al BAC?**
   Respuesta: porque el CPI obtenido (0.88) es menor a 1.0, es decir, el proyecto está gastando más de lo planeado por unidad de trabajo, así que se proyecta un costo final mayor al presupuesto original.
9. **¿Qué fórmula es el BAC?** Respuesta: BAC = Σ PV de todas las actividades del proyecto (el presupuesto total aprobado, parte de la Línea base).
10. **Si CV = 0 y SV = 0 a una fecha de estado, ¿qué se puede concluir?** Respuesta: el proyecto está exactamente alineado con la Línea base tanto en costo como en avance a esa fecha (caso ideal).
