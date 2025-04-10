#<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - LessonsLearned

### Sprint 3

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** José Manuel Miret, José Gonzalo Domínguez


### Integrantes
<div style="columns: 2; -webkit-columns: 2; -moz-columns: 2;">

- Mohamed Abouri  
- Mario Astudillo Fierro  
- María Barrancos Márquez  
- Rafael Cabello Ranea  
- Manuel Chica López  
- David Delgado Pallares  
- José Gonzalo Domínguez Moreno  
- Virginia Mesa Pérez  
- José Manuel Miret Martín  
- Alejandro Nicolade Bravo  
- Manuel Palacios Pineda  
- Pablo Rodríguez Sánchez  
- Rubén Romero Sánchez  
- Paula Sánchez Gómez  
- Ramón Vergara Garrido  

</div>

---

# Sprint 1

Durante este sprint nos hemos enfrentado a varios desafíos, principalmente derivados del hecho de que hemos comenzado el desarrollo de la aplicación desde cero. A continuación, detallamos cada uno de los problemas que hemos encontrado:

## Falta de idea de negocio clara

**Descripción:** 

La falta de una idea de negocio clara es un reto significativo que nuestro proyecto se ha encontrado, que provoca que trabajemos en la dirección equivocada. Tuvimos que hacer un cambio de proyecto y elegir una nueva idea. Durante esta fase de transición, la idea de negocio aún estaba muy general y no fue lo suficientemente definida, lo que dejó espacio a diversas interpretaciones por parte de los miembros del equipo. 

**Causa:**  

Falta de definición del producto software que se pretendía desarrollar y de su consecuente modelo de negocio.

**¿Qué se ha hecho?:** 

Para resolver esta falta de claridad, realizamos una reunión exhaustiva en la que definimos de manera precisa la idea de negocio. Esto aseguró que todos los miembros del equipo estuvieran alineados y compartiéramos una visión común. El feedback del profesorado y de otros compañeros fue una ayuda importante.

**Análisis de la solución:** 

Obtener un objetivo claro nos permitió alinear objetivos, distribuir las tareas con mayor eficiencia y tomar mejores decisiones técnicas. Nos ayudó también a conocer nuestro público objetivo y establecer un alcance del proyecto realista.  La aplicación de esta solución supuso una desviación en el cronograma inicial que nos supone una pequeña pérdida de tiempo.

**¿Qué se podría haber hecho?:** 

Una buena práctica en la dirección de proyectos es establecer una documentación mínima que definiera la visión y objetivos del proyecto. También, asignar a un miembro del equipo como Product Owner asegura una coherecia y cierta validez en el modelo de negocio. ****

## Problemas con la base de datos

**Descripción:** 

Inicialmente, se consideró utilizar CloudSQL de Google para la base de datos, sin embargo, se decidió cambiar y optar por un base datos PostgreSQL, mantenida por Azure.

**Causa:** 

A pesar de ser una base de datos óptima para nuestro alcance de proyecto, CloudSQL era un acoste adicional que no era viable teniendo la gratuidad de Azure.

**¿Qué se ha hecho?:** 

Se optó por utilizar PostgreSQL como alternativa para la infraestructura del proyecto

**Análisis de la solución:** 

El cambio a PostgreSQL en Azure se implementó de manera efectiva y sin grandes fricciones técnicas, ya que PostgreSQL es una base de datos robusta y ampliamente soportada. Sin embargo, este cambio requirió ajustes en la configuración de acceso y la gestión de credenciales, lo que implicó un tiempo adicional no contemplado en el cronograma inicial.

**¿Qué se podría haber hecho?:** 

Realizar un análisis de costes y viabilidad técnica más detallado desde la fase de planificación. Consultar las condiciones de uso gratuitas de las distintas plataformas cloud antes de tomar decisiones de infraestructura.

## Falta de comunicación

**Descripción:** 

Algunos miembros han trabajado por separado y se ha producido código duplicado, lo que ha llevado a la pérdida de tiempo y eliminación del trabajo de parte del equipo.

**Causa:** 

Se han asignado tareas de extensa duración a varias personas sin establecer una comunicación clara entre ellas.  ****

**¿Qué se ha hecho?:** 

Para evitar este problema, se ha decidido dividir las tareas más grandes en subtareas y mejorar la comunicación dentro del equipo. Se fomentará el trabajo colaborativo y la sincronización antes de desarrollar código

**Análisis de la solución:** 

La división en subtareas y mejoras en la comunicación ha tenido un impacto positivo inmediato. Se ha aumentado la transparencia del trabajo y mejorado la cohesión del equipo. No obstante, aún es necesario consolidar estas prácticas y revisar periódicamente la asignación de tareas para asegurar una correcta distribución del trabajo.

**¿Qué se podría haber hecho?:** 

Una de las soluciones más evidentes tras analizar el problema podría haber sido la definición clara de roles y responsabilidades, especialmente en tareas críticas o que implican colaboración entre varios miembros. Otra buen solución es reconocer la importancia de herramientas de gestión de tareas desde las primeras fases del proyecto.

## Ejecución tardía de tareas

**Descripción:** 

Durante el desarrollo del proyecto, varias tareas fueron terminadas fuera del plazo esperado. Esto provocó un efecto dominó  sobre otras tareas dependientes de estas y afectó negativamente al entregable del sprint. Este problema nos ocasinó estrés y acumulación de trabajo al  final del sprint.

**Causa:** 

Falta de estimaciones realistas en los tiempos de entrega, escasa priorización de tareas y un seguimiento insuficiente del avance del equipo. Además, se subestimó la carga de trabajo académico externa, lo que redujo la disponibilidad real de los miembros del equipo en momentos críticos.

**¿Qué se ha hecho?:** 

Una reorganización del cronograma, priorizando las tareas críticas. También, se empezó a utilizar herramientas del estilo Kanban y se hicero más reuniones de seguimiento (dailys). Finalmente, se dio un aviso general sobre la importancia de las fechas límites.

**Análisis de la solución:** 

La aplicación de estos cambios permitió una mejor planificación semanal y mayor visibilidad sobre el avance real del proyecto. Aunque no se pudo recuperar todo el tiempo perdido, se consiguió reducir la presión en las últimas semanas y entregar los entregables esenciales a tiempo. Sin embargo, la mejora en la ejecución debe consolidarse como un proceso continuo.

**¿Qué se podría haber hecho?:** 

No hay una solución clara pero por supuesto, hay algunas que podrían haber mejorado la situación. Por ejemplo, invertir más tiempo en la planificación inicial o alinear mejor los compromisos individuales con los intereses del proyecto. 

## Dificultad en la gestión de un equipo grande

**Descripción:** 

La gestión de un equipo de estas dimensiones ha sido uno de los grandes retos del inicio del proyecto. La coordinación entre los miembros del equipo no ha sido efectiva, lo que ha derivado en problemas mencionados anteriormente.

**Causa:** 

Hay falta de experiencia en la dirección de proyectos dentro del equipo de trabajo y las experiencias previas han sido en equipo con menos número de miembros. Debido a esto ha habido errores como no definir en el inicio los roles y responsabilidades de forma clara.  La ausencia de una estructura organizativa funcional limitó la capacidad de liderazgo distribuido y generó dependencia de decisiones centralizadas.

**¿Qué se ha hecho?:** 

Se clarificó los roles y responsabilidades del equipo de trabajo. Además, se establecieron líderes responsables de áreas concretas del proyecto, promoviendo así una gestión más descentralizada y efectiva. También se incrementó la frecuencia de reuniones breves de seguimiento (dailies) para mantener a todo el equipo alineado y facilitar la resolución temprana de conflictos o bloqueos.

**Análisis de la solución:**  

Se aumentó la eficiencia en la toma de decisiones y se  mejoró la comprensión de las tareas asignadas y redujo la duplicidad de esfuerzos. Sin embargo, la implementación se produjo en una fase avanzada del proyecto, por lo que su impacto fue más correctivo que preventivo.

**¿Qué se podría haber hecho?:** 

Desde el inicio del proyecto, se podría haber aplicado el proceso de *Planificación de la Gestión de los Recursos* del PMBOK, que incluye la definición de roles, responsabilidades, estructura organizacional y plan de desarrollo del equipo. También habría sido útil definir un *Plan de Gestión de las Comunicaciones* más detallado, con canales formales e informales bien definidos para asegurar el flujo constante de información.

# Sprint 2

Durante este sprint nos hemos enfrentado a varios desafíos. Algunos de ellos son los mismos que se presentaron la semana pasada, ya que la solución implementada no tuvo el resultado esperado, por lo que ha aumentado el número de problemas con respecto el anterior sprint. A continuación, detallamos cada uno de los problemas que hemos encontrado:

## Falta de comunicación

**Descripción:** Durante el transcurso del proyecto se detectaron fallos de comunicación entre los miembros del equipo, lo que provocó duplicidad de código, malentendidos en los requisitos y descoordinación en la ejecución de tareas. Esto afectó negativamente al cumplimiento de los plazos y la calidad de algunos entregables.

**Causa:** No se aplicó un plan de gestión de las comunicaciones desde el inicio del proyecto. Se asumió que la comunicación informal era suficiente para la coordinación del equipo, lo que resultó inefectivo a medida que el proyecto se volvía más complejo. **** 

**¿Qué se ha hecho?:** Se estableció un plan de comunicación con reuniones periódicas (reuniones semanales de seguimiento), asignación de responsables y uso de herramientas colaborativas (como Discord y Notion). Además, se reforzó la documentación escrita para reducir la ambigüedad y facilitar el traspaso de conocimiento.

**Análisis de la solución:** Estas medidas permitieron mejorar considerablemente el flujo de información y la transparencia dentro del equipo. Las reuniones más estructuradas ayudaron a alinear prioridades y detectar bloqueos a tiempo. La documentación también contribuyó a reducir errores. No obstante, su implementación tardía hizo que los beneficios se notaran solo en fases posteriores/finales del proyecto.

**¿Qué se podría haber hecho?:** Elaborar desde el inicio un Plan de Gestión de las Comunicaciones incluyendo definición de qué comunicar, cómo, con qué frecuencia y por qué canal.

## Ejecución tardía de tareas

Este problema es recurrente en el desarrollo del proyecto y se ha mencionado en los problemas encontrados de sprints anteriores.

**Descripción:** 

Durante el desarrollo del proyecto, varias tareas fueron terminadas fuera del plazo esperado. Esto provocó un efecto dominó  sobre otras tareas dependientes de estas y afectó negativamente al entregable del sprint. Este problema nos ocasinó estrés y acumulación de trabajo al  final del sprint.

**Causa:** 

Falta de estimaciones realistas en los tiempos de entrega, escasa priorización de tareas y un seguimiento insuficiente del avance del equipo. Además, se subestimó la carga de trabajo académico externa, lo que redujo la disponibilidad real de los miembros del equipo en momentos críticos.

**¿Qué se ha hecho?:** 

Una reorganización del cronograma, priorizando las tareas críticas. Los directores de proyecto dieron un toque de atención al equipo en general, destacando la importancia de las fechas límites.

**Análisis de la solución:** 

La reorganización del cronograma permitió reenfocar los esfuerzos del equipo en las tareas más críticas, lo cual fue esencial para recuperar parte del tiempo perdido. La intervención directa de los responsables del proyecto sirvió como llamada de atención y contribuyó a un mayor nivel de compromiso por parte del equipo. Sin embargo, la solución fue reactiva y no preventiva. Si bien se logró mitigar el impacto del retraso, no se abordaron del todo las causas raíz, como la falta de seguimiento continuo o la escasa estimación del esfuerzo real de algunas tareas.

**¿Qué se podría haber hecho?:** 

No hay una solución clara pero por supuesto, hay algunas que podrían haber mejorado la situación. Por ejemplo, invertir más tiempo en la planificación inicial o alinear mejor los compromisos individuales con los intereses del proyecto. 

## Dificultad en la gestión de equipo

Este problema es recurrente en el deserrallo del proyecto y se ha mencionado en los problemas encontrados de sprints anteriores.

**Descripción:**

Durante el desarrollo del proyecto, se han evidenciado dificultades en la gestión del equipo. Estas se reflejaron en una baja coordinación, fallos en la asignación de tareas, retrasos acumulados y una disminución del rendimiento colectivo. También se observaron situaciones de desmotivación y falta de compromiso por parte de algunos miembros.

**Causa:**

Estas dificultades fueron causadas principalmente por la falta de un plan de gestión de los recursos humanos desde el inicio del proyecto. No se definieron adecuadamente los roles, las responsabilidades, ni se desarrolló una estrategia para fomentar el rendimiento del equipo. Además, no se establecieron herramientas ni procesos claros para monitorear el desempeño y facilitar la resolución de conflictos.

**¿Qué se ha hecho?:**

Se aplicaron medidas correctivas tales como la redistribución de tareas según las fortalezas individuales, la implementación de reuniones de seguimiento más frecuentes y el uso de herramientas colaborativas como tableros digitales para visualizar el progreso. También se impulsaron espacios de comunicación más informal para mejorar la cohesión del equipo y se hizo hincapié en la importancia del cumplimiento de compromisos.

**Análisis de la solución:**

Estas acciones ayudaron a mejorar temporalmente la organización interna y facilitaron la identificación temprana de problemas. Sin embargo, la ausencia de una planificación inicial estructurada y de una cultura de equipo sólida limitó la efectividad de estas acciones correctivas. La solución fue reactiva y no preventiva, por lo que el impacto positivo llegó tarde en el cronograma del proyecto.

**¿Qué se podría haber hecho?:**

Se podría haber elaborado desde el inicio un **Plan de Gestión de los Recursos**. Este plan incluye la identificación de los roles y responsabilidades, un organigrama del equipo, un plan de capacitación si fuera necesario, y estrategias para desarrollar y liderar al equipo. 

## Falta de comunicación entre backend y frontend

**Descripción:**

Durante el desarrollo del proyecto, se identificaron desajustes entre el equipo de backend y el de frontend. Estos incluían endpoints no documentados, desacuerdos en los formatos de datos (por ejemplo, estructuras JSON), y una descoordinación en los tiempos de entrega. Esto generó bloqueos y frustración entre los desarrolladores.

**Causa:**

La raíz del problema se encuentra en la **ausencia de un plan de gestión de las comunicaciones**, así como en la falta de mecanismos claros de integración entre los equipos técnicos. No se establecieron entregables intermedios ni una documentación estandarizada de la API. Además, no se definieron reuniones conjuntas ni responsables de enlace técnico entre los dos equipos.

**¿Qué se ha hecho?:**

Se programaron reuniones periódicas de sincronización entre ambos equipos para resolver bloqueos y alinear expectativas. Se implementó una documentación en Swagger/OpenAPI de los endpoints. Además, se comenzó a dar importancia a la comunicación directa y continua por Discord para resolver dudas rápidamente.

**Análisis de la solución:**

Estas acciones contribuyeron a mejorar notablemente la comunicación y permitieron una integración más fluida entre el frontend y el backend. La documentación de las APIs y la creación de espacios de diálogo técnico fueron especialmente eficaces. Sin embargo, al tratarse de una solución implementada en fases avanzadas del proyecto, no evitó del todo los retrabajos iniciales.

**¿Qué se podría haber hecho?:**

Se debería haber definido qué información se compartiría entre backend y frontend (por ejemplo, especificaciones técnicas, cronogramas de endpoints, etc.). Además saber con antelación con qué frecuencia y a través de qué canales se llevarían a cabo estas comunicaciones.

## Problemas al combinar ramas

**Descripción:**

Durante el desarrollo del proyecto, se presentaron conflictos frecuentes al combinar ramas de código en el repositorio principal. Estos conflictos causaron pérdida de tiempo, errores de integración y, en algunos casos, la sobrescritura o eliminación de trabajo realizado por otros compañeros. Este problema también generó una desaceleración en el avance del proyecto y afectó la moral del equipo.

**Causa:**

La causa principal fue la **falta de una estrategia clara de control de versiones**, junto con una **ausencia de lineamientos estandarizados para el uso de Git**. Muchos desarrolladores trabajaban sobre la misma rama o tardaban demasiado en sincronizar sus ramas con la rama principal ( main o enhance), lo que aumentaba las probabilidades de conflicto. Además, no existía una figura responsable del control de calidad en las integraciones.

**¿Qué se ha hecho?:**

Se definió un **flujo de trabajo Git (Git Flow simplificado)**, en el que cada desarrollador trabaja sobre ramas de características (feature/, fix/ …) y realiza pull requests hacia la rama de desarrollo una vez finalizada la tarea. Además, se integró la herramienta **CodiumAI PR-Agent** para asistir en el análisis automático de *pull requests*, generando resúmenes, sugerencias y validaciones antes de la revisión manual, lo que mejoró la calidad y coherencia del código subido.

**Análisis de la solución:**

Estas medidas han sido efectivas para reducir los conflictos y mejorar el control sobre el código integrado. El uso de CodiumAI PR-Agent ha agilizado y estandarizado el proceso de revisión, permitiendo identificar posibles errores o inconsistencias de manera temprana. Aunque fue necesario un periodo inicial de adaptación, el equipo se ha beneficiado de una mejor organización y mayor calidad en las integraciones.

**¿Qué se podría haber hecho?:**
Desde el inicio del proyecto se debería haber definido un **Plan de Gestión de la Configuración**, incluyendo una estrategia de ramas, políticas de merge, y herramientas de automatización.

## Errores internos de la aplicación

**Descripción:**

Durante las pruebas funcionales y los primeros despliegues del sistema, se detectaron varios errores internos de la aplicación, como fallos en la lógica de negocio, errores no controlados en endpoints, y respuestas inconsistentes entre el frontend y el backend. Esto afectó negativamente la experiencia del usuario y provocó tiempos extra de depuración.

**Causa:**

La principal causa fue una **falta de pruebas exhaustivas y automatizadas** antes del despliegue, combinada con **una integración temprana de módulos no suficientemente validados**. Además, algunos desarrolladores no gestionaron correctamente los errores ni definieron adecuadamente las validaciones necesarias.

**¿Qué se ha hecho?:**

Se implementaron pruebas unitarias y se estableció una política de manejo centralizado de errores y se reforzó el uso de validadores para asegurar datos consistentes. En la gran mayoría de los errores, el equipo de trabajo ha respondido con buena actitud, invierto más tiempo y esfuerzo a la resolución de estos errores: No obstante, de haberse evitado los errores, se habría aumentado en gran medida la eficiencia del desarrollo.

**Análisis de la solución:**

La implementación de pruebas unitarias y validadores ha reducido la cantidad de errores en etapas posteriores, mejorando la estabilidad de la aplicación. El enfoque en el manejo centralizado de errores ha facilitado el diagnóstico de problemas. Sin embargo, el tiempo adicional invertido en corregir fallos que podrían haberse evitado impactó la eficiencia general del desarrollo.

**¿Qué se podría haber hecho?:**

Se debería haber organizado desde el inicio  la integración de pruebas automáticas como parte del flujo de integración continua (CI) y revisiones de código con foco en detección temprana de errores.

## Demora con usuarios pilotos

**Descripción:**

Se ha detectado una demora significativa en la respuesta a consultas, incidencias y feedback proporcionado por los usuarios pilotos durante la fase de validación del sistema.

**Causa:**

La demora se debió al retraso en el desarrollo y entrega de tareas y componentes del código que debían presentarse a los usuarios para su validación. Estos retrasos impactaron directamente en la capacidad de respuesta y seguimiento a los pilotos, al no disponer de versiones funcionales a tiempo.

**¿Qué se ha hecho?:**

Se replanificó el backlog ajustando los tiempos y prioridades para asegurar que las funcionalidades críticas estén disponibles para las siguientes iteraciones. Se realizó una revisión con el equipo técnico para identificar cuellos de botella y redistribuir carga de trabajo.

**Análisis de la solución:**

Estas acciones han permitido recuperar parcialmente la confianza de los usuarios, reducir la incertidumbre y garantizar que las próximas entregas cumplan con los compromisos establecidos. También se ha logrado mayor visibilidad del avance del proyecto mediante actualizaciones periódicas.

**¿Qué se podría haber hecho?:**

Estimar de forma más realista los tiempos de desarrollo y validación. Aplicar prácticas de integración continua más rigurosas para reducir tiempos de entrega.