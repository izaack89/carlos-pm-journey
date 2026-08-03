---
title: L4 — Cálculo de la ruta crítica del proyecto
curso: PMP
modulo: 01. Gestión del Tiempo y Recursos
leccion: L4
fuente: "[[documentation/01. Gestión del Tiempo y Recursos/PMP_SC1.1_Versión impresa_L4.pdf|Versión impresa L4]]"
status: por-estudiar
tags: [pmp, tiempo-recursos]
---

# L4 — Cálculo de la ruta crítica del proyecto

## Resumen (5-8 líneas)
La ruta crítica es uno de los cálculos más importantes de la planificación del cronograma: de todas las rutas o cadenas de actividades que llevan del inicio al fin del proyecto, siempre habrá una con la duración más larga, y esa es la ruta crítica. Para calcularla se requieren pasos previos: estimar las duraciones de las actividades, calcular sus holguras, aplicar adelantos y atrasos donde sea necesario, y analizar el diagrama de red. La duración de las actividades y sus recursos son mutuamente dependientes, por lo que se estiman en conjunto. La lección presenta tres técnicas de estimación de duración (análoga, paramétrica y de 3 puntos/PERT) y cierra conectando estimación → ruta crítica → holgura: las actividades críticas se ejecutan en serie y tienen holgura cero, de modo que cualquier retraso en ellas retrasa todo el proyecto.

## Conceptos clave
- **Ruta crítica**: de todas las rutas posibles del proyecto (inicio → fin), la de duración más larga. Determina la duración del proyecto.
- **Actividades críticas**: las que forman la ruta crítica; se ejecutan en serie (una detrás de la otra). Si una se retrasa, todo el proyecto se retrasa. Su holgura es **cero**.
- **Holgura**: tiempo permisible de retraso de una actividad no crítica sin afectar la terminación del proyecto.
- **Relación duración ↔ recursos**: la estimación de la duración de una actividad siempre está ligada a la estimación de los recursos necesarios; son mutuamente dependientes.
- **Estimación análoga**: usa datos de proyectos previos similares (duración, presupuesto, tamaño, recursos, complejidad) como base de comparación. Rápida, respuesta casi inmediata, pero de baja precisión: incertidumbre de entre **+50% y −50%**; su efectividad suele ser baja.
- **Estimación paramétrica**: determina la duración **cuantitativamente** con base en **al menos dos parámetros**.
- **Estimación de 3 puntos (PERT)**: Program Evaluation and Review Technique, desarrollada por la Oficina de Proyectos Especiales de la Marina de EE. UU. en **1958** para el diseño de misiles; pensada para proyectos grandes y complejos. Incluye identificación de actividades, secuenciación, estimación de duración y diagrama de red.
- **Distribución Beta vs Normal**: PERT se basa en una distribución **Beta**, similar a la Normal pero **asimétrica** y variable de caso en caso (la Normal es simétrica y siempre se comporta igual).
- **Tiempo estimado**: en la estimación de 3 puntos, el valor central de duración se obtiene con un promedio **probabilístico** (no aritmético). *(La fórmula clásica PERT es TE = (O + 4M + P) / 6; el PDF la describe como "promedio probabilístico" sin desarrollarla.)*

## Técnicas / fórmulas / procesos
**Pasos previos al cálculo de la ruta crítica:**
1. Estimar las duraciones de las actividades.
2. Calcular las holguras de las actividades.
3. Aplicar adelantos y atrasos donde sea necesario.
4. Analizar el diagrama de red.

**Cálculo de la ruta crítica con el diagrama de PERT:**
a. Analizar el diagrama de red (diagrama de PERT) del proyecto.
b. Identificar todas las rutas posibles del proyecto.
c. Conocer las duraciones de todas las actividades.
d. Calcular cuánto dura cada una de las rutas.
e. **La ruta más larga de todas es la ruta crítica.**

**Elección de técnica de estimación:** siempre subordinada a la cantidad de **información disponible** y a la **experiencia** del equipo en proyectos similares. Con las duraciones estimadas ya se puede calcular: duración de todas las rutas, duración de la ruta crítica (= duración del proyecto), holguras, y aplicar adelantos/atrasos.

## Aplicación práctica
- El PDF no desarrolla un ejemplo numérico; señala como práctica que al introducir datos en la técnica elegida hay que ser muy cuidadoso para que las estimaciones sean lo más cercanas a la realidad del proyecto.
- Herramientas de software recomendadas para gestionar tiempos y recursos: **Microsoft Project** (demo), **WBS Schedule Pro** (demo) y **Project Libre** (versión completa gratuita).

## Conexión con APL/PIDA
- En el [[README|proyecto PIDA]] (23 sitios LTE B41, cronograma de 12 semanas), la cadena Integración → Optimización → Aceptación funcionó como la "ruta crítica" real: un retraso en la integración del golden cluster (W2) habría corrido todo el plan hasta la Defensa (W12).
- La estimación análoga es lo que Carlos ya hace al usar el baseline histórico (FTR 82-88%, horas de re-trabajo de despliegues previos) para dimensionar el plan de trabajo del PIDA.
- La holgura explica por qué la aceptación por pares de semanas (integrado en W_n, aceptado en W_n+1) toleraba deslices sin mover los deadlines duros (1-jul y 11-ago), mientras que el burndown del [[Index-APL|curso APL]] vigilaba justo las actividades sin holgura.

## Preguntas de repaso
1. **¿Qué es la ruta crítica de un proyecto?** — De todas las rutas de actividades del inicio al fin, la que tiene la duración más larga; determina la duración total del proyecto.
2. **¿Cuánta holgura tienen las actividades críticas y qué implica?** — Holgura igual a cero: se ejecutan en serie y cualquier retraso en una de ellas retrasa todo el proyecto.
3. **¿Qué rango de incertidumbre tiene la estimación análoga y por qué?** — Entre +50% y −50%, porque se basa solo en analogías/comparaciones con proyectos previos, con poca información y baja precisión.
4. **¿En qué se diferencia la distribución Beta (base de PERT) de la Normal?** — La Beta es asimétrica y varía de caso en caso; la Normal es totalmente simétrica y siempre se comporta igual.
5. **¿Qué requiere la estimación paramétrica para determinar la duración?** — Determinarla cuantitativamente con base en al menos dos parámetros.
