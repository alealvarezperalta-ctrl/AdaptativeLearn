# 21. Respuestas propuestas para la entrevista técnica de modelado de base de datos

## 1. Propósito del documento

Este documento responde, de forma preliminar y fundamentada en la documentación actual de AdaptiveLearn, las preguntas definidas para la entrevista técnica de modelado de base de datos.

Su propósito es:

- consolidar decisiones iniciales de negocio y datos;
- traducir la visión pedagógica del proyecto a criterios de modelado relacional;
- identificar qué respuestas ya están claras y cuáles siguen siendo provisionales.

## 2. Criterio de lectura

Las respuestas aquí consignadas se basan en la documentación viva del proyecto y deben entenderse como:

- **definidas**, cuando ya existe suficiente soporte documental;
- **provisionales**, cuando la documentación orienta una decisión, pero aún conviene validarla con el grupo.

## 3. Respuestas propuestas

### 3.1. Institución, estructura académica y actores

**1. ¿Una institución podrá tener varios cursos, grados, grupos o sedes dentro del sistema?**  
Sí. La institución debe poder contener múltiples grados, cursos, grupos y, de forma proyectada, sedes.

**2. ¿Cómo se identificará a cada estudiante?**  
Se recomienda usar un identificador interno del sistema como clave primaria y, adicionalmente, permitir un código institucional opcional o requerido según el contexto.

**3. ¿Un estudiante podrá pertenecer a más de un grupo o curso al mismo tiempo?**  
Sí, al menos a nivel de diseño. Un estudiante puede estar vinculado a varios grupos o experiencias, especialmente si el sistema crece hacia escenarios institucionales más complejos.

**4. ¿Un docente podrá estar asociado a varios grupos, asignaturas o experiencias pedagógicas simultáneamente?**  
Sí. El modelo debe permitir relaciones múltiples entre docente, grupo, asignatura y experiencia.

**5. ¿Un estudiante podrá estar vinculado a varios docentes al mismo tiempo dentro de distintas asignaturas?**  
Sí. Esto es coherente con la lógica transversal del perfil del estudiante.

**6. ¿Un estudiante podrá tener más de un acudiente registrado?**  
Sí. El sistema debe permitir uno o varios acudientes autorizados por estudiante.

**7. ¿Qué información mínima debe almacenarse para cada tipo de actor?**  
Nombre, identificador, correo o medio de acceso, rol, estado de cuenta y vínculo institucional. En estudiantes además grado/grupo; en docentes asignaciones; en acudientes relación con el estudiante; en administrativos alcance institucional.

**8. ¿Se necesita conservar histórico de cambios en los datos de vinculación?**  
Sí, de forma recomendada. Debe registrarse al menos cambios relevantes de grupo, docente, institución o acudiente.

### 3.2. Gestión pedagógica y contexto de aprendizaje

**9. ¿Qué unidad pedagógica será la base operativa del sistema?**  
La unidad más útil para el sistema es la **experiencia de aprendizaje** o secuencia pedagógica configurada por el docente. Esta puede contener asignatura, tema, competencia, actividades y evaluaciones.

**10. ¿Un docente podrá definir varias competencias u objetivos dentro de una misma experiencia?**  
Sí. La experiencia debe poder agrupar uno o varios objetivos o resultados de aprendizaje.

**11. ¿Cada objetivo de aprendizaje debe quedar asociado a una asignatura específica o algunos podrán ser transversales?**  
Ambos casos deben ser posibles. En el MVP casi todos serán contextuales a una asignatura, pero el modelo debe aceptar objetivos transversales.

**12. ¿Qué datos exactos deben guardarse de una experiencia pedagógica creada por el docente?**  
Nombre, descripción, asignatura, tema, competencia u objetivo, grado o grupo destino, docente responsable, fecha de creación, estado, recursos asociados y criterios de evidencia.

**13. ¿Se requiere versionar experiencias pedagógicas cuando el docente las modifica con el tiempo?**  
Sí, de manera recomendable. Al menos debe conservarse historial de cambios importantes para no perder trazabilidad pedagógica.

**14. ¿El sistema debe permitir reutilizar una misma experiencia en distintos grupos o periodos académicos?**  
Sí. La reutilización es coherente con la lógica de eficiencia docente y repositorio pedagógico.

### 3.3. Diagnóstico, actividades y evaluación

**15. ¿Cómo se compone un diagnóstico inicial?**  
Como una estructura mixta compuesta por bloques, y dentro de cada bloque actividades o ítems.

**16. ¿Qué tipos de ítem deben existir desde la primera versión?**  
Selección múltiple, completar, ordenar, lectura breve con preguntas y una actividad breve con variación de mediación. Audio puede entrar desde el piloto si la capacidad técnica lo permite.

**17. ¿Cada pregunta o actividad debe quedar vinculada al objetivo de aprendizaje y al tipo de mediación usada?**  
Sí. Esa relación es clave para analítica pedagógica y para identificar mediaciones efectivas.

**18. ¿Qué información debe registrarse por cada intento del estudiante?**  
Respuesta dada, resultado, tiempo de respuesta, número de intento, uso de pista o ayuda, nivel de finalización, actividad asociada, recurso asociado y fecha/hora.

**19. ¿Cómo se clasificará un error?**  
Inicialmente por tipo de error pedagógico. En el piloto de inglés, por ejemplo: reconocimiento de estructura, uso del verbo, comprensión de significado, interpretación de consigna y producción básica.

**20. ¿Se deben guardar solo los resultados finales o también interacciones intermedias?**  
Se recomienda guardar ambas capas: resultado final e interacciones intermedias relevantes, al menos intentos y uso de ayudas.

**21. ¿Las evaluaciones posteriores tendrán la misma estructura que el diagnóstico o podrán ser de otro tipo?**  
Podrán ser de otro tipo. Deben ser comparables en propósito, no necesariamente idénticas en estructura.

**22. ¿Cómo se registrará la retroalimentación entregada al estudiante?**  
Debe registrarse con su tipo y origen: automática, generada por IA, validada por docente o manual.

### 3.4. Perfil de aprendizaje del estudiante

**23. ¿Qué variables del perfil serán obligatorias en la primera versión?**  
Nivel de dominio, ritmo de aprendizaje, formato de mediación más efectivo, nivel de autonomía y patrones de dificultad.

**24. ¿Cómo se almacenará la diferencia entre perfil transversal y perfil contextual?**  
Con dos capas relacionadas: una capa transversal por estudiante y una capa contextual asociada a asignatura, experiencia, tema u objetivo.

**25. ¿El perfil actual debe guardarse como estado consolidado y también con historial?**  
Sí. Debe existir un estado actual consultable y un historial de cambios para trazabilidad.

**26. ¿Cada cambio del perfil debe registrar fecha, valor anterior, valor nuevo, evidencias, confianza y actor?**  
Sí. Esa es la recomendación explícita del proyecto.

**27. ¿Qué niveles o escalas concretas usará cada variable?**  
Se recomienda escalas discretas y comprensibles. Por ejemplo: dominio `inicial / en desarrollo / logrado`; confianza `baja / media / alta`; autonomía `alta / media / baja` o equivalente ordenado.

**28. ¿La mediación pedagógica más efectiva se almacenará como única preferencia, ranking o evidencia comparativa?**  
La mejor decisión es guardar evidencia comparativa por contexto y, adicionalmente, una recomendación principal vigente. No debe reducirse a una etiqueta única fija.

**29. ¿Qué parte del perfil podrá ser reutilizada por otros docentes?**  
Principalmente la capa transversal: ritmo, autonomía, apoyos frecuentes y mediaciones que suelen funcionar. La capa contextual debe mantenerse asociada a la asignatura o experiencia que la originó.

### 3.5. Personalización y decisiones adaptativas

**30. ¿Cada decisión adaptativa debe quedar registrada como entidad propia?**  
Sí. Debe tener trazabilidad independiente.

**31. ¿Qué datos mínimos debe guardar una decisión adaptativa?**  
Estudiante, experiencia o contexto, fecha, evidencia utilizada, variable del perfil relacionada, mediación o recurso sugerido, dificultad sugerida, apoyo sugerido, nivel de confianza, explicación resumida y estado.

**32. ¿La recomendación del sistema debe guardar si fue aprobada, editada, rechazada o ignorada por el docente?**  
Sí. Esa información es esencial para gobernanza y aprendizaje del sistema.

**33. ¿Se necesita almacenar la relación entre decisión adaptativa y resultados posteriores?**  
Sí. Sin esa relación no puede medirse si la adaptación fue efectiva.

**34. ¿Una misma experiencia podrá generar varias decisiones adaptativas para un mismo estudiante?**  
Sí. El sistema es dinámico y puede ajustar sobre la marcha.

### 3.6. Recursos educativos y generación con IA

**35. ¿Qué tipos de recurso existirán formalmente en el sistema?**  
Texto, imagen, audio, video, juego, quiz, actividad interactiva, infografía y otros tipos parametrizables.

**36. ¿Cada recurso generado debe guardar versión, formato, objetivo, autoría, fecha y motor de IA?**  
Sí. Eso debe quedar registrado desde el diseño.

**37. ¿Se deben guardar los prompts o instrucciones de generación?**  
Sí, al menos en forma resumida o estructurada, porque son parte de la trazabilidad del recurso generado.

**38. ¿Un mismo recurso podrá reutilizarse con varios estudiantes, grupos o asignaturas?**  
Sí, siempre que su uso quede contextualizado y trazado.

**39. ¿Cómo se medirá la efectividad de un recurso?**  
Por desempeño posterior, finalización, reducción de errores, necesidad de apoyo, aceptación docente y, de forma agregada, por utilidad observada en contextos similares.

**40. ¿Es necesario diferenciar recursos generados automáticamente, editados por docente y cargados manualmente?**  
Sí. Esa diferencia debe modelarse.

### 3.7. Seguimiento, reportes y acompañamiento

**41. ¿Qué información debe aparecer en el reporte docente y cuál debe quedar interna?**  
El reporte docente debe mostrar resumen, resultado diagnóstico, perfil inicial, interpretación pedagógica, recomendación del sistema y acción sugerida. Datos técnicos internos más finos pueden quedar ocultos o disponibles solo en detalle avanzado.

**42. ¿Qué nivel de detalle podrán ver padres o acudientes?**  
Un nivel resumido: avance general, fortalezas, dificultades generales, participación y recomendaciones de acompañamiento. No deben ver detalle técnico del perfil.

**43. ¿Qué información agregada necesitan ver los administrativos?**  
Indicadores por institución, grupo, curso, docente, asignatura y, si se requiere, periodo académico.

**44. ¿Los reportes deben generarse como instantáneas guardadas, vistas dinámicas o ambas?**  
Lo más sólido es ambas. Vistas dinámicas para uso operativo e instantáneas para trazabilidad y seguimiento histórico.

**45. ¿Se requiere conservar historial de alertas, recomendaciones y reportes emitidos?**  
Sí. Es coherente con la lógica de seguimiento y auditoría.

### 3.8. Permisos, privacidad y trazabilidad

**46. ¿Qué datos del estudiante deben considerarse sensibles?**  
Identificación personal, datos de acceso, información pedagógica individual, historial del perfil, decisiones adaptativas, observaciones de acompañamiento y cualquier dato que permita inferencias delicadas sobre el aprendizaje.

**47. ¿Qué acciones deben quedar auditadas obligatoriamente?**  
Consulta de perfil, aprobación o rechazo de recursos, cambios manuales del perfil, asignación de actividades, consulta de información sensible y cambios de permisos o vínculos.

**48. ¿Se necesita registrar quién vio qué información y cuándo?**  
Sí, al menos para información sensible o pedagógicamente delicada.

**49. ¿El modelo debe contemplar consentimiento o autorización institucional para compartir parte del perfil?**  
Sí. Aunque aún no esté totalmente desarrollado en la documentación, el modelo debe prever esta capacidad.

**50. ¿Qué reglas de retención, anonimización o eliminación de datos deben contemplarse?**  
Retención por periodo académico o política institucional, anonimización para analítica agregada y eliminación o desactivación controlada cuando corresponda. Esta respuesta sigue siendo provisional y debe validarse jurídicamente.

### 3.9. Reglas operativas y crecimiento del sistema

**51. ¿Cuál será el alcance real del MVP en términos de entidades indispensables?**  
Indispensables: usuarios, roles, instituciones, grupos, estudiantes, vínculos, experiencias pedagógicas, objetivos, diagnóstico, actividades, respuestas, perfil actual, historial básico del perfil, decisiones adaptativas, recursos, asignaciones y reportes básicos.

**52. ¿El piloto inicial en inglés debe convivir con futuras asignaturas desde el inicio o modelarse solo para el piloto?**  
Debe modelarse desde el inicio con capacidad multiasignatura, aunque el piloto operativo sea solo inglés. El núcleo del producto es transversal.

**53. ¿Qué elementos deben diseñarse como catálogos parametrizables?**  
Roles, tipos de recurso, tipos de actividad, tipos de error, estados de decisión adaptativa, niveles de confianza, escalas del perfil y tipos de mediación.

**54. ¿Qué relaciones del negocio son obligatorias uno-a-muchos y cuáles podrían ser muchos-a-muchos?**  
Uno-a-muchos: institución a grupos, experiencia a actividades, estudiante a actualizaciones de perfil. Muchos-a-muchos: estudiantes-docentes, estudiantes-acudientes, recursos-experiencias, docentes-grupos, estudiantes-experiencias.

**55. ¿Qué consultas o reportes se consideran críticos desde el principio?**  
Perfil actual del estudiante, progreso por experiencia, errores frecuentes, efectividad de mediaciones, recursos asignados y usados, decisiones adaptativas por estudiante y reportes resumidos para acudientes y administrativos.

## 4. Decisiones ya bastante claras

La documentación actual ya permite sostener con buena claridad estas decisiones:

- el sistema es multiactor;
- el estudiante tiene perfil transversal y contextual;
- las decisiones adaptativas deben tener trazabilidad;
- los recursos generados requieren relación con objetivo, perfil y uso;
- el docente conserva validación y control final;
- la información visible depende del rol.

## 5. Respuestas que siguen siendo provisionales

Todavía conviene validar con el equipo:

- el nivel exacto de versionado pedagógico;
- el detalle técnico de auditoría;
- la política real de retención y anonimización;
- si el MVP registrará telemetría detallada o solo interacciones clave;
- el grado de complejidad inicial del modelo multiasignatura.

## 6. Siguiente uso recomendado

Con estas respuestas ya se puede construir un primer borrador de:

- entidades principales;
- atributos iniciales;
- relaciones cardinales;
- reglas de negocio del modelo relacional;
- alcance del diagrama entidad-relación del MVP.
