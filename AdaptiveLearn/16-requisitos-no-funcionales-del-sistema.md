# 16. Requisitos no funcionales del sistema

## 1. Propósito del documento

Este documento define los requisitos no funcionales iniciales de AdaptiveLearn. Su propósito es establecer las condiciones de calidad, comportamiento, seguridad, usabilidad, privacidad, trazabilidad y confiabilidad que el sistema debe cumplir para ser pedagógicamente útil, técnicamente sólido y aceptable en un entorno educativo real.

## 2. Idea central

Los requisitos funcionales describen qué debe hacer el sistema.

Los requisitos no funcionales describen **cómo debe comportarse** ese sistema para que su uso sea viable, confiable y seguro.

En AdaptiveLearn, estos requisitos son especialmente importantes porque la plataforma:

- trabaja con datos de estudiantes;
- influye en decisiones pedagógicas;
- utiliza IA para generar recursos;
- debe ser comprensible para docentes;
- debe sostener confianza institucional y familiar.

## 3. Principios generales

Los requisitos no funcionales de AdaptiveLearn deben seguir estos principios:

- proteger al estudiante y su información;
- garantizar utilidad pedagógica real;
- permitir uso sencillo por actores no técnicos;
- hacer visibles las decisiones importantes del sistema;
- mantener control humano sobre procesos sensibles;
- facilitar crecimiento progresivo del producto.

## 4. Categorías de requisitos no funcionales

Se propone organizar estos requisitos en once categorías principales.

## 5. Requisitos no funcionales por categoría

## 5.1. Usabilidad y experiencia de usuario

### RNF-01. Claridad de uso

El sistema debe ser comprensible para usuarios no técnicos, especialmente docentes, estudiantes y acudientes.

### RNF-02. Baja fricción de interacción

Las tareas principales del sistema deben poder realizarse con un número razonable de pasos y sin complejidad innecesaria.

### RNF-03. Lenguaje comprensible

La interfaz debe usar lenguaje claro, pedagógico y adecuado para cada actor.

### RNF-04. Adecuación por rol

La experiencia de uso debe adaptarse al rol del usuario, evitando mostrar información técnica innecesaria a quien no la necesita.

## 5.2. Accesibilidad

### RNF-05. Accesibilidad básica

El sistema debe diseñarse considerando principios básicos de accesibilidad digital.

### RNF-06. Diversidad de formatos

La plataforma debe favorecer el acceso a contenidos en distintos formatos para apoyar diversidad de necesidades de aprendizaje.

### RNF-07. Compatibilidad con distintos perfiles de usuario

El sistema debe procurar que estudiantes con diferentes niveles de habilidad digital puedan usarlo sin barreras excesivas.

## 5.3. Privacidad y protección de datos

### RNF-08. Protección de datos del estudiante

El sistema debe proteger la información personal y pedagógica del estudiante.

### RNF-09. Acceso limitado por rol

La visibilidad de información debe estar restringida según rol, pertinencia y nivel de autorización.

### RNF-10. Minimización de datos

El sistema no debe recopilar más información de la necesaria para cumplir su propósito pedagógico y operativo.

### RNF-11. Separación entre datos sensibles y datos operativos

La plataforma debe distinguir entre información de uso general e información sensible o restringida.

## 5.4. Seguridad

### RNF-12. Autenticación de usuarios

El sistema debe asegurar que cada usuario acceda únicamente a las funciones y datos que le corresponden.

### RNF-13. Protección contra accesos no autorizados

La plataforma debe contar con mecanismos para prevenir consultas o modificaciones indebidas.

### RNF-14. Integridad de la información

Los datos del estudiante, del docente y del sistema no deben alterarse sin autorización o registro.

## 5.5. Trazabilidad y auditoría

### RNF-15. Registro de acciones relevantes

El sistema debe conservar trazabilidad sobre acciones pedagógicas y administrativas importantes.

### RNF-16. Explicabilidad de cambios del perfil

Las actualizaciones relevantes del perfil del estudiante deben poder rastrearse y explicarse.

### RNF-17. Auditoría de decisiones sensibles

Las acciones relacionadas con recursos generados por IA, cambios manuales del perfil o acceso a información sensible deben quedar registradas.

## 5.6. Explicabilidad y transparencia

### RNF-18. Explicabilidad de recomendaciones

Cuando el sistema recomiende una adaptación o recurso, debe poder mostrar por qué lo hace.

### RNF-19. Transparencia pedagógica

El docente debe contar con información suficiente para comprender la lógica general de personalización aplicada.

### RNF-20. Evitar caja negra total

El sistema no debe funcionar como un mecanismo completamente opaco para quienes toman decisiones pedagógicas.

## 5.7. Confiabilidad y consistencia

### RNF-21. Estabilidad del comportamiento adaptativo

El sistema no debe cambiar de manera errática sus decisiones de personalización ante evidencias aisladas o insuficientes.

### RNF-22. Consistencia de datos

La información mostrada a distintos actores debe ser coherente con los permisos y con el estado real del sistema.

### RNF-23. Consistencia pedagógica

Los recursos generados y las adaptaciones propuestas deben mantenerse alineados con el objetivo de aprendizaje definido.

## 5.8. Calidad pedagógica

### RNF-24. Pertinencia pedagógica del recurso

Los materiales generados por el sistema deben responder al objetivo de aprendizaje y al nivel del estudiante.

### RNF-25. Coherencia didáctica

Las decisiones adaptativas del sistema deben tener sentido pedagógico y no ser solo variaciones estéticas de presentación.

### RNF-26. Respeto por el juicio docente

La plataforma debe preservar la capacidad del docente para validar, ajustar o descartar recomendaciones y recursos.

## 5.9. Rendimiento y disponibilidad

### RNF-27. Tiempo de respuesta razonable

Las funciones centrales del sistema deben operar con tiempos de respuesta adecuados al contexto educativo.

### RNF-28. Disponibilidad funcional

El sistema debe mantener disponibilidad suficiente para que su uso en clase o en tareas de seguimiento no se vea afectado de forma frecuente.

### RNF-29. Fluidez en interacción básica

Las tareas principales, como consultar perfil, asignar actividades o responder recursos, deben ejecutarse sin demoras excesivas.

## 5.10. Escalabilidad y crecimiento

### RNF-30. Crecimiento progresivo por actores y cursos

La plataforma debe poder crecer en cantidad de estudiantes, docentes, grupos y cursos sin perder coherencia funcional.

### RNF-31. Extensibilidad por áreas o asignaturas

El sistema debe poder adaptarse a distintas asignaturas sin requerir rediseño total del núcleo del producto.

### RNF-32. Evolución de tipos de recurso

La arquitectura debe permitir incorporar nuevos tipos de recurso o estrategias de mediación a futuro.

## 5.11. Ética y gobernanza de IA

### RNF-33. Supervisión humana

Las decisiones pedagógicas sensibles apoyadas por IA deben mantener supervisión humana.

### RNF-34. Uso responsable de IA

La generación de recursos con IA debe evitar sesgos, errores evidentes, contenidos inadecuados o pedagogía débil.

### RNF-35. Separación entre recomendación y decisión final

El sistema debe diferenciar claramente entre lo que sugiere y lo que el docente finalmente aprueba o aplica.

### RNF-36. Prudencia adaptativa

La plataforma no debe sobreadaptar al estudiante ni fijarlo en una única forma de mediación sin evidencia suficiente.

## 6. Requisitos no funcionales prioritarios para el MVP

Para una primera versión, se recomienda priorizar especialmente:

- usabilidad básica para docente y estudiante;
- protección de datos y acceso por rol;
- trazabilidad mínima de acciones relevantes;
- explicabilidad básica de decisiones adaptativas;
- validación docente de recursos generados por IA;
- consistencia pedagógica de recursos y actividades;
- tiempos de respuesta razonables en funciones críticas.

## 7. Riesgos si estos requisitos no se cumplen

Si los requisitos no funcionales no se atienden adecuadamente, el sistema puede:

- perder confianza docente;
- exponer información sensible de estudiantes;
- producir decisiones opacas o poco defendibles;
- generar recursos pedagógicamente pobres;
- frustrar a usuarios por mala experiencia de uso;
- volverse difícil de sostener institucionalmente.

## 8. Relación con la efectividad del sistema

La efectividad de AdaptiveLearn no depende solo de que personalice, sino también de que lo haga en condiciones confiables, comprensibles, seguras y pedagógicamente válidas.

Por ello, los requisitos no funcionales son parte directa del valor del sistema y no solo un aspecto técnico secundario.

## 9. Formulación resumida

Los requisitos no funcionales de AdaptiveLearn establecen las condiciones de calidad necesarias para que la plataforma sea usable, segura, confiable, explicable, pedagógicamente pertinente y sostenible en contextos educativos reales.

## 10. Preguntas pendientes

- ¿Qué estándares mínimos de accesibilidad queremos adoptar?
- ¿Qué nivel de explicabilidad será suficiente para el docente en la primera versión?
- ¿Qué información sensible requerirá mayor protección institucional?
- ¿Qué tiempos de respuesta serán aceptables para generación de recursos con IA?
- ¿Qué mecanismos se usarán para controlar calidad pedagógica de recursos generados?
