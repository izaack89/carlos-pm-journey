# ¿Qué le recomiendas a Doña Mary?

> PDF: [[documentation/01. Planeacion adaptativa/Qué le recomiendas a Doña Mary.pdf|Ver PDF original]]

En este recurso identificarás las acciones que, como líder ágil, le propondrías a Doña Mary para fortalecer y tomar en cuenta las preferencias de sus clientes.

---

Doña Mary quiere usar el **modelo Kano** pero desconfía de sus propias preferencias y las de sus colaboradores — son menos válidas que la opinión de los clientes.

**Solución:** Aplicar **encuestas periódicas** a los clientes del restaurante.

---

## Proceso de aplicación del Modelo Kano

### 1. Selección de características y funcionalidades

El equipo (host, meseros, chef, contador y Laura — encargada de redes sociales) selecciona **7 historias de usuario** a encuestar. Objetivo: **25 opiniones por cada una**.

### 2. Formato de la encuesta (dos preguntas por funcionalidad)

| Pregunta | Opciones |
|----------|----------|
| **Aspectos Funcionales:** Si *incorporamos* la característica "X" | Me encantaría / Es algo que debe estar / Me da lo mismo / Me disgustaría |
| **Aspectos Disfuncionales:** Si *NO incorporamos* la característica "X" | Me encantaría / Me da lo mismo / Me disgustaría |

### 3. Tabla de interpretación de resultados

| Funcional ↓ \ Disfuncional → | Me gustaría | Natural | Me disgusta |
|------------------------------|-------------|---------|-------------|
| **Me gustaría** | C (Cuestionable) | E (Excitadores) | D (Desempeño) |
| **Debe estar** | R (Reversa) | I (Indiferente) | B (Necesidades básicas) |
| **Indiferente** | R (Reversa) | I (Indiferente) | B (Necesidades básicas) |
| **Me disgusta** | R (Reversa) | R (Reversa) | C (Cuestionable) |

> **Cuestionable (C):** no hay congruencia en las respuestas del encuestado.

---

## Resultados del ejemplo con 7 funcionalidades

| Funcionalidad | Necesidades básicas | Desempeño | Excitadores | Indiferente | Reversa | Cuestionable | **Categoría** |
|---------------|:-------------------:|:---------:|:-----------:|:-----------:|:-------:|:------------:|---------------|
| F1 | **18** | 3 | 2 | 0 | 1 | 1 | Necesidades básicas |
| F2 | 3 | 2 | 6 | **12** | 2 | 0 | Indiferente |
| F3 | 5 | 5 | **9** | 1 | 5 | 0 | Excitadores |
| F4 | 5 | **13** | 1 | 1 | 3 | 2 | Desempeño |
| F5 | **14** | 3 | 2 | 3 | 3 | 0 | Necesidades básicas |
| F6 | **16** | 2 | 3 | 2 | 2 | 0 | Necesidades básicas |
| F7 | 1 | 3 | 4 | **13** | 3 | 1 | Indiferente |

### Conclusiones

- **Prioridad alta:** F1, F5 y F6 → categoría de **Necesidades básicas** — deben implementarse primero.
- **Mayor impacto potencial:** F3 → categoría de **Excitadores** — puede diferenciar el servicio.
- **Descartar:** F2 y F7 → categoría de **Indiferente** (poco valor percibido).

> La utilidad del modelo Kano radica en que se obtienen las opiniones de un grupo seleccionado de *stakeholders* para determinar las funcionalidades y características del producto que se deberían incorporar en la **siguiente iteración** (MVI).
