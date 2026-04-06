# 10. Componentes funcionales del sistema

## 1. Propósito del documento

Este documento define los componentes funcionales principales de AdaptiveLearn. Su propósito es describir qué grandes capacidades debe tener el sistema para cumplir su objetivo de diagnosticar cómo aprende el estudiante, personalizar la enseñanza y asistir al docente con apoyo de IA.

## 2. Idea central

AdaptiveLearn no debe entenderse como una sola herramienta, sino como un sistema compuesto por varios módulos funcionales que trabajan de manera coordinada.

Cada componente cumple una función específica, pero todos deben contribuir a un mismo propósito:

- conocer mejor al estudiante;
- ayudar al docente a tomar decisiones;
- personalizar recursos y evaluación;
- registrar evidencia del aprendizaje;
- mejorar la intervención pedagógica con el tiempo;
- construir memoria pedagógica reutilizable del estudiante.

## 3. Criterios de organización funcional

Los componentes del sistema deben organizarse de forma que:

- respondan a necesidades pedagógicas reales;
- mantengan coherencia con el enfoque por competencias;
- permitan crecimiento progresivo del producto;
- faciliten trazabilidad de decisiones;
- sean comprensibles para docentes, diseñadores y desarrolladores.

## 4. Componentes funcionales principales

Se propone una arquitectura funcional inicial compuesta por nueve grandes componentes.

## 4.1. Componente de gestión pedagógica del docente

### Función

Permitir que el docente defina qué desea enseñar, qué espera que el estudiante aprenda y qué evidencias servirán para verificar el logro.

### Responsabilidades

- crear o cargar temas, unidades o secuencias;
- definir objetivos de aprendizaje o competencias;
- establecer evidencias o actividades esperadas;
- revisar recursos sugeridos por el sistema;
- aprobar, ajustar o rechazar propuestas adaptativas;
- consultar progreso y recomendaciones.

### Valor pedagógico

Este componente asegura que la personalización no ocurra al margen del criterio docente, sino alineada con su intención formativa.

## 4.2. Componente de diagnóstico inicial

### Función

Recoger las primeras evidencias que permitan construir una línea base del estudiante.

### Responsabilidades

- aplicar evaluación diagnóstica;
- medir nivel inicial de desempeño;
- observar primeras dificultades;
- comparar respuesta a distintos formatos;
- entregar insumos al perfil inicial del estudiante.

### Valor pedagógico

Permite que la personalización comience desde una base de evidencias y no desde suposiciones generales.

## 4.3. Componente de perfil de aprendizaje del estudiante

### Función

Construir, almacenar y actualizar el perfil dinámico de aprendizaje del estudiante.

### Responsabilidades

- registrar variables principales del perfil;
- integrar nuevas evidencias;
- actualizar escalas y niveles de confianza;
- conservar historial de cambios;
- ofrecer una lectura pedagógica del estudiante;
- distinguir entre capa transversal del perfil y capa específica por asignatura.

### Valor pedagógico

Es el núcleo interpretativo del sistema y el puente entre datos observados y decisiones adaptativas.

Además, este componente hace posible que el conocimiento construido sobre cómo aprende el estudiante pueda ser útil a más de un docente, sin confundir información general con desempeño específico de una sola materia.

## 4.4. Componente de analítica e interpretación pedagógica

### Función

Analizar resultados, detectar patrones y producir información útil para la toma de decisiones.

### Responsabilidades

- identificar tendencias de desempeño;
- detectar patrones de dificultad;
- comparar progreso en el tiempo;
- interpretar relación entre recursos usados y resultados;
- generar alertas o recomendaciones para el docente.

### Valor pedagógico

Convierte datos dispersos en información accionable para personalizar y acompañar mejor.

## 4.5. Componente de personalización y decisión adaptativa

### Función

Traducir el perfil del estudiante y las evidencias recientes en decisiones concretas sobre cómo enseñar, practicar y evaluar.

### Responsabilidades

- seleccionar formato de mediación;
- ajustar nivel de dificultad;
- decidir nivel de apoyo;
- reorganizar secuencia de actividades;
- adaptar la forma de evaluación;
- proponer acciones de refuerzo o ampliación.

### Valor pedagógico

Hace operativa la personalización, permitiendo que el sistema responda pedagógicamente a cada estudiante.

## 4.6. Componente de generación de recursos con IA

### Función

Crear recursos didácticos personalizados a partir del objetivo de aprendizaje, el perfil del estudiante y las decisiones adaptativas definidas por el sistema.

### Responsabilidades

- generar explicaciones adaptadas;
- producir ejercicios personalizados;
- crear materiales visuales, textuales, auditivos o interactivos;
- sugerir evaluaciones adaptadas;
- mantener consistencia con el objetivo pedagógico definido por el docente.

### Valor pedagógico

Amplía la capacidad del docente para ofrecer recursos diversos sin tener que producir manualmente cada variante.

## 4.7. Componente de ejecución de actividades y evaluación

### Función

Presentar al estudiante los recursos, actividades y evaluaciones, y registrar lo que ocurre durante la interacción.

### Responsabilidades

- mostrar contenidos y recursos;
- aplicar actividades prácticas;
- registrar respuestas, tiempos e intentos;
- administrar evaluaciones formativas o de cierre;
- devolver retroalimentación al estudiante.

### Valor pedagógico

Es el espacio donde se concreta la experiencia de aprendizaje y se generan las evidencias del sistema.

## 4.8. Componente de repositorio de recursos y evidencias

### Función

Conservar los recursos generados, sus variantes, sus resultados y las evidencias asociadas a su uso.

### Responsabilidades

- almacenar recursos creados;
- guardar historial de uso y efectividad;
- permitir reutilización de materiales;
- vincular recursos con objetivos, perfiles y resultados;
- facilitar mejora progresiva del sistema.

### Valor pedagógico

Permite que el sistema aprenda del uso real y no genere siempre desde cero sin memoria pedagógica.

## 4.9. Componente de historial transversal del estudiante

### Función

Conservar y poner a disposición una base de conocimiento pedagógico reutilizable sobre cómo aprende el estudiante a través de distintas clases o asignaturas.

### Responsabilidades

- almacenar patrones transversales del perfil;
- separar información general del aprendizaje de evidencia específica por materia;
- permitir que nuevos docentes partan de una base inicial útil;
- mantener trazabilidad sobre el origen de cada evidencia;
- respetar reglas institucionales de visibilidad, privacidad y uso pedagógico.

### Valor pedagógico

Hace posible que la personalización educativa no comience desde cero en cada clase, sino que el sistema acumule conocimiento útil sobre el estudiante a lo largo del tiempo escolar.

## 5. Flujo funcional general

De manera resumida, el sistema debería operar así:

1. el docente define el objetivo de aprendizaje;
2. el sistema aplica diagnóstico inicial;
3. se construye el perfil inicial del estudiante;
4. el sistema analiza evidencias y decide una personalización;
5. genera recursos y actividades adaptadas;
6. el estudiante interactúa y produce nuevas evidencias;
7. el perfil se actualiza;
8. se consolida el historial transversal del estudiante;
9. el docente revisa progreso, recursos y recomendaciones.

## 6. Relación entre componentes

Los componentes no deben funcionar de manera aislada.

### Relación principal

- el docente define intención pedagógica;
- el diagnóstico y la interacción alimentan el perfil;
- el perfil alimenta la analítica y la personalización;
- la personalización orienta la generación de recursos;
- la ejecución de actividades produce nuevas evidencias;
- el repositorio conserva memoria del proceso;
- el historial transversal conserva conocimiento reutilizable del estudiante;
- el docente supervisa, interpreta y decide.

## 7. Componentes núcleo para una primera versión

Aunque el sistema completo puede crecer mucho, el MVP debería priorizar estos componentes como núcleo mínimo:

- gestión pedagógica del docente;
- diagnóstico inicial;
- perfil de aprendizaje;
- personalización y decisión adaptativa;
- generación de recursos con IA;
- ejecución de actividades y evaluación.

Los componentes de analítica avanzada, repositorio inteligente e historial transversal pueden comenzar con una versión más simple y crecer después.

## 8. Riesgos funcionales a evitar

La arquitectura funcional no debe:

- poner demasiada complejidad en la primera versión;
- separar demasiado lo pedagógico de lo técnico;
- generar recursos sin conexión con el perfil;
- tomar decisiones adaptativas sin trazabilidad;
- dejar al docente fuera del flujo principal.

## 9. Formulación funcional resumida

AdaptiveLearn puede entenderse como un sistema compuesto por módulos de gestión pedagógica, diagnóstico, perfil del estudiante, analítica, personalización, generación de recursos, ejecución de actividades, repositorio de recursos e historial transversal del estudiante, todos articulados para automatizar la personalización educativa sin perder control docente.

## 10. Preguntas pendientes

- ¿Qué componente debe desarrollarse primero desde el punto de vista del MVP?
- ¿Qué componentes pueden empezar con lógica simple y crecer después?
- ¿Qué datos debe intercambiar cada componente con los demás?
- ¿Qué acciones deben quedar automatizadas y cuáles sujetas a aprobación docente?
- ¿Cómo se visualizará este sistema en términos de pantallas o experiencia de usuario?
