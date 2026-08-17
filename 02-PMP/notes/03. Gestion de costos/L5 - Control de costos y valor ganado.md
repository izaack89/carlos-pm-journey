---
title: Control de costos y valor ganado
curso: PMP
modulo: 03. Gestion de costos
leccion: L5
fuente: "[[documentation/03. Gestion de costos/Control de costos.pdf|Control de costos]]"
complementos: ["Métricas del estado de proyecto en costo.pdf", "Métricas de desempeño y software de monitoreo.pdf", "Tasa de rendimiento para corregir el desempeño del proyecto.pdf"]
status: por-estudiar
tags: [pmp, costos, evm]
---

# Control de costos y valor ganado

## Resumen

Durante la ejecución surgen desafíos inesperados (retrasos de materiales, cambios en costos). La técnica de **valor ganado** (*Earned Value Management*, EVM; el material también la llama "técnica del valor agregado") permite anticiparse determinando **tres análisis fundamentales**:

1. **Estado del proyecto** a una fecha determinada de revisión del avance (**fecha de estado**): ¿va a tiempo, atrasado o adelantado? ¿gasta lo debido, más o menos que el valor del trabajo realizado? → métricas CV, %CV, CPI, SV, %SV, SPI.
2. **Pronóstico** de qué sucedería si se sigue con los mismos rendimientos: costo estimado de finalización (EAC), costo restante (ETC), variación a la terminación (VAC) y duración estimada (EACt).
3. **Corrección** necesaria para regresar al presupuesto original o línea base de costo: tasa de rendimiento requerida **TCPI**.

Si no se toman en cuenta estos tres aspectos, lo más probable es que el proyecto no termine bien.

## Conceptos clave (con definiciones completas)

- **Fecha de estado**: fecha determinada de revisión del avance sobre la cual se calculan todas las métricas. En la gráfica de curva "S" es la línea vertical sobre la que se leen PV, EV y AC.
- **PV — Valor Planeado** (*Planned Value*): lo que se debería llevar gastado según la línea base a la fecha de estado. También llamado **Costo Presupuestado del Trabajo Programado (CPTP)** o *Budget Cost of Work Schedule* (**BCWS**). Se lee sobre la curva "S" (línea base de costo).
- **EV — Valor Ganado** (*Earned Value*): valor (a costo presupuestado) del trabajo **realmente realizado** a la fecha de estado. También **Costo Presupuestado del Trabajo Realizado (CPTR)** o *Budget Cost of Work Performed* (**BCWP**). Se calcula en función del % de avance físico reportado.
- **AC — Gasto real** (*Actual Cost*): lo realmente gastado en el trabajo realizado a la fecha de estado. También **Costo Real del Trabajo Realizado (CRTR)** o *Actual Cost of Work Performed* (**ACWP**).
- **Situación ideal**: **PV = EV = AC** (el trabajo planeado es el realizado y el gasto real es igual a ambos). Si EV < PV se hace menos trabajo del planeado; si AC > EV se gasta más de lo que vale el trabajo realizado.
- **BAC** (*Budget At Completion*): presupuesto total planeado del proyecto a la terminación (valor final de la línea base de costo).
- **PD**: duración planeada del proyecto.
- **EAC** (*Estimate At Completion*): costo estimado del proyecto a la terminación, según el rendimiento real.
- **ETC** (*Estimate To Complete*): costo estimado que falta por gastar para terminar el proyecto.
- **VAC** (*Variance At Completion*): variación de costo a la terminación (entre el presupuesto original y el nuevo costo de finalización).
- **EACt**: estimación de la duración del proyecto al finalizar (nueva duración prevista).
- **TCPI** (*To Complete Performance Index*): tasa de rendimiento en costo a la que se debe trabajar en el tiempo restante (después de la última revisión) para regresar a la línea base de costo.

## Desarrollo del contenido

### Tabla completa de fórmulas EVM

| Métrica | Fórmula | Interpretación |
|---|---|---|
| Variación de costo | **CV = EV − AC** | CV = 0 gastas lo debido · **CV > 0 (+) debajo del costo** (gastas menos de lo que vale el trabajo) · **CV < 0 (−) sobrecosto** |
| % de variación de costo | **%CV = CV/EV × 100** | % de sobrecosto o de ahorro |
| Índice de desempeño en costo | **CPI = EV/AC** | **CPI = 1** eficiencia adecuada · **CPI > 1 alto rendimiento financiero (debajo del costo)** · **CPI < 1 bajo rendimiento (sobrecosto: gastas más de lo debido)** |
| Variación de programa | **SV = EV − PV** | SV = 0 a tiempo · **SV > 0 (+) adelantado** · **SV < 0 (−) atrasado** |
| % de variación de programa | **%SV = SV/PV** (×100) | % de adelanto o atraso |
| Índice de desempeño en programa | **SPI = EV/PV** | **SPI = 1** a tiempo · **SPI > 1 avance rápido (adelanto)** · **SPI < 1 avance lento (atraso)** |
| Costo estimado al finalizar | **EAC = BAC/CPI** | Nuevo cálculo del costo total del proyecto basado en el rendimiento real |
| Costo estimado para finalizar | **ETC = EAC − AC** | Cálculo del costo para completar el trabajo restante |
| Variación de costo a la finalización | **VAC = BAC − EAC** | Variación entre el presupuesto original y el nuevo costo de finalización (negativa = sobrecosto final) |
| Duración estimada al finalizar | **EACt = PD/SPI** | Nueva duración de previsión total (PD = duración planeada) |
| Índice de desempeño a la conclusión | **TCPI = (BAC − EV)/(BAC − AC)** | Rendimiento requerido en lo que resta para terminar en el BAC |

**Regla mnemotécnica**: las variaciones y los índices SIEMPRE empiezan con EV. Variación = resta (EV −), índice = división (EV /). "C" de costo empareja con **AC**; "S" de *schedule* empareja con **PV**. Negativo/menor que 1 = malo; positivo/mayor que 1 = bueno (excepto TCPI, donde >1 = hay que apretar).

### Interpretación del TCPI (ojo: se invierte)

- **TCPI = 1**: mantener el rendimiento en costo actual para terminar en el BAC planeado.
- **TCPI > 1**: hay que **aumentar** el rendimiento (eficiencia financiera) para regresar al presupuesto. Ej. del material: TCPI = 1.3 → trabajar al 130 %, es decir **recortar gastos en 30 %**: lo que antes se hacía con $100 ahora debe hacerse con $70. De lo contrario, EAC > BAC.
- **TCPI < 1**: se puede **bajar** el desempeño financiero. Ej.: TCPI = 0.70 → eficiencia al 70 %, se pueden **aumentar gastos en 30 %** (abrir flujo de caja para pagar cuentas detenidas). De lo contrario se terminará con EAC < BAC.

### Lectura gráfica (curva "S" y fecha de estado)

Sobre la línea vertical de la **fecha de estado** se ubican: **PV** en la curva "S" de línea base, **EV** en la curva de valor ganado (avance) y **AC** en la curva de gasto real. La curva punteada posterior a la fecha de estado es la **proyección del gasto real**: si el rendimiento se mantiene, el proyecto termina en **EAC** (por encima del BAC → usar reservas de administración; VAC = distancia EAC-BAC; ETC = distancia EAC-AC) y con duración **EACt** mayor a la **PD**.

### Software de monitoreo y control

- La técnica de valor ganado se aplica con software especializado; el más común es **Microsoft Project**, que aplica las mismas fórmulas y genera reportes: cronograma de seguimiento (Gantt con % complete y Actual Cost por actividad), tabla de métricas EVM (PV/BCWS, EV/BCWP, AC, CV, %CV, CPI, SV, %SV, SPI, BAC, EAC, VAC, TCPI), gráfica de **cash flow** (barras por semana + curva de costo acumulado) y gráfica de tendencia de **SPI y CPI** por semana.
- Ejemplo ilustrado del material: proyecto de 8 semanas, avance programado 33 % a fin de la semana 3, AC = $200,000, con métricas a nivel proyecto PV = $104,000, EV = $116,000, CV = −$84,000 (−72 %), CPI = 0.58, SV = $12,000 (12 %), SPI = 1.12, BAC = $316,000, EAC = $544,828, VAC = −$228,828, TCPI = 1.72 (adelantado en programa pero con fuerte sobrecosto).
- Reflexión del material: distinguir **avance físico** (trabajo ensamblado/realizado → alimenta EV) de **avance financiero** (dinero gastado → AC).

## Ejemplos numéricos del material (paso a paso)

### Ejemplo 1 — Proyecto de 8 semanas, BAC $400,000 (fecha de estado: semana 3)

Datos: PD = 8 semanas, BAC = $400,000. A la semana 3: **PV = $120,000, EV = $90,000, AC = $130,000**.

**Estado en costo:**
- CV = EV − AC = 90,000 − 130,000 = **−40,000** (sobrecosto)
- %CV = CV/EV = −40,000/90,000 = **−44 %** (de sobrecosto)
- CPI = EV/AC = 90,000/130,000 = **0.69** (índice bajo)

**Estado en programa:**
- SV = EV − PV = 90,000 − 120,000 = **−30,000** (atraso)
- %SV = SV/PV = −30,000/120,000 = **−25 %** (de atraso)
- SPI = EV/PV = 90,000/120,000 = **0.75** (desempeño lento)

Conclusión: a la semana 3 el proyecto lleva **25 % de atraso y 44 % de sobrecosto** → tomar acciones correctivas.

**Pronóstico (si no se corrige):**
- EAC = BAC/CPI = 400,000/0.69 = **$579,710**
  *(Nota: el PDF titula la fórmula EAC = BAC/CPI pero en el cálculo sustituye 0.69, el CPI, aunque el texto dice "/SPI" — errata del material; el valor correcto usa CPI.)*
- ETC = EAC − AC = 579,710 − 130,000 = **$449,710** *(el PDF imprime "57,971 − 130,000 = −72,029", errata evidente de dedazo; concepto: lo que falta por gastar = EAC − AC).*
- VAC = BAC − EAC = 400,000 − 579,710 = **−$179,710** (sobrecosto final)
- EACt = PD/SPI = 8/0.75 = **10.67 semanas** (en lugar de 8)

**Corrección (TCPI):**
- TCPI = (BAC − EV)/(BAC − AC) = (400,000 − 90,000)/(400,000 − 130,000) = 310,000/270,000 = **1.15**
- Interpretación: aumentar el rendimiento financiero al **115 %** a partir de la semana 4, es decir **recortar gastos 15 %** en lo que resta, para regresar al presupuesto de $400,000.

### Ejemplo 2 — Las 4 paredes (fecha de estado: semana 2)

Planteamiento: construir 4 paredes secuenciales (A→B→C→D), sin traslapes; cada pared cuesta **$1,000** y toma **1 semana** (5 días hábiles). Por tanto **BAC = $4,000** y **PD = 4 semanas**.

Al final de la semana 2:
- Pared A: 100 % concluida, gasto real $1,200.
- Pared B: 20 % de avance, gasto real $400.

**Determinación de las variables:**
- **PV** = valor de las 2 paredes que deberían estar construidas = 2 × $1,000 = **$2,000**.
- **EV** = 100 % de A ($1,000) + 20 % de B ($200) = **$1,200**.
- **AC** = $1,200 + $400 = **$1,600**.

**Estado en costo:**
- CV = 1,200 − 1,600 = **−400** (sobrecosto)
- %CV = −400/1,200 = **−33.33 %**
- CPI = 1,200/1,600 = **0.75** (bajo)

**Estado en programa:**
- SV = 1,200 − 2,000 = **−800** (atraso)
- %SV = −800/2,000 = **−40 %**
- SPI = 1,200/2,000 = **0.60** (lento)

Conclusión: a la semana 2, **40 % de atraso y 33 % de sobrecosto** → acciones correctivas.

**Pronóstico:**
- EAC = BAC/CPI = 4,000/0.75 = **$5,333** (costo de las 4 paredes si no se corrige el desempeño)
- ETC = EAC − AC = 5,333 − 1,600 = **$3,733** *(el PDF lo imprime con signo negativo "−3,733"; es el monto que falta por gastar).*
- VAC = BAC − EAC = 4,000 − 5,333 = **−1,333** (sobrecosto final)
- EACt = PD/SPI = 4/0.60 = **6.7 semanas** (vs. 4 planeadas → atraso general de 2.7 semanas)

**Corrección:**
- TCPI = (4,000 − 1,200)/(4,000 − 1,600) = 2,800/2,400 = **1.17**
- Interpretación: eficiencia financiera al **117 %** en las 2 semanas restantes → **recortar gastos 17 %**: lo que antes se hacía con $100, ahora con $87, para intentar regresar al presupuesto de $4,000.

## Conexión con APL/PIDA

- El seguimiento semanal W1-W9 del PIDA (fechas de corte como el 30-jun/W4 con 7/23 sitios aceptados) es exactamente el mecanismo de "fecha de estado" del EVM: el burndown de sitios aceptados hace el papel de curva EV frente a la curva planeada (PV); el desfase integración→aceptación que corrió el cierre a W9 es un SPI < 1 detectado a tiempo.
- Métricas PIDA como FTR ≥90 % y re-trabajo −10 % son índices de desempeño análogos a CPI/SPI: umbrales contra línea base que disparan acciones correctivas en las retros (W3/W5/W7/W9), igual que un CPI < 1 dispara el análisis de TCPI.

## Preguntas de repaso tipo quiz

1. **¿Cuáles son los tres análisis fundamentales de la técnica de valor ganado?**
   R: (1) Estado del proyecto a la fecha de estado (¿a tiempo/atrasado/adelantado?, ¿gasto correcto o no?), (2) pronóstico si se mantienen los rendimientos (EAC, ETC, VAC, EACt), (3) tasa de rendimiento para corregir y regresar al presupuesto original (TCPI).

2. **Empareja las siglas en español/inglés de PV, EV y AC.**
   R: PV = CPTP = BCWS (Budget Cost of Work Schedule); EV = CPTR = BCWP (Budget Cost of Work Performed); AC = CRTR = ACWP (Actual Cost of Work Performed).

3. **¿Qué indica CV = 0, CV > 0 y CV < 0?**
   R: CV = 0 gastas exactamente lo que debes en el trabajo hecho; CV > 0 gastas menos de lo que vale el trabajo realizado (debajo del costo); CV < 0 sobrecosto.

4. **Un proyecto tiene SPI = 1.12 y CPI = 0.58. ¿Cómo está?**
   R: Adelantado en programa (SPI > 1: avance más rápido de lo planeado) pero con bajo rendimiento en costo (CPI < 1: fuerte sobrecosto). Es el caso del ejemplo de MS Project del material.

5. **¿Qué significa un TCPI de 1.3? ¿Y de 0.70?**
   R: 1.3 → aumentar la eficiencia financiera al 130 % en lo que resta: recortar gastos 30 % (hacer con $70 lo que se hacía con $100). 0.70 → reducir la eficiencia al 70 %: se pueden aumentar gastos en 30 % (abrir el flujo de caja); si no, se terminará con EAC < BAC.

6. **Ejercicio numérico (del material).** PD = 8 semanas, BAC = $400,000; a la semana 3: PV = $120,000, EV = $90,000, AC = $130,000. Calcula CV, %CV, CPI, SV, %SV y SPI.
   R: CV = 90,000−130,000 = **−40,000** (sobrecosto); %CV = −40,000/90,000 = **−44 %**; CPI = 90,000/130,000 = **0.69**; SV = 90,000−120,000 = **−30,000** (atraso); %SV = −30,000/120,000 = **−25 %**; SPI = 90,000/120,000 = **0.75**. Diagnóstico: 25 % de atraso y 44 % de sobrecosto.

7. **Ejercicio numérico (pronóstico).** Con los datos anteriores (CPI = 0.69, SPI = 0.75), calcula EAC, VAC y EACt.
   R: EAC = 400,000/0.69 = **$579,710**; VAC = 400,000 − 579,710 = **−$179,710** (sobrecosto final); EACt = 8/0.75 = **10.67 semanas**. ETC = EAC − AC = 579,710 − 130,000 = **$449,710** por gastar.

8. **Ejercicio numérico (4 paredes).** BAC = $4,000, PD = 4 semanas. Semana 2: pared A 100 % con AC $1,200; pared B 20 % con AC $400. Determina PV, EV, AC y todas las métricas.
   R: PV = **$2,000**; EV = 1,000 + 200 = **$1,200**; AC = **$1,600**. CV = **−400**; %CV = **−33.33 %**; CPI = **0.75**; SV = **−800**; %SV = **−40 %**; SPI = **0.60**. Pronóstico: EAC = 4,000/0.75 = **$5,333**; VAC = **−1,333**; EACt = 4/0.60 = **6.7 semanas**. TCPI = (4,000−1,200)/(4,000−1,600) = **1.17** → recortar gastos 17 % en las 2 semanas restantes.

9. **Ejercicio numérico (TCPI).** BAC = $400,000, EV = $90,000, AC = $130,000. Calcula e interpreta el TCPI.
   R: TCPI = (400,000−90,000)/(400,000−130,000) = 310,000/270,000 = **1.15** → aumentar el rendimiento financiero al 115 % desde la semana 4 (recortar gastos 15 %) para regresar al presupuesto de $400,000.

10. **¿Cuál es la situación ideal entre PV, EV y AC y qué significa?**
    R: **PV = EV = AC**: el trabajo planeado es el mismo que se está realizando y el gasto real es igual al trabajo planeado y realizado. Es la condición que todo responsable de proyecto busca.

11. **¿Con qué se calcula el EV en la práctica: avance físico o financiero?**
    R: Con el **avance físico** (p. ej., % de componentes de la pared ensamblados) valuado a costo presupuestado. El avance financiero (dinero gastado) es el AC. Confundirlos distorsiona todas las métricas.

12. **¿Qué software menciona el material para monitoreo y control con EVM y qué produce?**
    R: **Microsoft Project**: aplica las mismas fórmulas y genera cronograma de seguimiento, tabla EVM (PV, EV, AC, CV, %CV, CPI, SV, %SV, SPI, BAC, EAC, VAC, TCPI), gráfica de flujo de caja con curva "S" y gráfica de tendencia SPI/CPI por semana.
