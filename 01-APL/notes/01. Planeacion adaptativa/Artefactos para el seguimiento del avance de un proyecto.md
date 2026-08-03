# Artefactos para el seguimiento del avance de un proyecto

> PDF: [[documentation/01. Planeacion adaptativa/Artefactos para el seguimiento del avance de un proyecto.pdf|Ver PDF original]]

En este recurso revisarás tres artefactos que nos ayudan a dar seguimiento al avance que se tiene en un momento dado dentro de una iteración y uno más que nos ayudará a establecer el nivel de desempeño del equipo para mejorar constantemente nuestras estimaciones.

---

Una vez que la iteración inicie, la **reunión diaria del equipo de desarrollo** permitirá reportar las historias de usuario que ya iniciaron para llevarlas a la columna "En progreso", y conforme alguna historia de usuario vaya siendo finalizada, se llevará a la columna "Terminado" del tablero *Kanban*.

Recuerda que una **historia de usuario** puede estar compuesta por varias tareas, de tal manera que para considerarla "Terminada" deberán haberse finalizado todas las tareas que la integran.

En algunos *softwares*, como *DevOps*, las "Tareas" son las que se mueven entre columnas, mientras que en la historia de usuario solo se cambia el "estatus".

Los *story points* asignados a cada historia de usuario que se vaya finalizando, serán los que tomarás en cuenta para reportar el avance dentro de la iteración en las siguientes gráficas.

---

## Burndown Chart

Este artefacto es una gráfica en la cual:

- Se muestran en una línea de manera **descendente**, los *story points* que al paso del tiempo están previstos para ser completados en la iteración hasta llegar a cero al final de la iteración.
- En otra línea, se muestran los *story points* que el equipo **realmente va completando** al paso del tiempo, lo que permite tanto al equipo de desarrollo como al *Product owner* y a los *stakeholders* visualizar de manera sencilla el desempeño del equipo.

Esta gráfica es conveniente para dar seguimiento a una iteración en la cual se prevé que **no habrá cambios** en el número de historias de usuario que están planeadas a realizar.

---

## Cumulative Flow Diagram (CFD)

Para realizar un **análisis más completo del desempeño del equipo** en una iteración, puedes utilizar el diagrama de flujo acumulativo (*Cumulative Flow Diagram*) cuyo objetivo es mostrar **qué tan estable es el flujo de trabajo**. En este diagrama podemos identificar **métricas** importantes para tomar decisiones.

- El **eje horizontal** del CFD representa el periodo durante el cual se visualizan los datos.
- El **eje vertical** muestra en bandas de diferentes colores, el número de elementos de trabajo, historias de usuario o tareas, que se encuentran en las diferentes etapas del tablero *Kanban* durante diferentes momentos de la iteración.
- La **línea superior** de cada banda indica el momento en que la tarea ingresa al estado correspondiente.
- La **línea inferior** indica el momento en el que pasa a otro estado.

### Métricas del CFD

- ***To do***: El trabajo pendiente por realizar en un momento en el tiempo.
- ***Cycle time***: El tiempo que tarda en desarrollarse una tarea desde su inicio hasta su finalización en diferentes momentos en el tiempo.
- ***Work in Progress (WIP)***: La cantidad de trabajo que se encuentra en desarrollo en diferentes momentos en el tiempo.
- ***Done***: La cantidad de trabajo terminado a lo largo de la duración de la iteración.

### Interpretación

- Cuando la **distancia del *cycle time* se alarga** significa que la eficiencia en el desarrollo ha bajado — puede ser por algún "cuello de botella" o baja en el rendimiento del equipo.
- Cuando la **banda de *WIP* se ensancha**, significa que existe mucho trabajo "En progreso". Se recomienda limitar el WIP para que el equipo se enfoque en terminar tareas en lugar de tener varias iniciadas.

> *"Stop starting, Start finishing"* — "Dejar de empezar, empezar a terminar". Se atribuye a David J. Anderson en un stand up meeting en 2004.

Limitando la cantidad de tareas que pueden estar en la columna "En progreso" del tablero *Kanban*, el equipo se enfocará en finalizar los trabajos en curso, en lugar de dejarlos a medias e iniciar nuevos.

---

## Burnup Chart

Para dar seguimiento al **proyecto de manera global** es recomendable utilizar la gráfica *Burnup Chart*. En esta gráfica:

- La línea del *backlog* representa la **cantidad de trabajo estimada en *story points*** para todo el proyecto.
- La línea de **"pronóstico"** refleja el avance estimado que se espera ir acumulando en cada iteración.
- La línea de **"terminado"** muestra el trabajo acumulado que realmente se ha finalizado a lo largo del proyecto.
- En el **eje horizontal** se muestran la cantidad de iteraciones que integran el proyecto.

---

## Gráfica de velocidad del equipo

La **gráfica de velocidad** nos ayuda a analizar el desempeño del equipo y resulta muy útil para **estimar futuras iteraciones** con el propósito de **definir y mantener un ritmo constante de trabajo**.

Al final de cada iteración, se toma la **medida de los logros del equipo** y se consideran para el número de historias de usuario que pueden ser consideradas para la siguiente iteración. Normalmente después de **tres o cuatro iteraciones**, se logra obtener un promedio que permita al equipo mayor precisión en la estimación de las iteraciones subsecuentes.

La **efectividad del desempeño de equipo** en proyectos ágiles es evaluada de manera **colectiva a nivel equipo de desarrollo**. La velocidad puede verse afectada por factores externos como mayor complejidad en subsecuentes historias de usuario, obstáculos que se presenten, incidentes o riesgos materializados.
