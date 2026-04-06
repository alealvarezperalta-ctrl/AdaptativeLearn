# 08. Reglas de actualización del perfil de aprendizaje

## 1. Propósito del documento

Este documento define las reglas iniciales mediante las cuales AdaptiveLearn actualiza el perfil de aprendizaje del estudiante a lo largo del tiempo. Su objetivo es establecer cómo el sistema interpreta nuevas evidencias, cuándo modifica una variable del perfil y qué condiciones deben cumplirse para que esos cambios sean pedagógicamente confiables.

## 2. Idea central

El perfil de aprendizaje del estudiante no debe depender únicamente de un diagnóstico inicial. Debe construirse y refinarse a partir de la interacción continua del estudiante con contenidos, actividades, ejercicios y evaluaciones.

La actualización del perfil debe ser:

- progresiva;
- basada en evidencias;
- resistente a cambios bruscos por eventos aislados;
- comprensible para el docente;
- útil para tomar decisiones adaptativas.

## 3. Principios de actualización

Las reglas de actualización del perfil deben responder a estos principios:

- **acumulación de evidencia:** una sola interacción no debe redefinir por completo el perfil;
- **prioridad a tendencias:** importa más el patrón observado que un evento puntual;
- **recencia controlada:** las evidencias recientes deben pesar más, pero sin borrar completamente el historial;
- **estabilidad razonable:** el perfil no debe cambiar de forma errática;
- **explicabilidad:** el docente debe poder entender por qué el sistema actualizó una variable;
- **reversibilidad:** el perfil puede cambiar si nuevas evidencias muestran una evolución distinta.

## 4. Fuentes de evidencia para actualizar el perfil

El sistema deberá usar como fuentes principales de actualización:

- resultados en diagnósticos;
- resultados en quizzes y microevaluaciones;
- desempeño en actividades prácticas;
- número de intentos;
- tiempo de respuesta;
- uso de pistas, ayudas o retroalimentación;
- finalización o abandono de actividades;
- desempeño según tipo de recurso;
- mejora o estancamiento entre actividades similares.

## 5. Regla general de actualización

Se propone que ninguna variable del perfil se actualice de forma automática por una única evidencia aislada, salvo en casos claramente excepcionales.

La lógica base debe ser:

- recoger evidencias nuevas;
- compararlas con el estado actual del perfil;
- detectar si existe una tendencia consistente;
- actualizar solo si la nueva tendencia supera un umbral mínimo de confianza;
- registrar el motivo del cambio para que sea visible al docente.

## 6. Tipos de actualización

Para la primera versión del sistema, conviene distinguir tres tipos de actualización.

### 6.1. Confirmación

Ocurre cuando nuevas evidencias refuerzan lo que el perfil ya indicaba.

Ejemplo:

- el estudiante ya mostraba mejor respuesta a recursos visuales;
- nuevas actividades visuales confirman mejor rendimiento y menor necesidad de ayuda.

En este caso, el sistema no cambia la categoría, pero aumenta la confianza en esa interpretación.

### 6.2. Ajuste gradual

Ocurre cuando nuevas evidencias sugieren un cambio moderado en una variable del perfil.

Ejemplo:

- el estudiante estaba en nivel de dominio inicial;
- después de varias actividades y una microevaluación, muestra desempeño consistente de nivel en desarrollo.

En este caso, el sistema actualiza la variable de forma progresiva.

### 6.3. Alerta de cambio significativo

Ocurre cuando aparecen evidencias que contradicen fuertemente el perfil actual o muestran una variación importante.

Ejemplo:

- el estudiante venía resolviendo con autonomía;
- en varias actividades recientes comienza a requerir ayuda constante y abandona tareas similares.

En este caso, el sistema puede:

- marcar una alerta interna;
- sugerir revisión docente;
- esperar confirmación adicional antes de cambiar una variable crítica.

## 7. Actualización por variable

## 7.1. Nivel de dominio

### Regla propuesta

El nivel de dominio debe actualizarse cuando exista evidencia suficiente de mejora, mantenimiento o retroceso respecto al objetivo actual.

### Cambia cuando

- al menos varias actividades del mismo objetivo muestran una tendencia similar;
- la evaluación y la práctica apuntan en la misma dirección;
- los errores disminuyen o aumentan de forma consistente.

### No cambia cuando

- existe una sola respuesta atípica;
- el rendimiento varía de forma inconsistente;
- no hay suficiente evidencia acumulada.

## 7.2. Ritmo de aprendizaje

### Regla propuesta

El ritmo debe actualizarse con base en patrones de tiempo, repetición e intervalos de mejora, no por una sola sesión.

### Cambia cuando

- el estudiante requiere repetidamente más o menos tiempo que el esperado;
- se observa un patrón estable en cantidad de intentos;
- la velocidad de mejora se mantiene durante varias actividades similares.

### No cambia cuando

- existe una sola actividad excepcionalmente lenta o rápida;
- factores externos parecen haber afectado el tiempo de respuesta.

## 7.3. Formato de mediación más efectivo

### Regla propuesta

El sistema debe actualizar esta variable solo cuando existan diferencias suficientemente claras entre el desempeño del estudiante con distintos formatos.

### Cambia cuando

- varios recursos del mismo formato muestran mejores resultados;
- ese formato reduce necesidad de ayuda y mejora finalización;
- la ventaja se repite en más de una sesión o actividad.

### No cambia cuando

- el estudiante solo interactuó una vez con un formato;
- no existe diferencia significativa entre formatos;
- el desempeño mejora por dificultad menor y no por formato.

## 7.4. Nivel de autonomía

### Regla propuesta

La autonomía debe actualizarse según la capacidad real del estudiante para resolver tareas con distinto nivel de apoyo.

### Cambia cuando

- se observa una reducción sostenida en uso de ayudas;
- el estudiante completa actividades similares con menos intervención;
- demuestra independencia en tareas donde antes requería acompañamiento.

### No cambia cuando

- la actividad era excepcionalmente sencilla;
- la ayuda solicitada responde a un factor puntual y no a un patrón.

## 7.5. Patrones de dificultad

### Regla propuesta

Las dificultades deben actualizarse cuando un error o bloqueo deja de ser ocasional y pasa a repetirse de forma reconocible.

### Cambia cuando

- el mismo tipo de error aparece en varias actividades;
- el estudiante falla repetidamente en un mismo punto;
- se observa persistencia del problema incluso con apoyo.

### No cambia cuando

- el error aparece una sola vez;
- no se repite en actividades similares;
- no existe claridad sobre el tipo de dificultad.

## 8. Confianza de la actualización

Para evitar decisiones precipitadas, se recomienda que cada cambio del perfil tenga asociado un nivel de confianza.

### Escala sugerida de confianza

- **Baja:** evidencia todavía insuficiente o poco consistente.
- **Media:** tendencia observable, pero aún necesita confirmación.
- **Alta:** patrón claramente sostenido por múltiples evidencias.

### Uso de la confianza

- si la confianza es baja, el sistema observa pero no cambia decisiones importantes;
- si la confianza es media, puede sugerir ajustes moderados;
- si la confianza es alta, puede adaptar con mayor firmeza y mostrar recomendaciones más claras al docente.

## 9. Reglas de recencia

Las evidencias recientes deben tener mayor peso, pero no deben borrar por completo el historial.

### Recomendación inicial

- considerar un historial acumulado;
- dar prioridad interpretativa a las evidencias más recientes;
- evitar que un cambio reciente elimine automáticamente una tendencia previa;
- permitir que el perfil refleje evolución y no solo fotografía instantánea.

## 10. Reglas de estabilidad

El sistema debe evitar cambios bruscos y frecuentes en variables importantes.

Para ello se recomienda:

- exigir más de una evidencia para cambiar una categoría principal;
- usar confirmación progresiva antes de modificar variables sensibles;
- registrar cuándo una variable está en observación, sin cambiarla todavía;
- mostrar al docente si un cambio es preliminar o ya estable.

## 11. Registro de cambios

Cada actualización del perfil debe dejar trazabilidad.

El sistema debería registrar al menos:

- variable afectada;
- valor anterior;
- valor nuevo;
- evidencias principales que justifican el cambio;
- nivel de confianza;
- fecha de actualización.

Esto permitirá explicabilidad y revisión pedagógica.

## 12. Rol del docente en la actualización

Aunque el sistema actualice automáticamente parte del perfil, el docente debe conservar visibilidad y capacidad de revisión.

El docente debe poder:

- ver cómo se actualizó una variable;
- comprender qué evidencias influyeron;
- confirmar o cuestionar cambios significativos;
- intervenir cuando la interpretación automática no refleje la realidad del aula.

## 13. Regla funcional resumida

En AdaptiveLearn, una variable del perfil de aprendizaje solo debe actualizarse cuando exista evidencia suficiente, consistente y pedagógicamente interpretable de que el comportamiento del estudiante muestra una tendencia nueva o confirmada.

## 14. Ejemplo de actualización

### Estado inicial del perfil

- Nivel de dominio: Inicial
- Ritmo de aprendizaje: Moderado
- Formato más efectivo: Mixto
- Autonomía: Dependiente
- Dificultad: Recurrente, procedimental

### Nuevas evidencias

- mejora sostenida en tres actividades similares;
- menor uso de pistas;
- mejor desempeño con recursos visuales;
- quiz breve con resultado superior al diagnóstico.

### Resultado esperado

- Nivel de dominio pasa de Inicial a En desarrollo.
- Formato más efectivo pasa de Mixto a Visual predominante.
- Autonomía pasa de Dependiente a Semiautónomo.
- La dificultad procedimental sigue presente, pero baja su intensidad.

## 15. Preguntas pendientes

- ¿Cuántas evidencias mínimas se exigirán por variable?
- ¿Qué cambios pueden hacerse de forma automática y cuáles deben requerir revisión docente?
- ¿Cómo se representará la confianza en la interfaz?
- ¿Qué variables deben cambiar más rápido y cuáles más lentamente?
- ¿Cómo diferenciar una dificultad temporal de un patrón real?
