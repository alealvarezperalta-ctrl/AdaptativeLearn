# 14. Requisitos funcionales del sistema

## 1. Propósito del documento

Este documento define los requisitos funcionales iniciales de AdaptiveLearn. Su propósito es traducir la visión pedagógica, los flujos de uso, los componentes funcionales y la lógica de personalización en capacidades concretas que el sistema debe ofrecer.

## 2. Idea central

Un requisito funcional describe algo que el sistema debe ser capaz de hacer.

En el caso de AdaptiveLearn, los requisitos funcionales deben expresar de manera clara cómo la plataforma:

- apoya al docente;
- interactúa con el estudiante;
- construye y actualiza perfiles;
- identifica mediaciones pedagógicas más efectivas;
- genera recursos con IA;
- personaliza enseñanza y evaluación;
- gestiona la información según actores y permisos.

## 3. Criterios de formulación

Los requisitos funcionales de AdaptiveLearn deben:

- ser claros y verificables;
- responder a una necesidad pedagógica o de gestión real;
- estar alineados con la lógica de competencias y personalización;
- evitar ambigüedad innecesaria;
- ser lo suficientemente concretos para orientar diseño y desarrollo.

## 4. Estructura propuesta

Para mantener orden, los requisitos se agrupan por áreas funcionales.

## 5. Requisitos funcionales por área

## 5.1. Gestión de usuarios, roles y vinculación

### RF-01. Registro y gestión de actores

El sistema debe permitir registrar y administrar usuarios con distintos roles, al menos:

- docente;
- estudiante;
- padre, madre o acudiente;
- administrativo institucional.

### RF-02. Asociación entre actores

El sistema debe permitir vincular estudiantes con:

- uno o varios docentes;
- un curso o grupo;
- la institución correspondiente;
- uno o más acudientes autorizados.

### RF-03. Control de acceso por rol

El sistema debe restringir funcionalidades e información visible según el rol del usuario.

## 5.2. Gestión pedagógica del docente

### RF-04. Creación de espacios pedagógicos

El sistema debe permitir al docente crear o gestionar cursos, grupos, clases o espacios de trabajo.

### RF-05. Definición de objetivos de aprendizaje

El sistema debe permitir al docente definir:

- tema o unidad;
- objetivo de aprendizaje;
- competencia o resultado esperado;
- evidencias que desea observar.

### RF-06. Configuración inicial de una experiencia

El sistema debe permitir que el docente prepare una experiencia de aprendizaje antes de asignarla a sus estudiantes.

## 5.3. Diagnóstico inicial del estudiante

### RF-07. Aplicación de diagnóstico inicial

El sistema debe permitir aplicar actividades diagnósticas al estudiante antes de iniciar la personalización.

### RF-08. Registro de evidencias diagnósticas

El sistema debe registrar al menos:

- respuestas;
- errores;
- tiempos de respuesta;
- intentos;
- uso de ayudas, cuando aplique.

### RF-09. Generación de perfil inicial

A partir del diagnóstico, el sistema debe generar una primera versión del perfil de aprendizaje del estudiante.

## 5.4. Gestión del perfil de aprendizaje

### RF-10. Creación del perfil del estudiante

El sistema debe crear un perfil de aprendizaje para cada estudiante.

### RF-11. Registro de variables del perfil

El sistema debe almacenar como mínimo las variables principales definidas por el proyecto, entre ellas:

- nivel de dominio;
- ritmo de aprendizaje;
- formato de mediación más efectivo;
- nivel de autonomía;
- patrones de dificultad.

### RF-12. Actualización progresiva del perfil

El sistema debe actualizar el perfil del estudiante con base en nuevas evidencias de interacción y desempeño.

### RF-13. Historial del perfil

El sistema debe conservar historial de cambios y actualizaciones del perfil.

### RF-14. Distinción entre perfil transversal y contextual

El sistema debe diferenciar la información del perfil que puede reutilizarse entre clases de aquella que es específica de una asignatura, tema o docente.

## 5.5. Personalización y decisión adaptativa

### RF-15. Generación de decisiones adaptativas

El sistema debe traducir el perfil del estudiante en decisiones de personalización.

### RF-15A. Identificación de mediaciones pedagógicas efectivas

El sistema debe identificar, con base en evidencias acumuladas, qué tipos de mediación pedagógica parecen más efectivos para cada estudiante en relación con un objetivo de aprendizaje.

### RF-16. Adaptación del formato del contenido

El sistema debe poder seleccionar o sugerir distintos formatos de mediación, por ejemplo:

- visual;
- auditivo;
- textual o guiado;
- práctico o interactivo;
- combinado.

### RF-17. Adaptación de dificultad y apoyo

El sistema debe ajustar dificultad, secuencia y nivel de apoyo con base en el perfil y en el desempeño reciente del estudiante.

### RF-18. Adaptación de evaluación

El sistema debe poder sugerir o configurar evaluaciones personalizadas según el nivel y progreso del estudiante.

## 5.6. Generación de recursos con IA

### RF-19. Generación de recursos didácticos

El sistema debe generar recursos educativos personalizados con apoyo de IA.

### RF-20. Tipos de recursos generables

El sistema debe poder generar, al menos de forma progresiva:

- explicaciones;
- ejercicios;
- evaluaciones;
- recursos visuales;
- recursos interactivos;
- otros materiales de apoyo.

### RF-21. Coherencia pedagógica del recurso

El sistema debe vincular cada recurso generado con el objetivo de aprendizaje y con la lógica adaptativa aplicada.

### RF-22. Validación docente de recursos

El sistema debe permitir al docente revisar, aprobar, editar o rechazar recursos generados antes de su asignación final al estudiante.

## 5.7. Ejecución de actividades y evaluación

### RF-23. Asignación de actividades

El sistema debe permitir asignar al estudiante actividades y recursos personalizados.

### RF-24. Interacción del estudiante

El sistema debe permitir que el estudiante interactúe con recursos, ejercicios y evaluaciones desde su espacio de trabajo.

### RF-25. Registro de desempeño

El sistema debe registrar el comportamiento del estudiante durante la interacción con las actividades.

### RF-26. Retroalimentación

El sistema debe proporcionar retroalimentación al estudiante durante o después de la actividad, según el diseño pedagógico.

## 5.8. Seguimiento y analítica

### RF-27. Visualización del progreso del estudiante

El sistema debe mostrar al docente el progreso del estudiante de forma comprensible y útil para la intervención pedagógica.

### RF-28. Identificación de patrones relevantes

El sistema debe detectar y mostrar patrones de desempeño, dificultades recurrentes y tendencias de evolución.

### RF-29. Recomendaciones pedagógicas

El sistema debe ofrecer recomendaciones al docente con base en el perfil y en la analítica del estudiante.

### RF-30. Reportes resumidos para acompañamiento

El sistema debe generar reportes resumidos para estudiantes, padres o acudientes y otros actores autorizados.

## 5.9. Reutilización transversal del conocimiento del estudiante

### RF-31. Conservación del historial transversal

El sistema debe conservar información transversal del estudiante que pueda ser útil en distintas clases o asignaturas.

### RF-32. Disponibilidad del perfil para otros docentes autorizados

El sistema debe permitir que otros docentes autorizados consulten la parte transversal del perfil del estudiante.

### RF-33. Protección de la información contextual

El sistema debe evitar que información específica de una clase se reutilice sin contexto o se presente como general.

## 5.10. Roles, visibilidad y supervisión

### RF-34. Vista diferenciada por actor

El sistema debe ofrecer interfaces y vistas diferenciadas según el rol del usuario.

### RF-35. Acceso de padres o acudientes

El sistema debe permitir que los acudientes accedan a información resumida del progreso del estudiante, sin otorgarles funciones de intervención pedagógica.

### RF-36. Acceso de administrativos

El sistema debe permitir que administrativos autorizados consulten información agregada o resumida para supervisión institucional.

### RF-37. Registro de acciones relevantes

El sistema debe registrar acciones importantes relacionadas con:

- aprobación de recursos;
- cambios del perfil;
- asignación de actividades;
- consulta de información sensible;
- acciones manuales sobre decisiones adaptativas.

## 6. Requisitos funcionales prioritarios para el MVP

Aunque el sistema completo tendrá muchas capacidades, para una primera versión se recomienda priorizar:

- gestión básica de docente y estudiante;
- creación de una experiencia de aprendizaje;
- diagnóstico inicial;
- generación de perfil inicial;
- actualización básica del perfil;
- generación de recursos personalizados con IA;
- validación docente;
- asignación de actividades;
- recolección de evidencias;
- visualización básica de progreso.

## 7. Riesgos al definir requisitos funcionales

Los requisitos funcionales no deben:

- volverse demasiado abstractos;
- mezclar requisitos funcionales con decisiones técnicas internas;
- prometer automatización total sin validación pedagógica;
- ignorar restricciones de permisos y visibilidad;
- crecer sin priorización para el MVP.

## 8. Formulación resumida

Los requisitos funcionales de AdaptiveLearn describen las capacidades concretas que necesita la plataforma para diagnosticar al estudiante, construir y actualizar su perfil, personalizar recursos y evaluación, asistir al docente y permitir una gestión diferenciada de la información según actores y roles.

## 9. Preguntas pendientes

- ¿Qué requisitos deben considerarse obligatorios en la primera versión y cuáles pueden esperar?
- ¿Qué requisitos necesitarán validación pedagógica antes de implementarse?
- ¿Qué requisitos dependerán de la infraestructura o del proveedor de IA?
- ¿Qué funciones del sistema serán totalmente automáticas y cuáles requerirán confirmación docente?
- ¿Cómo se traducirán estos requisitos en historias de usuario o backlog de desarrollo?
