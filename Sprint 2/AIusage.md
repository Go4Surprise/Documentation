<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - AIusage

### Sprint 2

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** María Barrancos

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

# **Uso de IA en el Proyecto**

**27/03/2025**

La Inteligencia Artificial (IA) continúa consolidándose como un recurso clave en nuestro flujo de trabajo. A medida que avanzamos en el desarrollo del proyecto Go4Surprise, hemos podido integrar la IA de manera más estratégica y consciente, extrayendo un mayor valor de sus capacidades para el desarrollo, depuración, documentación y mejora de código.

## 1. Generación de Código y Optimización

Durante el Sprint 2, se ha intensificado el uso de modelos como **ChatGPT**, **GitHub Copilot**, **Claude** y **Gemini** para la creación y mejora de código. Esto ha permitido:

- Acelerar la implementación de nuevas funcionalidades.
- Optimizar funciones previamente desarrolladas.
- Detectar errores de lógica que pasaban desapercibidos en revisiones manuales.

Además, se ha trabajado en la integración de pruebas unitarias y de integración desde el momento de escribir código, reforzando la **calidad desde la base**.

### Buenas prácticas reforzadas:

- Validación de código IA con testing automático.
- Revisión cruzada antes de fusionar ramas.
- Uso responsable y documentado de fragmentos generados por IA.

---

## 2. Apoyo en Documentación

La IA ha seguido siendo una aliada clave en la **generación de documentación técnica y funcional**. Se ha usado para:

- Redactar especificaciones de endpoints.
- Crear estructuras de manuales de usuario.
- Dar formato claro a reportes de avance y descripciones de funcionalidades.

Además, varios compañeros han aprovechado la IA para **mejorar la redacción y claridad** de textos largos, evitando repeticiones, ambigüedades y mejorando el tono técnico.

---

## 3. Revisión y Mejora del Código

La revisión de código asistida por IA ha sido una de las implementaciones más exitosas del sprint. Herramientas como **Qodo-AI PR-Agent** y asistentes automáticos en GitHub han facilitado:

- Detectar vulnerabilidades o código redundante.
- Mejorar la organización y estructura del código.
- Sugerir refactorizaciones claras y documentadas.

### Avance respecto al Sprint 1:

- Reducción del tiempo medio de revisión de PRs en un 30%.
- Menos bugs en integración.
- Comentarios más detallados y contextuales.

---

## 4. Ejemplos Reales de Uso

### ✅ Depuración de Bug en Móviles
Un fallo relacionado con el cierre automático de sesión tras inactividad en móviles fue resuelto con la ayuda de ChatGPT. La IA sugirió revisar el uso del `refresh token`, detectó una mala implementación del flujo de renovación y propuso un enfoque con `Silent Refresh`.

**Resultado:** Solución efectiva en menos de 2 horas.

**Prompt usado:**
```
En una app móvil con autenticación mediante tokens JWT, ¿cómo puedo implementar un sistema de refresh token que evite cerrar sesión automáticamente cuando el token principal expira? Estoy usando React Native y el backend en Node.js. El token expira a los 15 minutos.
```

La respuesta incluyó:
- Un esquema del ciclo de vida del `access` y `refresh token`.
- Código para almacenar el `refresh token` de forma segura (por ejemplo, usando SecureStore).
- Ejemplo práctico de `Silent Refresh` automático antes de que expire el `access token`.

---

### ✅ Generación de pruebas unitarias para funciones críticas
En el módulo de matchmaking, se utilizaron prompts para generar tests con Jest y Vitest, incluyendo mocks personalizados. Esto permitió asegurar cobertura en funciones sensibles sin invertir demasiado tiempo en su redacción manual.

---

## 5. Limitaciones y Alucinaciones de la IA

Aunque la IA ha sido útil, **no está exenta de errores o "alucinaciones"**:

- 📌 Se sugirió una función `setTimeoutAndRefresh()` inexistente, lo que generó confusión inicial.
- 📌 Se propuso una estructura errónea de rutas en React Router v6 basada en documentación antigua.
- 📌 Algunas sugerencias de rendimiento eran innecesarias o incluso contraproducentes.

**Lección:**  
No basta con copiar y pegar. Hay que **probar, validar y adaptar**. La IA no sustituye al juicio crítico del equipo, sino que lo complementa.

---

## 6. Sugerencias para la Implementación de IA en Próximos Sprints

Para seguir progresando, proponemos:

- **Definir criterios de uso interno:** ¿Cuándo usar IA? ¿Quién valida su output?
- **Capacitación constante del equipo** en herramientas emergentes de IA.
- **Documentar todo uso relevante de IA** en las tareas y commits.
- **Evaluar impacto real** de su uso en productividad, calidad del código y tiempos de entrega.

---

## 7. Evaluación General del Sprint 2

✅ **Progreso:** Uso más maduro, menos dependiente y más estratégico.  
✅ **Calidad:** Mejora evidente en documentación y organización del código.  
✅ **Colaboración:** El equipo intercambia prompts y soluciones, mejorando el aprendizaje colectivo.

---

## 8. Nuevos Conocimientos Adquiridos

A lo largo del Sprint 2, el uso de herramientas de IA no solo ha servido como apoyo técnico, sino también como una fuente activa de **aprendizaje continuo**. Algunos de los nuevos conocimientos que se han adquirido incluyen:

- **Mejor comprensión del manejo de autenticación y tokens** en entornos móviles, incluyendo estrategias como `Silent Refresh` y almacenamiento seguro.
- **Optimización de queries y rendimiento en bases de datos**, gracias a sugerencias generadas por IA para refactorizar consultas SQL.
- **Buenas prácticas de testing moderno**, como el uso de mocks, spies y tests paramétricos con Jest y Vitest.
- **Integración con servicios externos (API REST, Azure)** mediante configuraciones más eficientes sugeridas por la IA.
- **Manejo de errores y validación del lado cliente/servidor**, con estructuras de control más robustas.
- **Mejora en habilidades de redacción técnica**, al observar cómo la IA estructura explicaciones, descripciones de endpoints y documentación clara.

Este aprendizaje ha tenido un impacto positivo en la autonomía técnica de los miembros del equipo, reduciendo la dependencia de tutores o documentación externa para resolver dudas complejas.

---

## 9. Enlaces a Consultas de IA

| Miembro del equipo | Tema de la consulta | Enlace a conversación |
| --- | --- | --- |
| Manuel Palacios | Casos de uso matchmaking | https://chatgpt.com/share/67d3459a-fe14-8011-b21f-fda093cc0340 |
| Manuel Palacios | Métricas de rendimiento | https://chatgpt.com/share/67d345fd-b32c-8011-9f8c-1a4ec52392b8 |
| Manuel Palacios | Añadir un vídeo en markdown | https://chatgpt.com/share/67d34617-9e2c-8011-b8a1-c02297bb0063 |
| Pablo Rodríguez | Arreglar bug en móviles | https://chatgpt.com/share/67d348f7-f100-8004-83f6-77f74b6becf1 |
| Pablo Rodríguez | Conexión a la base de datos | https://chatgpt.com/share/67d349b1-41c8-8004-a1ba-ba82fc78ac05 |
| Pablo Rodríguez | Conexión a Azure | https://chatgpt.com/share/67d34a16-ba84-8004-82a3-7131535444a7 |
