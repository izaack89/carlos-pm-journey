# Planeación adaptativa — Lección 6: ¿Cómo ajustar la planificación?

> PDF: [[documentation/01. Planeacion adaptativa/Planeación adaptativa_Lección 6_versión_impresa.pdf|Ver PDF original]]

Versión impresa de la Lección 6, que cubre los ajustes del backlog, el Minimum Value Increment (MVI), el Modelo Kano, la evolución de atributos, lecciones aprendidas, tipos de conocimiento y el cierre del proyecto.

---

## Introducción

Una de las principales características de la planificación adaptativa es una **replanificación constante**. Los objetivos generales ayudan a mantener el enfoque, pero las necesidades van cambiando y los **requisitos se van adaptando** a esas necesidades nuevas o cambiantes.

La comunicación constante con el cliente/PO y la experiencia de haber creado una versión funcional inicial ayudan a **identificar si los requisitos originales siguen siendo válidos** o existen nuevos requerimientos. Esto lleva a **ajustar el backlog del proyecto** entre iteraciones.

---

## Ajustes del backlog

El **Minimum Value Increment (MVI)** se refiere a la **cantidad de valor mínima** que el equipo de desarrollo puede generar en la **siguiente iteración** del proyecto.

Conforme avanzan las iteraciones, el equipo, el PO y los *stakeholders* entienden mejor las necesidades y la capacidad del equipo. Se deben tomar en cuenta las **prioridades del backlog** para establecer las HU que generen la **mayor cantidad de valor con el menor esfuerzo e inversión**.

### ¿Cómo se determina el MVI?

Se pueden utilizar las **mismas técnicas que para el MVP**, incorporando:
- La **experiencia adquirida** en iteraciones realizadas
- **Variaciones** en componentes del backlog y equipos de desarrollo
- El **mayor conocimiento de los *stakeholders*** que han revisado la funcionalidad generada y pueden clarificar requisitos y expectativas

Ver también: [[notes/01. Planeacion adaptativa/Ajustes del backlog|Ajustes del backlog]]

---

## Modelo Kano

Teoría de desarrollo de productos y satisfacción del cliente desarrollada por el profesor **Noriaki Kano** en la década de 1980. Clasifica las **preferencias del cliente en cinco categorías** para lograr el mejor escenario de satisfacción.

### Las cinco categorías

**1. Necesidades básicas**
Atributos que el cliente **espera que estén siempre presentes**. No generan satisfacción especial, pero su ausencia genera **total insatisfacción**. *Ejemplo: que en un restaurante te sirvan la sopa caliente.*

**2. Necesidades de desempeño**
Tienen una **relación directa** con el nivel de satisfacción — a mayor nivel del atributo, mayor satisfacción. Su ausencia no genera insatisfacción, pero su presencia genera satisfacción **proporcional**. *Ejemplo: la calidad de la comida.*

**3. Excitadores**
Atributos que **sorprenden al cliente** ya que no los espera → generan **satisfacción adicional** que puede llevar la experiencia a otro nivel. *Ejemplo: un postre o café gratis al terminar de comer.*

**4. Indiferentes**
**No afectan significativamente** la satisfacción — si están presentes o no, no generan impacto. *Ejemplo: música ambiental que ni se nota.*

**5. De reversa**
Si están presentes, **generan insatisfacción** — resultan contraproducentes. *Ejemplo: un menú digital lento y difícil de navegar.*

### Diagrama de categorías

El diagrama Kano muestra en el eje vertical la **satisfacción/insatisfacción** y en el eje horizontal la **presencia/ausencia** de atributos:
- Las **necesidades básicas** están en la zona inferior (su ausencia genera insatisfacción)
- Los **excitadores** están en la zona superior (sorpresa positiva)
- Las **necesidades de desempeño** crecen linealmente

### Evolución de atributos

Los atributos categorizados como **excitadores** con el tiempo van migrando a **desempeño** o incluso llegan a ser **necesidades básicas**. *Ejemplo: el acceso a internet en un smartphone pasó de ser un excitador a una necesidad básica.*

| Funcionalidad (smartphone) | Categoría actual |
|----------------------------|------------------|
| Solo pueda ser usado por una sola compañía telefónica | **De reversa** |
| Cuente con una cinta para sujetarlo a la mano | **Indiferente** |
| Duración de batería mínima de 24 horas | **De desempeño** |
| Conexión a la red más actualizada | **Necesidades básicas** |
| Elegir el color a tu entera satisfacción | **Excitadores** |

Ver también: [[notes/01. Planeacion adaptativa/Qué le recomiendas a Doña Mary|¿Qué le recomiendas a Doña Mary?]]
Ver también: [[notes/01. Planeacion adaptativa/Veamos un ejemplo|Veamos un ejemplo — Evolución de categorías Kano]]

---

## Lecciones aprendidas

El registro de lecciones aprendidas es un **activo muy valioso** para la organización.

### Reuniones de retrospectiva

El momento más conocido para identificar y documentar lecciones aprendidas son las **reuniones de retrospectiva** — el equipo reflexiona sobre lo que han hecho bien y detectan **áreas de oportunidad**, documentan lecciones aprendidas e identifican acciones para futuras iteraciones.

### Entorno interno y externo

Las lecciones aprendidas se pueden identificar en **cualquier momento**, tanto en el entorno interno como externo del proyecto:

- **Interno:** Procesos organizacionales, seguridad, cultura y estructura, instalaciones, infraestructura, procesos de compras, disponibilidad y manejo de recursos
- **Externo:** Duplicidad de esfuerzos, estándares de la industria, tendencias sociales y tecnológicas, regulaciones, riesgos

### Situaciones comunes en proyectos (PMI, PMBOK 7a ed., p. 151)

| Situación | Sugerencia de adaptación |
|-----------|--------------------------|
| Entregables de calidad deficiente | Añadir más ciclos de verificación de retroalimentación y pasos de control de calidad |
| Miembros del equipo inseguros de cómo proceder | Añadir más pasos de orientación, entrenamiento y verificación |
| Largas demoras en espera de aprobaciones | Simplificar decisiones con menos personas autorizadas hasta ciertos umbrales |
| Demasiado trabajo en curso o altas tasas de desecho | Usar mapeo del flujo de valor y tableros Kanban para visualizar el trabajo |
| Interesados no se comprometen o comparten información negativa | Evaluar si se comparte suficiente información; mejorar ciclos de retroalimentación |
| Falta de visibilidad del avance del proyecto | Comprobar que se recopilan y discuten medidas apropiadas en reuniones |
| Incidentes/riesgos siguen emergiendo | Explorar causas raíz para determinar lagunas en procesos o actividades |

### Documentación de lecciones aprendidas

La preservación y gestión es un **proceso organizacional** — conviene que un área (como la **PMO**) se haga responsable de mantenerlas actualizadas, indexadas y con fácil acceso.

### Tipos de conocimiento

**Conocimiento explícito:** Se puede expresar o comunicar a través de **palabras, símbolos u otros medios gráficos**. Son hechos, datos e información almacenables y recuperables. Se encuentra en documentos escritos, bases de datos, manuales, memorias técnicas, planos, archivos multimedia, foros wikis.

**Conocimiento tácito:** No es fácil de documentar — tiene que ver con la **experiencia, habilidades, cultura, ética y conocimientos prácticos** de una persona. Se adquiere a través de la interacción, la observación, la intuición y la práctica.

**Formas de documentar conocimiento tácito:**
- **Tomar notas** al observar la realización de un trabajo o conversar con expertos
- **Grabar conversaciones** de trabajo o mentoría (con autorización)
- Usar el **documento de seguimiento de acuerdos** para documentar razones de decisiones

El conocimiento tácito se comparte cuando el equipo está **co-ubicado** y trabaja en parejas o en conjunto. Se recomienda contar con un **War Room** para trabajo colaborativo.

---

## Cierre del proyecto

En planificación adaptativa, el proceso de cierre sucede de **manera iterativa** — se asegura que los objetivos hayan sido cumplidos y que los entregables sean aceptados por los *stakeholders*. Ocurre mínimo al finalizar cada **lanzamiento**.

### Cierre formal

Al finalizar el proyecto completo:
- Establecer que la **totalidad de los objetivos fueron cumplidos**
- Incorporar la **lista de acuerdos tomados** durante el desarrollo para cambios y ajustes al backlog
- Procurar que todos los participantes hayan **plasmado su visión** en las retrospectivas
- La **última retrospectiva** conviene enfocarla en el proyecto global — cómo evolucionó el equipo y la relación con *stakeholders*

### Entregables del cierre

- **Documentación generada** a lo largo del ciclo de vida
- **Evidencias de la transferencia de conocimiento**
- **Firma del cliente** en el documento de aceptación final

---

## Ideas para llevar

- La planificación adaptativa requiere una **re-planificación constante** para adaptar el proyecto a necesidades cambiantes
- Los cambios se realizan mediante el **refinamiento del backlog** — incorporando, modificando o eliminando HU
- La experiencia del **MVP** y la retroalimentación de *stakeholders* son aportes valiosos para la adaptación
- El **MVI** permite agregar valor en los términos más convenientes para la organización
- El **modelo Kano** es una excelente herramienta para conocer preferencias de clientes y determinar el MVI
- Las **lecciones aprendidas** son el método más eficaz para aplicar experiencias a futuras situaciones — tanto explícitas como tácitas

---

## Bibliografía

- Cobb, C. (2011). *Making Sense of Agile Project Management. Balancing control and agility*. Editorial Wiley.
- Griffiths, M. (2018). *PMI-ACP® Exam Prep*. RMC Publishing. Updated Second Edition.
- Kano, N. (1989). *Continuos Improvement: Quality Control in Circles in Japanese Industry Volume 19*. U of M Center for Japanese Studies.
- Lawrence, C. (2021). *The Engineer's Complete Guide to Backlog Grooming*. Stepsize.
- Project Management Institute. (2021). *Guía de los Fundamentos para la Dirección de Proyectos. PMBOK Guide*. 7a edición. Pp. 151.
- Roldán, N. (2020). *Modelo de Kano*. Economipedia.
