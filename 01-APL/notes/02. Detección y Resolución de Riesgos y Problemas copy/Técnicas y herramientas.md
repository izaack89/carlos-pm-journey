# Técnicas y herramientas

> PDF: [[documentation/02. Detección y Resolución de Riesgos y Problemas copy/5.1 Técnicas y herramientas.pdf|Ver PDF original]]

---

Técnicas y herramientas


Javier ha dedicado tiempo para analizar la experiencia en
otros proyectos y ha identificado la importancia de gestionar
riesgos con base en la experiencia adquirida para lo cual
requiere identificar la prioridad de atención y está
comparando las herramientas apropiadas para ello.

Técnicas y herramientas

Matriz de probabilidad e impacto
La matriz de probabilidad e impacto es una herramienta que se utiliza para evaluar la probabilidad de ocurrencia de los
riesgos con su impacto sobre los objetivos del proyecto en el caso de que se materialicen. La matriz específica las combinaciones
de probabilidad e impacto en diferentes cuadrantes que representan un nivel de prioridad con lo cual se pueden asignar
prioridades a los riesgos con la finalidad de focalizar esfuerzos de análisis y definición de respuestas, el resultado es la
ubicación de los riesgos en cuadrantes que permiten clasificarlos típicamente como Muy Alto, Alto, Moderado, Bajo y Muy
Bajo.
A continuación, se muestra un ejemplo de una matriz de probabilidad e impacto:
MA
A
M
B
MB

Oportunidades

MA

B

M

M

A

A

A

A

M

M

B

B

B

M

A

A

A

A

M

B

B

B

B

M

A

A

A

A

M

B

B

B

B

B

M

A

A

M

B

B

B

B

B

B

B

M

M

B

B

B

B

MB

B

M
Impacto

A

MA

MA

A

M
Impacto

B

MB

A
M
B
MB

Probabilidad

Probabilidad

Amenazas

Figura 2.1 Ejemplo de Matriz de Prioridad e Impacto. Fuente: Elaboración propia.

Técnicas y herramientas

Se puede usar una escala numérica para cada elemento de la clasificación con la finalidad de facilitar un cálculo automatizado,
por ejemplo, en una hoja de datos:
Probabilidad

Escala

Impacto

Escala

MA

MA

A

A

M

M

B

B

MB

MB

Figura 2.2 Ejemplo de escala numérica para probabilidad e impacto. Fuente: Elaboración propia.

Un ejemplo en el que podemos aplicar la escala de probabilidad/impacto es el siguiente:
Clave Probabilidad Impacto

Descripción del riesgo

R01

Si no se instalan los servidores en la primera semana de mayo entonces se tendrá un desfase en la instalación
de la solución de un mes.

R02

Si no se cuenta con participación de los usuarios en la ejecución de pruebas de UAT desde la 1er semana de
mayo a la primer semana de junio entonces no se podrá cerrar la etapa de pruebas.

Técnicas y herramientas

Clave Probabilidad Impacto

Descripción del riesgo

R03

Si no se cuenta con el VoBo del área de arquitectura a los mecanismos de cifrado de datos sensibles,
entonces no se podrá programar la instalción de la solución en el ambiente productivo.

R04

Si no se cuenta con el set de datos de prueba en la última semana de abril las pruebas de UAT se retrasarán y
la disponibilidad de usuarios tendrá que reprogramarse.

R05

Si no se cuenta con la liberación de presupuesto restante del proyecto durante las pruebas de UAT entonces
se retrasará el último pago al proveedor y el periodo de garantía puede verse comprometido.

Figura 2.3 Ejemplo de lista de riesgos clasificada en probabilidad e impacto. Fuente: Elaboración propia.

R04


R02


Oportunidades

R01

R03

R05

Impacto

Impacto

Probabilidad

Probabilidad

Amenazas

Figura 2.4 Ejemplo de matriz de Probabilidad e Impacto bajo con escala numérica y riesgos identificados. Fuente: Elaboración propia.

Técnicas y herramientas

El Estándar para la Gestión de Riesgos en portafolios, programas y proyectos publicado por el Project Management Institute,
página 139 lista una serie de características adicionales a la probabilidad e impacto que se pueden usar para complementar la
priorización de los riesgos para su posterior análisis y definición de acciones:
Acción

Definición

Urgencia

Periodo dentro del cual se debe implementar una respuesta a un riesgo con el objetivo de ser efectiva.
Un periodo breve indica una urgencia elevada.

Proximidad

Es el periodo antes de que el riesgo pudiera tener un impacto sobre uno o más objetivos. Un periodo
breve indica una elevada proximidad.

Detectabilidad

Facilidad con que se pueden detectar y reconocer los resultados de que un riesgo ocurra o esté a
punto de ocurrir. Cuando la ocurrencia del riesgo se puede detectar fácilmente, la detectabilidad es
alta.

Inactividad

Periodo que puede transcurrir después de ocurrido el riesgo, antes de que se descubra su impacto. Un
periodo breve indica una baja inactividad.

Manejabilidad

Facilidad con la que un dueño del riesgo puede gestionar la aparición o el impacto del riesgo. Cuando
la gestión es fácil, la manejabilidad es alta.

Controlabilidad

Es el grado en que un dueño del riesgo sea capaz de controlar el resultado de este. Cuando el
resultado implica que se puede controlar fácilmente la controlabilidad es alta.

Técnicas y herramientas

Acción
Conectividad

Definición
Medida en que un riesgo está relacionado con otros riesgos individuales. Cuando un riesgo está
conectado con muchos otros riesgos la conectividad es alta.

Impacto estratégico La posibilidad de que un riesgo tenga un efecto positivo o negativo sobre los objetivos estratégicos de
la organización. Cuando un riesgo tiene un efecto importante sobre los objetivos estratégicos, el
impacto es alto.
Impacto sobre
interesados

El grado en que se percibe que un riesgo importa por parte de uno o más interesados. Cuando un
riesgo es percibido como muy significativo, el impacto sobre los interesados es alto.
Figura 2.5 Otros parámetros para priorizar riesgos. Fuente: Elaboración propia.

Técnicas y herramientas

Una estrategia para realizar el análisis cualitativo consiste en tener una sesión de trabajo con el equipo para que cada
uno comente sobre situaciones los problemas que enfrentaron en proyectos similares, con ello es posible aplicar la técnica
“análisis de afinidad” para asociar las contribuciones y así tener un mapa más compacto. En las siguientes imágenes se puede
apreciar un ejemplo sobre la evolución del análisis de riesgos aplicando el análisis de afinidad:
El no contar con
la aceptación de
entregables
implicó
retrabajo

Los
requerimientos
de usabilidad se
fueron
definiendo
sobre la marcha

Los usuarios
indicaron que no
era lo que
esperaban

Las HU’s eran
más complejas
de lo esperado

El equipo no
tenía la
experiencia
técnica
necesaria

El equipo no era
suficiente para
cumplir con los
compromisos
del Sprint

Figura 2.6 Ejemplo de análisis de problemas. Fuente: Elaboración propia.

Técnicas y herramientas

Aplicando el análisis de afinidad tenemos lo siguiente:
Equipo de trabajo
Requerimientos

Los
requerimientos
de usabilidad se
fueron
definiendo
sobre la marcha

Los usuarios
indicaron que no
era lo que
esperaban

El equipo no
tenía la
experiencia
técnica
necesaria

El no contar con
la aceptación de
entregables
implicó
retrabajo
Las HU’s eran
más complejas
de lo esperado

El equipo no era
suficiente para
cumplir con los
compromisos
del Sprint

Operación
Figura 2.7 Ejemplo de análisis de afinidad. Fuente: Elaboración propia.

Técnicas y herramientas

El siguiente paso consiste en definir un identificador y asignar la probabilidad de ocurrencia y el impacto que se puede tener
basado en la experiencia del equipo, las escalas a manera son las definidas en la estrategia de gestión de riesgos:
Probabilidad / Impacto: Muy Alto, Alto, Medio, Bajo, Muy Bajo
Equipo de trabajo
R05

R01
Requerimientos

R02

R03

Los
requerimientos
de usabilidad se
fueron
definiendo
sobre la marcha
P: MA I: MA

El no contar con
la aceptación de
entregables
implicó
retrabajo

Los usuarios
indicaron que no
era lo que
esperaban

El equipo no
tenía la
experiencia
técnica
necesaria

P: B I: MA

P: B I: M
R06
R04

P: M I: A
Las HU’s eran
más complejas
de lo esperado
Operación

El equipo no era
suficiente para
cumplir con los
compromisos
del Sprint
P: A I: MA

P: B I: MB

Figura 2.8 Ejemplo de asignación de probabilidad e impacto. Fuente: Elaboración propia.

Análisis cualitativo

Finalmente generamos la matriz de amenazas y oportunidades:

Oportunidades
R03

R03


R02
R04

R05

R01

Impacto

Impacto

Probabilidad

Probabilidad

Amenazas

Figura 2.9 Segundo ejemplo de Matriz de amenazas y oportunidades. Fuente: Elaboración propia.

Técnicas y herramientas

Al realizar el análisis cualitativo de riesgos, la lista de riesgos se complementa asignando un responsable a cada riesgo quien se
encargará de la atención, resolución y rendición de cuentas.
Clave Probabilidad Impacto

Descripción del riesgo

Responsable

R01

Los usuarios indicaron que no era lo que esperaban.

John Do

R02

El no contar con la aceptación de entregables implica retrabajo.

John Do

R03

Los requerimientos de usabilidad se definen sobre la marcha.

John Do

R04

No tener licencias suficientes para acceder al repositorio del proyecto.

John Do

R05

El equipo no tiene experiencia técnica necesaria.

John Do

R06

El equipo no es suficiente para cumplir con los compromisos de los Sprints.

John Do

Figura 2.10 Ejemplo de Lista de riesgos. Fuente: Elaboración propia.

Recuerda revisar y comparar las diferentes técnicas y herramientas que te pueden ayudar para realizar el análisis cualitativo de
riesgos. Sigamos adelante.

Descarga el documento desde el apartado
de "Archivos adjuntos" de la plataforma.

Técnicas y herramientas
