![imagen.png](imagenes/imagen.png)

<aside>
ISPP - Grupo 10

Go4Surprise

</aside>

# Plan de pruebas

**Miembros del equipo:**

- Abouri, Mohamed

- Astudillo, Mario

- Barrancos, María

- Cabello, Rafael

- Chica, Manuel

- Delgado, David

- Domínguez, Gonzalo

- Mesa, Virginia

- Miret, José Manuel

- Nicolade, Alejandro

- Palacios, Manuel

- Rodrígez, Pablo

- Romero, Rubén

- Sánchez, Paula

- Vergara, Ramón

# 1. Alcance

- Se probarán las funcionalidades descritas en los apuntes, incluyendo pruebas unitarias, de integración, de extremo a extremo, de aceptación y de rendimiento.
- No se probarán aspectos fuera del alcance de la asignatura, como pruebas de seguridad avanzadas o pruebas de carga extremadamente pesadas.

# 2. Estrategia de Pruebas

Para garantizar la calidad y robustez del software, seguiremos esta estrategia:

- **Pruebas de camino feliz y Pruebas negativas:**
    - Realizaremos pruebas de camino feliz para validar el flujo principal de la aplicación.
    - También ejecutaremos pruebas negativas para verificar cómo el sistema maneja situaciones inesperadas o errores.
- **Pruebas Manuales y Automáticas:**
    - Utilizaremos una combinación de pruebas manuales y automáticas:
        - **Pruebas Manuales:**
            - Realizaremos exploración manual para descubrir posibles problemas no cubiertos por casos de prueba específicos.
            - Validaremos la interfaz de usuario, flujos de trabajo y escenarios de uso.
        - **Pruebas Automáticas:**
            - Implementaremos pruebas automatizadas para casos repetitivos y regresiones.
            - Utilizaremos herramientas como Selenium, JUnit o PyTest para automatizar pruebas de UI y lógica de negocio.
- **Casos de Prueba Específicos:**
    - Definiremos casos de prueba específicos para cada tipo de test:
        - **Pruebas Unitarias:**
            - Verificamos funciones individuales y componentes a nivel de código.
            - Validamos entradas válidas e inválidas.
        - **Pruebas de Integración:**
            - Probamos la comunicación entre módulos y servicios.
            - Verificamos la integración con base de datos y APIs externas.
        - **Pruebas de Aceptación:**
            - Validamos que el sistema cumpla con los requisitos del cliente.
            - Probaremos la usabilidad y la experiencia del usuario.
        - **Pruebas de Rendimiento:**
            - Establecemos umbrales de rendimiento aceptables (tiempos de respuesta, capacidad de carga).
            - Ejecutamos pruebas de carga y estrés para evaluar el rendimiento bajo diferentes condiciones.

# 3. Recursos necesarios

Los recursos necesarios para llevar a cabo nuestro plan de pruebas es el siguiente:

- Equipo de desarrollo: Miembros del equipo de desarrollo de Go4Surprise responsables de implementar las pruebas.
- Herramientas de prueba: JMeter, Selenium, JUnit 5, Gatling, entre otras.
- Ambientes de pruebas: entornos de desarrollo, preproducción y producción para pruebas de rendimiento.

# 4. Casos de Prueba:

Los casos de prueba son escenarios específicos diseñados para verificar el correcto funcionamiento de un software. Aquí están los diferentes tipos de pruebas y los escenarios que se presentan en nuestra aplicación:

- **Pruebas Unitarias**
    - **Objetivo**: Probar cada entidad teniendo en cuenta todas sus funciones en la [view.py](http://view.py) cubriendo la cobertura de más del 90% después del análisis de SonarCloud.
    - **Escenarios**:
        - Hacer prueba de views de la entidad `bookings`
        - Hacer prueba de views de la entidad `users`
        - Hacer prueba de views de la entidad `experiences`
        - Hacer prueba de views de la entidad `reviews`
- **Pruebas de Integración**
    - **Objetivo**: Asegurar que la conexión con elementos externos funcione correctamente y que la información intercambiada se procese adecuadamente. No estamos probando de nuevo la lógica de la aplicación, sino la interacción con otros sistemas. En este caso, usaremos Go4Surprise.
    - **Escenarios:**
        - **Pruebas de integración de base de datos:**
            1. Iniciar una base de datos.
            2. Conectar la aplicación Go4Surprise a la base de datos.
            3. Activar una función dentro del código de Go4Surprise que escriba datos en la base de datos.
            4. Verificar que los datos esperados se hayan escrito en la base de datos leyendo los datos de la base de datos.
            
        - **Pruebas de integración de servicio externo:**
            1. Iniciar aplicación Go4Surprise.
            2. Iniciar una instancia de cada servicio externo o un doble de prueba con la misma interfaz.
            3. Activar una función dentro del código de Go4Surprise que lea de la API de cada servicio externo.
            4. Verificar que la aplicación Go4Surprise puede analizar correctamente la respuesta de cada servicio externo.
        
- **Pruebas de Aceptación**
    - **Objetivo**: Verificar que el sistema cumpla con los requisitos del cliente descritos en los escenarios de aceptación. Probar la usabilidad y la experiencia del usuario en situaciones normales y de excepción.
    - **Escenarios:**
        - Ver el perfil de usuario y editarlo.
        - Registro de usuario
        - Primer inicio de usuario
        - Inicio de sesión
        - Listado, cancelación y creación de una reserva
        - Pago de la reserva
        - FALTA RESEÑAS
        
- **Pruebas de Rendimiento**
    - **Objetivo**: Realizar pruebas de carga para determinar el comportamiento del sistema bajo diferentes niveles de carga. Ejecutar pruebas de estrés para identificar el punto de quiebre del sistema y su capacidad de recuperación. Para estas pruebas usaremos herramientas de JMeter.
    - **Escenarios:**
        - Evaluar la eficiencia del proceso de registro y edición del perfil.
        - Medir la rapidez en la creación y visualización de las reservas.
        - FALTAN COSAS
        
    - **Umbrales de rendimiento**: Este tiene que cumplir con unos umbrales:
        - **Capacidad de manejo de carga:**
        - **Tiempo de carga de  la página inicial:**
        - **Tiempo de Inicio de Sesión y autenticación:**
        - **Tiempo de Creación de Reservas:**

# 5. Criterios de Aceptación

Las pruebas se considerarán exitosas si todas las funcionalidades probadas cumplen con los criterios de aceptación definidos. Estos criterios ayudarán a garantizar que la aplicación cumpla con los estándares de calidad y satisfaga las necesidades de los usuarios:

- **Registro de Usuario:**
    - **Given** un usuario no registrado
    - **When** el usuario completa el formulario de registro con información válida
    - **Then** el usuario debería ser redirigido al inicio de sesión para verificar el correo y acceder a. la aplicación.
    
- **Primer inicio de sesión**
    - **Given** un usuario registrado
    - **When** el usuario inicia sesión con credenciales válidas por primera vez
    - **Then** el usuario deberá recibir un correo de verificación para acceder a la aplicación y deberá tener acceso a un formulario.
    
- **Inicio de sesión:**
    - **Given** un usuario autenticado
    - **When** el usuario inicia sesión con credenciales válidas
    - **Then** el usuario debería acceder a la página principal de la aplicación.
    
- **Perfil de Usuario:**
    - **Given** un usuario autenticado
    - **When** el usuario accede a la página de perfil
    - **Then** el usuario debería poder ver y editar su información.
    
- **Listado de Reserva:**
    - **Given** un usuario autenticado
    - **When** el usuario accede al listado de reservas
    - **Then** el usuario debería poder ver sus reservas pendientes

- **Cancelación de Reserva:**
    - **Given** un usuario autenticado
    - **When** el usuario cancela la reserva en las primeras 24 horas después de su compra.
    - **Then** el usuario debería recibir un correo de confirmación de la cancelación y la información sobre su reembolso.
    
- **Creación de reserva:**
    - **Given** un usuario autenticado
    - **When** el usuario crea una reserva
    - **Then** el usuario es redirigido al pago de la reserva
    
- **Pago de la Reserva:**
    - **Given** un usuario autenticado
    - **When** el usuario realiza correctamente el pago de la reserva
    - **Then** el usuario debería ver su reserva en su listado de reservas y debería poder ver una cuenta atrás en la página principal.
    

FALTA RESEÑAS 

# 6. Resultados

# 7. Conclusiones de los Resultados

# 8. Aprobaciones

Se solicitarán las firmas de los