# 20. Preguntas para entrevista técnica de modelado de base de datos

## 1. Propósito del documento

Este documento reúne las preguntas iniciales que el equipo de trabajo debe responder para modelar la base de datos relacional de AdaptiveLearn.

Su objetivo es servir como guía de entrevista técnica para identificar:

- entidades principales;
- atributos clave;
- relaciones entre actores, procesos y evidencias;
- reglas de negocio que impactan el modelo de datos.

## 2. Contexto de partida

Estas preguntas se construyen a partir de la documentación actual de AdaptiveLearn, especialmente de los documentos relacionados con:

- visión general del producto;
- perfil de aprendizaje del estudiante;
- componentes funcionales del sistema;
- flujo de uso por actores;
- datos del sistema y visibilidad de la información;
- requisitos funcionales;
- caso piloto definido.

Aunque el prompt de referencia menciona el modelo educativo MOCAVI, esta entrevista se ha formulado en coherencia con la documentación actual de AdaptiveLearn, que hasta el momento se ha desarrollado con enfoque de software educativo personalizado y lógica pedagógica basada en competencias.

## 3. Funcionalidades y dominios de información identificados

De la documentación revisada, se proyectan al menos los siguientes dominios de información que probablemente requerirán modelado relacional:

- gestión de usuarios y roles;
- instituciones, cursos, grupos y asignaciones;
- estudiantes y sus vínculos con docentes y acudientes;
- experiencias pedagógicas, temas, competencias y objetivos;
- diagnósticos, actividades y evaluaciones;
- respuestas, intentos, errores y evidencias de desempeño;
- perfil de aprendizaje del estudiante;
- historial de actualización del perfil;
- decisiones adaptativas y mediaciones pedagógicas sugeridas;
- recursos educativos generados, aprobados, asignados y reutilizados;
- reportes, alertas y seguimiento;
- visibilidad, permisos y trazabilidad de acciones.

## 4. Preguntas para la entrevista técnica

### 4.1. Institución, estructura académica y actores

1. ¿Una institución podrá tener varios cursos, grados, grupos o sedes dentro del sistema?
2. ¿Cómo se identificará a cada estudiante: con un identificador interno del sistema, con código institucional, con ambos o con otro esquema?
3. ¿Un estudiante podrá pertenecer a más de un grupo o curso al mismo tiempo?
4. ¿Un docente podrá estar asociado a varios grupos, asignaturas o experiencias pedagógicas simultáneamente?
5. ¿Un estudiante podrá estar vinculado a varios docentes al mismo tiempo dentro de distintas asignaturas?
6. ¿Un estudiante podrá tener más de un acudiente registrado?
7. ¿Qué información mínima debe almacenarse para cada tipo de actor: docente, estudiante, acudiente y administrativo?
8. ¿Se necesita conservar histórico de cambios en los datos de vinculación, por ejemplo cambio de grupo, cambio de docente o cambio de acudiente?

### 4.2. Gestión pedagógica y contexto de aprendizaje

9. ¿Qué unidad pedagógica será la base operativa del sistema: asignatura, curso, tema, unidad, secuencia didáctica o experiencia de aprendizaje?
10. ¿Un docente podrá definir varias competencias u objetivos dentro de una misma experiencia?
11. ¿Cada objetivo de aprendizaje debe quedar asociado a una asignatura específica o algunos podrán ser transversales?
12. ¿Qué datos exactos deben guardarse de una experiencia pedagógica creada por el docente?
13. ¿Se requiere versionar experiencias pedagógicas cuando el docente las modifica con el tiempo?
14. ¿El sistema debe permitir reutilizar una misma experiencia en distintos grupos o periodos académicos?

### 4.3. Diagnóstico, actividades y evaluación

15. ¿Cómo se compone un diagnóstico inicial: por bloques, preguntas, actividades, ítems o una mezcla de estas estructuras?
16. ¿Qué tipos de ítem deben existir desde la primera versión: selección múltiple, completar, ordenar, audio, lectura, arrastrar y soltar u otros?
17. ¿Cada pregunta o actividad debe quedar vinculada al objetivo de aprendizaje y al tipo de mediación usada?
18. ¿Qué información debe registrarse por cada intento del estudiante: respuesta, tiempo, número de intentos, uso de pista, estado de finalización, dispositivo u otra?
19. ¿Cómo se clasificará un error: por tipo de error pedagógico, por competencia, por regla gramatical, por nivel de dificultad o por otra taxonomía?
20. ¿Se deben guardar solo los resultados finales de una actividad o también cada interacción intermedia del estudiante?
21. ¿Las evaluaciones posteriores tendrán la misma estructura que el diagnóstico o podrán ser de otro tipo?
22. ¿Cómo se registrará la retroalimentación entregada al estudiante: automática, generada por IA, validada por docente o manual?

### 4.4. Perfil de aprendizaje del estudiante

23. ¿Qué variables del perfil del estudiante serán obligatorias en la primera versión de la base de datos?
24. ¿Cómo se almacenará la diferencia entre perfil transversal del estudiante y perfil contextual por asignatura o tema?
25. ¿El perfil actual debe guardarse como estado consolidado y, además, tener un historial detallado de cambios?
26. ¿Cada cambio del perfil debe registrar fecha, valor anterior, valor nuevo, evidencias asociadas, nivel de confianza y actor que lo validó?
27. ¿Qué niveles o escalas concretas usará cada variable del perfil, por ejemplo nivel de dominio, autonomía o ritmo?
28. ¿La “mediación pedagógica más efectiva” se almacenará como una única preferencia principal, como ranking de mediaciones o como evidencia comparativa por contexto?
29. ¿Qué parte del perfil podrá ser reutilizada por otros docentes y qué parte debe quedar restringida a la asignatura o experiencia que la originó?

### 4.5. Personalización y decisiones adaptativas

30. ¿Cada decisión adaptativa del sistema debe quedar registrada como entidad propia?
31. ¿Qué datos mínimos debe guardar una decisión adaptativa: motivo, evidencia usada, recurso recomendado, dificultad sugerida, apoyo sugerido, nivel de confianza y estado?
32. ¿La recomendación del sistema debe guardar si fue aprobada, editada, rechazada o ignorada por el docente?
33. ¿Se necesita almacenar la relación entre una decisión adaptativa y los resultados posteriores para medir si fue efectiva?
34. ¿Una misma experiencia podrá generar varias decisiones adaptativas para un mismo estudiante a lo largo del tiempo?

### 4.6. Recursos educativos y generación con IA

35. ¿Qué tipos de recurso existirán formalmente en el sistema: texto, imagen, audio, video, juego, quiz, actividad interactiva, infografía u otros?
36. ¿Cada recurso generado debe guardar versión, formato, objetivo pedagógico, autoría, fecha de generación y motor de IA utilizado?
37. ¿Se deben guardar los prompts, configuraciones o instrucciones con las que fue generado un recurso?
38. ¿Un mismo recurso podrá reutilizarse con varios estudiantes, grupos o asignaturas?
39. ¿Cómo se medirá la efectividad de un recurso: por desempeño, finalización, reducción de errores, aprobación docente u otra métrica?
40. ¿Es necesario diferenciar recursos generados automáticamente, recursos editados por el docente y recursos cargados manualmente?

### 4.7. Seguimiento, reportes y acompañamiento

41. ¿Qué información debe aparecer en el reporte docente y cuál debe estar disponible solo como dato interno del sistema?
42. ¿Qué nivel de detalle podrán ver padres o acudientes sobre el estudiante?
43. ¿Qué información agregada necesitan ver los administrativos: por institución, por curso, por docente, por asignatura o por periodo?
44. ¿Los reportes deben generarse como instantáneas guardadas, como vistas dinámicas o de ambas formas?
45. ¿Se requiere conservar historial de alertas pedagógicas, recomendaciones y reportes emitidos?

### 4.8. Permisos, privacidad y trazabilidad

46. ¿Qué datos del estudiante deben considerarse sensibles y tener restricciones especiales de acceso?
47. ¿Qué acciones del sistema deben quedar auditadas obligatoriamente, por ejemplo consulta de perfil, aprobación de recursos, edición manual o cambio de permisos?
48. ¿Se necesita registrar quién vio qué información y cuándo la consultó?
49. ¿El modelo debe contemplar consentimiento o autorización institucional para compartir parte del perfil del estudiante entre docentes o con acudientes?
50. ¿Qué reglas de retención, anonimización o eliminación de datos deben contemplarse desde el diseño?

### 4.9. Reglas operativas y crecimiento del sistema

51. ¿Cuál será el alcance real del MVP en términos de entidades indispensables y cuáles pueden dejarse para una segunda etapa?
52. ¿El piloto inicial en inglés debe convivir en la base con futuras asignaturas desde el inicio o se modelará primero solo para el piloto?
53. ¿Qué elementos del sistema deben diseñarse como catálogos parametrizables desde la primera versión, por ejemplo tipos de rol, tipos de recurso, tipos de error o niveles del perfil?
54. ¿Qué relaciones del negocio son obligatorias uno-a-muchos y cuáles podrían ser muchos-a-muchos?
55. ¿Qué consultas o reportes se consideran críticos desde el principio y deberían orientar el diseño relacional?

## 5. Uso recomendado de estas preguntas

Se recomienda responder estas preguntas en una sesión de entrevista técnica con el grupo de trabajo y luego convertir las respuestas en:

- listado inicial de entidades;
- diccionario preliminar de atributos;
- mapa de relaciones;
- reglas de negocio;
- prioridades de modelado para el MVP.

## 6. Formulación resumida

La entrevista técnica para modelar la base de datos de AdaptiveLearn debe profundizar no solo en usuarios y tablas básicas, sino también en la estructura pedagógica del sistema, el perfil dinámico del estudiante, la lógica adaptativa, la trazabilidad de decisiones y la reutilización transversal de la información del aprendizaje.
