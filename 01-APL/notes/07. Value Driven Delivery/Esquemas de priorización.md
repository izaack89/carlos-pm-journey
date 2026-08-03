# Esquemas de priorización

> PDF: [[documentation/07. Value Driven Delivery/Esquemas de priorización.pdf|Ver PDF original]]

---

Esquemas de priorización
Conoce los principales esquemas de priorización, para
que puedas decidir cuál es el que te conviene utilizar
en tus proyectos.


Principales esquemas de priorización
y su funcionamiento
MoSCow. El nombre de este esquema es un acrónimo que se genera a partir de las siguientes frases en idioma inglés,
observa a detalle la siguiente tabla.

“Must have”

“Should have”

“Could have”

“Would like but not
this time” o “Won’t
have”

“Debe tener”

“Debería tener”

“Podría tener”

“Me gustaría, pero no lo tendrá”

Son requisitos
esenciales

Requisitos importantes,
pero no esenciales

Representan mejoras
al producto

Deseables, pero no
justificable

• Indispensable
• Sin alternativa
• Sin sustituto

Esquemas de priorización

• Deseable

• No indispensable pero
importante

• No indispensable,
importancia relativa

• Se puede sustituir

• Agrega valor algunas veces

• Agrega valor siempre

• Tiene alternativas

• No se justifica por
costo-beneficio

Ejemplo de esquema
MoSCoW
Para entender esto mejor, retoma el ejemplo del sistema
administrativo que viste en la lección 2, y toma específicamente
el módulo de administración de información de clientes. Vamos
a suponer que tenemos aquí la lista de características a evaluar,
podrían ser historias de usuario, pero vamos a usar una lista de
características.

¿En qué clasificación pondrías características como: validación del código postal de la dirección, funcionalidad
para validar tipo de empaque preferido por el cliente, etc.?
Definitivamente esa decisión la deben tomar las personas que serán usuarios y/o dueños del producto final, con base en sus
necesidades y requerimientos, pero podríamos proponer lo siguiente.

“Must have”
• Validación de clientes
duplicados
• Validación de código
postal en la dirección

“Should have”

“Could have”

“Would like but not
this time” o “Won’t
have”

• Funcionalidad para
captura y validación
de mapa de ubicación

• Funcionalidad para
validar tipo de empaque
que prefiere el cliente

• Captura de color de
envoltura preferido
por el cliente

En este caso te enfocarías en implementar primero las historias o características que se encuentran en la clasificación “Must
have”, después las que quedaron en la categoría de “Should have” y así sucesivamente hasta terminar con las que se incluyeron
en la categoría “Would like but not this time” o “Won't have”. Recuerda que al terminar cada iteración se revisa de
nuevo la priorización del backlog y podría haber cambios.

Esquemas de priorización

Monopoly Money
Este segundo esquema es también sencillo y bastante aceptado
entre los equipos de trabajo
Consiste en listar las características
del producto y asignar a los interesados
una cierta cantidad de “dinero”. Ellos
deberán asignar montos de ese “dinero” a
cada característica o historia de usuario,
sin sobrepasar la cantidad total asignada.
Tomemos nuevamente el ejemplo del módulo
de administración de información de clientes,
podríamos generar este listado y suponer que
los interesados han asignado así los montos de
un total de 1,350 pesos, revisa la distribución
a continuación.

Esquemas de priorización

Característica o funcionalidad

Monto
asignado

Validación de clientes duplicados

Captura de color de envoltura preferido por el cliente

Funcionalidad para captura y validación de mapa
de ubicación

Validación de código postal en la dirección

Funcionalidad para validar tipo de empaque que
prefiere el cliente

De esta manera, estarías dando prioridad a la implementación de clientes duplicados y a la validación del
código postal en la dirección.
Funciona bien este esquema si se consideran solamente características de negocio, es decir, sin incluir temas como documentación
del sistema, por ejemplo. Esos temas pueden ser evaluados posteriormente como requerimientos no funcionales, con el área
adecuada - tal vez el área de tecnología -, usando este mismo método.

Método de los 100 puntos
Es un esquema también
bastante práctico
Consiste en asignar a cada interesado 100 puntos, para
que los reparta entre las diferentes características,
funcionalidades, o historia de usuario, como ellos lo
consideren adecuado, de esta forma, estarán votando por
cada elemento de la lista.
Tomando el mismo ejemplo, podríamos tener la siguiente
distribución.

Esquemas de priorización

Característica o
funcionalidad

Puntos asignados
por el interesado Total

Validación de clientes
duplicados

Captura de color de envoltura
preferido por el cliente

Funcionalidad para captura y
validación de mapa de ubicación

Validación de código postal
en la dirección

Funcionalidad para validar tipo
de empaque que prefiere el
cliente

Votación por puntos o multi-votación
Ese esquema es similar al de Monopoly Money, pero en lugar de asignar una cantidad de “dinero” a cada interesado, asignas
puntos, votos, o estrellas y cada interesado colocará en cada característica o funcionalidad las estrellas que
considere adecuadas y al final serán sumadas; por ejemplo, supongamos que asignas 15 estrellas a cada participante y
ellos distribuyen esas estrellas de la siguiente manera.

Característica
o funcionalidad
Validación de clientes duplicados

Puntos asignados
por el interesado Total

***** ***** ******

*

Captura de color de envoltura
preferido por el cliente
Funcionalidad para captura y
validación de mapa de ubicación

***

***

**

Validación de código postal
en la dirección

****** ****

*****

Funcionalidad para validar tipo de
empaque que prefiere el cliente
Esquemas de priorización

*

**

**

Darás mayor prioridad a las características o historias
que tengan un mayor número de votos o estrellas. La
votación puede realizarse de manera pública o privada.
¿Qué ventajas verías en realizarla de una forma o de
la otra? Por lo general se recomienda que sea privada para
evitar que los primeros votos ejerzan influencia sobre los
últimos. Algunos autores sugieren que, para determinar
la cantidad de estrellas o votos a ser asignadas a cada interesado,
se use el 20% del total de elementos a ser evaluados,
por ejemplo, si tienes 100 elementos, estarías asignando 20
estrellas a cada interesado (100 X 0.2 = 20).
Este es un enfoque práctico.

Business Value / Story Points
Este esquema de priorización consiste en asignar a cada historia de
usuario o a cada característica del producto, dos valores o dos números:
• El primer número indica el valor que esa historia
tiene para el negocio, se puede definir una escala de 1 a
10 donde un número más alto significa que esa historia
tiene un mayor valor para la empresa, es decir, si se
asigna un valor de 10 para una historia, significa que esa
historia tiene el máximo valor posible para la organización.
•
• Puede definirse también una escala de 1 a 3 donde se
indique que 1 significa un valor bajo, 2 significa un valor
medio, y 3 significa un valor alto para el negocio.
•
• El segundo número es una medida del esfuerzo
que se requiere para implementar esa historia
de usuario. En este caso se puede utilizar la cantidad de
story points asignados a dicha historia. Recuerda que los

Esquemas de priorización

story points los determinan los desarrolladores de
tu equipo, ellos evalúan la dificultad o el esfuerzo que ellos
estiman será requerido para la implementación de cada
historia, asignando una mayor cantidad de story points a
las historias que requerirán un mayor esfuerzo. Por lo tanto,
los story points son útiles para el fin que perseguimos con
este esquema.
Una vez que se determinan esos dos valores para
cada historia, se procede a dividir el valor de negocio
de cada historia entre los story points asignados,
y las historias con mayor cociente, son las que se
seleccionan para ser implementadas primero.

Prioridad de historias =

Valor para el negocio
Story Points

Veamos nuevamente nuestro ejemplo, aplicando ahora este esquema, supongamos que para este ejemplo usaremos una escala
del 1 al 10 para que los usuarios asignen el valor de negocio a cada característica o funcionalidad requerida para este módulo.

Valor para el negocio
(determinado por el
usuario)

Story Points
(asignados por los
desarrolladores)

Resultado de la
división

Validación de clientes
duplicados

Captura de color de envoltura
preferido por el cliente

0.33

Funcionalidad para captura y
validación de mapa de ubicación

1.33

1.66

Característica
o funcionalidad

Validación de código postal
en la dirección
Funcionalidad para validar tipo
de empaque que prefiere el
cliente

Esquemas de priorización

Puedes ver entonces que, en este caso, la decisión sería
iniciar con la validación del código postal de la dirección,
luego implementar la validación de clientes duplicados,
después implementar la funcionalidad para validar el tipo
de empaque que prefiere el cliente, y así sucesivamente,
o es probable que se decida implementar solamente las
características que aparecen en la tabla con el mayor
cociente, es decir, con el mayor resultado de la división,
tal vez las 3 primeras solamente.
¿Qué opinas de este esquema?, ¿qué ventajas o
desventajas ves que pudiera tener comparándolo
con los que viste previamente?

Urgencia
Este esquema de urgencia es similar al anterior (Business
Value / Story Points), pero en lugar de utilizar story points
usaremos una escala de valores que indique la urgencia
que se tiene para implementar cada historia de
usuario, esta escala va del 1 al 5, donde 5 significa
la urgencia máxima.
Una vez más es el usuario o el product owner el que
determina este nivel de urgencia para cada historia de
usuario.
¿Qué aspectos crees que debería considerar el usuario
para determinar el nivel de urgencia de las historias?
Seguro vino a tu mente una situación en la que es urgente
resolver algún problema o aprovechar alguna oportunidad
de negocio, o tal vez pensaste en el caso en que se tiene
una fecha límite para cumplir con algún requerimiento
regulatorio, probablemente recordaste un proyecto previo

Esquemas de priorización

Como puedes ver, hay muchas consideraciones para
que el usuario defina la urgencia para implementar
cada historia, incluso podría ser una combinación
de varias de estas circunstancias.
De esta manera los dos criterios a utilizar son: Valor para
el negocio y Urgencia, y asignaremos valores del 1 al 5 para
cada uno de estos criterios, obteniendo las dos escalas que
se muestran en la siguiente tabla, en color gris.

Figura 1. Esquema de urgencia

Valor para el negocio

en el que fue urgente implementar alguna funcionalidad,
porque por temas contractuales, hubieran aplicado una
penalización por no entregar algún producto en una fecha
determinada.

Urgencia

Esquemas de priorización

Los valores que puedes ver dentro de la tabla, en colores verde, amarillo, naranja y rojo, se generan
multiplicando cada nivel de urgencia por cada nivel de valor para el negocio, por ejemplo, el 25 de la casilla roja
se obtiene multiplicando la urgencia 5 por el número 5 que corresponde al valor para el negocio.
Estos valores representan esta combinación de valor para el negocio y urgencia, para cada una de las historias de usuario que
tienes en el backlog.
Tomando el mismo ejemplo que hemos usado para describir los esquemas anteriores, y aplicándolo a este esquema, tenemos
la distribución de la tabla a continuación.

Característica
o funcionalidad
Validación de clientes
duplicados
Captura de color de envoltura
preferido por el cliente
Funcionalidad para captura y
validación de mapa de ubicación
Validación de código postal
en la dirección
Funcionalidad para validar tipo
de empaque que prefiere el
cliente
Esquemas de priorización

Valor para el negocio
Valor para
(determinado por elUrgencia
el negocio
usuario)

Resultado
multiplicación

Color

Rojo

Verde

Amarillo

Naranja

Verde

Por lo anterior, el orden para implementar las características
del backlog sería el siguiente: primero la historia que tiene
el color rojo, que es la de la validación de cliente duplicado,
después la historia con color naranja, que es la validación del
código postal en la dirección. Posteriormente la historia con
el color amarillo y al final las historias con color verde, que en
este caso se elegirá primero la que tiene mayor resultado en la
multiplicación, es decir, la que corresponde a la funcionalidad
para validar tipo de empaque que prefiere el cliente.
Hemos finalizado este tema. Es momento de conocer la importancia
de los diferentes esquemas vistos en este recurso, continúa con
el estudio de la lección y consolida los aprendizajes adquiridos.
Reflexiona en torno a las siguientes preguntas:
• ¿Has utilizado alguno de estos esquemas en tu organización?
• ¿Cuál crees que sería el más aceptado por tu equipo?
• ¿Cuál te parece más práctico?
• ¿Sugerirías algún cambio o ajuste en tu empresa con respecto
a la forma en que se prioriza el contenido del backlog?

Descarga el documento desde el apartado
de "Archivos adjuntos" de la plataforma.
