---
title: L2 — Panorama general de la gestión del tiempo y los recursos
curso: PMP
modulo: 01. Gestión del Tiempo y Recursos
leccion: L2
fuente: "[[documentation/01. Gestión del Tiempo y Recursos/PMP_SC1.1_Versión impresa_L2.pdf|Versión impresa L2]]"
status: por-estudiar
tags: [pmp, tiempo-recursos]
---

# L2 — Panorama general de la gestión del tiempo y los recursos

## Resumen (5-8 líneas)
Los proyectos existen para entregar valor agregado a las áreas de la empresa, y para lograrlo hay que desarrollarlos en tiempo y forma: cumplir tiempos de inicio y fin, respetar hitos, seguir la secuencia adecuada y optimizar los recursos. Todo proyecto, sin importar la industria, pasa por los grupos de procesos del ciclo de vida (inicio, planificación, ejecución, monitoreo y control, cierre), esquema propuesto por el PMI en el PMBOK y alineado con ISO, ANSI e IEEE. La lección define la estructura de descomposición del trabajo (EDT/WBS) — proyecto → fases → etapas → actividades — y los términos base de tiempo y recursos: duración, hitos, recursos, estimación, secuencia, diagrama de red, PDM, cronograma (Gantt), ruta crítica y EVM/SPI. Cierra con los 6 procesos recomendados para gestionar tiempos y recursos, desde desglosar actividades hasta elaborar el cronograma.

## Conceptos clave
- **Grupos de procesos**: cubren todo el ciclo de vida del proyecto — inicio, planificación, ejecución, monitoreo y control, cierre. Esquema del **PMI (PMBOK)**, aceptado y alineado con ISO, ANSI, IEEE.
- **EDT (WBS)**: descomposición de *todo el trabajo necesario y sólo el trabajo necesario* para completar el proyecto. Niveles: proyecto → fases → etapas → actividades.
  - **Fase**: conjunto de etapas/paquetes de trabajo relacionados por un área técnica común o un entregable parcial o final. Código de 2 dígitos (1.1, 1.2, 1.3).
  - **Etapa** (paquete de trabajo): conjunto de actividades relacionadas para finalizar un trabajo específico. 3er nivel de la EDT, código de 3 dígitos (1.1.3, 1.2.1).
  - **Actividad**: acción de intervención para alcanzar un objetivo específico parcial. Nivel más bajo de la EDT; ya no se puede desglosar más y la realiza una misma persona/grupo en un mismo momento con los mismos recursos. Código de 4 dígitos (1.1.3.1).
- **Duración de las actividades**: cantidad de unidades de tiempo (horas, días, semanas) que consume una actividad. Los tiempos se calculan siempre a nivel de actividades; los de etapas/fases son el agregado hacia arriba de la EDT.
- **Hitos**: eventos que marcan un cambio, inicio o fin de etapa/fase. Pueden o no asociarse a un entregable. **No consumen recursos: duración cero y costo cero.**
- **Recursos de las actividades**: todo tipo de recursos necesarios — financieros, humanos, materiales, técnicos.
- **Estimación**: cálculo de la magnitud esperada de una variable futura (tiempo, costo, recursos); la cantidad con mayor probabilidad de ocurrir según el comportamiento previo y la información disponible.
- **Secuencia**: orden en que se deben/pueden realizar las actividades.
- **Diagrama de Red**: gráfico de bloques que representa todas las actividades e indica su orden a lo largo del ciclo de vida.
- **PDM (Precedence Diagramming Method)**: método común para dibujar el diagrama de red — bloques unidos por flechas que indican el flujo; identifica todas las rutas posibles del hito de inicio al hito de fin.
- **Cronograma / Diagrama de Gantt**: gráfico de barras con actividades, duraciones y recursos sobre una escala de tiempo, unidas con flechas de secuencia.
- **Ruta crítica**: la ruta de mayor duración entre inicio y fin; si una de sus actividades se retrasa, todo el proyecto se retrasa.
- **EVM (Earned Value Management)**: técnica analítica de indicadores de desempeño; el más relevante para tiempos es el **SPI (Schedule Performance Index)**. Sirve para monitorear y controlar el desempeño a lo largo del ciclo de vida.

## Técnicas / fórmulas / procesos
Los **6 procesos del área de gestión del tiempo y los recursos** (en orden; duración y recursos se estiman en paralelo e interactúan):

1. **Desglosar las actividades**: llegar al nivel más bajo del WBS y definir las actividades específicas.
2. **Secuenciar las actividades**: según características operativas, técnicas, restricciones y relaciones, identificar el orden para obtener los productos en el menor tiempo posible.
3. **Estimar la duración de las actividades**: con base en conocimiento previo, experiencia y documentación de actividades iguales o similares. A más información disponible, estimación más cercana a la realidad.
4. **Estimar los recursos de las actividades**: la disponibilidad de recursos (humanos, financieros, materiales, equipo, técnicos) es una de las restricciones que más influye; puede condicionar la duración o viceversa — cualquier variación en uno provoca cambios en el otro.
5. **Calcular la Ruta Crítica (CPM — Critical Path Method)**: calcula la duración total, identifica todas las rutas, las actividades críticas (sin margen de retraso) y las holguras de las no críticas → puntos de flexibilidad del cronograma.
6. **Elaborar el Cronograma**: concentrar toda la información en un software (MS Project, WBS Schedule Pro, ProjectLibre) y generar el diagrama de Gantt.

## Aplicación práctica
- El PDF presenta el trabajo del proyecto en **forma tabular y gráfica** (EDT con códigos 1.1 / 1.1.3 / 1.1.3.1) y advierte que ni la tabla ni el gráfico contienen aún duraciones ni recursos — esos se agregan con los procesos de estimación.
- Ejemplo de duraciones por etapas: las relaciones temporales y de secuencia entre etapas se deben respetar durante la ejecución para terminar en tiempo y forma.
- Preguntas de reflexión del curso: ¿cómo estimas duraciones y asignas recursos hoy?, ¿qué herramienta usas?, ¿un análisis de ruta crítica habría evitado contratiempos pasados?

## Conexión con APL/PIDA
- En el [[README|proyecto PIDA]] Carlos ya vivió esto: el Plan de Trabajo de 12 semanas es un Gantt real con actividades secuenciadas (setup W1 → integración W2-W7 → aceptación W3-W8 → cierre), hitos duros (1-jul Entrega de avance, 11-ago Reporte PIDA) y recursos asignados (3 integradores, 3 optimizadores, cuadrillas).
- La "integración del golden cluster en W2" funcionó como actividad de ruta crítica: su validación en W3 condicionaba escalar los 20 sitios restantes — un retraso ahí retrasaba todo el despliegue.
- La estimación por información disponible conecta con lo aprendido en el [[Index-APL|curso APL]]: el burndown y las métricas (FTR, re-trabajo) son el equivalente ágil del monitoreo tipo EVM/SPI.

## Preguntas de repaso
1. **¿Qué es la EDT y cuál es su regla de oro?** La descomposición de todo el trabajo necesario y sólo el necesario para completar el proyecto; niveles proyecto → fases → etapas → actividades.
2. **¿Cuánto duran y cuestan los hitos?** Cero: no consumen recursos de ningún tipo, duración de cero días y costo cero.
3. **¿A qué nivel de la EDT se calculan los tiempos?** Siempre a nivel de actividades; etapas y fases agregan las duraciones hacia arriba.
4. **¿Qué es la ruta crítica y por qué importa?** La ruta de mayor duración del diagrama de red/Gantt; si cualquiera de sus actividades se retrasa, se retrasa todo el proyecto.
5. **¿Qué indicador de EVM mide el desempeño del cronograma?** El SPI (Schedule Performance Index).
6. **¿Cómo interactúan la estimación de duraciones y la de recursos?** Íntimamente: la disponibilidad de recursos puede definir la duración o viceversa; variar uno cambia el otro.
