# Técnicas para la estimación de un proyecto

> PDF: [[documentation/01. Planeacion adaptativa/Técnicas para la estimación de un proyecto.pdf|Ver PDF original]]

En esta lectura identificarás las tres técnicas para llevar a cabo la estimación de un proyecto dependiendo del tamaño de la historia de usuario o de la épica.

---

La mayoría de las estimaciones en proyectos resultan inexactas. Para enfrentar esto, se utilizan **diferentes técnicas según el tamaño de la HU o la épica**:

## 1. Story Points

Los *story points* son **unidades de medida** para expresar una estimación del esfuerzo total necesario para implementar completamente un elemento del backlog.

- Los equipos asignan puntos a cada HU en relación con la **cantidad de trabajo, complejidad y riesgo**.
- Son valores preliminares para abordar la incertidumbre.
- Con el tiempo, se convierten en la referencia principal para entender cuánto trabajo puede desarrollar el equipo en un período — genera **consenso y compromiso**.
- La abstracción motiva al equipo a enfocarse en la **dificultad del trabajo**, no en el tiempo.

## 2. Planning Poker

Técnica para estimar HU usando la **serie Fibonacci** (1, 2, 3, 5, 8, 13, 21, 34…), porque el tamaño puede ser lineal pero la **complejidad e incertidumbre crecen de manera exponencial**.

### Cartas especiales
| Carta | Significado |
|-------|-------------|
| **0** | Sin relevancia |
| **∞** | No es posible determinar el esfuerzo |
| **?** | Desconocimiento del tema |
| ☕ | Solicitar una pausa |

### Proceso del Planning Poker
1. **Elegir un punto de referencia** — una HU que se considere en la media
2. **Analizar la historia** en equipo — máximo 3 minutos
3. **Estimación individual simultánea** — todos muestran su carta al mismo tiempo
4. Si hay **consenso** → registrar el resultado
5. Si hay **disparidad** → escuchar argumentos de la estimación más alta y más baja → repetir el proceso
6. Si no hay consenso en el segundo intento → registrar el **promedio** o la estimación del experto

> El Planning Poker no representa tiempo de desarrollo; es una forma de dimensionar el **esfuerzo relativo** entre HUs para distribuirlas en iteraciones.

## 3. Estimación por tallas de camiseta

Para **épicas** que no pueden estimarse con Planning Poker (marcadas con ∞) o que carecen de detalle suficiente. El enfoque es más **intuitivo** que preciso, y evita la percepción de precisión que dan los números.

| Talla | Descripción |
|-------|-------------|
| **S** | Small — pequeño |
| **M** | Medium — mediano |
| **L** | Large — largo |
| **XL** | Extra large — extra largo |
| **XXL** | Super extra large — súper extra largo |

- S y M → épicas con cierto nivel de detalle o conocimiento
- L, XL, XXL → actividades complejas que necesitan mayor desglose o más personas involucradas

La finalidad es estimar **a grosso modo** si la épica puede realizarse en una iteración o cuántas serán requeridas. Conforme avanza el proyecto, las épicas se desagregan en Historias de Usuario con mayor detalle.
