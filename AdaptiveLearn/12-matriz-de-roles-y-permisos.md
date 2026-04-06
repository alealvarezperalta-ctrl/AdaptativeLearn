# 12. Matriz de roles y permisos

## 1. Propósito del documento

Este documento define la matriz inicial de roles y permisos de AdaptiveLearn. Su objetivo es establecer con claridad qué puede hacer cada actor dentro del sistema, qué información puede consultar y qué acciones quedan restringidas según su función pedagógica, de acompañamiento o de supervisión.

## 2. Idea central

AdaptiveLearn necesita una estructura de permisos coherente con su propósito pedagógico.

No todos los actores deben:

- ver la misma información;
- tomar las mismas decisiones;
- intervenir sobre el mismo nivel del sistema;
- acceder a datos sensibles con el mismo alcance.

La matriz de permisos debe proteger el rol del docente, garantizar el acompañamiento del estudiante, permitir la observación de familias y administrativos, y conservar trazabilidad sobre quién hace qué dentro de la plataforma.

## 3. Principios generales de permisos

La definición de permisos debe seguir estos principios:

- **pertinencia:** cada actor accede solo a lo necesario para su rol;
- **mínimo privilegio:** nadie debe tener más permisos de los que requiere;
- **protección pedagógica:** las decisiones formativas centrales siguen bajo control docente;
- **protección de datos:** la información del estudiante debe mostrarse con niveles adecuados de sensibilidad;
- **trazabilidad:** las acciones relevantes deben poder auditarse;
- **claridad institucional:** los permisos deben ser comprensibles y sostenibles.

## 4. Roles principales considerados

Para esta primera versión documental se trabajará con cuatro roles principales:

- docente;
- estudiante;
- padre, madre o acudiente;
- administrativo institucional.

En el futuro podrían existir subroles adicionales, pero esta primera matriz debe mantener claridad y simplicidad.

## 5. Tipos generales de permiso

Se propone clasificar los permisos en cinco tipos:

- **crear/configurar**
- **consultar**
- **aprobar o validar**
- **interactuar o ejecutar**
- **supervisar o monitorear**

## 6. Matriz general de permisos

| Acción o capacidad | Docente | Estudiante | Padres/acudientes | Administrativos |
|---|---|---|---|---|
| Crear curso, grupo o espacio de trabajo | Sí | No | No | No |
| Vincular estudiantes a un grupo | Sí | No | No | Limitado |
| Definir objetivos de aprendizaje | Sí | No | No | No |
| Activar diagnóstico inicial | Sí | No | No | No |
| Responder diagnóstico | No | Sí | No | No |
| Consultar perfil pedagógico completo del estudiante | Sí | No | No | Limitado |
| Consultar versión resumida del progreso | Sí | Sí | Sí | Sí, agregada |
| Editar manualmente el perfil del estudiante | Limitado | No | No | No |
| Aprobar recursos generados por IA | Sí | No | No | No |
| Editar recursos antes de asignarlos | Sí | No | No | No |
| Asignar actividades o evaluaciones | Sí | No | No | No |
| Resolver actividades y evaluaciones | No | Sí | No | No |
| Ver retroalimentación individual detallada | Sí | Sí | Limitado | No |
| Ver analítica del grupo | Sí | No | No | Sí |
| Ver analítica institucional agregada | Limitado | No | No | Sí |
| Ver alertas pedagógicas individuales | Sí | No | Limitado | Limitado |
| Recibir recomendaciones de acompañamiento | Sí | Sí | Sí | No |
| Supervisar adopción y uso institucional | No | No | No | Sí |
| Modificar configuración general del sistema | No | No | No | Limitado |

## 7. Interpretación por rol

## 7.1. Docente

### Rol funcional

Es el actor con mayor responsabilidad pedagógica directa.

### Permisos centrales

- configurar el proceso de enseñanza;
- revisar perfil y progreso del estudiante;
- validar recursos, actividades y evaluaciones;
- intervenir pedagógicamente con base en la información del sistema.

### Restricciones recomendadas

- no debería modificar libremente el historial automático del perfil sin trazabilidad;
- no debería acceder a configuraciones institucionales que no correspondan a su curso o grupo.

## 7.2. Estudiante

### Rol funcional

Es el actor que ejecuta la experiencia de aprendizaje.

### Permisos centrales

- acceder a recursos asignados;
- responder actividades y evaluaciones;
- consultar su progreso en formato comprensible;
- recibir retroalimentación y próximos pasos.

### Restricciones recomendadas

- no puede alterar el perfil;
- no puede acceder a datos de otros estudiantes;
- no puede modificar decisiones adaptativas ni recursos aprobados por el docente.

## 7.3. Padres, madres o acudientes

### Rol funcional

Son actores de acompañamiento familiar.

### Permisos centrales

- consultar progreso general del estudiante;
- observar fortalezas y dificultades generales;
- recibir recomendaciones para acompañamiento en casa;
- mantenerse informados del proceso.

### Restricciones recomendadas

- no deben intervenir en decisiones pedagógicas;
- no deben editar información del perfil;
- no deben ver analítica técnica o comparativa sensible;
- no deben acceder a información de otros estudiantes.

## 7.4. Administrativos institucionales

### Rol funcional

Son actores de supervisión y seguimiento institucional.

### Permisos centrales

- consultar indicadores agregados;
- observar niveles de adopción, participación y uso;
- revisar reportes de seguimiento por grupo o institución;
- acompañar decisiones institucionales de implementación.

### Restricciones recomendadas

- no deben modificar directamente recursos de clase;
- no deben intervenir en decisiones didácticas del docente;
- no deben ver más detalle individual del necesario para su rol.

## 8. Niveles de acceso a la información del estudiante

Para proteger adecuadamente la información del estudiante, se recomienda trabajar con cuatro niveles de acceso.

### 8.1. Nivel completo pedagógico

Visible para el docente.

Incluye:

- perfil detallado;
- historial de actualizaciones;
- evidencias de aprendizaje;
- decisiones adaptativas;
- alertas pedagógicas;
- recomendaciones del sistema.

### 8.2. Nivel personal de aprendizaje

Visible para el estudiante.

Incluye:

- actividades asignadas;
- progreso general;
- retroalimentación;
- metas o próximos pasos.

No necesariamente incluye el modelo técnico completo del perfil.

### 8.3. Nivel de acompañamiento familiar

Visible para padres o acudientes.

Incluye:

- avance general;
- fortalezas;
- dificultades generales;
- recomendaciones de acompañamiento;
- alertas relevantes para apoyo familiar.

### 8.4. Nivel de supervisión institucional

Visible para administrativos.

Incluye:

- indicadores agregados;
- información resumida por curso, grupo o institución;
- tendencias generales;
- nivel de adopción y seguimiento.

## 9. Acciones que deberían requerir validación especial

En la primera versión, ciertas acciones deberían quedar especialmente controladas:

- aprobación final de recursos generados por IA;
- asignación de evaluaciones personalizadas;
- cambios manuales sobre el perfil del estudiante;
- acceso a información sensible individual por fuera del rol docente;
- cambios de configuración institucional.

## 10. Acciones que deben quedar registradas

Por criterios de trazabilidad y confianza, el sistema debería registrar al menos:

- quién creó o modificó un curso o grupo;
- quién aprobó un recurso generado por IA;
- cuándo se asignó una actividad o evaluación;
- cuándo se consultó o revisó información sensible del estudiante;
- cuándo se hizo un ajuste manual sobre una decisión del sistema.

## 11. Relación entre permisos y flujo del sistema

La matriz de roles y permisos debe mantenerse alineada con el flujo general de uso.

Esto implica que:

- en las primeras etapas domina el rol docente;
- durante la ejecución domina el rol del estudiante;
- durante el acompañamiento y seguimiento participan padres y administrativos;
- en todas las etapas debe mantenerse la distinción entre intervención, observación y supervisión.

## 12. Riesgos a evitar

La definición de permisos no debe:

- dar demasiado poder a actores que no tienen rol pedagógico directo;
- exponer información sensible sin necesidad;
- impedir al docente ejercer control real sobre el proceso;
- convertir a padres o administrativos en editores del aprendizaje;
- dejar acciones relevantes sin trazabilidad.

## 13. Formulación resumida

La matriz de roles y permisos de AdaptiveLearn organiza el acceso y la intervención de docentes, estudiantes, padres o acudientes y administrativos, garantizando que cada actor participe con el nivel de acción, consulta y supervisión adecuado a su función dentro del proceso educativo personalizado.

## 14. Preguntas pendientes

- ¿Qué subroles administrativos existirán dentro de la institución?
- ¿Qué tan detallada será la información visible para padres o acudientes?
- ¿Qué acciones manuales del docente quedarán registradas como auditoría?
- ¿Qué permisos excepcionales existirán para soporte técnico o administración de plataforma?
- ¿Cómo se configurarán estos permisos en la interfaz real del sistema?
