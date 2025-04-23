
<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - LessonsLearnedS1

### PPL

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** José Manuel Miret, José Gonzalo Domínguez


### Integrantes
<div style="columns: 2; -webkit-columns: 2; -moz-columns: 2;">

- Mohamed Abouri  
- Mario Astudillo Fierro  
- María Barrancos Márquez  
- Rafael Cabello Ranea  
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

# Análisis detallado de las condiciones de fallo

Durante el desarrollo y despliegue de la aplicación, se utilizó la **misma instancia de base de datos para los entornos de desarrollo y producción**. Esto derivó en una serie de errores críticos en la aplicación en producción, incluyendo la **imposibilidad de iniciar sesión**, realizar reservas u otras operaciones que requerían integridad y disponibilidad de los datos. Estos errores impactaron directamente la experiencia de los usuarios finales y comprometieron la estabilidad del sistema en funcionamiento.

# Listado de problemas

Durante este sprint nos hemos enfrentado a varios desafíos, principalmente derivados del hecho de que hemos comenzado el desarrollo de la aplicación desde cero. Estos problemas han afectado directa o indirectamente al despliegue  final del sprint 1 y al consecuente suspenso. A continuación, detallamos cada uno de ellos y su relación con la condición de fallo mencionda anteriormente:

## Falta de idea de negocio clara

Identificado por el equipo antes de la entrega. Tras observar los efectos negativos en el despliegue y en la dirección general del proyecto, el equipo reconoció que la raíz estaba en una idea de negocio mal definida.

**Análisis detallado de las condiciones del fallo respecto al entregable:** 

La falta de una idea de negocio clara fue uno de los problemas estructurales más críticos del proyecto. Esto generó **desalineación en la visión del producto**, decisiones técnicas sin justificación y un desarrollo sin foco, lo que finalmente impactó el **despliegue**. La indefinición del producto llevó a una gestión ineficiente de recursos y tiempo, y a errores como compartir la base de datos entre entornos de desarrollo y producción.

| Origen técnico | Origen a nivel de proceso |
| --- | --- |
| No hay una causa técnica directa. | Falta de definición del producto software que se pretendía desarrollar y de su consecuente modelo de negocio. |

**Fuente del error:**

- **Quién lo introdujo**: El equipo completo, al no dedicar tiempo suficiente a definir el producto.
- **Rol/es**: La mayoría actuaban como desarrolladores, elaborando los documentos con falta de conocimiento debido a una idea de negocio poco precisa y muy ambigua. También se incluyen el director de proyecto y el asistente del proyecto.

**Responsables:**

- **Quién no permitió que el fallo llegara al entregable**: El director de proyecto al elaborar una reunión urgente con el equipo, y como consecuencia el resto del equipo.

**Relación con el fallo en el despliegue:**

Tuvo un **efecto en cadena** que impactó negativamente en varias áreas del proyecto, incluyendo el **despliegue** y el **correcto desarrollo de la aplicación**. Al no tener un producto bien definido validado desde el inicio, se tomaron decisiones sin una base sólida. Esto derivó en la improvisación de algunas soluciones, como por ejemplo el uso compartido de la base de datos entre los entornos de desarrollo y producción.

**Solución aplicada:** 

Para resolver esta falta de claridad, realizamos una reunión exhaustiva en la que definimos de manera precisa la idea de negocio. Esto aseguró que todos los miembros del equipo estuvieran alineados y compartiéramos una visión común. El feedback del profesorado y de otros compañeros fue una ayuda importante.

**Análisis de la solución:** 

Obtener un objetivo claro nos permitió alinear objetivos, distribuir las tareas con mayor eficiencia y tomar mejores decisiones técnicas. Nos ayudó también a conocer nuestro público objetivo y establecer un alcance del proyecto realista.  Sin embargo, fue una solución **correctiva tardía**, que implicó desviaciones en el cronograma y la necesidad de rehacer tareas previas.

**Estado del problema tras la solución:** Resuelta, ya que desde aquella reunión todo el equipo tuvo una mejor definición de la idea de negocio, sin ninguna duda debido a una posible ambigüedad existente.

**¿Qué se podría haber hecho?:** 

Una buena práctica en la dirección de proyectos es establecer una documentación mínima que definiera la visión y objetivos del proyecto. También, asignar a un miembro del equipo como Product Owner asegura una coherecia y cierta validez en el modelo de negocio. A su vez se podría haber elaborado un **Canvas de modelo de negocio** para validar la viabilidad del producto antes de avanzar al diseño técnico.

## Cambio inesperado en la base de datos

Identificado por el equipo antes de la entrega, durante la primera semana del Sprint 1.

**Descripción:** 

Inicialmente, se consideró utilizar CloudSQL de Google para la base de datos, sin embargo, se decidió cambiar y optar por un base de datos PostgreSQL, mantenida por Azure.

| Origen técnico | Origen a nivel de proceso |
| --- | --- |
| A pesar de ser una base de datos óptima para nuestro alcance de proyecto, CloudSQL era un coste adicional que no era viable teniendo la gratuidad de Azure. | Falta de planificación y de estudio de las diferentes opciones en la fase inicial. |

**Fuente del error:**

- **Quién lo introdujo**: El encargado a gestionar la base de datos junto con el director de proyecto y el asistente del proyecto, al no dedicar suficiente tiempo a la evaluación de si la tecnología elegida era la correspondiente.
- **Rol/es**: Actuaban como desarrollador software full-stack, director de proyecto y asistente del proyecto.

**Responsables:**

- **Quién permitió que el fallo no llegara al entregable**: El encargado a gestionar la base de datos, al identificar a tiempo antes de que el desarrollo de la aplicación ampliase.
- **Rol/es**: Actuaba como desarrollador software full-stack.

**Relación con el fallo en el despliegue:**
El cambio inesperado en la base de datos, aunque técnicamente viable, tuvo un impacto directo en el resultado final del proyecto, y puede considerarse un **factor contribuyente clave al fallo en producción**. Al sustituir CloudSQL por PostgreSQL en Azure, se generaron **cambios no planificados en la configuración del entorno de datos**, que no fueron adecuadamente reflejados ni en la documentación técnica ni en las prácticas de despliegue.

**Solución aplicada:** 

Se decidió sustituir CloudSQL por PostgreSQL alojado en Azure, aprovechando que esta opción estaba incluida gratuitamente en el entorno educativo.

**Análisis de la solución:** 

El cambio a PostgreSQL en Azure se implementó de manera efectiva y sin grandes fricciones técnicas, ya que PostgreSQL es una base de datos robusta y ampliamente soportada. Sin embargo, este cambio requirió ajustes en la configuración de acceso y la gestión de credenciales, lo que implicó un tiempo adicional no contemplado en el cronograma inicial.

**Estado del problema tras la solución:** Resuelta. La migración a PostgreSQL fue completada y el entorno actualizado correctamente tras el fallo. Se incluyeron nuevos protocolos de documentación técnica y validación de cambios.

**¿Qué se podría haber hecho?:** 

Realizar un análisis de costes y viabilidad técnica más detallado desde la fase de planificación. Consultar las condiciones de uso gratuitas de las distintas plataformas cloud antes de tomar decisiones de infraestructura.

## Falta de comunicación

Identificado por el equipo después de la entrega, después de que todo el equipo hiciera una retrospectiva en conjunto en una reunión después del entregable.

A su vez, fue identificador por el profesorado, en la primera semana del proyecto. Llegaron a esa conclusión después de haber analizado todos los fallos durante la presentación de la primera semana del sprint.

**Descripción:** 

Algunos miembros han trabajado por separado y se ha producido código duplicado, lo que ha llevado a la pérdida de tiempo y eliminación del trabajo de parte del equipo.

| Origen técnico | Origen a nivel de proceso |
| --- | --- |
| Falta de uso de herramientas colaborativas desde el inicio (como tableros de tareas, repositorios bien organizados o pull requests sistematizados). | Se han asignado tareas de extensa duración a varias personas sin establecer una comunicación clara entre ellas.  **** |

**Fuente del error:**

- **Quién lo introdujo**: El director de proyecto y el asistente del proyecto, al no prestar suficiente atención al equipo durante la primera semana. A su vez, el equipo de desarrollo tuvo un grán desinterés durante la primera semana del sprint.
- **Rol/es**: Los principales responsables actuaban como director de proyecto y asistente del proyecto, mientras que el resto del equipo actuaba como desarrolladores.

**Responsables:**

- **Quién permitió que el fallo llegara al entregable**: El director de proyecto y el asistente del proyecto, al no poder poner una solución más eficiente antes de que el siguiente sprint iniciase.
- **Rol/es**: Actuaban como director de proyecto y asistente del proyecto.

**Relación con el fallo en el despliegue:**
La falta de comunicación efectiva entre los miembros del equipo durante el desarrollo del proyecto fue un factor importante que afectó directamente al resultado final. El fallo en producción no solo fue técnico, sino organizativo: se impidió asegurar que lo que se desplegó era el resultado coordinado y coherente del trabajo de todos los equipos.

**Solución aplicada:** 

Para evitar este problema, se ha decidido dividir las tareas más grandes en subtareas y mejorar la comunicación dentro del equipo. Se fomentará el trabajo colaborativo y la sincronización antes de desarrollar código.

**Análisis de la solución:** 

La división en subtareas y mejoras en la comunicación ha tenido un impacto positivo inmediato. Se ha aumentado la transparencia del trabajo y mejorado la cohesión del equipo. No obstante, aún es necesario consolidar estas prácticas y revisar periódicamente la asignación de tareas para asegurar una correcta distribución del trabajo.

**Estado del problema tras la solución:** En progreso. La solución aplicada continuó durante el siguiente sprint, es por ello que el problema no fue solucionado completamente y el problema continuó existiendo tras finalizar esta etapa del proyecto. Sin embargo, vimos que durante el Sprint 1 empezó a tener efecto, es por ello que no modificamos la solución aplicada.

**¿Qué se podría haber hecho?:** 

Una de las soluciones más evidentes tras analizar el problema podría haber sido la definición clara de roles y responsabilidades, especialmente en tareas críticas o que implican colaboración entre varios miembros. Otra buen solución es reconocer la importancia de herramientas de gestión de tareas desde las primeras fases del proyecto. 

## Ejecución tardía de tareas

Identificado por el equipo antes de la entrega, después de la primera semana del Sprint 1, tras ver la cantidad de tareas restantes para la segunda semana que ya deberían de haber estado terminadas.

**Descripción:** 

Durante el desarrollo del proyecto, varias tareas fueron terminadas fuera del plazo esperado. Esto provocó un efecto dominó  sobre otras tareas dependientes de estas y afectó negativamente al entregable del sprint. Este problema nos ocasionó estrés y acumulación de trabajo al  final del sprint. A su vez, debido a que un miembro abandonó al equipo de forma voluntaria debido a falta de tiempo para dedicarle a la asignatura hizo que sus tareas no fueran completadas durante la primera semana, lo que hizo que se acumularan para la segunda semana.

| Origen técnico | Origen a nivel de proceso |
| --- | --- |
| Subestimación de la complejidad técnica de algunas tareas (por ejemplo, integraciones entre módulos o el propio despliegue). | Falta de estimaciones realistas en los tiempos de entrega, escasa priorización de tareas y un seguimiento insuficiente del avance del equipo. Además, se subestimó la carga de trabajo académico externa, lo que redujo la disponibilidad real de los miembros del equipo en momentos críticos. |

**Fuente del error:**

- **Quién lo introdujo**: El equipo de desarrollo, debido al grán desinterés durante la primera semana del sprint.
- **Rol/es**: Actuaban como desarrolladores software.

**Responsables:**

- **Quién permitió que el fallo no llegara al entregable**: El director de proyecto.

**Relación con el fallo en el despliegue:**
La ejecución tardía de tareas tuvo una influencia directa en el fallo final durante el despliegue, ya que redujo drásticamente el tiempo disponible para realizar pruebas integradas y validaciones funcionales del entorno productivo. Muchas de las tareas críticas se completaron a último momento, lo que obligó a realizar ajustes apresurados, sin la debida verificación. 

**Solución aplicada:** 

Una reorganización del cronograma, priorizando las tareas críticas. También, se elaboró una replanificación del sprint 1, junto con la planificación temprana del sprint 2, donde se introdujeron algunas tareas que no dio tiempo a realizar durante la segunda semana. Finalmente, se dio un aviso general sobre la importancia de las fechas límites.

**Análisis de la solución:** 

La aplicación de estos cambios permitió una mejor planificación semanal y mayor visibilidad sobre el avance real del proyecto. Aunque no se pudo recuperar todo el tiempo perdido, se consiguió reducir la presión en las últimas semanas y entregar los entregables esenciales a tiempo. Sin embargo, la mejora en la ejecución debe consolidarse como un proceso continuo.

**Estado del problema tras la solución:** En progreso. La solución aplicada continuó durante el siguiente sprint, es por ello que el problema no fue solucionado completamente y el problema continuó existiendo tras finalizar esta etapa del proyecto. Sin embargo, vimos que durante el Sprint 1 empezó a tener efecto, es por ello que continuamos con la solución aplicada.

**¿Qué se podría haber hecho?:** 

No hay una solución clara pero por supuesto, hay algunas que podrían haber mejorado la situación. Por ejemplo, invertir más tiempo en la planificación inicial o alinear mejor los compromisos individuales con los intereses del proyecto. 

## Dificultad en la gestión de un equipo grande

Identificado por el equipo antes de la entrega, sobre todo por el Director de proyecto que tuvo grandes problemas en el inicio del proyecto.

**Descripción:** 

La gestión de un equipo de estas dimensiones ha sido uno de los grandes retos del inicio del proyecto. La coordinación entre los miembros del equipo elaborada por el director de proyecto no fue suficientemente efectiva al inicio, lo que ha derivado en algunos de los problemas mencionados anteriormente.

| Origen técnico | Origen a nivel de proceso |
| --- | --- |
| No hay realmente ningún aspecto técnico. | Hay falta de experiencia en la dirección de proyectos dentro del equipo de trabajo y las experiencias previas han sido en equipo con menos número de miembros. Debido a esto ha habido errores como no definir en el inicio los roles y responsabilidades de forma clara.  La ausencia de una estructura organizativa funcional limitó la capacidad de liderazgo distribuido y generó dependencia de decisiones centralizadas. |

**Fuente del error:**

- **Quién lo introdujo**: El director de proyecto, el cual nunca ha tenido experiencia en tener ese rol previamente con tanta cantidad de personas. A su vez, el resto del equipo también fue responsable, por no haber identificado en la anterior etapa el problema y haber mostrado ayuda.
- **Rol/es**: Actuaban como desarrolladores software la mayoría, menos el principal responsable del problema, el cual ha sido director de proyecto.

**Responsables:**

- **Quién permitió que el fallo no llegara al entregable**: El director de proyecto.

**Relación con el fallo en el despliegue:**
La dificultad en la gestión de un equipo grande tuvo un impacto significativo en el fallo final durante el despliegue, ya que la falta de coordinación entre los distintos miembros y áreas del proyecto provocó **desalineación técnica**, **duplicidad de esfuerzos** y **ausencia de responsables claros durante la fase crítica de integración**. En términos de gestión de proyectos, esta situación representa una debilidad tanto en la **Gestión de Recursos Humanos** como en la **Gestión de la Integración del Proyecto**, dos áreas clave del PMBOK.

**Solución apliacada:** 

Se añadió un nuevo rol dentro del equipo, conocido como **Asistente del proyecto**, el cual se encarga de ayudar al director de proyecto en la organización del equipo, gestión del producto final y gestión del cronograma en el caso de que este lo necesitase. Además, se establecieron líderes responsables de áreas concretas del proyecto, promoviendo así una gestión menos centralizada. También se incrementó la organización de las reuniones semanales de seguimiento para mantener a todo el equipo alineado y facilitar la resolución temprana de conflictos o bloqueos.

**Análisis de la solución:**  

Se aumentó la eficiencia en la toma de decisiones y se  mejoró la comprensión de las tareas asignadas y redujo la duplicidad de esfuerzos. Sin embargo, la implementación se produjo en una fase avanzada del proyecto, por lo que su impacto fue más correctivo que preventivo.

**Estado del problema tras la solución:** Resuelta. Gracias a la solución aplicada en cuanto se identificó el problema, se evitó que la situación escalara y se mitigaron posibles consecuencias mayores. Aunque el problema fue resuelto de forma efectiva, su aparición desencadenó otros incidentes que se describen en distintas secciones de este documento.

**¿Qué se podría haber hecho?:** 

Desde el inicio del proyecto, se podría haber aplicado el proceso de *Planificación de la Gestión de los Recursos* del PMBOK, que incluye la definición de roles, responsabilidades, estructura organizacional y plan de desarrollo del equipo. También habría sido útil definir un *Plan de Gestión de las Comunicaciones* más detallado, con canales formales e informales bien definidos para asegurar el flujo constante de información.

# Metodología de desarrollo de software.

Para nuestro producto hemos optado por la metodología Scrum una de las más utilizadas en empresas y startups, centrada en el trabajo en equipo, la entrega iterativa y la adaptación constante. Su objetivo es permitir a los equipos desarrollar productos de alta calidad de forma rápida y flexible, respondiendo bien a los cambios y mejorando continuamente.

**Sprints:** Los ciclos de desarrollo que hemos definido son de una duración de 2 semanas coincidiendo con la periodicidad de los entregables y versiones de nuestro producto. En cada uno de los sprints se ha desarrollado un sprint planning, elaborado por el director de proyecto y definiendo las tareas, junto con el plazo y el responsable.

**Scrum Team:** Durante el sprint 1 se definieron los siguientes roles para el desarrollo del proyecto.

- **Director de proyecto:** José Manuel Miret.
- **Asistente del Project Manager y Portavoz del equipo:** Pablo Rodríguez.
- **Desarrolladores backend:**  Manuel Palacios, Alejandro Nicolalde, David Delgado.
- **Desarrolladores frontend:** Paula Sánchez, Mario Astudillo, Rubén Romero, Manuel Chica, María Barrancos (actualmente no continúa en el equipo).
- **Desarrolladores fullstack:** José Gonzalo Domínguez, Rafael Cabello, Mohamed Abouri, Virginia Mesa, Ramón Vergara.