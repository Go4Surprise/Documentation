
<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - Revision

### Sprint 1

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

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

## Resumen del documento

Este documento busca facilitar la revisión del software por parte de personas externas al equipo de trabajo. Se proporcionan lo casos de uso que han sido implementados, evitando errores de probar casos de uso previstos en la planificación, pero no implementados todavía, así como una guía sobre como interactuar con el software para probar su funcionalidad. A su vez se facilitarán las credenciales necesarias, los requisitos potenciales del sistema y un enlace a un vídeo en formato .mp4 en el que se muestra una demo del software.

## 1. Casos de uso
A continuación listamos los casos de uso desarrollados en nuestro sistema y proporcionamos una guía paso a paso para que los puedan probar.

1. **Registro en el sistema**
Para crear una nueva cuenta en nuestro sistema, deberá pulsar el enlace que hay en las palabras "Regístrate aquí" de la pantalla principal. Una vez haya sido redirigido a nuestra pantalla de registro, deberá rellenar el formulario con sus datos personales y pulsar en el botón de "Registrarse". Si el registro ha sido aceptado, será redirigido a la pantalla de inicio de sesión.

2. **Inicio de sesión**
Para iniciar sesión en nuestro sistema, se deberá pulsar el botón de "Iniciar sesión" de la pantalla principal. A continuación deberá introducir unas credenciales correctas (usuario y contraseña) y pulsar en el botón de "Acceder". Si sus credenciales son correctas, deberá ser redirigido a un formulario para conocer sus preferencias si todavía no lo ha completado, en caso contrario, será enviado a la pantalla de inicio de nuestra aplicación.

3. **Selección de preferencias**
Tras crear una nueva cuenta e identificarse en nuestro sistema, deberá completar un rápido y divertido formulario para que podamos conocerle un poco mejor. Cada una de las preguntas es de opción múltiple, es decir, puede seleccionar varias respuestas, a no ser que seleccione "Nada en especial". Una vez haya seleccionado las opciones que más le agraden, deberá pulsar el botón de "Siguiente" para avanzar a la siguiente pregunta. Una vez haya respondido las 6 preguntas, será redirigido a la pantalla de inicio de nuestra aplicación.

4. **Reserva de una experiencia**
Para poder registrar una reserva en nuestro sistema, deberá pulsar el botón de "Sorpréndeme" que aparece al principio de la página. Este botón le llevará a un formulario, el cuál deberá rellenar con datos importantes para la gestión de su experiencia, tales como lugar, duración de la experiencia, precio, participantes y fecha. Una vez haya terminado, deberá pulsar el botón de "Register Booking". Si todo ha sido registrado sin problemas, deberá ser enviado a la pantalla de inicio de la aplicación. Si quiere consultar información sobre sus reservas, puede pulsar sobre el botón "MIS RESERVAS", en el menú superior de su pantalla, donde podrá ver los detalles de sus reservas con nuestra aplicación.


## 2. Datos necesarios para la revisión
En este apartado se presenta una tabla con todos los datos necesarios para llevar a cabo la revisión del proyecto:

| Información | Detalles  |
| --- | --- |
| Url de la landing page | https://go4app-landing.netlify.app |
| Usuario 1  |  |
| Usuario 2 |  |
| Usuario administrador |  |
| Url de la plataforma desplegada  | https://go4-frontend-dot-ispp-2425-g10.ew.r.appspot.com/ |
| Url del repositorio de Github de código | https://github.com/Go4Surprise/Go4Surprise |
| Url del repositorio de Github de documentación  | https://github.com/Go4Surprise/Documentation |


## Requisitos potenciales para usar el sistema

1. **Registro de usuario obligatorio:**  
   - El usuario debe crear una cuenta para poder comprar una experiencia.  
   - Se requiere verificar el correo electrónico para validar la cuenta.  

2. **Acceso a ubicación (opcional/recomendado):**  
   - Activar el acceso a la ubicación puede ser recomendable para personalizar las experiencias según la ciudad o área del usuario.  


3. **Acceso a correo electrónico:**  
   - El usuario debe proporcionar y tener acceso a un correo electrónico válido, ya que la información final del evento (dirección y hora) se enviará por email un día antes del evento.  

4. **Acceso a Internet:**  
   - Se requiere conexión a Internet para navegar por la plataforma, registrarse, seleccionar una experiencia y recibir confirmaciones.  


5. **Disponibilidad geográfica:**  
   - El servicio está disponible únicamente en las ciudades o zonas específicas donde haya oferta de experiencias (esto puede variar y debe consultarse en la plataforma).  
