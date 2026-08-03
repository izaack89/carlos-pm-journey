# APL_SC2.2_version_impresa_L6

> PDF: [[documentation/07. Value Driven Delivery/APL_SC2.2_version_impresa_L6.pdf|Ver PDF original]]

---

Value Driven Delivery
Lección 2: Validando la generación de valor
Introducción
Validando la generación de valor
¿Te ha sucedido lo siguiente?
En tu rol de Agile Project Leader tú y tu equipo de trabajo, se reúnen con el
cliente para comprender los requerimientos del proyecto.
Agendan reuniones con el equipo de TI, con los usuarios finales, con el
equipo de seguridad y, en general, con varias áreas de la organización para
recolectar y analizar sus requerimientos.
Todos se sienten tranquilos porque los requerimientos fueron
recolectados, documentados y analizados. Inician entonces el diseño y el
desarrollo del nuevo sistema seguros de que el proyecto será todo un éxito.
Al final, el cliente no rechaza el nuevo sistema, pero te pide cambios y
ajustes.
Esta es una situación muy común, ¿pero por qué sucede?, ¿fue un error de
tu equipo o fue un error del cliente?
Este problema te generará costos adicionales porque tú y tu equipo
tendrán que realizar trabajo adicional que no tenían considerado;
adicionalmente, el sistema no estará listo para usarse productivamente en
la fecha inicialmente estimada.
¿Puedes tú como Agile Project Leader hacer algo para evitar este problema
o, al menos, minimizarlo?


Veamos cómo a través de la validación constante de valor puedes
enfrentar esta situación y evitar este tipo de problemas.


Pruebas constantes, frecuentes y retroalimentación
Para visualizar este contenido, dirigirte a la sección de “Archivos
adjuntos” del recurso Pruebas constantes, frecuentes y
retroalimentación.


Integración continua
Ahora vamos a revisar el desafío que representa la integración del código,
así como sugerencias
para la implementación de la integración continua, y su aplicación en las
empresas.
El problema de la integración del código
Retomemos el ejemplo del desarrollo del sistema administrativo para la
empresa en la que laboras. Tú, en tu rol de Agile Project Leader, diriges al
equipo de desarrollo; es un sistema bastante grande, te han asignado 16
desarrolladores. Cada desarrollador selecciona del backlog una
característica a desarrollar, y trabaja en generar el código correspondiente.
Todos los desarrolladores trabajan y al final del sprint, que dura
aproximadamente dos semanas, integran todo el código y entran en la
etapa a la que muchos desarrolladores llaman integration hell, el infierno
de la integración.
¿Por qué supones que le dan este nombre a esta etapa del desarrollo de
una aplicación? Muy probablemente te ha tocado vivir esta experiencia y
has visto que, al integrar el código de todos los desarrolladores y realizar
una prueba del código unificado, surgen errores e inconsistencias.
Cada desarrollador realizó pruebas a su código, sin embargo, las pruebas
del código integrado muestran que hay muchas fallas. La mayoría de estas
fallas surgen precisamente de las inconsistencias generadas durante la
integración del código.
Aunque los desarrolladores conocen y siguen los estándares definidos
para su trabajo, es imposible evitar totalmente estas inconsistencias y
estas fallas. ¿Y qué podemos hacer entonces, si hemos dicho que es
imposible evitar totalmente esta situación?
Integración continua


La integración continua es la respuesta al problema anterior. No va a
eliminar estas
fallas, pero sí ayudará a minimizar los efectos negativos, así como a que
las correcciones requeridas en esta etapa de integración se realicen con
mayor facilidad y en un menor tiempo, ¿quieres ver cómo lograr esto?
En el área de la ingeniería de software y desarrollo de software se aplica
con éxito la práctica llamada Integración Continua, la cual consiste en
incorporar al repositorio de código, con la mayor frecuencia posible, el
código nuevo y/o código modificado. De esta manera, el código es
compilado y probado de manera automática cada vez que un desarrollador
confirma la integración de su nuevo código en el control de versiones.
El objetivo es realizar este proceso con la mayor frecuencia posible ya que,
de esta manera, los cambios, las pruebas y las correcciones se realizan
sobre porciones pequeñas de código, lo cual facilita el trabajo de los
desarrolladores y lo hace más eficiente. Una buena práctica es realizar la
integración y las pruebas al menos una vez al día.
Veamos ahora cómo aplicaría todo esto a nuestro ejemplo: el equipo
necesitará definir cómo integrarán el código generado y cómo realizarán
las pruebas para validar que funciona adecuadamente. También necesitará
herramientas para automatizar el proceso.
Existen en el mercado varias herramientas o sistemas de integración
continua que ayudan a automatizar este proceso, en general estas
herramientas contienen los siguientes elementos básicos:
• Repositorio de código: Este elemento del sistema es el lugar donde se
integra el código que es desarrollado y modificado por tu equipo de
trabajo.
• Sistema de control de versiones: Este componente se encarga de realizar
el control de versiones para el código que está siendo desarrollado o
modificado.


• Herramientas de construcción: Es el conjunto de herramientas que el
desarrollador utiliza para crear su código y compilarlo, son ambientes
integrados de desarrollo o IDEs (Integrated Development Environment).
• Herramientas de pruebas: Estas herramientas se encargan de realizar las
pruebas unitarias al código. Las pruebas son programadas usando estas
herramientas.
• Iniciador de pruebas: Este componente inicia las pruebas cada vez que un
desarrollador confirma un nuevo código o código modificado a través de
una instrucción commit, es decir, la confirmación de un conjunto de
cambios provisionales. En algunos casos se programa el inicio de las
pruebas con base en intervalos de tiempo, por ejemplo, cada hora.
• Reporteador de resultados incorrectos: Este componente se encarga de
notificar al equipo cuando las pruebas realizadas no son satisfactorias, se
puede hacer a través de un correo electrónico.
Proceso automatizado

Resultado no
Errores
satisfactorio
Tu equipo de
Cuando el resultado no Cuando se corre una
desarrolladores utiliza es satisfactorio, es decir, prueba y surgen errores,
las herramientas de
las herramientas de
los responsables de
construcción y crea o
prueba detectan que los revisar el código y
modifica el código
resultados obtenidos no corregir los errores
correspondiente a las son los esperados,
inmediatamente son los
características que está entonces el reportador desarrolladores que
desarrollando y lo
de resultados genera
confirmaron el código
coloca en el repositorio, una notificación para el antes de la prueba.
y cada vez que ellos
equipo de
=
confirman su código por desarrolladores.
Así, el equipo trabaja de
medio de un commit,
=
manera colaborativa y
inicia el proceso
siempre tienes un
automatizado.
Tu equipo trabaja
código deployable, es
=
entonces en las
decir, un código que


Se actualiza la
correcciones necesarias puede ser migrado al
información sobre las y el proceso se repite
ambiente productivo ya
versiones del código, se hasta que en las pruebas que debe estar funcional
utilizan las herramientas se obtengan resultados en todo momento.
de prueba para realizar satisfactorios.
las pruebas que se han
programado en estas
herramientas.
Como puedes ver, es un proceso constante y es más sencillo realizarlo de
esta manera, en lugar de esperar el ciclo del sprint, es decir, en el que
después de dos semanas intentas integrar todo el código y tomaría
bastante tiempo y esfuerzo encontrar y corregir los errores, serían más
errores y más código el que hay que revisar.


Aplicación y sugerencias de implementación
Ahora vas a revisar sugerencias para la implementación de la integración
continua y su aplicación en las empresas.
Aplicación en las empresas
Muchas personas están a favor de un sistema de integración continua,
dado que automatiza las pruebas y el control de versiones, por tanto, los
desarrolladores se concentran en la creación o modificación de su código,
y de manera constante, reciben retroalimentación con los resultados de las
pruebas.
Con esta forma de trabajo los desarrolladores pueden realizar ajustes y
correcciones de manera constante y sobre porciones pequeñas de código,
todo esto agiliza el proceso de desarrollo. Sin embargo, algunas personas
opinan que no vale la pena la inversión inicial de tiempo requerida para
preparar el ambiente y el sistema de integración continua, incluyendo la
programación de las pruebas. Adicionalmente, consideran que no es
práctico tener recursos dedicados al sistema de integración.
En las organizaciones, las áreas de desarrollo toman decisiones sobre las
prácticas que quieren implementar para realizar su trabajo, ¿qué aspectos
considerarías tú y qué criterios establecerías para tomar esta decisión en
la empresa en la que laboras?
La integración continua puede aportar mejoras a la práctica de DevOps,
más adelante revisaremos este concepto, ya que se trata de una práctica
implementada en muchas empresas.
Sugerencias para su implementación:
¿Y qué requieres para implementar la integración continua? A continuación,
revisaremos algunas sugerencias generales que te ayudarán a una exitosa
implementación:
1. Mantener un único repositorio de código:


Gestionar adecuadamente los archivos de código usados para construir
el sistema administrativo para tu empresa te facilitará el trabajo de
desarrollo y también la distribución a otros ambientes o la liberación a
producción.
2. Automatizar los procesos de construcción y pruebas:
Esto facilitará el trabajo de los desarrolladores, trabajarán de manera
más eficiente y se enfocarán en la construcción y corrección del código.
3. Realizar las pruebas en un ambiente lo más parecido posible al
ambiente de producción
De esta manera minimizas los riesgos de errores causados por las
diferencias entre ambientes.
4. Implementar los ambientes necesarios para el proceso
Podría ser un ambiente de desarrollo, uno de pruebas y otro de
producción, o podrías agregar un ambiente de calidad, por ejemplo.
También es importante automatizar las liberaciones a cada ambiente.
5. Revertir código y analizarlo
Los desarrolladores que confirman (commit) código son responsables de
revertirlo y analizarlo para corregir en caso de que las pruebas
correspondientes no sean exitosas, se sugiere que inicien estas acciones
en cuanto se reportan los resultados desfavorables de las pruebas.
6. Asegurar realización de pruebas unitarias
Tus desarrolladores deben realizar pruebas unitarias de su código antes
de realizar el commit.
Ahora que has revisado lo que involucra la integración continua, reflexiona:
• Si tú has implementado la integración continua, ¿qué otros puntos
recomendarías para maximizar la probabilidad de una implementación
exitosa?


• ¿Qué ventajas aportaría la integración continua al proceso de desarrollo de
aplicaciones en tu empresa?
• ¿Qué retos consideras que podrías enfrentar si implementas la integración
continua en la empresa en la que laboras?


DevOps / DevSecOps
Para visualizar este contenido, dirigirte a la sección de “Archivos
adjuntos” del recurso DevOps / DevSecOps.


Ideas para llevar
Hagamos un resumen de lo que te llevas en esta lección.
Ahora que has terminado de revisar esta lección, ¿qué te llevas sobre la
implementación de metodologías ágiles?

Bibliografía
• Anastasov, M. (2021). Continuous Integration (CI) explined.

Semaphore. https://semaphoreci.com/continuous-integration

• Griffiths, M. (2015). PMI-ACP Exam Prep (2a edición 128-136).
RMC Publications, Inc.

• Hall, T. (s.f.). DevOps best practices. Atlassian.

https://www.atlassian.com/devops/what-is-devops/devops-bestpractices

• Minick E., (s.f.). What is Continuous Integration. IBM.

https://www.ibm.com/topics/continuous-integration
