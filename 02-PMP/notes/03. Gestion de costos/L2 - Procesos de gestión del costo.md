---
title: L2 — Procesos de gestión del costo
curso: PMP
modulo: 03. Gestion de costos
leccion: L2
fuente: "[[documentation/03. Gestion de costos/Procesos para gestionar costos en el proyecto.pdf|Procesos para gestionar costos en el proyecto]]"
complementos: [Procesos para la gestión del costo (2).pdf, La estimación, presupuestación y control de costos en mi proyecto.pdf]
status: por-estudiar
tags: [pmp, costos, procesos, evm]
---

# L2 — Procesos de gestión del costo

## Resumen

Este bloque desarrolla en detalle los **4 procesos del área de conocimiento Gestión del costo**, siguiendo el enfoque de entradas → herramientas y técnicas → salidas (ITTOs) de la *Guía práctica: Grupos de procesos* del PMI: **1) Planear la administración del costo**, **2) Estimar los costos**, **3) Determinar el presupuesto** y **4) Controlar los costos**. Continúa con el caso práctico completo de un proyecto de **construcción residencial** (Carlos y María), que aplica los 4 procesos con cifras reales: estimación por técnicas (analogía, paramétrica, ascendente, tres puntos), cálculo de reservas de contingencia y de administración, presupuesto total, flujo de caja mensual con curva "S", y finalmente las **métricas de Valor Ganado (EVM)** completas con su interpretación.

## Conceptos clave (con definiciones completas)

- **Planear la administración del costo**: proceso en el que se establecen las políticas, procedimientos y documentación para planear, administrar, ejecutar y controlar los costos del proyecto.
- **Estimar los costos**: proceso en el que se desarrolla una aproximación de los costos de los recursos necesarios para completar las actividades del proyecto.
- **Determinar el presupuesto**: proceso en el que se suman los costos estimados de actividades individuales o paquetes de trabajo a fin de establecer una línea base de costo.
- **Controlar los costos**: proceso en el que se compara la línea base de costo contra lo que realmente se va gastando en la ejecución del proyecto, para influir sobre los factores que crean variaciones de costo y controlar los cambios en el presupuesto.
- **Línea base de costo**: el presupuesto final aprobado, listo para aplicarse en la ejecución (no incluye la reserva de gestión/administración).
- **BAC (Budget at Completion)**: presupuesto planeado total, es decir, la línea base de costo.
- **SV (Schedule Variance)**: variación del cronograma; si es negativa hay atraso (menos trabajo del planeado).
- **SPI (Schedule Performance Index)**: índice de desempeño en programa; si es menor a 1, significa atraso.
- **CV (Cost Variance)**: variación de costo; si es positiva, se está gastando menos de lo planeado.
- **CPI (Cost Performance Index)**: índice de desempeño en costo; si es mayor a 1, significa que el proyecto es eficiente en el uso de recursos.
- **EAC (Estimate at Completion)**: costo estimado a la terminación del proyecto.
- **VAC (Variance at Completion)**: cantidad por debajo (o encima) de lo presupuestado al finalizar el proyecto.
- **TCPI (To-Complete Performance Index)**: tasa de rendimiento que se debe implementar en lo que resta del proyecto para regresar al presupuesto original (BAC).
- **Reserva de contingencia**: monto adicional (en el caso práctico, 10 % de los costos directos de cada actividad) para cubrir riesgos identificados dentro del alcance del proyecto; forma parte de la línea base de costo.
- **Reserva de administración (o de gestión)**: monto adicional (en el caso práctico, 20 % de la línea base de costo) para cubrir trabajo no previsto dentro del alcance del proyecto; **no** forma parte de la línea base de costo, pero sí del presupuesto total del proyecto.
- **Curva "S"**: representación gráfica del flujo de caja acumulado de un proyecto a lo largo del tiempo, con forma de "S".

## Desarrollo del contenido

### 0. Contexto: High Tech Products y el enfoque de procesos del PMI

El PMO de High Tech Products (HTP) — empresa que solo logra terminar 2 o 3 proyectos cumpliendo el presupuesto asignado originalmente, debido a sobrecostos y demoras — investiga las mejores prácticas de la **"Guía práctica: Grupos de procesos"** del PMI para gestionar efectivamente los costos.

El PMI ha utilizado por años un enfoque basado en procesos (ver *PMBOK Guide*), que integra las buenas prácticas comúnmente aceptadas en dirección de proyectos. El **ciclo de vida del proyecto** se maneja mediante los **5 grupos de procesos**: Iniciación, Planificación, Ejecución, Monitoreo y control, Cierre — en total se identifican **49 procesos diferentes**, cada uno con entradas, herramientas/técnicas y salidas (ITTOs), donde las salidas de un proceso pueden ser entradas de otros procesos interrelacionados. La cantidad y aplicabilidad de procesos depende del tipo de proyecto y de las políticas/procedimientos de la organización.

Del total de 49 procesos, **4 corresponden al área de Gestión del costo**:
- **Planear la administración del costo** (grupo Planificación)
- **Estimar los costos** (grupo Planificación)
- **Determinar el presupuesto** (grupo Planificación)
- **Controlar los costos** (grupo Monitoreo y control)

### 1. Planear la administración del costo

Proceso en el que se establecen las políticas, procedimientos y documentación para planear, administrar, ejecutar y controlar los costos del proyecto.

**Entradas:**
- Acta de constitución del proyecto.
- Plan de gestión del proyecto (en específico, el plan de gestión de cronograma y el plan de riesgos).
- Factores ambientales-empresariales.
- Activos de los procesos organizacionales (políticas y procedimientos de la organización).

**Técnicas y herramientas:**
- Juicio de expertos.
- Análisis de datos.
- Reuniones.

**Salidas:**
- **Plan de gestión del costo.**

### 2. Estimar los costos

Se desarrolla una aproximación de los costos de los recursos necesarios para completar las actividades del proyecto.

**Entradas:**
- Los planes que definen estrategias y acciones en cada área crítica del proyecto (deben actualizarse constantemente). La entrada más importante es el **plan de gestión del proyecto**, que debe incluir planes específicos para gestión del costo, calidad y línea base del alcance.
- **Registro de lecciones aprendidas, registro de riesgos, cronograma del proyecto, lista de requerimientos** y otros factores ambientales.
- Activos organizacionales relevantes.

**Técnicas y herramientas:**
- **Técnicas de estimación**: análoga, paramétrica, ascendente o definitiva, y la estimación de tres puntos.
- Análisis de datos.
- Sistemas de información para la administración del proyecto.
- Técnicas para la toma de decisiones.

**Salidas:**
- Estimados de costos.
- Bases de estimación.
- Actualizaciones a documentos del proyecto: bitácora de asunciones, registro de lecciones aprendidas, registro de riesgos.

### 3. Determinar el presupuesto

Aquí se suman los costos estimados de actividades individuales o paquetes de trabajo a fin de establecer una **línea base de costo**.

**Entradas:**
1. Plan de gestión del proyecto (plan de gestión del costo, plan de gestión de los recursos, línea base de alcance).
2. Documentos del proyecto (bases de estimación, estimados de costo, cronograma del proyecto).
3. Documentos del negocio (caso de negocios, plan de gestión de beneficios).
4. Acuerdos contractuales.
5. Factores ambientales.
6. Activos de los procesos organizacionales.

**Técnicas y herramientas:**
1. Juicio de expertos.
2. Técnica de agregación del costo.
3. Análisis de alternativas / análisis de reservas.
4. Revisión de información histórica.
5. Reconciliación de los límites de flujo de caja.
6. Análisis del financiamiento al proyecto.

**Salidas:**
1. **Línea base de costo** (p. ej., el presupuesto finalmente aprobado y listo para aplicar en la ejecución).
2. Requerimientos de fondeo del proyecto.
3. Actualizaciones a documentos del proyecto: estimaciones de costos, registro de riesgos.

### 4. Controlar los costos

Se compara la línea base de costo contra lo que realmente se va gastando en la ejecución del proyecto, para influir sobre los factores que crean variaciones de costo y controlar los cambios en el presupuesto.

**Entradas:**
1. Plan de gestión del proyecto (plan de gestión del costo, línea base de costo, línea base de medición del desempeño).
2. Documentos del proyecto (registro de lecciones aprendidas).
3. Requerimientos de fondeo del proyecto.
4. Datos del desempeño del trabajo (avance y gasto a fechas de revisión de avance).
5. Activos de los procesos organizacionales.

**Técnicas y herramientas:**
1. Juicio de expertos.
2. Análisis de datos: **análisis de valor ganado** (para medir variación de estatus, calcular pronóstico de terminación y el TCPI), análisis de variación, análisis de tendencias, análisis de reservas.
3. Índice de desempeño para completar el proyecto (TCPI).
4. Sistema de información de la administración del proyecto (software).

**Salidas:**
1. Información del desempeño del trabajo (reportes de estado y progreso).
2. Pronóstico de costos (reportes de tendencia y pronóstico de terminación).
3. Solicitud de cambios.
4. Actualizaciones al plan de administración del proyecto (plan de administración del costo, línea base de costo, línea base de medición del desempeño).
5. Actualizaciones a documentos del proyecto (bitácora de asunciones, estimados de costo, registro de lecciones aprendidas, registro de riesgos).

## Ejemplos y casos del material

### Caso práctico integral: construcción residencial de Carlos y María

El curso desarrolla un caso completo de estimación, presupuestación y control de costos en la construcción de una casa (proyecto "Carlos y María"), organizado en 4 misiones con ejercicios y retroalimentación numérica:

**Misión 1 — Recolección de datos e información base**: se identifican actividades del proyecto (desarrollo de contrato, firma, financiamiento, permisos, construcción, plomería, electricidad, acabados, inspección, entrega) con sus costos directos y duraciones.

**Misión 2 — Técnicas de estimación aplicadas por actividad**, con su rango de precisión característico:

| Técnica | Rango de precisión típico | Aplicación en el caso |
|---|---|---|
| Estimación por analogía | -25 % a +75 % | Actividades con poca información detallada |
| Estimación paramétrica | -10 % a +25 % | Actividades con relación cuantitativa conocida (costo por unidad) |
| Estimación ascendente (bottom-up) | -5 % a +10 % | Actividades bien definidas y desglosadas |
| Estimación de tres puntos (PERT) | No aplica un rango fijo — se calcula con optimista/pesimista/más probable | Actividades con incertidumbre significativa |

**Misión 3 — Presupuestación**: cálculo de la **reserva de contingencia** (10 % de los costos directos de cada actividad) y elaboración del **resumen de costos** del proyecto:

| Concepto | Cantidad |
|---|---|
| 1. Costos directos (recursos asignados en las actividades) | $795,200 |
| 2. Gastos indirectos ($1,000/día × 133 días) | $133,000 |
| 3. Reserva para contingencias (10 % de costos directos) | $79,520 |
| 4. Subtotal (Línea base de costo) | $1,007,720 |
| 5. Reserva de la administración (20 % de la línea base de costo) | $201,544 |
| 6. **Presupuesto total del proyecto** | **$1,209,264** |

Ejercicio de flujo de caja mensual y acumulado (Misión 3, Ejercicio 2) — cronograma de desembolsos por actividad de enero a julio de 2024, con **flujo mensual** y **flujo acumulado** graficados como **curva "S"** (el flujo acumulado va de $101,936 en enero hasta $1,007,720 (línea base) en julio).

**Misión 4 — Control de costos (EVM)**:
- Ejercicio 1: cálculo del **% de avance planeado** y **costo planeado** por actividad a la fecha de corte, más gastos indirectos incurridos (43 días × $1,000/día = $43,000). Total de costo planeado a la fecha: $128,128.
- Ejercicio 2 — **tabla completa de métricas de Valor Ganado** con interpretación:

| Métrica | Resultado | Interpretación |
|---|---|---|
| BAC | $1,007,720 | Presupuesto planeado total, es decir, la línea base de costo. |
| SV | -$28,001 | Hay un atraso en el proyecto (menos trabajo de lo planeado). |
| %SV | -16 % | Porcentaje de atraso. |
| SPI | 0.84 | Índice de desempeño en programa; menor a 1 = atraso. |
| CV | $8,126 | Se está gastando menos de lo planeado. |
| %CV | 6 % | Porcentaje de gasto por debajo del trabajo realizado. |
| CPI | 1.06 | Índice de desempeño en costo; mayor a 1 = eficiente. |
| EAC | $950,504 | Costo estimado a la terminación, menor a lo planeado. |
| VAC | $57,215 | Cantidad por debajo de lo presupuestado al finalizar. |
| TCPI | 0.99 | Tasa de rendimiento a implementar en lo que resta del proyecto para volver al BAC. |

**Lectura combinada del caso**: el proyecto está **atrasado en cronograma** (SPI 0.84, SV negativo) pero es **eficiente en costo** (CPI 1.06, CV positivo) — un patrón real y común: ir lento pero gastando menos de lo presupuestado a la fecha, con proyección de terminar por debajo del presupuesto total (EAC < BAC, VAC positivo).

## Conexión con APL/PIDA

- La secuencia de 4 procesos (planear → estimar → presupuestar → controlar) es exactamente el ciclo que Carlos aplicó de facto en PIDA: el "Plan Trabajo" y el Golden Cluster funcionaron como línea base de costo/alcance, y el seguimiento semanal (documento vivo `2 Seguimiento_...xlsx`) cumplió el rol de "Controlar los costos" con datos de desempeño del trabajo.
- El re-trabajo técnico medido en horas-hombre (**−11.9 %** de reducción, documento vivo `Retrabajo técnico.xlsx`) es un ejemplo directo de **CV/CPI** aplicado a esfuerzo en vez de dinero: reducir horas de re-trabajo mejora la eficiencia de costo igual que un CPI > 1 en este caso práctico.
- El FTR 96 % con aceptación desplazada a W9 en PIDA es análogo al patrón SPI < 1 / CPI > 1 del caso de Carlos y María: buen desempeño de calidad y costo, pero atraso de cronograma por un desfase estructural (integración→aceptación) — la misma disociación entre eficiencia de costo y cumplimiento de plazo que documentan las métricas EVM de este bloque.

## Preguntas de repaso tipo quiz

1. **P:** ¿Cuáles son los 4 procesos de la Gestión del costo y en qué grupos de procesos se ubican?
   **R:** Planear la administración del costo, Estimar los costos y Determinar el presupuesto (grupo Planificación); Controlar los costos (grupo Monitoreo y control).

2. **P:** ¿Cuál es la salida principal del proceso "Planear la administración del costo"?
   **R:** El Plan de gestión del costo.

3. **P:** ¿Cuál es la salida principal del proceso "Determinar el presupuesto"?
   **R:** La línea base de costo (además de los requerimientos de fondeo del proyecto y actualizaciones a documentos).

4. **P:** En el caso de Carlos y María, si los costos directos son $795,200 y la reserva de contingencia es 10 % de estos, ¿cuánto es la reserva de contingencia?
   **R:** $79,520.

5. **P:** ¿Qué diferencia hay entre la línea base de costo y el presupuesto total del proyecto?
   **R:** La línea base de costo = costos directos + gastos indirectos + reserva de contingencia (subtotal, $1,007,720 en el caso). El presupuesto total del proyecto = línea base de costo + reserva de administración ($1,209,264 en el caso).

6. **P:** En la tabla de métricas EVM del caso, el SPI es 0.84 y el CPI es 1.06. ¿Qué significa esto en conjunto?
   **R:** El proyecto está atrasado en cronograma (SPI < 1) pero es eficiente en el uso del presupuesto (CPI > 1) — va lento pero gastando menos de lo planeado.

7. **P:** ¿Qué mide el TCPI y qué significa un valor de 0.99?
   **R:** El TCPI (To-Complete Performance Index) mide la tasa de rendimiento que debe implementarse en el resto del proyecto para completar dentro del presupuesto original (BAC). Un valor de 0.99 significa que se requiere un desempeño ligeramente menor al 100 % de eficiencia para lograrlo (viable, cercano a lo normal).

8. **P:** ¿Cuál de las 4 técnicas de estimación de costos tiene el rango de precisión más amplio (-25 % a +75 %)?
   **R:** La estimación por analogía.

9. **P:** ¿Qué representa la "curva S" en la gestión de costos?
   **R:** La representación gráfica del flujo de caja acumulado del proyecto a lo largo del tiempo.

10. **P:** ¿Qué distingue a la reserva de contingencia de la reserva de administración (gestión)?
    **R:** La reserva de contingencia cubre riesgos identificados dentro del alcance del proyecto y sí forma parte de la línea base de costo; la reserva de administración cubre trabajo no previsto dentro del alcance y no forma parte de la línea base de costo, pero sí del presupuesto total del proyecto.
