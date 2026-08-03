# Implementar el Plan de respuesta a riesgos

> PDF: [[documentation/02. Detección y Resolución de Riesgos y Problemas copy/8. Implementar el Plan de respuesta a riesgos.pdf|Ver PDF original]]

---

Implementar el Plan de
respuesta a riesgos
Javier y el equipo, tras analizar los riesgos identificados han reconocido y acordado las acciones de respuestas
para cada uno de ellos, con la finalidad de dar un seguimiento oportuno han decidido utilizar un tablero Kanban
para dar y evaluar la atención a las mismas a través de los estados siguientes:
Por hacer

En curso

Listo

Corresponde al “backlog”, esto es,
acciones que aún no se ejecutan.

Corresponde a las acciones que
están en ejecución.

Corresponde a las acciones que
se han terminado de ejecutar.

Un poco de historia

El concepto de Kanban fue desarrollado en Japón por la empresa Toyota en la década de los años 50
con la finalidad de hacer más eficientes los procesos de producción con el objetivo de reducir tiempos
muertos del personal, desperdicio de material y costos de almacenamiento. Kanban significa “letrero”.
En un tablero Kanban se establecen estados para las actividades del proceso con la finalidad de
identificar la evolución en su atención, así como reglas para realizar la transición entre ellos, tales
como responsables, complejidad, dependencia y/o fechas compromiso.
Un tablero Kanban es una representación visual del flujo de trabajo y simboliza un medio de
comunicación efectivo y transparente para identificar impedimentos, los cuales están asociados de
manera intrínseca a las actividades en proceso que no tienen avance después de algún tiempo de
iniciada su atención, lo cual es una alerta para tomar acciones preventivas.

La implementación de las respuestas a los riesgos por lo regular se lleva a cabo de acuerdo con lo estipulado
en el plan de gestión de riesgos en el que se definen los lineamientos para hacer uso del presupuesto de reserva
y actualizar las líneas base del proyecto, ¿líneas base? ¿esto aplica para un proyecto adaptativo (ágil)?
¡Por supuesto!


Todo proyecto, indistintamente, del enfoque a través del cual sea ejecutado requiere contar con un acuerdo sobre
restricciones típicas tales como Costo y Tiempo, es importante tener presente que los recursos son limitados,
así, un proyecto ágil puede nacer con un presupuesto de X pesos para ser ejecutado en un periodo de Y meses,
esto se conoce como restricciones del proyecto y la ejecución normalmente inicia con una serie de supuestos
(liberación de permisos por la autoridad, fecha de contratación de proveedores, etcétera).
Los resultados esperados de la respuesta a riesgos se incorporan como parte del alcance y las actividades
asociadas se agregan al cronograma (proyecto predictivo) o backlog (proyecto adaptativo).
En el caso de un proyecto ágil, el plan de respuesta a riesgos consiste en:
1. Para cada riesgo se definen las acciones de respuesta.
2. Para cada acción de respuesta a riesgos se define un responsable y una fecha compromiso.
3. Se gestiona la ejecución de las acciones de respuesta a riesgos a través de un tablero Kanban.
Un ejemplo de plan de respuesta a riesgos se muestra a continuación tomando de referencia la lista de riesgos
siguiente:
Clave

Descripción del riesgo

Acción de respuesta

RDP1

Si las historias no tienen criterios de
aceptación no se tiene referencia para
cumplir con las expectativas de los usuarios.

Revisar los criterios de aceptación antes
de la planeación del sprint.

RDP2

Si el equipo de desarrollo no genera evidencia
de pruebas unitarias no se tiene certeza de
que puedan iniciar las pruebas de usuarios.

Generar evidencia de las pruebas unitarias
antes de pasar a pruebas de usuario.

RDP3

Si los usuarios no presentan las historias
antes de la planeación de un sprint se pueden
tener imprecisiones en la valoración por
ambigüedades y/o dudas.

Asegurar que los usuarios presenten las
historias para resolver ambigüedades.

El tablero Kanban quedaría configurado de la siguiente manera, aquí es en donde se establece un responsable y
fecha compromiso de atención por cada acción:
Por hacer 3

En curso

Listo

Todo lo demás 3 incidencias
Revisar los criterios de aceptación
antes de la planeación del sprint.
RDP1

Generar evidencia de las pruebas unitarias
antes de pasar a pruebas de usuario.
RDP2

Asegurar que los usuarios presenten las
historias para resolver ambigüedades.
RDP3

Figura 2.2 Tablero Kanban para gestión de respuesta a riesgos. Fuente: Elaboración propia.


Robert Tarne, (2011) en la conferencia titulada “Taking off the agile training wheels, advance agile project
management using Kanban” menciona las siguientes recomendaciones:

Limitar el trabajo en progreso (WIP)
Ha habido una serie de estudios que han demostrado que la multitarea es ineficiente. En un estudio
(Rubenstein, Meyers y Evans, p.776), los investigadores concluyeron que el cambio de tareas puede
costar entre un 20 y un 40 por ciento de pérdida de eficiencia. Por ejemplo, si un programador estaba
trabajando en dos tareas que deberían tomar cinco horas cada una, si realizaba múltiples tareas entre
las dos tareas, el tiempo total para completar podría ser de hasta 14 horas en total, en lugar de 10 horas
si se concentrara en una tarea a la vez.
En Kanban, hay un límite establecido sobre cuántas tareas pueden estar en cualquier paso a la vez para
evitar la ineficiencia introducida con la multitarea. Por ejemplo, puede haber un límite de tres elementos
en la cola de desarrollo. Si ya hay tres elementos en esta cola, no se moverá ningún elemento nuevo del
Análisis de causa raíz hasta que uno de los elementos en Desarrollo se complete y se mueva a Prueba.
En este momento, un elemento de Análisis de causa raíz podría pasarse a Desarrollo.

Medir y administrar el flujo
El sistema de producción de Toyota desarrolló la idea de “tomar” actividades. Las tarjetas Kanban
indican cuándo un integrante del equipo está listo para trabajar con nuevas tarjetas. El trabajo no se
toma en su totalidad desde un principio, solo cuando se completa una tarea se puede iniciar otra tarea
en función de los límites de trabajo en curso que se establecen para cada paso.
La forma más fácil de administrar el flujo de trabajo de un equipo es a través de un tablero Kanban.
El equipo puede reunirse todos los días utilizando la ceremonia de revisión diaria para analizar las tareas
que están en progreso. A medida que avanza el trabajo, las tarjetas se mueven de una cola de trabajo
a la siguiente.
En dicho artículo se hace referencia a un estudio de D.J. Anderson en que menciona que un equipo de
trabajo concluyó que estimar era un desperdicio pues el valor de tener estimaciones detalladas para
cada actividad es bajo en comparación con el esfuerzo de desarrollar estas estimaciones y, por lo tanto,
el equipo decide dejar de hacer estimaciones para las actividades.

Hacer que las políticas de procesos sean explícitas
El proceso que sigue el equipo se basa en políticas. Algunas de estas están bajo el control del equipo
mientras que otras políticas son dictadas por la organización. Por ejemplo, el equipo puede decidir
un límite WIP de tres elementos para el estado “En proceso”, pero aumentar el límite a cuatro cuando
se agrega un nuevo miembro del equipo. Hacer que las políticas sean explícitas ayuda a eliminar las
suposiciones sobre las reglas de trabajo. También facilita el siguiente paso, la mejora continua.

Mejora continua
Otra ventaja de limitar WIP es que creará tiempo de inactividad ocasional. Por ejemplo, un tester puede
esperar a que el siguiente elemento de la columna “en proceso” se mueva a la columna de prueba. Si
bien al principio esto puede no parecer ideal, en realidad, es este tiempo de inactividad el que brinda la
capacidad de identificar mejoras en el proceso. Si la gente está demasiado ocupada pasando de una
tarea a otra; no tendrán tiempo para pensar en mejoras.


En la organización en que colaboras, ¿qué herramientas utilizan para gestionar y dar seguimiento a los riesgos?
¿Por qué consideras que es importante planear la ejecución de las respuestas a riesgos?
¿Qué consecuencias se pueden tener en un proyecto si no se da un seguimiento adecuado a la ejecución de
respuestas a los riesgos?

Practica lo que has aprendido
En la organización en que colaboras, ¿qué herramientas utilizan para gestionar y dar seguimiento a los riesgos?
¿Por qué consideras que es importante planear la ejecución de las respuestas a riesgos?
¿Qué consecuencias se pueden tener en un proyecto si no se da un seguimiento adecuado a la ejecución de
respuestas a los riesgos?
Apoya a Javier en generar el plan de respuesta para los riesgos que se han identificado (recuerda que estos se
han definido en temas previos)
No

R01

R02

R03

R04

R05

R06

Riesgo

Respuesta

Los usuarios indicaron que no era lo
que esperaban.

El no contar con la aceptación de
entregables implica retrabajo.

Los requerimientos de usabilidad se
definen sobre la marcha.

No tener licencias suficientes para
acceder al repositorio del proyecto.

El equipo no tiene experiencia técnica
necesaria.

El equipo no es suficiente para
cumplir con los compromisos de los
Sprints.


Definir la respuesta a riesgos es un paso fundamental dentro de la gestión de riesgos, pues detonará las acciones
a seguir para su tratamiento, es importante tener en cuenta que el equipo del proyecto no necesariamente debe
hacerse cargo de todos los riesgos, una vez que se analizan se establece la respuesta a tomar y, posteriormente,
se asignan responsables y fechas compromiso para dar seguimiento a su mitigación.
Oportunidad

Amenaza
•
•
•
•
•

Escalar
Evitar
Transferir
Mitigar
Aceptar

•
•
•
•
•

Escalar
Explotar
Compartir
Mejorar
Aceptar

Descarga el documento desde el apartado
de "Archivos adjuntos" de la plataforma.
