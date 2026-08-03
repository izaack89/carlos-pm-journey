# Técnicas y herramientas (1)

> PDF: [[documentation/02. Detección y Resolución de Riesgos y Problemas copy/Técnicas y herramientas (1).pdf|Ver PDF original]]

---

Técnicas y herramientas
Reconoce las técnicas y herramientas más utilizadas para realizar
el análisis cuantitativo de los riesgos.


Javier, al momento cuenta con una lista priorizada de riesgos
del proyecto, el equipo ha sugerido ciertas acciones de
mitigación las cuales son actividades adicionales a las que se
tienen planeadas por lo que Javier ha tomado conciencia de
que dicho esfuerzo (horas/recurso) demandarán un costo, el
cual no está contemplado en la estimación de costos del
proyecto y no tiene certeza del monto adicional que
representan.
En tu experiencia, ¿las acciones de mitigación han tenido
impacto en el cronograma del proyecto y en el presupuesto
de éste?
El análisis cuantitativo de riesgos permite dimensionar
el impacto que se puede tener en los costos estimados y es de
gran valor para complementar el presupuesto del proyecto
con una reserva para contingencias, la cual, el Project
Manager tendrá la responsabilidad de administrar para
ejecutar las acciones de mitigación con la finalidad de evitar
que los riesgos se materialicen. Existen varias técnicas y/o
herramientas para realizar el análisis cuantitativo, a
continuación, describiremos algunas de las más utilizadas.

Técnicas y herramientas

Análisis de Monte Carlo
La Guía del PMBOK®, séptima edición, página 433, indica que el
análisis de Monte Carlo se usa para generar simulaciones, para
evaluar riesgos en costo, la simulación utiliza las estimaciones de
costos del proyecto y la salida es un modelo de análisis
cuantitativo de riesgos.

Existen diferentes soluciones informáticas para
iterar el modelo de análisis cuantitativo de riesgos varios
miles de veces, los valores de entrada (estimaciones de
costos, estimaciones de duración o ramas probabilísticas) se
eligen al azar para cada iteración. Las salidas representan el
rango de posibles resultados para el proyecto, por ejemplo,
fecha de finalización del proyecto, costo final del proyecto.
Una salida típica es un histograma que representa el número
de iteraciones donde se produjo un resultado de la
simulación en particular, o bien, una distribución de
probabilidad acumulada (curva S) que representa la
probabilidad de lograr cualquier resultado en particular. A
continuación, se muestra un ejemplo de curva S de un
análisis de Monte Carlo sobre riesgos de costos:

En el Estándar para la Gestión de Riesgos en portafolios,
programas y proyectos publicado por el Project
Management Institute, página 142-143 se describen las
siguientes técnicas las cuales se pueden usar para, con base
en ciertos escenarios y/o información disponible, realizar la
cuantificación de costos de riesgos.


Meta
$2.2M


85% de probabilidad
de costar
$2.45M o menos

Valor
esperado
$2.35M


23% de probabilidad de
cumplimiento de la meta

$2.0M

$2.1M

$2.2M

$2.3M

$2.4M

$2.5M

$2.6M

$2.7M

Probabilidad acumulada (%)

Probabilidad acumulada (%)

Grado de incertidumbre

$2.8M

Costo total previsto del proyecto

Figura 2.1 Ejemplo de Curva S de análisis Monte Carlo, Guía del PMBOK®, sexta
edición, página 433 .

Técnicas y herramientas

Valor Monetario
Esperado (EMV)
El Valor Monetario Esperado (EMV) es una técnica
estadística que se utiliza para cuantificar los riesgos, lo que, a su
vez, está considerado dentro del cálculo de la reserva para
contingencias. EMV es un cálculo de un valor, tal como el
promedio ponderado o el costo o beneficios esperados,
cuando los resultados son inciertos. Se identifican todos los
resultados alternativos razonables, se estiman sus probabilidades
de ocurrencia (se asume 100%) y sus valores.

El cálculo de EMV se realiza para todo el evento ponderando
los posibles resultados individuales según sus probabilidades
de ocurrencia, la fórmula es:

Probabilidad
de ocurrencia

35%

Valor Monetario Esperado (EMV) = Probabilidad × Impacto

Impacto

= $25,000 USD * 4 (semanas) *2 (proveedores)
= $200,000

Un ejemplo de uso del EMV en la gestión de riesgos es el
siguiente.
Se ha identificado el siguiente riesgo:
Si el proveedor “A” no finaliza la etapa de análisis en el mes
2 del proyecto, se tendrá un retraso en las actividades de la
fase de Diseño en la que están involucrados los proveedores
“B” y “C” con quienes se tienen pagos comprometidos de
$25,000 USD por semana, dichos pagos se deben liberar,
aunque no inicien sus actividades. Se ha estimado que el
retraso tiene una probabilidad de ocurrencia del 35%.
Restan 3 semanas para finalizar la etapa de Análisis.

Técnicas y herramientas

EMV

$ 70,000

Dado el ejemplo anterior, se tienen que contemplan un
presupuesto de $70,000 para lidiar con el riesgo,
programando acciones de mitigación dentro de un nuevo
Sprint con una duración de 2 semanas pues restan 3 en la
etapa de Análisis.

Análisis mediante
árbol de decisiones
Los árboles de decisiones se utilizan como herramienta para
seleccionar el mejor curso de acción entre varias alternativas, las
trayectorias alternativas a través del proyecto se muestran en el
árbol de decisiones usando ramas que representan diferentes
decisiones o eventos, cada uno de los cuales puede tener costos
asociados y riesgos individuales del proyecto (tanto amenazas
como oportunidades). El final de la rama se representa a través de
un punto y es el resultado de seguir esa trayectoria en particular,
lo cual puede ser positivo o negativo. Dentro del árbol de
decisiones se utiliza el Valor Monetario Esperado en cada rama
con la finalidad de identificar la trayectoria más adecuada.

Definición de
Decisión
Decisión a ser tomada

Nodo de Decisión

Nodo de Oportunidad

Entrada: Costo de cada decisión

Entrada: Probabilidad de escenario,
Recompensa si ocurre

Salida: Decisión tomada

Salida: Valor Monetario Esperado (EMV)
60%

Demanda fuerte
($200M)

Valor Neto de Ruta
Calculado: Beneficios menos
costos a lo largo de la ruta

$80M
$80M - $200M - $120M

Construir nueva planta
(Invertir $120M)
$36M - 0.60 ($80M) + 0.40 (-$30M)
¿Construir o
modernizar?
EMV para decisión - $46M
(el mayor entre $36M y
$46M)

40%

EMV de Construir
Nueva planta considerando la demanda

Demanda débil
($90M)

-30M
-$30M - $90M - $120M

60%

Demanda fuerte
($120M)

$70M
70M - $120M - $50M

Nodo de Decisión
Nodo de Oportunidad
Final del Ramal

Modernizar planta
(Invertir $50M)
$36M - 0.60 ($70M) + 0.40 (-$10M)
EMV de Construir
Planta considerando la demanda

40%

Demanda débil
($60M)

$10M
$10M - $60M - $50M

Nota 1: El árbol de deción muestra cómo una decisión entre estrategias de capital alternativas (representadas como “nodos de decisión”) cuando el entorno contiene elementos inciertos (representados como “nodos
de oportunidad”).
Nota 2: Aquí, se toma una decisión sobre si invertir USD 120M para construir una nueva planta o en lugar de eso invertir sólo USD 50M millones para modernizar la planta existente. Para cada decisión se debe tomar
en cuenta la demanda (que es incierta, y por lo tanto representa un nodo de oportunidad). Por ejemplo, la fuerte demanda apunta a ingresos con la nueva planta de USD 200M, pero sólo a USD 120M para la
planta modernizada, quizás debido a las limitaciones de capacidad de esta útima. El final de cada rama muestra el efecto neto de los beneficios menos los costos. Para cada rama de decisión, se agregan
todos los efectos (ver áreas sombreadas) a fin de determinar el Valor Monetario Esperado (EMV) conjunto de la decisión. No olvide tener en cuenta los costos de la inversión. A partir de los cálculos de las
áreas sombreadas, la planta modernizada presenta un EMV más alto, de $46M, que también es el EMV de la decsión general. (Esta opción también representa el menor riesgo, evitando el resultado de una
pérdida de $30M en el peor caso posible).

Figura 2.2 Ejemplo de árbol de decisión, Guía del PMBOK®, sexta edición, página 433.

Técnicas y herramientas

Análisis de Árbol de
Fallas (FMEA)
El análisis de modos de falla y efectos (FMEA) o análisis de
árbol de fallas utiliza un modelo estructurado para identificar
los diversos elementos que pueden causar fallas del sistema por sí
mismos, o bien, en combinación con otros, en función de la lógica
del sistema.

El análisis de árbol de fallas se utiliza a menudo en
contextos de ingeniería, pero se puede adoptar su uso con el
objetivo de identificar riesgos mediante el análisis de cómo
pueden surgir impactos del riesgos o probabilidad de falla (o
de confiabilidad, tiempo medio entre fallas, etc.) del sistema
en general, lo que indica el nivel de calidad del sistema o
producto. Si el nivel de confiabilidad no es aceptable, el árbol
de fallas puede indicar dónde se puede hacer más confiable
en el sistema, por lo que resulta sumamente útil en la fase de
diseño e ingeniería de un programa o proyecto.
Un ejemplo para aplicar el FMEA es el análisis de falla de un
sistema de protección contra incendios, podemos asumir que
hay dos posibles modos de fallo:
1. Fallo en el sistema de detección de incendios

Falla en el sistema
anti incendios

Falla en el Sistema
de detección de
fuego

Falla en el sistema
supresor de fuego

Falla en el sensor
detector de
humo

Falla en el sensor
detector de calor

No hay agua en
el sistema de
rociados

Boquillas de
aspersión
bloqueadas

Sensor de Humo
falló

Sensor de calor
falló

Bomba falló

Boquilla falló

2. Los mecanismos del sistema fallan
Figura 2.3 Ejemplo de árbol de falla. Fuente: Elaboración propia.

Técnicas y herramientas

Si el sistema de detección de incendios no ha funcionado,
significa que los detectores de humo han fallado y también
los detectores de temperatura (ambos tienen que fallar), por
el contrario, si la extinción del fuego ha fallado, significa que
no había agua en el sistema o que las boquillas de los
aspersores estaban bloqueadas, cualquiera de ambas
situaciones es suficiente para que el sistema fallara.

muy útil para determinar la(s) causa(s) raíz y aplicar
acciones correctivas. Puede aplicarse en casi cualquier
contexto, desde los fallos más simples hasta los más
complejos.

Si se llega a la conclusión de que el problema ha sido la falta
de agua en los aspersores, entonces la causa raíz es la bomba
de agua, que no tiene suficiente capacidad para todo el
sistema y el análisis puede parar por aquí.
En el caso de que se tenga agua disponible, se puede seguir
utilizando el árbol para analizar otras causas de fallo, por
ejemplo, si ha fallado la bomba, se puede analizar si ha sido
por falta de mantenimiento, equipo al final de su vida útil,
insuficiente para las necesidades del edificio, etcétera).
Investigar la causa raíz nos permite hacer los cambios
apropiados para tomar acciones correctivas y,
adicionalmente, el riesgo asociado a un activo. Aunque no se
aplica sistemáticamente en todas las industrias y/o
proyectos, el análisis de árbol de fallos es una herramienta

Técnicas y herramientas

En el Estándar para la Gestión de Riesgos en portafolios, programas y proyectos publicado por el Project Management
Institute, página 436 se indica una vez aplicado el análisis cuantitativo se obtienen los resultados siguientes:

Resultado
Evaluación de la
exposición a los riesgos
del proyecto

Descripción
Posibilidades de éxito
Son indicadas por la probabilidad de que el proyecto logre sus objetivos clave, por ejemplo, la fecha de finalización,
cumplimiento de hitos intermedios, ejecución del presupuesto planeado, etcétera.
Grado de variabilidad inherente restante
Es un conjunto de posibles resultados del proyecto.
Son el resultado de las salidas clave del análisis cuantitativo de riesgos tales como curvas S junto con una
interpretación narrativa de los resultados pudiendo incluir:

Análisis probabilístico
detallado del proyecto

Lista priorizada de
riesgos
Tendencias de los
resultados del análisis
cuantitativo

Técnicas y herramientas

• La cantidad de reserva para contingencias necesaria para proporcionar un determinado nivel de confianza.
• Identificación de los riesgos individuales del proyecto u otras fuentes de incertidumbre que tienen el mayor efecto
sobre la ruta crítica.
• Los principales condicionantes del riesgo general del proyecto que tienen mayor influencia en la incertidumbre de
los resultados del proyecto.
Incluye aquellos riesgos individuales del proyecto que representan la mayor amenaza o suponen la mayor
oportunidad para el proyecto.
A medida que se repite el análisis en diferentes momentos durante el ciclo de vida del proyecto se van recopilando
tendencias que pueden ser tomadas de referencia para planificar las respuestas a los riesgos.

Recuerda, que conocer algunas de las técnicas y
herramientas más utilizadas para realizar análisis
cuantitativos es muy útil para generar un presupuesto de
contingencia que ayude a gestionar los riesgos en los
proyectos.

Descarga el documento desde el apartado
de "Archivos adjuntos" de la plataforma.
