
<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - Guía de Revisión del Software

### Sprint 2

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** Manuel Palacios

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

# Contribución al documento

| Fecha | Miembro del equipo | Contribución |
| --- | --- | --- |
| 12/03/2025 | Manuel Palacios Pineda | Primera versión basada en el documento del Sprint 1 |
| 12/03/2025 | Manuel Palacios Pineda | Casos de uso de identificación de usuario |
| 12/03/2025 | Manuel Palacios Pineda | Casos de uso de reservas y administración |

# Resumen del documento

Este documento busca facilitar la revisión del software por parte de personas externas al equipo de trabajo. Se proporcionan lo casos de uso que han sido implementados, evitando errores de probar casos de uso previstos en la planificación, pero no implementados todavía, así como una guía sobre como interactuar con el software para probar su funcionalidad. A su vez se facilitarán las credenciales necesarias, los requisitos potenciales del sistema y un enlace a un vídeo en formato .mp4 en el que se muestra una demo del software.


# 1. Datos necesarios para la revisión
En este apartado se presenta una tabla con todos los datos necesarios para llevar a cabo la revisión del proyecto:

| Información | Detalles  |
| --- | --- |
| Url de la landing page | https://go4app-landing.netlify.app |
| Usuario 1  | ManuelPalacios |
| Contraseña usuario 1 | ispp1234 |
| Usuario 2 | hello |
| Contraseña usuario 2 | hello1 |
| Usuario administrador | RafaelCabello |
| Contraseña usuario administrador | ispp1234 |
| Número de tarjeta para probar la pasarela de pago | 4242 4242 4242 4242 (fecha de caducidad y CVV aleatorios) |
| Url de la plataforma desplegada  | https://go4-frontend-dot-ispp-2425-g10.ew.r.appspot.com |
| Url del repositorio de Github de código | https://github.com/Go4Surprise/Go4Surprise |
| Url del repositorio de Github de documentación  | https://github.com/Go4Surprise/Documentation |
| Url del la herramienta de gestión del tiempo | https://app.timecamp.com/ |
| Guía de acceso a los tiempos | Una vez identificado, navegar a "Projects" en la barra lateral izquierda. Una vez en Projects, pulsar en el icono "Time Report" que hay en la sección de "ISPP". Se abrirá una nueva pestaña donde podrá personalizar el rango de fechas y las personas de las que quiere ver el tiempo registrado. Navegando hacia abajo podrá ver el tiempo por persona pinchando en "People" |
| E-mail de acceso a la herramienta de gestión del tiempo | go4surprise.ispp@gmail.com |
| Contraseña de acceso a la herramienta de gestión del tiempo | P4bl0-4pru3b4n0s |


# 2. Casos de uso
A continuación listamos los casos de uso desarrollados en nuestro sistema y proporcionamos una guía paso a paso para que los puedan probar. Una vez en nuestra aplicación, encontrará una página principal informativa. Pulse sobre el botón "Comenzar" en la parte superior derecha.

## Identificación de usuario

### 1. **Registro en el sistema (ligeras modificaciones respecto al Sprint 1):**
- Para crear una nueva cuenta en nuestro sistema, deberá pulsar el botón verde "Crear una cuenta" de la pantalla de inicio.
- Una vez haya sido redirigido a nuestra pantalla de registro, deberá rellenar el formulario con sus datos personales, aceptar nuestra
política de privacidad y condiciones de uso y pulsar en el botón azul "Registrarse".
- Si el registro ha sido aceptado, será redirigido a la pantalla de inicio de sesión.
- Antes de iniciar sesión, deberá verificar su correo electrónico, para ello, vaya a su bandeja de correo y pulse sobre el enlace que le hemos enviado. (Compruebe la bandeja de Spam)
- Si no ha habido errores, deberá ver una pantalla verificando su registro. Para continuar a nuestra aplicación, pulse sobre el botón azul "Continuar".
- Al ser su primera vez en la aplicación, deberá contestar un rápido cuestionario para conocer sus preferencias. [Punto 3](#3-selección-de-preferencias-ligeras-modificaciones-respecto-al-sprint-1)


### 2. **Inicio de sesión (implementado en Sprint 1):**
- Para iniciar sesión en nuestro sistema, deberá rellenar el formulario de la pantalla principal con sus credenciales, y pulsar sobre
el botón azul "Iniciar sesión".
- Si sus credenciales son correctas, será redirigido a la pantalla principal de nuestra aplicación.
- Inicio de sesión con Google: no implementado


### 3. **Selección de preferencias (ligeras modificaciones respecto al Sprint 1):**
- Tras entrar por primera vez en nuestro sistema, deberá completar un rápido y divertido formulario para que podamos conocer sus preferencias y brindarle la mejor experiencia posible.
- Pulse sobre el botón azul "Empezar cuestionario". El formulario está formado por 6 preguntas, cada una de ellas es de opción múltiple, es decir, puede seleccionar varias respuestas, a no ser que seleccione "Nada en especial".
- Para pasar a la siguiente pregunta deberá pulsar sobre el botón negro "Siguiente". Si quiere cambiar alguna respuesta antes de terminar el formulario, podrá volver atrás pulsandos sobre el botón negro "Atrás"
- Una vez haya respondido las 6 preguntas, será redirigido a la pantalla principal de nuestra aplicación.


### 4. **Gestión del perfil (implementado en Sprint 2):**
- En la pantalla principal de la aplicación, encontrará un icono de usuario en parte superior derecha de la pantalla. Si pulsa sobre el icono, será enviado a la pantalla de gestión de su usuario.
- Si pulsa sobre el botón "Editar perfil", podrá modificar su nombre, apellidos, nombre de usuario, correo y número de teléfono. Para confirmar los cambios deberá pulsar sobre le botón azul "Guardar". Si no quiere confirmar los cambios, pulse el botón rojo "Cancelar".
- Si pulsa sobre el botón "Cambiar contraseña", podrá modificar la contraseña de su cuenta. Tendrá que introducir su contraseña actual y la nueva contraseña. Para confirmar los cambios deberá pulsar sobre le botón azul "Guardar". Si no quiere confirmar los cambios, pulse el botón rojo "Cancelar".
- Si pulsa sobre el botón "Historial de reservas", podrá ver las reservas que ha hecho en el pasado.
- Si pulsa sobre el botón rojo "Cerrar sesión", será redirigido a la pantalla de inicio y se habrá cerrado su sesión en la aplicación.
- Eliminar cuenta: no implementado


### 5. **He olvidado mi contraseña (implementado en Sprint 2):**
- Si ha olvidado su contraseña y quiere acceder a nuestro sistema, pulse sobre las letras azules "¿Has olvidado la contraseña?" bajo el botón de "Iniciar sesión".
- A continuación deberá introducir el correo electrónico asociado a la cuenta a la que quiere recuperar el acceso. Tras introducir el correo, pulse sobre el botón azul "Enviar enlace".
- Si recibe un mensaje verde "El correo ha sido enviado correctamente" vaya a su bandeja de correo y pulse sobre el enlace que le hemos enviado. (Compruebe la bandeja de Spam)
- Habrá sido redirigido a un formulario donde debe introducir la nueva contraseña de su cuenta (dos veces, para asegurar que no se equivoque). Una vez haya terminado el formulario, pulse sobre el botón azul "Restablecer".
- Si no ha habido ningún error, será redirigido a la pantalla de inicio, donde podrá iniciar sesión con su nueva contraseña.



## Reserva de experiencias

### 6. **Reserva de una experiencia (cambios importantes respecto al Sprint 1):**
- Para poder registrar una reserva en nuestro sistema, deberá pulsar el botón azul "Sorpréndeme" que aparece en el centro de la pantalla.
- Este botón le llevará a un formulario, el cuál deberá rellenar con datos importantes para la gestión de su experiencia.
- Tanto para elegir la ciudad, como para descartar categorías, puede ver más opciones deslizando hacia un lado. Las categorías descartadas aparecerán en un tono grisáceo.
- En notas adicionales ponga posibles alergias, lesiones o cualquier información que vea relevante.   
- Verá un desglose del coste de la experiencia al final del formulario.
- Para confirmar la reserva pulse en el botón azul "REALIZAR RESERVA"
- A continuación verá un resumen de la reserva. Para continuar, pulse el botón azul "Proceder al pago".
- Rellene los datos necesarios para realizar el pago de la reserva.
- Si todo se ha registrado sin problemas, deberá ser enviado a la pantalla de inicio de la aplicación.


### 7. **Gestión de mis reservas (cambios importantes respecto al Sprint 1):**
- En la parte superior de la pantalla principal aparecerá cuántos días quedan para su próxima experiencia con nosotros.
- Si quiere consultar información sobre sus reservas, puede pulsar sobre el botón azul "Mis Reservas" que aparece en el centro de la pantalla (solo aparecerá si su usuario tiene reservas con nuestra aplicación).
- Si la reserva se ha confirmado, la tarjeta de la reserva aparecerá con un tono verde claro.
- Puede cancelar las reservas hasta 24 horas después de confirmarla.
- Para cancelar una reserva, pulse sobre el botón rojo "Cancelar", y a continuación pulse en el botón rojo "Sí".
- Si la reserva se ha cancelado, la tarjeta de la reserva aparecerá con un tono gris.



## Panel de administrador
Si inicias sesión como un usuario administrador, en la página principal de la aplicación, encontrarás un botón "Admin" en la parte superior derecha de la pantalla. Si pulsas sobre él serás redirigido al panel del administrador

### 8. **Gestión de usuarios (implementado en Sprint 2):**
- Si pulsas sobre la tarjeta "Gestión de Usuarios", se mostrará una lista de todos los usuarios del sistema. Pulsando sobre cualquiera de los usuarios podrás acceder a los detalles del mismo.
- Puedes editar un usuario pulsando sobre el botón azul "Editar". Tras hacer los cambios pertinentes, podrás guardar los cambios pulsando el botón verde "Guardar" en la parte superior derecha. A su lado hay un botón gris "Cancelar" para descartar los cambios realizados.
- Eliminar usuario: no implementado


### 9. **Gestión de reservas (implementado en Sprint 2)**
- Si pulsas sobre la tarjeta "Gestión de Reservas", se mostrará una lista de todos las reservas del sistema. Pulsando sobre cualquiera de las reservas podrás acceder a los detalles de la misma.
- Puedes editar una reserva modificando directamente los campos del formulario (modificar experiencia y sus detalles: no implementado). También está la opción de modificar la pista que recibirá el usuario 48 horas antes de la experiencia. Para guardar los cambios, pulsa sobre el botón azul "Actualizar Reserva".
- Si volvemos al listado de reservas, podemos eliminar cualquier reserva pulsando sobre el botón rojo "Eliminar". Aparecerá una pestaña de confirmación, debemos pulsar el botón rojo "ELIMINAR" para confirmar la operación.



# 3. Requisitos potenciales para usar el sistema

1. **Acceso a Internet:**  
   - Se requiere conexión a Internet para navegar por la plataforma, registrarse, seleccionar una experiencia y recibir confirmaciones.

2. **Registro de usuario obligatorio:**  
   - El usuario debe crear una cuenta para poder comprar una experiencia.  
   - Se requiere verificar el correo electrónico para validar la cuenta.  

3. **Acceso a correo electrónico:**  
   - El usuario debe proporcionar y tener acceso a un correo electrónico válido, ya que la información final del evento (dirección y hora) se enviará por email un día antes del evento.  
 


# 4. Demo de la aplicación

Enlace al vídeo de la demo en formato .mp4: [\[Enlace a la demo\]](https://drive.google.com/file/d/1CVfznMEtAUXETZ83HgVxtZcD6xQV9SoD/view?usp=drive_link)
