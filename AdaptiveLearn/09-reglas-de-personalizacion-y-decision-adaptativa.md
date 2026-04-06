# 09. Reglas de personalización y decisión adaptativa

## 1. Propósito del documento

Este documento define cómo AdaptiveLearn transforma el perfil de aprendizaje del estudiante en decisiones concretas de personalización. Su objetivo es establecer qué tipo de adaptaciones puede realizar el sistema, bajo qué condiciones y con qué criterios pedagógicos.

## 2. Idea central

El valor del perfil de aprendizaje no está solo en describir al estudiante, sino en permitir que el sistema actúe pedagógicamente de manera útil.

Por ello, AdaptiveLearn debe convertir la información del perfil en decisiones adaptativas sobre:

- recursos;
- actividades;
- secuencia didáctica;
- nivel de apoyo;
- evaluación;
- recomendaciones para el docente.

Estas decisiones deben basarse en la identificación progresiva de mediaciones pedagógicas efectivas, y no en etiquetas rígidas del estudiante.

## 3. Principios de decisión adaptativa

Las decisiones adaptativas del sistema deben cumplir estos principios:

- responder a evidencias del perfil y no a supuestos arbitrarios;
- mantener coherencia con el objetivo de aprendizaje definido por el docente;
- priorizar la utilidad pedagógica sobre la novedad tecnológica;
- ser explicables para el docente;
- evitar cambios excesivos o contradictorios;
- permitir supervisión y ajuste humano.

## 4. Insumos para la personalización

Para tomar decisiones adaptativas, el sistema deberá considerar como mínimo:

- nivel de dominio;
- ritmo de aprendizaje;
- formato de mediación más efectivo;
- nivel de autonomía;
- patrones de dificultad;
- objetivo de aprendizaje actual;
- evidencias recientes de desempeño;
- nivel de confianza del perfil.

## 5. Tipos principales de personalización

En la primera versión, se propone que AdaptiveLearn personalice cinco dimensiones.

### 5.1. Personalización del formato del contenido

El sistema podrá decidir si presenta el contenido principalmente de forma:

- visual;
- auditiva;
- textual o guiada;
- práctica o interactiva;
- combinada.

### 5.2. Personalización de la dificultad

El sistema podrá ajustar:

- complejidad del ejercicio;
- cantidad de pasos requeridos;
- nivel de reto;
- grado de abstracción;
- carga de práctica.

### 5.3. Personalización del nivel de apoyo

El sistema podrá definir si el estudiante recibe:

- guía paso a paso;
- pistas graduales;
- ejemplos previos;
- retroalimentación inmediata;
- práctica autónoma con mínima intervención.

### 5.4. Personalización de la secuencia

El sistema podrá reorganizar:

- orden de actividades;
- necesidad de repaso previo;
- cantidad de ejercicios antes de evaluar;
- transición entre explicación, práctica y evaluación.

### 5.5. Personalización de la evaluación

El sistema podrá adaptar:

- tipo de actividad evaluativa;
- dificultad de los ítems;
- cantidad de apoyo previo al cierre;
- formato de comprobación del aprendizaje.

## 6. Reglas base por variable del perfil

## 6.1. Regla basada en nivel de dominio

### Si el nivel de dominio es Inicial

El sistema debería:

- ofrecer explicaciones más simples;
- priorizar práctica guiada;
- reducir dificultad inicial;
- evitar evaluación de cierre demasiado temprana;
- reforzar contenidos previos si es necesario.

### Si el nivel de dominio es En desarrollo

El sistema debería:

- combinar explicación y práctica;
- mantener reto moderado;
- ofrecer retroalimentación frecuente;
- incluir actividades de consolidación.

### Si el nivel de dominio es Logrado

El sistema debería:

- ofrecer práctica de transferencia;
- aumentar autonomía;
- reducir apoyo innecesario;
- preparar evaluación de comprobación.

### Si el nivel de dominio es Avanzado

El sistema debería:

- ofrecer ampliación;
- proponer retos más complejos;
- acelerar la progresión;
- evitar repetición innecesaria.

## 6.2. Regla basada en ritmo de aprendizaje

### Si el ritmo es Lento

El sistema debería:

- fragmentar la secuencia;
- aumentar repeticiones útiles;
- ofrecer más tiempo y más ejemplos;
- evitar saltos bruscos entre actividades.

### Si el ritmo es Moderado

El sistema debería:

- mantener progresión estándar;
- ajustar solo si aparecen dificultades específicas.

### Si el ritmo es Ágil

El sistema debería:

- reducir redundancias;
- acelerar transición hacia práctica autónoma;
- ofrecer ampliación o reto adicional.

## 6.3. Regla basada en formato de mediación más efectivo

### Si el formato predominante es Visual

El sistema debería priorizar:

- infografías;
- esquemas;
- imágenes explicativas;
- secuencias visuales paso a paso.

### Si el formato predominante es Auditivo

El sistema debería priorizar:

- audios;
- explicaciones narradas;
- diálogos;
- instrucciones habladas.

### Si el formato predominante es Práctico/interactivo

El sistema debería priorizar:

- ejercicios interactivos;
- simulaciones;
- microjuegos;
- actividades de resolución activa.

### Si el formato predominante es Textual/guiado

El sistema debería priorizar:

- explicaciones escritas estructuradas;
- ejemplos guiados;
- instrucciones paso a paso;
- resúmenes organizados.

### Si el formato es Mixto o sin predominancia clara

El sistema debería:

- combinar formatos;
- observar nuevas evidencias;
- evitar asumir una preferencia prematura.

## 6.4. Regla basada en nivel de autonomía

### Si el estudiante es Dependiente

El sistema debería:

- ofrecer guía fuerte;
- dividir tareas en pasos;
- activar ayudas visibles;
- notificar al docente si el patrón persiste.

### Si el estudiante es Semiautónomo

El sistema debería:

- combinar apoyo y resolución independiente;
- retirar ayudas gradualmente;
- promover práctica con intervención puntual.

### Si el estudiante es Autónomo

El sistema debería:

- priorizar trabajo independiente;
- reducir ayudas automáticas;
- enfocarse en reto, consolidación o transferencia.

## 6.5. Regla basada en patrones de dificultad

### Si la dificultad es Conceptual

El sistema debería:

- volver a explicar la idea central;
- usar ejemplos variados;
- simplificar la comprensión base;
- evitar aumentar dificultad demasiado rápido.

### Si la dificultad es Procedimental

El sistema debería:

- descomponer el proceso en pasos;
- ofrecer práctica guiada;
- reforzar orden y ejecución.

### Si la dificultad es De interpretación

El sistema debería:

- simplificar consignas;
- usar ejemplos de lectura guiada;
- reforzar comprensión de instrucciones y contexto.

### Si la dificultad es De transferencia

El sistema debería:

- variar contextos de aplicación;
- proponer ejercicios similares con pequeñas diferencias;
- reforzar el uso flexible de lo aprendido.

## 7. Reglas combinadas

En la práctica, el sistema no tomará decisiones con una sola variable, sino con combinaciones.

### Ejemplo 1

- Nivel de dominio: Inicial
- Ritmo: Lento
- Formato: Visual
- Autonomía: Dependiente

### Respuesta sugerida

- explicación visual simplificada;
- práctica guiada paso a paso;
- dificultad baja o moderada;
- alto nivel de apoyo;
- evaluación breve al final del bloque.

### Ejemplo 2

- Nivel de dominio: Logrado
- Ritmo: Ágil
- Formato: Mixto
- Autonomía: Autónomo

### Respuesta sugerida

- menor apoyo;
- práctica de transferencia;
- reto ampliado;
- secuencia más rápida;
- evaluación de mayor complejidad.

## 8. Regla de prudencia adaptativa

El sistema no debe modificar demasiadas variables al mismo tiempo sin evidencia suficiente.

Se recomienda que en cada ciclo de adaptación:

- priorice uno o dos cambios principales;
- mantenga estable lo que ya está funcionando;
- observe el efecto de la adaptación antes de volver a cambiar;
- permita al docente comprender qué cambió y por qué.

## 9. Rol del docente en la decisión adaptativa

Aunque el sistema pueda sugerir o ejecutar ciertas adaptaciones, el docente debe conservar control sobre:

- aprobar recursos generados;
- modificar secuencias sugeridas;
- aceptar o rechazar recomendaciones;
- decidir cuándo intervenir directamente;
- interpretar si la adaptación propuesta es pertinente para su contexto.

## 10. Salidas visibles para el docente

El sistema debería mostrar al docente:

- qué decisión adaptativa tomó o recomienda;
- qué variable del perfil la motivó;
- qué evidencia reciente la respalda;
- qué objetivo pedagógico busca atender;
- qué puede hacer el docente si desea ajustarla.

## 11. Regla funcional resumida

En AdaptiveLearn, una decisión adaptativa debe producirse cuando el perfil del estudiante y las evidencias recientes indiquen que una modificación en contenido, apoyo, secuencia, actividad o evaluación aumentará la probabilidad de aprendizaje útil y pertinente.

## 12. Riesgos a evitar

Las reglas de personalización no deben:

- sobrepersonalizar sin necesidad;
- repetir siempre el mismo formato;
- reducir el reto de forma excesiva;
- generar experiencias incoherentes con el objetivo de aprendizaje;
- ocultar al docente por qué el sistema tomó una decisión.

## 13. Preguntas pendientes

- ¿Qué adaptaciones podrá ejecutar el sistema automáticamente y cuáles solo sugerirá?
- ¿Cuál será el orden de prioridad cuando varias variables indiquen decisiones distintas?
- ¿Qué decisiones requerirán validación docente obligatoria?
- ¿Cómo se medirá si una adaptación realmente fue efectiva?
- ¿Cada cuánto debe reevaluarse una decisión adaptativa?
