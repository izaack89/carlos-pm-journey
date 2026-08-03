---
title: L3 — Secuenciación de las actividades del proyecto
curso: PMP
modulo: 01. Gestión del Tiempo y Recursos
leccion: L3
fuente: "[[documentation/01. Gestión del Tiempo y Recursos/PMP_SC1.1_Versión impresa_L3.pdf|Versión impresa L3]]"
status: por-estudiar
tags: [pmp, tiempo-recursos]
---

# L3 — Secuenciación de las actividades del proyecto

## Resumen (5-8 líneas)
La restricción de tiempo es una de las condiciones determinantes de todo proyecto, por lo que al planificar los tiempos hay que secuenciar las actividades: definir el mejor orden y secuencia lógica para terminar en el menor tiempo posible cumpliendo las especificaciones. Se descompone la EDT hasta las actividades individuales (el nivel de 4 niveles es recomendación, no obligación), se genera la lista completa de actividades e hitos, y a partir de ella se definen las precedencias. Entre bloques existen 4 tipos de relaciones lógicas (FS, SS, FF, SF) que gobiernan cuándo puede iniciar o terminar cada actividad. Con la tabla de precedencias y el método PDM se dibuja el diagrama de red y se identifican todas las rutas del proyecto desde el hito de inicio hasta el hito de fin.

## Conceptos clave
- **Secuenciación de actividades**: definir el mejor orden y secuencia lógica para que el proyecto termine en el menor tiempo posible cumpliendo todas sus especificaciones iniciales.
- **Descomposición de la EDT**: descomponer cada etapa en **actividades individuales** que producen resultados parciales; éstos se **suman/agregan hacia los niveles superiores** (etapas → fases → proyecto) hasta los resultados totales.
- Los **4 niveles de la EDT** (proyecto, fases, etapas, actividades) son **sólo una recomendación, no obligatorios**: si la complejidad y duración lo exigen se puede descomponer en más niveles, siempre que el nivel más bajo contenga actividades individuales que ya no se pueden desglosar.
- **Lista de actividades e hitos**: obtenerla completa aumenta las probabilidades de terminar el proyecto exitosamente; es el insumo para definir orden y secuencia.
- **Predecesor / sucesor**: en cualquier diagrama de bloques hay un bloque antes del actual y otro después; las relaciones lógicas definen cómo se condicionan.
- **Tabla de precedencias**: lista de actividades convertida en tabla que registra las precedencias definidas por el equipo considerando dependencias y relaciones lógicas.
- **ID de actividad**: identificador simple (letras mayúsculas desde la A) asignado sólo a las actividades para que el diagrama de red sea más sencillo de leer que con nombres completos o códigos EDT. Recomendado, no indispensable.

## Técnicas / fórmulas / procesos
**Los 4 tipos de relaciones lógicas entre bloques:**

| Relación | Siglas | Regla |
|---|---|---|
| Final a Inicio | **FS** (Finish to Start) | El sucesor no puede **iniciar** hasta que **termine** el predecesor. La más común. |
| Inicio a Inicio | **SS** (Start to Start) | El sucesor no puede **iniciar** hasta que haya **iniciado** el predecesor (no implica iniciar al mismo tiempo). |
| Final a Final | **FF** (Finish to Finish) | El sucesor no puede **finalizar** hasta que **termine** el predecesor (no implica terminar al mismo tiempo). |
| Inicio a Final | **SF** (Start to Finish) | El sucesor no puede **finalizar** hasta que **inicie** el predecesor. La menos utilizada; útil en programación de rutas no críticas. |

**Pasos para obtener el diagrama de Red de un proyecto (aplicación):**
1. Descomponer la EDT hasta su nivel más bajo.
2. Obtener la lista de actividades de todo el proyecto a partir de la EDT.
3. Asignar a cada bloque (proyecto, fases, etapas, actividades) su código EDT.
4. Asignar un ID (letras A, B, C…) sólo a las actividades.
5. Analizar dependencias y relaciones lógicas en equipo y definir las precedencias → tabla de precedencias.
6. Dibujar el diagrama de red según la tabla de precedencias con el método **PDM**.
7. Identificar gráficamente **todas las rutas** o cadenas de actividades del hito de inicio al hito de fin.

**Checklist de cierre de la lección** (procesos a no olvidar al secuenciar): orden y secuencia para el éxito · desarrollar y descomponer la EDT hasta nivel de actividades · generar códigos EDT · generar lista de actividades · convertirla en tabla de precedencias · identificar relaciones lógicas · identificar dependencias · aplicar PDM · contar el número de rutas del proyecto.

## Aplicación práctica
- El PDF guía la aplicación a un proyecto propio ya trabajado: partir del diagrama EDT, derivar la lista de actividades, codificarla, asignar IDs con letras y construir la tabla de precedencias en equipo antes de dibujar la red con PDM e identificar las rutas de inicio a fin.
- Referencia normativa: PMBOK 6ª y 7ª ed. e **ISO 21500** (Gestión de Proyectos, Programas y Portafolios). Herramientas sugeridas: Microsoft Project (demo), WBS Schedule Pro (demo), ProjectLibre (gratuito completo).

## Conexión con APL/PIDA
- En el [[README|proyecto PIDA]] las dependencias reales eran mayormente FS y SS: la aceptación de sitios (W3-W8) sólo podía arrancar tras integrar (relación tipo SS escalonada — la integración de una semana se acepta en la siguiente), y escalar los 20 sitios dependía de terminar la validación del golden cluster (FS).
- La tabla de precedencias es el equivalente predictivo del **backlog priorizado con Kanban** que Carlos usó en el [[Index-APL|curso APL]]: ambos hacen explícito el orden del trabajo, pero PDM lo fija en diseño mientras Kanban lo gestiona por flujo.
- Los hitos de inicio/fin del diagrama de red equivalen a los hitos duros del cronograma de 12 semanas (kickoff, Entrega de avance 1-jul, Reporte PIDA 11-ago).

## Preguntas de repaso
1. **¿Es obligatorio descomponer la EDT en exactamente 4 niveles?** No, es una recomendación; puede haber más niveles siempre que el más bajo contenga actividades individuales indivisibles.
2. **¿Qué significa una relación SS entre dos actividades?** Que el sucesor no puede iniciar hasta que al menos haya iniciado el predecesor — no que deban iniciar simultáneamente.
3. **¿Cuál es la relación lógica menos utilizada y para qué sirve?** SF (Inicio a Final): el sucesor no puede finalizar hasta que inicie el predecesor; se usa sobre todo en programación de rutas no críticas.
4. **¿Por qué asignar IDs de letras a las actividades del diagrama de red?** Para que el diagrama sea más sencillo y fácil de entender que con nombres completos o códigos EDT; es recomendado pero no indispensable.
5. **¿Qué método se aplica para dibujar el diagrama de red a partir de la tabla de precedencias?** El PDM (Precedence Diagramming Method), identificando después todas las rutas del hito de inicio al de fin.
