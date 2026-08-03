# DevOps DevSecOps

> PDF: [[documentation/07. Value Driven Delivery/DevOps DevSecOps.pdf|Ver PDF original]]

---

DevOps / DevSecOps
Conoce los requerimientos adicionales para asegurar
la generación de valor, las ventajas y los retos que
representan.


Requerimientos
adicionales para
generar valor
Pensando nuevamente en nuestro ejemplo del desarrollo de
un sistema administrativo para la empresa, hemos hablado ya
bastante sobre realizar pruebas constantes y frecuentes para
asegurar la calidad de nuestro código, también hemos comentado
sobre la retroalimentación constante y frecuente para validar y
verificar con nuestros usuarios la generación de valor, es decir,
que el sistema que estamos generando está proporcionando la
funcionalidad requerida, la seguridad necesaria, la practicidad
y facilidad de uso solicitadas, y también hemos hablado de lo
que es TDD, que consiste en desarrollar el código con base en
las pruebas y sus resultados esperados, ya que todo esto se define
antes de iniciar la generación del código.

DevOps / DevSecOps

Todo lo anterior es importante para generar valor, es decir, generar código que funcione como se requiere y de manera sencilla,
práctica y eficiente, pero hay dos requerimientos adicionales que deben cumplirse para asegurar que estamos generando el
valor requerido por la empresa.

DevOps

El primero de estos requerimientos está relacionado con el objetivo de agilizar los
procesos para transformar una idea o un requerimiento en una pieza de software
estable para generar valor al usuario o a la organización: a esto se le conoce
como DevOps.

DevSecOps

El segundo de estos requerimientos adiciona lo relacionado con la seguridad, o
DevSecOps, con el fin de proporcionar piezas de software que cumplan con los
requerimientos de seguridad, y que a lo largo del tiempo puedan integrar fácilmente
nuevos requerimientos en esta importante área.

Retomando nuestro ejemplo del desarrollo del sistema administrativo para la empresa, tú, en tu rol de Agile Project Leader,
tienes que comunicarte constantemente con el equipo de operaciones y el de seguridad de tu organización, lograr que tu equipo
de trabajo colabore con estas dos áreas de tu empresa, de tal forma que logren que el nuevo sistema sea seguro, eficiente y
también estable, y que durante su desarrollo, se realicen integraciones constantes de las funcionalidades solicitadas.

DevOps / DevSecOps

¿Qué es DevOps?
DevOps es una práctica relacionada con la ingeniería
de software que se caracteriza por integrar los
requerimientos de las áreas de desarrollo
y de operaciones de TI de la organización.
DevOps no es un conjunto de herramientas, ni un estándar,
ni un producto, pero sí aprovecha las ventajas de varios
productos y herramientas para lograr sus objetivos. El
objetivo de DevOps es considerar y unificar los
requerimientos de ambas áreas de TI. En el caso del
área de desarrollo, un objetivo básico es lograr desarrollos
y liberaciones rápidas y de calidad, que generen valor a
los usuarios. En el caso del área de operaciones de TI,
el objetivo es la estabilidad de los sistemas, ya que esto
es un punto básico para generar valor a los usuarios.

DevOps / DevSecOps

La práctica de DevOps plantea los siguientes objetivos:
a) Mejorar la velocidad para desarrollar, probar y liberar
a producción el código.
b) Minimizar la ocurrencia de errores al generar nuevas
versiones.
c) Minimizar el tiempo entre generación de nuevas
versiones.
d) Minimizar el tiempo de liberación al ambiente
productivo.
e) Minimizar el tiempo de reacción cuando se presentan
fallas.

Como lo hemos comentado, DevOps no es una herramienta,
pero sí utiliza herramientas para automatizar los procesos
con los que se relaciona, por ejemplo, algunas herramientas
apoyan la automatización en temas relacionados con la
generación de código como, por ejemplo:
a) Generar código
b) Realizar pruebas
c) Reporte de problemas
d) Análisis de código para resolución de problemas
e) Corrección de defectos
Ejemplos de algunas herramientas que sirven para esto son:
Jenkins, Maven, Gradle, Bamboo, Team City, etc. Estas
herramientas de automatización permiten ahorrar
tiempo y minimizar errores humanos, fomentan la
integración continua y el deployment continuo. Toma en
cuenta que con las prácticas de DevOps no se busca un Big
Bang, sino la integración continua de las funcionalidades
requeridas, es decir, se busca aprovechar la reutilización
y la escalabilidad del código.
Un aspecto básico de DevOps es el monitoreo proactivo,
durante el cual, tanto el equipo de operaciones, como el de

DevOps / DevSecOps

desarrollo, reciben información de este monitoreo, con el
fin de que analicen y encuentren la causa de los problemas
o posibles riesgos, los mitiguen y resuelvan lo antes posible
y de manera proactiva, no reactiva.
Para lograr los objetivos antes mencionados, las prácticas
de DevOps se basan en el uso de microservicios, es decir,
ya no se desarrollan aplicaciones monolíticas que son
difíciles de mantener y actualizar. Los microservicios,
por el contrario, se basan en la creación de entidades
simples y sencillas, con mantenimiento sencillo,
tecnológicamente flexibles, con una estabilidad
óptima, y que sean escalables.
Los microservicios están débilmente acoplados (loosely
coupled) e interactúan a través de APIs (Application
Programming Interface), además, se diseña una
arquitectura de microservicios específica para el caso en
cuestión. Estos microservicios pueden ser creados en
diferentes entornos y construirse con diferentes
herramientas, lenguajes o tecnologías. También
pueden ejecutarse en diferentes nodos, esto aumenta de
manera importante la modularidad, la cual aporta al
logro de los objetivos de DevOps.

También se requieren herramientas para realizar
y automatizar funciones como:
a) La construcción del código
b) Virtualización y contenerización
c) Gestión de las configuraciones
d) Monitoreo
e) Orquestación

R

Dev
il
DevOps / DevSecOps

Ops
Te

st

on

M

Bu

d

De

i to

r

te

Cod
e

se
a
e
l
e

y
plo

Pla
n

Como se ha comentado, existe una gran variedad de
herramientas en el mercado, y el área de TI de cada
organización, selecciona las más adecuadas con base en
diversos criterios como facilidad de uso, plataformas
soportadas, etc. Tú, en tu rol de Agile Project Leader
necesitas entender qué herramientas ha seleccionado tu
empresa para estos fines, validar que tu equipo cuente con
el entrenamiento requerido, que entiendan los objetivos de
DevOps y que trabajen de manera colaborativa y constante
con los equipos del área de operaciones, para que al final,
el sistema administrativo que estás desarrollando, cumpla
con las características mencionadas.

Op

a
r
e

¿Qué es DevSecOps?

R

Dev
il
DevOps / DevSecOps

Ops
Te

st

on

M

Bu

d

De

i to

r

te

Cod
e

e
s
a
e
el

y
plo

Pla
n

Sec

Op

a
r
e

El siguiente paso es integrar las prácticas de seguridad
con el desarrollo y las operaciones, de tal forma que, el
código que se vaya desarrollando, además de cumplir
con las prácticas de DevOps, integre también las
prácticas de seguridad establecidas en la
organización o a nivel industria.
La práctica de DevSecOps también integra la ejecución
de pruebas de seguridad en cada fase del proceso
de desarrollo de software y, al igual que DevOps,
DevSecOps también utiliza herramientas y procesos que
promueven la colaboración entre los desarrolladores, los
especialistas de seguridad y los equipos de operaciones
de la organización, con el fin de construir aplicaciones
seguras, estables y eficientes.

Ventajas

Al aplicar las prácticas de DevOps y de DevSecOps
en la organización todos ganan y se termina la
rivalidad que siempre había existido entre las áreas
de desarrollo, operaciones y seguridad de las
empresas. Pero ¿por qué existía esta rivalidad?
Porque cada área veía solamente su objetivo:

DevOps / DevSecOps

Al área de desarrollo le interesaba
solamente entregar rápido los sistemas
porque siempre los presionaban y
siempre recibían quejas por retrasos.

El área de operaciones quería sistemas
estables, no le gustaba el hecho de que
el área de desarrollo liberara un código
que fallara, de que tomaran mucho
tiempo para arreglarlo, y tardaran en
entregar nuevas versiones, además de
que la liberación de cada nueva versión
era toda una pesadilla.

La prioridad del área de seguridad
era realizar pruebas y asegurar que
el código incluyera los requerimientos
de seguridad antes de ser liberado
a producción, y también tener la
tranquilidad de que el código sería
actualizado, siempre que surgieran
nuevos requerimientos de seguridad.

Retos
Como puedes ver, todos estos objetivos se contraponen,
pero ahora, gracias a las prácticas de DevOps y
DevSecOps, se integran.

• ¿Cómo se vería beneficiada la empresa en la que laboras
con la implementación de las prácticas de DevOps y de
DevSecOps?

Las arquitecturas de microservicios no están siendo usadas
todavía en muchas organizaciones, además, introducir estas
prácticas y arquitecturas no es un tema sencillo, sin
embargo, es de gran importancia para que la organización
cuente con una estrategia adecuada de TI que le permita
flexibilidad, seguridad, estabilidad y adaptabilidad en sus
aplicaciones, lo cual es básico para la supervivencia y el
crecimiento de la organización.

• ¿Cómo plantearías un proyecto de modernización
en tu empresa para adoptar estas prácticas?
• ¿Cuáles son los primeros pasos que deberías plantearte?

Descarga el documento desde el apartado
de "Archivos adjuntos" de la plataforma.

Ahora que has visto cómo se integran las prácticas de
DevOps y DevSecOps, reflexiona:

DevOps / DevSecOps
