---
title: L1 — Panorama general
curso: PMP
modulo: 01. Gestión del Tiempo y Recursos
leccion: L1
fuente: "[[documentation/01. Gestión del Tiempo y Recursos/Panorama general de la gestión del tiempo y los recursos.pdf|Panorama general]] · [[documentation/01. Gestión del Tiempo y Recursos/Procesos que componen el área de administración del tiempo y recursos del proyecto.pdf|Procesos del área]]"
status: por-estudiar
tags: [pmp, tiempo-recursos]
---

# L1 — Panorama general de la gestión del tiempo y los recursos

## Resumen (5-8 líneas)
La sociedad del siglo XXI exige resultados más ajustados en tiempo y con mayor inmediatez, por lo que cumplir los tiempos de inicio y fin de cada actividad, respetar los hitos, trabajar con la secuencia y orden adecuados y **optimizar los recursos** se han vuelto procesos centrales de la gestión de proyectos. Todo proyecto —sin importar industria— atraviesa 5 grupos de procesos (Inicio, Planeación, Ejecución, Monitoreo y Control, Cierre), esquema propuesto por el PMI en el PMBoK y alineado con ISO, ANSI e IEEE. Para administrar tiempos y recursos se recomienda una cadena de 6 procesos: desglosar actividades → secuenciar → estimar duraciones y recursos (en paralelo) → calcular la ruta crítica → desarrollar el cronograma. El objetivo del tema es conocer las técnicas, herramientas y mejores prácticas para adaptarlas a los propios proyectos.

## Conceptos clave
- **Resultados**: obtención del producto o productos generados por el proyecto, que deben cumplir especificaciones y restricciones de tiempo, costo, recursos, etc., establecidas incluso antes de que el proyecto inicie.
- **Hitos**: puntos importantes en la ejecución (entregas parciales y finales, revisiones, autorizaciones).
- **Secuencia y orden**: las fases/etapas deben respetar un orden establecido; no respetarlo puede provocar fallas en todo el proyecto (ejemplo: Primaria → Secundaria → Preparatoria → Universidad). Otras actividades pueden ir **en paralelo** (idiomas, cursos, seminarios).
- **Grupos de procesos (5)**: Inicio · Planeación · Ejecución · Monitoreo y Control · Cierre — cubren todo el ciclo de vida y están íntimamente relacionados con el ciclo de mejora continua (Planear-Hacer-Verificar-Actuar).
- **PMBoK (PMI)**: origen del esquema de grupos de procesos, aceptado por ISO, ANSI, IEEE; es el estándar más aceptado globalmente. Su 7ª edición (2021) cambió el enfoque hacia **principios y áreas de dominio**, pero declara que los proyectos no dejan de atravesar los grupos de procesos.
- **EDT/WBS**: estructura de desglose del trabajo; el desglose de actividades implica llegar a su nivel más bajo (actividades específicas, debajo del nivel de etapas o paquetes de trabajo).
- **Ruta crítica (CPM)**: método para calcular la duración total del proyecto e identificar las actividades críticas que no admiten retraso.
- **Holgura**: tiempo de flexibilidad de las actividades que NO están en la ruta crítica; da visión de los puntos de flexibilidad del cronograma.

## Técnicas / fórmulas / procesos

### Los 6 procesos del área de gestión del tiempo y los recursos
1. **Desglosar las actividades** — llegar al nivel más bajo del WBS: definir las actividades específicas con las que se trabajarán todos los demás procesos.
2. **Secuenciar actividades** — según características operativas, técnicas, restricciones y relaciones, identificar el orden: secuencia lineal (unas tras otras) o en paralelo, para obtener los productos en el menor tiempo posible (se modela con el Diagrama de Red).
3. **Estimar la duración de las actividades** — con base en conocimiento previo, experiencia y documentación de actividades similares; a más información disponible, estimación más cercana a la realidad. La duración de etapas = suma de duraciones de sus actividades (respetando secuencias); igual para fases y proyecto.
4. **Estimar los recursos de las actividades** — la disponibilidad de recursos (humanos, financieros, materiales, equipo/maquinaria, técnicos) es una de las restricciones más influyentes; duración y recursos **interactúan íntimamente**: variar uno provoca cambios en el otro.
   *(Los procesos 3 y 4 se ejecutan en paralelo.)*
5. **Calcular la Ruta Crítica (CPM)** — obtener la duración total, identificar todas las rutas posibles, las actividades críticas (sin margen de retraso) y las holguras de las no críticas.
6. **Desarrollar el cronograma** — concentrar toda la información en un software que genera el diagrama de barras en escala de tiempo (cronograma o Diagrama de Gantt). Se recomienda software especializado: Microsoft Project (el más popular), WBS Schedule Pro, o software libre como Project Libre.

### Tres preguntas guía del tema
- ¿Qué significa gestionar adecuadamente los tiempos y recursos de mis proyectos?
- ¿Cuáles procesos recomiendan las metodologías/estándares internacionales como mejores prácticas?
- ¿Cómo puedo adaptar esas mejores prácticas a mis proyectos?

## Aplicación práctica
- **Formación Académica** como proyecto: etapas secuenciales obligatorias (Primaria→Universidad) + actividades paralelas (inglés, francés, futbol, robótica, diplomados).
- **Ejemplos de proyectos y fases** (Fig. 1.2): película (preproducción→producción→postproducción) · software (requerimientos→diseño→codificación→pruebas) · web (preproducción→producción→evaluación→mantenimiento) · sala de emergencias (diagnóstico→tratamiento→evaluación) · casa (cimientos→paredes→techo).
- **Proyecto de construcción** (ejemplo del PDF de procesos): EDT desglosada hasta actividades de la fase Cimientos (preparar terreno: limpiar, sacar desperdicios, nivelar; hacer base: excavar zanjas, preparar materiales, colar hormigón), con hitos de inicio/fin de fase, Gantt (proyecto 28d, Cimientos 10d) y Diagrama de Red con secuencias.

## Conexión con APL/PIDA
- Los 5 grupos de procesos + mejora continua son la versión predictiva de lo que Carlos ya vivió ágilmente en el [[Index-APL|curso APL]]: su despliegue LTE de 23 sitios recorrió Inicio (kickoff W1), Planeación (Plan de Trabajo 12 semanas), Ejecución (W2–W8), Monitoreo y Control (Kanban + burndown + FTR) y Cierre (Reporte PIDA).
- El proceso "secuenciar actividades" (lineal vs paralelo) es exactamente la lógica del Gantt del PIDA: golden cluster primero (W2–W3) y luego despliegue masivo en paralelo con optimización/aceptación (W3–W8).
- Las "actividades críticas sin retraso" del CPM se corresponden con los deadlines duros del PIDA (Entrega de avance 1-jul, Reporte PIDA 11-ago) y con la gestión de bloqueos <72h del log de impedimentos.

## Preguntas de repaso
1. **¿Cuáles son los 5 grupos de procesos que atraviesa todo proyecto?** — Inicio, Planeación, Ejecución, Monitoreo y Control, y Cierre; relacionados con el ciclo de mejora continua (Planear-Hacer-Verificar-Actuar).
2. **¿Qué cambió la 7ª edición del PMBoK (2021) y qué se mantiene?** — Cambió el enfoque central de grupos de procesos a principios y áreas de dominio, pero declara que los proyectos siguen atravesando todos los grupos de procesos.
3. **Enumera en orden los 6 procesos para gestionar tiempos y recursos.** — Desglosar actividades → Secuenciar actividades → Estimar duración + Estimar recursos (en paralelo) → Calcular la Ruta Crítica → Desarrollar el cronograma.
4. **¿Qué relación existe entre la estimación de duraciones y la de recursos?** — Interactúan íntimamente: la disponibilidad de recursos puede influir en la duración y viceversa; cualquier variación en uno provoca cambios en el otro.
5. **¿Qué aporta el Método de la Ruta Crítica además de la duración total?** — Identifica todas las rutas posibles, las actividades críticas que no admiten retraso y las holguras de las actividades no críticas (puntos de flexibilidad del cronograma).
