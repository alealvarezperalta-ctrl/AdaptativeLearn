# 13. Datos del sistema y visibilidad de la información

## 1. Propósito del documento

Este documento define qué tipos de datos maneja AdaptiveLearn, cómo se organizan dentro del sistema y qué nivel de visibilidad debe tener cada tipo de información según el rol del usuario.

Su propósito es asegurar coherencia entre la lógica pedagógica del sistema, la protección de la información del estudiante, la reutilización transversal del perfil y la gobernanza de acceso ya definida en documentos anteriores.

## 2. Idea central

AdaptiveLearn no solo genera recursos y actividades. También construye, interpreta y conserva información pedagógica valiosa sobre el estudiante, su progreso, sus dificultades y su forma de aprender.

Por esta razón, el sistema necesita distinguir con claridad:

- qué datos existen;
- para qué sirven;
- qué datos son pedagógicos y cuáles son administrativos;
- cuáles son sensibles;
- quién puede verlos;
- cuáles pueden reutilizarse entre clases y cuáles deben mantenerse dentro de un contexto específico.

## 3. Principios generales de manejo de información

La gestión de datos en AdaptiveLearn debe seguir estos principios:

- **pertinencia pedagógica:** recopilar solo información útil para acompañar el aprendizaje;
- **mínima exposición:** no mostrar más información de la necesaria para cada rol;
- **separación por capas:** diferenciar datos generales, pedagógicos, institucionales y sensibles;
- **distinción contextual:** separar información transversal del estudiante de la evidencia específica de una asignatura;
- **trazabilidad:** poder identificar origen, uso y cambios de información relevante;
- **protección del estudiante:** evitar usos inadecuados, sobreinterpretaciones o exposición innecesaria.

## 4. Tipos principales de datos del sistema

Se propone organizar los datos del sistema en siete grupos principales.

## 4.1. Datos de identificación y vinculación

Son los datos necesarios para reconocer al estudiante dentro del sistema y vincularlo a cursos, grupos o instituciones.

### Ejemplos

- nombre;
- identificador interno;
- curso o grado;
- grupo;
- institución;
- docente(s) asociados;
- acudiente(s) vinculados.

### Función

Permiten ubicar al estudiante en la estructura operativa del sistema.

## 4.2. Datos pedagógicos del perfil

Son los datos que describen cómo aprende el estudiante y cómo evoluciona su perfil de aprendizaje.

### Ejemplos

- nivel de dominio;
- ritmo de aprendizaje;
- nivel de autonomía;
- formatos de mediación más efectivos;
- patrones de dificultad;
- nivel de confianza del perfil;
- historial de actualizaciones del perfil.

### Función

Constituyen el corazón adaptativo del sistema.

## 4.3. Datos de desempeño y evidencia de aprendizaje

Son los datos producidos por el estudiante al interactuar con actividades, recursos y evaluaciones.

### Ejemplos

- respuestas correctas e incorrectas;
- puntajes;
- tiempos de respuesta;
- número de intentos;
- uso de pistas;
- nivel de finalización;
- progreso entre actividades similares.

### Función

Sirven para evaluar aprendizaje, actualizar el perfil y orientar decisiones adaptativas.

## 4.4. Datos del proceso adaptativo

Son los datos que describen cómo el sistema tomó decisiones de personalización y qué hizo en respuesta al perfil del estudiante.

### Ejemplos

- recurso recomendado;
- formato seleccionado;
- nivel de dificultad aplicado;
- secuencia adaptada;
- tipo de apoyo activado;
- decisión sugerida al docente;
- estado de aprobación docente.

### Función

Permiten explicar por qué el sistema personalizó de una determinada manera.

## 4.5. Datos de recursos y contenidos

Son los datos asociados a los materiales generados, reutilizados o asignados por el sistema.

### Ejemplos

- explicaciones generadas;
- ejercicios personalizados;
- recursos visuales, auditivos o interactivos;
- evaluaciones adaptadas;
- historial de uso de un recurso;
- efectividad observada del recurso.

### Función

Permiten mantener memoria pedagógica y reutilizar materiales útiles.

## 4.6. Datos de acompañamiento y seguimiento

Son datos orientados a la comunicación y seguimiento por parte de docentes, familias y administrativos.

### Ejemplos

- reportes de progreso;
- alertas pedagógicas;
- recomendaciones de acompañamiento;
- reportes resumidos para acudientes;
- indicadores agregados de curso o institución.

### Función

Facilitan el seguimiento del proceso sin necesidad de exponer toda la información interna del sistema.

## 4.7. Datos de auditoría y trazabilidad

Son los datos que registran acciones relevantes realizadas dentro del sistema.

### Ejemplos

- quién aprobó un recurso;
- cuándo se asignó una actividad;
- cuándo se modificó manualmente un perfil;
- qué actor consultó cierta información sensible;
- fecha y motivo de una actualización importante.

### Función

Aseguran confianza, control y revisión institucional.

## 5. Capas de información del estudiante

AdaptiveLearn debe organizar la información del estudiante en capas para evitar confusión y uso inapropiado.

## 5.1. Capa básica de identificación

Incluye datos necesarios para reconocer y vincular al estudiante dentro del sistema.

## 5.2. Capa pedagógica transversal

Incluye información útil en diferentes asignaturas o contextos.

### Ejemplos

- ritmo de aprendizaje;
- nivel de autonomía;
- formatos de mediación que suelen funcionar mejor;
- patrones generales de necesidad de apoyo.

## 5.3. Capa pedagógica contextual

Incluye información específica de una asignatura, tema, docente o secuencia concreta.

### Ejemplos

- nivel de dominio en un objetivo específico;
- dificultades en un contenido concreto;
- resultados de una unidad particular;
- decisiones adaptativas aplicadas en una clase determinada.

## 5.4. Capa de seguimiento y comunicación

Incluye información resumida y traducida para estudiantes, familias o actores no pedagógicos directos.

### Ejemplos

- avance general;
- fortalezas observadas;
- dificultades generales;
- recomendaciones de apoyo.

## 6. Visibilidad por actor

## 6.1. Docente

El docente debe tener acceso amplio a la capa pedagógica necesaria para intervenir.

### Debe poder ver

- perfil pedagógico del estudiante;
- evidencias de aprendizaje;
- decisiones adaptativas del sistema;
- historial de progreso;
- recursos generados y asignados;
- alertas relevantes;
- parte transversal y parte contextual del perfil.

### No necesariamente debe ver

- configuraciones institucionales completas;
- datos de auditoría que no afecten su trabajo diario.

## 6.2. Estudiante

El estudiante debe ver información útil para aprender, no el modelo técnico completo del sistema.

### Debe poder ver

- actividades asignadas;
- retroalimentación;
- progreso general;
- metas o próximos pasos;
- recursos disponibles para su aprendizaje.

### No debería ver

- interpretaciones técnicas complejas del perfil;
- comparaciones sensibles con otros estudiantes;
- historial interno de decisiones adaptativas.

## 6.3. Padres, madres o acudientes

Los acudientes deben tener visibilidad suficiente para acompañar, pero no para intervenir pedagógicamente.

### Deben poder ver

- avance general del estudiante;
- fortalezas y dificultades generales;
- participación;
- recomendaciones de apoyo;
- alertas relevantes para acompañamiento.

### No deberían ver

- detalle técnico del perfil;
- comparativas con otros estudiantes;
- decisiones pedagógicas internas del docente;
- información que pueda ser malinterpretada fuera de contexto.

## 6.4. Administrativos

Los administrativos deben ver información útil para seguimiento institucional y toma de decisiones de gestión.

### Deben poder ver

- indicadores agregados por grupo o curso;
- reportes institucionales;
- niveles de adopción y uso;
- tendencias generales de desempeño o participación.

### Solo de forma limitada podrían ver

- información individual resumida cuando exista una razón institucional válida.

### No deberían ver

- detalle fino del perfil pedagógico individual salvo necesidad justificada;
- decisiones didácticas internas que correspondan al docente.

## 7. Qué información puede reutilizarse entre clases

Una de las capacidades estratégicas de AdaptiveLearn es conservar conocimiento útil del estudiante entre distintas clases.

### Puede reutilizarse

- ritmo de aprendizaje;
- nivel general de autonomía;
- formatos de mediación usualmente efectivos;
- necesidad frecuente de apoyo;
- patrones generales de persistencia o bloqueo.

### Debe contextualizarse antes de reutilizarse

- dificultades específicas de una asignatura;
- nivel de dominio en un tema concreto;
- efectividad de recursos ligados a un contenido particular;
- resultados de evaluaciones de una clase determinada.

### No debería trasladarse como verdad universal

- una conclusión puntual basada en una sola actividad;
- una dificultad observada solo en un tema específico;
- una preferencia aparente con evidencia insuficiente.

## 8. Niveles de sensibilidad de la información

Se propone clasificar la información en cuatro niveles de sensibilidad.

### 8.1. Información operativa básica

Información necesaria para el uso normal del sistema.

### 8.2. Información pedagógica interna

Información útil para decisiones docentes, pero que no necesariamente debe mostrarse a otros actores.

### 8.3. Información resumida de acompañamiento

Información traducida para estudiantes y familias.

### 8.4. Información sensible o restringida

Información que requiere control especial por su potencial impacto pedagógico, ético o institucional.

### Ejemplos

- historial detallado del perfil;
- alertas individuales delicadas;
- registros de auditoría;
- decisiones manuales sobre el perfil del estudiante.

## 9. Reglas de visibilidad recomendadas

Para una primera versión del sistema, se recomienda:

- mostrar al docente la información pedagógica completa necesaria para intervenir;
- mostrar al estudiante información útil y comprensible;
- mostrar a familias una versión resumida y orientada al acompañamiento;
- mostrar a administrativos información principalmente agregada;
- restringir la exposición de información sensible individual;
- indicar siempre el contexto de una información antes de reutilizarla.

## 10. Riesgos a evitar

La gestión de visibilidad de datos no debe:

- mezclar información transversal con información específica de una materia;
- exponer al estudiante a etiquetas rígidas;
- permitir lecturas simplistas del perfil;
- dar acceso excesivo a actores sin rol pedagógico directo;
- ocultar por completo al docente cómo se construyó la información;
- compartir más datos de los necesarios para acompañamiento o supervisión.

## 11. Formulación resumida

AdaptiveLearn debe organizar sus datos en capas pedagógicas, contextuales, operativas y de seguimiento, permitiendo que cada actor acceda solo a la información pertinente para su rol, y diferenciando con claridad qué parte del perfil del estudiante es transversal y cuál pertenece a un contexto específico de aprendizaje.

## 12. Preguntas pendientes

- ¿Qué datos exactos integrarán la capa transversal del estudiante?
- ¿Qué datos verán los acudientes en la práctica y en qué formato?
- ¿Qué información individual podrán consultar los administrativos y bajo qué condiciones?
- ¿Qué datos deben quedar ocultos incluso dentro de la institución?
- ¿Cómo se representará visualmente esta separación de capas en la interfaz del sistema?
