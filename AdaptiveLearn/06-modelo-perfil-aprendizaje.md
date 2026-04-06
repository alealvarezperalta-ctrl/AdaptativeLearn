# 06. Modelo de perfil de aprendizaje del estudiante

## 1. Propósito del documento

Este documento define el modelo inicial de perfil de aprendizaje del estudiante para AdaptiveLearn. Su propósito es establecer qué debe conocer el sistema sobre cada estudiante, cómo obtiene esa información y de qué manera la usa para personalizar recursos, actividades y evaluaciones en apoyo al docente.

## 2. Idea central

AdaptiveLearn no debe limitarse a medir si el estudiante responde bien o mal. Su valor diferencial consiste en ayudar al docente a comprender mejor **cómo aprende el estudiante**, qué tipo de mediaciones pedagógicas parecen favorecerle, dónde presenta dificultades y qué apoyos necesita para avanzar.

El perfil de aprendizaje no debe entenderse como una etiqueta fija, sino como una representación dinámica y actualizable del estudiante a partir de evidencias observables.

Además, este perfil debe aspirar a ser **transversal y reutilizable** entre diferentes docentes y diferentes clases, siempre que se mantenga la distinción entre información general del aprendizaje del estudiante y evidencia específica de cada asignatura.

## 3. Finalidad pedagógica del perfil

El perfil de aprendizaje debe servir para tres funciones principales:

- **comprender** al estudiante desde una perspectiva pedagógica útil;
- **adaptar** recursos, actividades y explicaciones a sus necesidades;
- **identificar** mediaciones pedagógicas más efectivas para su aprendizaje;
- **evaluar** el progreso con mayor pertinencia y personalización.

De forma complementaria, el perfil también debe permitir:

- **transferir conocimiento pedagógico útil** entre docentes, para que la comprensión del estudiante no dependa exclusivamente de una sola clase.

En consecuencia, el perfil no es un fin en sí mismo. Su valor depende de qué tan bien ayuda al docente a tomar decisiones y qué tan bien permite al sistema automatizar apoyos personalizados.

## 4. Principios de diseño del perfil

El modelo de perfil de aprendizaje de AdaptiveLearn debe cumplir estos principios:

- ser **pedagógicamente útil**, no solo técnicamente interesante;
- basarse en **evidencias observables** y no en supuestos abstractos;
- mantenerse **dinámico** y actualizado con nuevas interacciones;
- evitar clasificaciones rígidas o etiquetas permanentes;
- traducirse en **decisiones adaptativas concretas**;
- ser comprensible para el docente y no una “caja negra”;
- distinguir entre información **transversal** y evidencia **contextual o disciplinar**.

## 5. Carácter transversal del perfil

AdaptiveLearn debe construir un perfil del estudiante con dos niveles de información:

### 5.1. Capa transversal

Incluye información útil en distintas asignaturas o contextos, por ejemplo:

- ritmo de aprendizaje;
- nivel de autonomía;
- formatos de mediación que suelen funcionar mejor;
- patrones generales de persistencia o necesidad de apoyo.

### 5.2. Capa contextual o disciplinar

Incluye información específica de un área, asignatura o tema, por ejemplo:

- nivel de dominio en un objetivo particular;
- dificultades asociadas a un contenido concreto;
- desempeño en actividades específicas de una clase.

### Implicación pedagógica

Esto permite que un docente nuevo no reciba solo datos aislados, sino una base de comprensión inicial sobre cómo acompañar mejor a ese estudiante, incluso antes de observarlo durante mucho tiempo en su propia clase.

## 6. Variables principales del perfil

Para una primera versión del sistema, se propone trabajar con cinco variables principales.

### 6.1. Nivel de dominio

Describe el grado de comprensión o desempeño del estudiante respecto al objetivo de aprendizaje actual.

Permite responder preguntas como:

- ¿el estudiante domina el tema?;
- ¿se encuentra en un nivel inicial, intermedio o logrado?;
- ¿requiere refuerzo previo antes de avanzar?

### 6.2. Ritmo de aprendizaje

Describe la velocidad relativa con que el estudiante avanza cuando trabaja un contenido o habilidad.

Permite observar:

- cuánto tiempo necesita para comprender una explicación;
- cuántos intentos requiere antes de lograr una tarea;
- si necesita más práctica o puede avanzar con mayor rapidez.

### 6.3. Formato de mediación más efectivo

Describe con qué tipos de recurso o presentación del contenido el estudiante responde mejor.

Ejemplos:

- recursos visuales;
- explicaciones auditivas;
- actividades prácticas;
- secuencias guiadas paso a paso;
- materiales interactivos.

Esta variable debe entenderse como una **preferencia dinámica observada**, no como una etiqueta definitiva del tipo “este estudiante solo aprende así”.

### 6.4. Nivel de autonomía

Describe el grado en que el estudiante puede trabajar y resolver actividades con independencia.

Permite identificar:

- si resuelve sin ayuda;
- si requiere pistas frecuentes;
- si necesita acompañamiento paso a paso;
- si puede transferir lo aprendido a tareas similares.

### 6.5. Patrones de dificultad

Describe errores, bloqueos o dificultades recurrentes observadas durante el proceso de aprendizaje.

Puede incluir:

- errores repetidos;
- confusiones frecuentes;
- fallos en instrucciones o procedimientos;
- dificultades para transferir lo aprendido;
- puntos del proceso donde se detiene o abandona.

## 7. Variables secundarias o complementarias

Existen otras variables que pueden ser valiosas, pero que no deberían ser centrales en la primera versión del sistema.

### 7.1. Participación

Refleja si el estudiante inicia, mantiene y finaliza las actividades propuestas.

### 7.2. Persistencia

Refleja si el estudiante continúa intentando resolver una tarea aun cuando encuentra dificultad.

### 7.3. Motivación observada

Puede inferirse indirectamente por comportamiento, participación y continuidad, pero no debe tratarse al inicio como una variable diagnóstica fuerte, ya que su medición es menos estable y más ambigua.

## 8. Cómo se obtiene el perfil

El perfil de aprendizaje se construye a partir de dos fuentes principales:

- diagnóstico inicial;
- interacción continua.

## 9. Diagnóstico inicial

El diagnóstico inicial debe ser breve, funcional y suficiente para ofrecer una primera lectura del estudiante.

Su propósito no es clasificar de forma definitiva, sino establecer una línea base.

Debe permitir estimar:

- nivel inicial de desempeño;
- primeras dificultades observables;
- necesidad de apoyo;
- respuesta inicial frente a distintos formatos de mediación;
- condiciones mínimas para personalizar la siguiente intervención.

### Evidencias esperadas en el diagnóstico inicial

- respuestas correctas e incorrectas;
- tipo de error cometido;
- tiempo de respuesta;
- necesidad de pistas o apoyo;
- desempeño en actividades presentadas en formatos distintos.

## 10. Interacción continua

El perfil debe actualizarse de manera progresiva con cada nueva interacción del estudiante en la plataforma.

Esta actualización continua permite que el sistema deje de depender solo de un diagnóstico puntual y construya una visión más rica y precisa del estudiante a lo largo del tiempo.

### Evidencias que deben alimentar la actualización del perfil

- resultados en quizzes y microevaluaciones;
- número de intentos por actividad;
- errores repetidos;
- tiempo invertido en tareas;
- uso de ayudas, pistas o retroalimentación;
- nivel de finalización de actividades;
- desempeño según tipo de recurso utilizado;
- mejora o estancamiento en actividades similares;
- consistencia entre actividades de práctica y evaluación.

## 11. Qué variables son realmente útiles para el docente

No toda variable que el sistema pueda medir será igualmente útil para el docente. Para la primera versión, las más relevantes son:

- **nivel de dominio**, para saber desde dónde intervenir;
- **patrones de dificultad**, para entender en qué falla el estudiante;
- **nivel de autonomía**, para decidir cuánto acompañamiento necesita;
- **formato de mediación más efectivo**, para adaptar la enseñanza;
- **ritmo de aprendizaje**, para ajustar secuencia, carga y profundidad.

Estas variables son útiles porque permiten transformar datos en decisiones pedagógicas concretas.

## 12. Utilidad del perfil para otros docentes

Cuando el perfil se construye correctamente, puede servir también a otros docentes del mismo estudiante.

Esto no significa trasladar automáticamente conclusiones rígidas de una materia a otra. Significa ofrecer información pedagógica inicial útil, por ejemplo:

- si el estudiante suele responder mejor a ciertos formatos;
- si necesita mayor o menor nivel de guía;
- si tiende a avanzar con ritmo más lento o más ágil;
- si requiere apoyos frecuentes para sostener la actividad.

### Condición importante

La reutilización del perfil entre docentes debe:

- compartir principalmente información transversal;
- distinguir claramente qué parte proviene de una asignatura específica;
- evitar que un docente interprete como universal algo que solo ocurrió en un contexto puntual;
- mantenerse bajo criterios éticos, institucionales y de privacidad.

## 13. Cómo usa el sistema el perfil para personalizar

El perfil del estudiante debe traducirse en acciones adaptativas visibles y concretas.

### 13.1. Adaptación de recursos

El sistema podrá:

- cambiar el formato del recurso;
- generar materiales más visuales, auditivos, prácticos o guiados;
- ofrecer ejemplos adicionales;
- presentar explicaciones más simples o más profundas.

### 13.2. Adaptación de actividades

El sistema podrá:

- ajustar la dificultad de los ejercicios;
- cambiar el tipo de actividad;
- ofrecer práctica guiada o autónoma;
- proponer refuerzo o ampliación según desempeño.

### 13.3. Adaptación de la secuencia

El sistema podrá:

- reorganizar el orden de las actividades;
- volver a contenidos previos si detecta vacíos;
- incluir pasos intermedios;
- acelerar el avance si observa dominio suficiente.

### 13.4. Adaptación de la evaluación

El sistema podrá:

- proponer evaluaciones más acordes al nivel observado;
- variar el tipo de ítems o formato de comprobación;
- ofrecer evaluación progresiva;
- detectar si el estudiante necesita una nueva oportunidad con apoyo antes del cierre.

### 13.5. Información para el docente

El sistema deberá mostrar al docente:

- cómo está aprendiendo el estudiante;
- qué dificultades recurrentes presenta;
- qué tipo de recurso parece funcionar mejor;
- qué nivel de apoyo requiere;
- qué recomendaciones de intervención conviene considerar.

## 14. Límites importantes del modelo

El perfil no debe:

- etiquetar al estudiante de manera permanente;
- reemplazar el juicio profesional del docente;
- asumir que una sola forma de aprender define toda la experiencia del estudiante;
- convertir correlaciones observadas en verdades absolutas;
- tomar decisiones irreversibles sin supervisión docente.

## 15. Formulación funcional del perfil

En términos operativos, el perfil de aprendizaje del estudiante en AdaptiveLearn puede definirse así:

> Conjunto dinámico de variables observables que describe el nivel de dominio, ritmo, autonomía, dificultades y formas de mediación más efectivas para un estudiante, con el fin de personalizar recursos, actividades y evaluación, ofrecer al docente información útil para intervenir pedagógicamente y conservar conocimiento reutilizable sobre cómo aprende el estudiante en distintos contextos.

## 16. Recomendación para la primera versión

Para evitar complejidad innecesaria, la primera versión del sistema debe trabajar solo con el núcleo mínimo del perfil:

- nivel de dominio;
- ritmo de aprendizaje;
- formato de mediación más efectivo;
- nivel de autonomía;
- patrones de dificultad.

Este núcleo es suficiente para comenzar a validar si AdaptiveLearn puede automatizar personalización educativa de forma útil, clara y medible.

## 17. Preguntas pendientes

- ¿Qué escala usará cada variable del perfil?
- ¿Cómo se visualizará este perfil para el docente?
- ¿Con qué frecuencia se actualizará el perfil?
- ¿Qué umbrales activarán cambios adaptativos automáticos?
- ¿Qué parte de estas decisiones requerirá aprobación del docente?
- ¿Qué parte del perfil será transversal y qué parte quedará asociada a una asignatura?
