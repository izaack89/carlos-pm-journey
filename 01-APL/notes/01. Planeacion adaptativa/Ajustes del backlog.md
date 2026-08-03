# Ajustes del backlog

> PDF: [[documentation/01. Planeacion adaptativa/Ajustes del backlog.pdf|Ver PDF original]]

## Introducción

El *backlog* es la **lista ordenada y priorizada de las funcionalidades y elementos** que se deberán desarrollar para cumplir los objetivos del proyecto y las expectativas de los interesados, de manera tal que representa el **trabajo pendiente por realizar** en el proyecto.

Originalmente se creó el *backlog* del proyecto con los **objetivos** documentados en "la visión del proyecto" y las **épicas e historias de usuario** detectadas en ese momento y se generó un **mapa de ruta** con las liberaciones y las iteraciones previstas.

## Enfoques adaptativos

Los **enfoques adaptativos** están sujetos a un **alto nivel de incertidumbre** por lo que, los cambios al paso del tiempo son esperados. Al finalizar la primera iteración y cada una de las subsecuentes, es posible que se vayan **detectando nuevos requerimientos**, la necesidad de **modificar** algunos de los existentes o nuevas historias de usuario como consecuencia de algunos planes de respuesta a riesgos identificados.

También con el conocimiento adquirido es posible que algunas épicas se desglosen en historias de usuario con características mejor definidas para poder ser priorizadas e incluidas en las próximas iteraciones.

## ¿Y en qué momento es conveniente realizar ajustes y/o nuevos requerimientos?

Ya sea al final de cada iteración o en momentos clave del proyecto, el *Product owner* y el **equipo de desarrollo** tienen la oportunidad de **realizar los ajustes pertinentes para adaptar el trabajo pendiente** en el proyecto a las necesidades actuales del cliente. Normalmente esto se realiza mediante una **reunión** convocada por el *Product owner*, donde en conjunto con algunos *stakeholders* y el equipo de desarrollo **realizan el ajuste correspondiente al *backlog* del producto**, esto se conoce como *"backlog grooming"*, *"backlog refinement"* o en español refinamiento del backlog.

### Objetivo del refinamiento del backlog

El **objetivo** de la sesión de refinamiento es mantener un ***backlog* saludable** al tiempo que mantiene al equipo de desarrollo actualizado y en sintonía, no solo con el trabajo de la próxima iteración sino siempre **orientado a los objetivos del proyecto**.

Mantener el *backlog* actualizado es responsabilidad del *Product owner*, tu labor como líder ágil, es asegurarte que el equipo de desarrollo haya participado, comprendido y esté de acuerdo con los ajustes realizados.

## Situaciones emergentes a lo largo del ciclo de vida del proyecto

En este proceso se toman en cuenta algunas **situaciones emergentes** a lo largo del ciclo de vida del proyecto:

1. Nuevas prioridades del cliente
2. Ajustes como consecuencia del feedback obtenido
3. Planes de respuesta a riesgos identificados
4. Reparación de errores y deuda técnica
5. Nuevas relaciones entre historias de usuario
6. Dificultades o *stoppers* existentes

### 1. Nuevas prioridades del cliente

Al inicio del proyecto se tenía la visión de construir las aplicaciones para que los usuarios pudieran utilizarlas desde una computadora, pero recopilando intereses de los usuarios piloto, surge el requisito del acceso a ellas desde dispositivos móviles.

Es común que las **necesidades reales** de los *stakeholders* pueden no tener una visión completa al inicio del proyecto. Normalmente en proyectos adaptativos, conforme se avanza en el desarrollo **surgen nuevas expectativas o se clarifican algunas necesidades**.

**Un enfoque ágil en la definición de requisitos**: Obtener características y funcionalidad en la etapa inicial puede resultar inexacto. Conforme el proyecto avanza tanto el cliente como el equipo tiene mayor entendimiento de las necesidades.

### 2. Ajustes como consecuencia del feedback obtenido

En cada una de las iteraciones que lo requiera, se solicita un *feedback* para ajustar y enriquecer el producto o servicio.

### 3. Planes de respuesta a riesgos identificados

Durante la prueba piloto de la nueva aplicación, se detectó que la arquitectura sobre la cual trabajan las aplicaciones **no cuenta con los esquemas de seguridad** que garanticen la autenticación de los usuarios, por lo que se detecta la posibilidad de usurpación de identidad. El equipo de desarrollo detecta la necesidad de atacar este riesgo y **propone la implementación de una API** que permita esquemas completos para el manejo de seguridad y trazabilidad de operaciones.

Esto implica **nuevas características para la arquitectura** y la **inclusión de nuevas historias de usuario al *backlog* con alta prioridad** antes de incluir nuevas aplicaciones para evitar re-trabajos posteriores.

### 4. Reparación de errores, pendientes y deuda técnica

Los equipos de trabajo no son perfectos, es posible que al finalizar parte de los trabajos hayan prevalecido algunos errores y las historias de usuario hayan sido aceptadas con restricciones, en muchos casos también conocidos como *"punch list"*.

La **deuda técnica** significa **trabajo adicional pendiente por realizar**. Al igual que la deuda financiera, en ocasiones se va "pagando" en parcialidades — puede ser dividida en varias historias de usuario para futuras iteraciones.

### 5. Nuevas dependencias entre historias de usuario

Una de las razones de la participación del equipo de desarrollo en el *backlog grooming* es **identificar las dependencias entre tareas ya sean obligatorias o discrecionales** que hayan surgido entre ellas a fin de asegurar que el trabajo se mantenga ordenado respetando las dependencias.

En el **enfoque adaptativo** la dependencia más utilizada es ***Finish to Start***: será necesario ajustar primero la arquitectura (Actividad A), antes de desarrollar cualquier otra aplicación (Actividad B) para evitar re-trabajos.

### 6. Dificultades o stoppers existentes

El ajuste del *backlog* puede incluir la **reducción de prioridad o incluso la eliminación de algunas historias de usuario**, ya sea porque se detecta la imposibilidad de realizarse o porque se decide que ya no se considera necesaria cierta funcionalidad que inicialmente había sido considerada.

Durante el refinamiento del *backlog* es posible:
- Incluir nuevas historias de usuario
- Cambiar la prioridad de algunas de ellas
- Refinar algunas épicas para determinar las historias de usuario que la integran
- Eliminar algunas historias de usuario

De tal manera que el *backlog* **refleje la actualidad del trabajo que realmente está pendiente por ser realizado**.

## En conclusión

El *backlog* es un **instrumento de conexión entre el *Product owner* y el equipo de desarrollo**. Si el *backlog* aumenta, es importante **mantener la estructura de procesos definida originalmente** — las nuevas épicas o historias de usuario deben ser estimadas por el equipo de desarrollo antes de ser incorporadas.

El refinamiento asegura **mantener el proyecto alineado con los objetivos cambiantes en todo momento**. Como líder ágil, debes asegurarte de que el *Product owner* en conjunto con el equipo de desarrollo revisen la "Hoja de ruta" para analizar si el refinamiento del *backlog* afecta las fechas de lanzamiento.
