# 07. Escalas del perfil de aprendizaje

## 1. Propósito del documento

Este documento define una propuesta inicial de escalas para las variables del perfil de aprendizaje en AdaptiveLearn. Su función es convertir el modelo conceptual del perfil en una estructura más clara, observable y utilizable por el sistema y por el docente.

## 2. Criterio general de diseño

Las escalas del perfil deben cumplir cuatro condiciones:

- ser fáciles de interpretar por el docente;
- basarse en evidencias observables;
- permitir actualización progresiva;
- traducirse en decisiones adaptativas concretas.

Por esta razón, en la primera versión se recomienda usar escalas simples, cortas y pedagógicamente comprensibles, evitando modelos demasiado complejos.

## 3. Variables principales y sus escalas

## 3.1. Nivel de dominio

### Propósito

Indicar qué tan cerca está el estudiante de lograr el objetivo de aprendizaje actual.

### Escala propuesta

- **Inicial:** el estudiante presenta comprensión limitada y requiere apoyo constante.
- **En desarrollo:** el estudiante muestra avances parciales, pero aún comete errores relevantes o necesita apoyo frecuente.
- **Logrado:** el estudiante alcanza el objetivo esperado con un nivel adecuado de precisión y comprensión.
- **Avanzado:** el estudiante supera lo esperado para el objetivo actual y puede transferir lo aprendido a situaciones similares o más complejas.

### Evidencias que la actualizan

- resultado en diagnóstico;
- respuestas correctas e incorrectas;
- desempeño en actividades de práctica;
- resultado en microevaluaciones;
- consistencia entre práctica y evaluación.

### Uso adaptativo

- seleccionar dificultad de actividades;
- decidir si el estudiante requiere refuerzo, práctica o ampliación;
- definir si puede avanzar o debe reforzar contenidos previos.

## 3.2. Ritmo de aprendizaje

### Propósito

Indicar cuánto tiempo, repetición o apoyo necesita el estudiante para progresar en un objetivo de aprendizaje.

### Escala propuesta

- **Lento:** requiere más tiempo, más repeticiones o mayor descomposición de la tarea.
- **Moderado:** avanza con tiempos y apoyos esperados.
- **Ágil:** progresa con rapidez y necesita menos repeticiones para alcanzar el objetivo.

### Evidencias que la actualizan

- tiempo de respuesta;
- número de intentos;
- tiempo total invertido en completar actividades;
- velocidad de mejora entre actividades similares.

### Uso adaptativo

- ajustar longitud de la secuencia didáctica;
- aumentar o reducir práctica;
- decidir si el sistema presenta pasos intermedios o avanza más rápido.

## 3.3. Formato de mediación más efectivo

### Propósito

Identificar con qué tipo de presentación del contenido el estudiante responde mejor en términos de comprensión y progreso.

### Escala propuesta

En esta variable no conviene usar una escala lineal, sino una clasificación dinámica por predominancia observada.

- **Visual predominante**
- **Auditivo predominante**
- **Práctico/interactivo predominante**
- **Textual/guiado predominante**
- **Mixto o sin predominancia clara**

### Aclaración importante

Esta variable no debe usarse como una etiqueta rígida. El sistema debe tratarla como una preferencia dinámica basada en evidencias recientes y acumuladas.

### Evidencias que la actualizan

- mejor desempeño con ciertos formatos;
- mayor finalización de actividades en un formato específico;
- menor necesidad de ayuda cuando el contenido se presenta de cierta manera;
- mayor velocidad de comprensión con ciertos recursos.

### Uso adaptativo

- seleccionar el formato principal del recurso;
- combinar formatos cuando no haya predominancia clara;
- sugerir al docente el tipo de mediación más prometedor.

## 3.4. Nivel de autonomía

### Propósito

Indicar cuánto apoyo necesita el estudiante para trabajar con éxito en las actividades propuestas.

### Escala propuesta

- **Dependiente:** necesita apoyo frecuente, pistas constantes o guía paso a paso.
- **Semiautónomo:** puede avanzar por sí mismo en parte del proceso, pero requiere apoyo puntual.
- **Autónomo:** resuelve la mayoría de tareas sin ayuda y mantiene un desempeño estable.

### Evidencias que la actualizan

- cantidad de pistas solicitadas;
- necesidad de retroalimentación para continuar;
- número de interrupciones o bloqueos;
- desempeño en tareas sin ayudas explícitas.

### Uso adaptativo

- definir el nivel de apoyo del recurso;
- decidir si una actividad será guiada o autónoma;
- alertar al docente cuando el estudiante requiere acompañamiento adicional.

## 3.5. Patrones de dificultad

### Propósito

Identificar la naturaleza y persistencia de las dificultades que presenta el estudiante.

### Escala propuesta

Esta variable tampoco debe manejarse como una escala única, sino como dos dimensiones complementarias:

### a. Frecuencia de la dificultad

- **Ocasional**
- **Recurrente**
- **Persistente**

### b. Tipo de dificultad

- **Conceptual:** no comprende la idea o contenido central.
- **Procedimental:** entiende en parte, pero falla al ejecutar pasos o aplicar reglas.
- **De interpretación:** tiene dificultad para comprender consignas, preguntas o situaciones.
- **De transferencia:** resuelve en un contexto, pero no aplica lo aprendido en otro similar.

### Evidencias que la actualizan

- errores repetidos;
- fallos en actividades similares;
- patrones de respuesta incorrecta;
- puntos frecuentes de abandono o bloqueo.

### Uso adaptativo

- decidir si el sistema debe reforzar concepto, procedimiento, interpretación o transferencia;
- ajustar el tipo de actividad correctiva;
- escalar una alerta al docente cuando la dificultad sea persistente.

## 4. Variables complementarias

Estas variables no forman parte del núcleo principal del perfil en la primera versión, pero pueden ayudar a enriquecer la lectura del estudiante.

### 4.1. Participación

#### Escala propuesta

- **Baja**
- **Media**
- **Alta**

#### Evidencias

- inicio de actividades;
- continuidad en las tareas;
- finalización de sesiones o recursos.

### 4.2. Persistencia

#### Escala propuesta

- **Baja**
- **Media**
- **Alta**

#### Evidencias

- cantidad de reintentos;
- permanencia ante tareas difíciles;
- abandono temprano o continuidad.

## 5. Recomendación técnica y pedagógica

Para la primera versión de AdaptiveLearn, se recomienda que el sistema:

- trabaje con pocas escalas;
- use categorías comprensibles para el docente;
- actualice cada variable solo cuando exista evidencia suficiente;
- muestre al docente no solo el valor de la escala, sino también una breve explicación de por qué el sistema la asigna.

## 6. Ejemplo de lectura integrada del perfil

Un estudiante podría aparecer así:

- **Nivel de dominio:** En desarrollo
- **Ritmo de aprendizaje:** Lento
- **Formato de mediación más efectivo:** Visual predominante
- **Nivel de autonomía:** Semiautónomo
- **Patrones de dificultad:** Recurrente, de tipo procedimental

### Interpretación pedagógica

Esto sugeriría que el estudiante:

- aún no domina completamente el objetivo actual;
- necesita más tiempo y práctica que otros;
- responde mejor cuando el contenido se presenta visualmente;
- puede avanzar solo en parte del proceso;
- requiere refuerzo específico en la ejecución de tareas o pasos.

### Respuesta adaptativa esperada

El sistema podría:

- ofrecer una explicación visual paso a paso;
- proponer práctica guiada antes de la evaluación final;
- reducir temporalmente la dificultad;
- entregar al docente una recomendación de acompañamiento puntual.

## 7. Reglas iniciales de interpretación

Para evitar conclusiones apresuradas, se recomienda que el sistema:

- no cambie una escala importante con una sola evidencia aislada;
- considere tendencias y no solo eventos puntuales;
- permita revisar historial reciente y acumulado;
- mantenga visible para el docente que el perfil es dinámico y revisable.

## 8. Preguntas pendientes

- ¿Cuántas evidencias mínimas deben requerirse para actualizar cada escala?
- ¿Cómo se combinarán evidencias distintas para asignar una categoría?
- ¿Qué parte de estas escalas será visible al estudiante?
- ¿Qué parte será exclusiva para el docente?
- ¿Qué umbrales activarán recomendaciones automáticas o alertas?
