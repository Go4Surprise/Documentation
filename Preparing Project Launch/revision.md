
<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - Guía de Revisión del Software

### Preparing Project Launch

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** Manuel Palacios

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

# Contribución al documento

| Fecha | Miembro del equipo | Contribución |
| --- | --- | --- |
| 01/05/2025 | Manuel Palacios Pineda | Primera versión basada en el documento del Sprint 3 |

# Resumen del documento

Este documento busca facilitar la revisión del software por parte de personas externas al equipo de trabajo. Se proporcionan lo casos de uso que han sido implementados, evitando errores de probar casos de uso previstos en la planificación, pero no implementados todavía, así como una guía sobre como interactuar con el software para probar su funcionalidad. A su vez se facilitarán las credenciales necesarias, los requisitos potenciales del sistema y un enlace a un vídeo en formato .mp4 en el que se muestra una demo del software.


# 1. Datos necesarios para la revisión
En este apartado se presenta una tabla con todos los datos necesarios para llevar a cabo la revisión del proyecto:

| Información | Detalles  |
| --- | --- |
| Url de la landing page | https://go4app-landing.netlify.app |
| Usuario 1  | ManuelPalacios |
| Contraseña usuario 1 | ispp1234 |
| Usuario 2 | JorgeMartin |
| Contraseña usuario 2 | ispp1234 |
| Usuario administrador | RafaelCabello |
| Contraseña usuario administrador | ispp1234 |
| Número de tarjeta de la pasarela de pago | 4242 4242 4242 4242 (fecha de caducidad y CVV aleatorios) |
| Correo electrónico PayPal | sb-g9ols39719922@personal.example.com |
| Contraseña PayPal | ,TqB5-:n |
| Url de la plataforma desplegada  | https://s3-go4-frontend-dot-ispp-2425-g10.ew.r.appspot.com/ |
| Url del repositorio de Github de código | https://github.com/Go4Surprise/Go4Surprise |
| Url del repositorio de Github de documentación  | https://github.com/Go4Surprise/Documentation |
| Url del la herramienta de gestión del tiempo | https://app.timecamp.com/ |
| Guía de acceso a los tiempos | Una vez identificado, navegar a "Projects" en la barra lateral izquierda. Una vez en Projects, pulsar en el icono "Time Report" que hay en la sección de "ISPP". Se abrirá una nueva pestaña donde podrá personalizar el rango de fechas y las personas de las que quiere ver el tiempo registrado. Navegando hacia abajo podrá ver el tiempo por persona pinchando en "People" |
| E-mail de acceso a la herramienta de gestión del tiempo | go4surprise.ispp@gmail.com |
| Contraseña de acceso a la herramienta de gestión del tiempo | P4bl0-4pru3b4n0s |


# 2. Casos de uso
A continuación listamos los casos de uso desarrollados en nuestro sistema y proporcionamos una guía paso a paso para que los puedan probar. Una vez en nuestra aplicación, encontrará una página principal informativa. Pulse sobre el botón "Comenzar" en la parte superior derecha.

## Identificación de usuario

### 1. **Registro en el sistema (ligeras modificaciones respecto al Sprint 2):**
- Para crear una nueva cuenta en nuestro sistema, deberá pulsar el botón verde "Registrate" de la pantalla de inicio.
- Una vez haya sido redirigido a nuestra pantalla de registro, deberá rellenar el formulario con sus datos personales, aceptar nuestra
política de privacidad y condiciones de uso y pulsar en el botón azul "Registrarse".
- Si el registro ha sido aceptado, será redirigido a la pantalla de inicio de sesión.
- Antes de iniciar sesión, deberá verificar su correo electrónico, para ello, vaya a su bandeja de correo y pulse sobre el botón "Verificar mi correo" en el email que le hemos enviado. (Compruebe la bandeja de Spam)
- Si no ha habido errores, deberá ver una pantalla verificando su registro. Para continuar a nuestra aplicación, pulse sobre el botón azul "Continuar".
- Al ser su primera vez en la aplicación, deberá contestar un rápido cuestionario para conocer sus preferencias. [Punto 3](#3-selección-de-preferencias-ligeras-modificaciones-respecto-al-sprint-2)


### 2. **Inicio de sesión: (implementado en Sprint 1)**
- Para iniciar sesión en nuestro sistema, deberá rellenar el formulario de la pantalla principal con sus credenciales, y pulsar sobre
el botón azul "Iniciar sesión".
- Si sus credenciales son correctas, será redirigido a la pantalla principal de nuestra aplicación.
- Inicio de sesión con Google: no implementado al completo


### 3. **Selección de preferencias (ligeras modificaciones respecto al Sprint 2):**
- Tras entrar por primera vez en nuestro sistema, deberá completar un rápido y divertido formulario para que podamos conocer sus preferencias y brindarle la mejor experiencia posible.
- Pulse sobre el botón azul "Empezar cuestionario". El formulario está formado por 6 preguntas, cada una de ellas es de opción múltiple, es decir, puede seleccionar varias respuestas, a no ser que seleccione "Nada en especial".
- Para pasar a la siguiente pregunta deberá pulsar sobre el botón rosa "Siguiente" en la parte inferior de la pantalla. Si quiere cambiar alguna respuesta antes de terminar el formulario, podrá volver atrás pulsando sobre el botón blanco "Atrás"
- Una vez haya respondido las 6 preguntas, será redirigido a la pantalla principal de nuestra aplicación.


### 4. **Gestión del perfil (ligeras modificaciones respecto al Sprint 2):**
- En la pantalla principal de la aplicación, encontrará un icono de usuario en la parte superior derecha de la pantalla (si tiene foto de perfil, le aparecerá en lugar del icono de usuario). Si pulsa sobre el icono, será enviado a la pantalla de gestión de su usuario.
- Si pulsa sobre el botón "Editar perfil", podrá modificar su nombre, apellidos, nombre de usuario, correo, número de teléfono y fecha de nacimiento. Además, hemos incluido la posibilidad de poner una foto de perfil. Para ello, deberá pulsar sobre el botón azul "Seleccinar Imagen". Busque en sus archivos la foto que más le guste y selecciónela.  Para confirmar los cambios deberá pulsar sobre el botón azul "Guardar". Si no quiere confirmar los cambios, pulse el botón rojo "Cancelar".
- Si pulsa sobre el botón "Cambiar contraseña", podrá modificar la contraseña de su cuenta. Tendrá que introducir su contraseña actual y la nueva contraseña. Para confirmar los cambios deberá pulsar sobre le botón azul "Guardar". Si no quiere confirmar los cambios, pulse el botón rojo "Cancelar".
- Si pulsa sobre el botón "Reservas", podrá ver las reservas que ha hecho en nuestra aplicación.
- Si pulsa sobre el botón rojo "Cerrar sesión", será redirigido a la pantalla de inicio y se habrá cerrado su sesión en la aplicación.
- Eliminar cuenta: no implementado al completo


### 5. **He olvidado mi contraseña (implementado en Sprint 2):**
- Si ha olvidado su contraseña y quiere acceder a nuestro sistema, pulse sobre las letras azules "¿Has olvidado la contraseña?" bajo el botón de "Iniciar sesión".
- A continuación deberá introducir el correo electrónico asociado a la cuenta a la que quiere recuperar el acceso. Tras introducir el correo, pulse sobre el botón azul "Enviar enlace".
- Si recibe un mensaje verde "El correo ha sido enviado correctamente" vaya a su bandeja de correo y pulse sobre el botón "Verificar mi correo" en el email que le hemos enviado. (Compruebe la bandeja de Spam). Si no puede pulsar sobre el botón, compruebe que ha marcado este email como no sospechoso.
- Habrá sido redirigido a un formulario donde debe introducir la nueva contraseña de su cuenta (dos veces, para asegurar que no se equivoque). Una vez haya terminado el formulario, pulse sobre el botón azul "Restablecer".
- Si no ha habido ningún error, será redirigido a la pantalla de inicio, donde podrá iniciar sesión con su nueva contraseña.



## Reserva de experiencias

### 6. **Reserva de una experiencia (ligeras modificaciones respecto al Sprint 2):**
- Para poder registrar una reserva en nuestro sistema, deberá pulsar el botón azul "Sorpréndeme" que aparece en el centro de la pantalla.
- Este botón le llevará a un formulario, el cuál deberá rellenar con datos importantes para la gestión de su experiencia. 
- Verá un desglose del coste de la experiencia al final del formulario.
- Para confirmar la reserva pulse en el botón azul "REALIZAR RESERVA"
- A continuación verá un resumen de la reserva. Para continuar, pulse el botón azul "Proceder al pago".
- Escoja su método de pago favorito y rellene los datos necesarios para realizar el pago de la reserva. Pulse el botón azul "Pagar".
- Si todo se ha registrado sin problemas, deberá ser enviado a la pantalla principal de la aplicación.
- Si comprueba su correo electrónico, verá un email con los detalles de su reserva.


### 7. **Gestión de mis reservas (cambios importantes respecto al Sprint 2):**
- En la parte superior de la pantalla principal aparecerá cuántos días quedan para su próxima experiencia con nosotros.
- Si quiere consultar información sobre sus reservas, debe navegar hacia la sección de "Reservas" en la [gestión del perfil](#4-gestión-del-perfil-ligeras-modificaciones-respecto-al-sprint-2).
- En esta pantalla podrá visualizar los detalles de sus reservas activas, pasadas y canceladas.
- Puede cancelar su reserva pulsando en el botón rojo "Cancelar" de cada reserva, y a continuación pulsando sobre el botón rojo "Sí". Si comprueba su correo, le habremos enviado un email confirmando su cancelación.
- Puede añadir la experiencia a Google Calendar pulsando el botón azul "Añadir a Google Calendar".

Para las reservas de dentro de 48 horas, se enviará un mensaje al correo elctrónico asociado a su cuenta con una pista sobre la experiencia. Cuando queden 24 horas, se enviará un mensaje con los detalles de la experiencia al completo. Los correos electrónicos se enviarán automáticamente a las 08:00 a.m.


### 8. **Sistema de reseñas (implementado en el Sprint 3):**
- Nuestra aplicación permite dejar reseñas en experiencias que ya hayan ocurrido. Para facilitar la revision de la aplicación, los usuarios "JorgeMartin" y "ManuelPalacios" tienen 3 reservas cada uno aptas para recibir una reseña.
- Para dejar una reseña de una experiencia, visite la página de gestión de reservas como se ha indicado en el [punto 7](#7-gestión-de-mis-reservas-cambios-importantes-respecto-al-sprint-2).
- Una vez en "Mis Reservas", debe seleccionar la opción de ver solamente sus reservas pasadas pulsando el botón "Pasadas" de la parte superior de la pantalla.
- Para cada reserva, puede dejar una reseña pulsando sobre el botón amarillo "Dejar Reseña".
- Cabe destacar que solo puede añadir una reseña por reserva, por lo que si ya ha dejado su opinión sobre una experiencia, solamente aparecerá el mensaje de confirmación "Reseña enviada".
- Al pulsar el botón "Dejar Reseña", deberá poner una puntuación de 0 a 5 estrellas, un comentario, y añadir las fotos o vídeos correspondientes a su experiencia. Para confirmar la reseña, pulse el botón azul "Enviar". Si no quiere seguir adelante, pulse el botón gris "Cancelar".
- Si vuelve a la página principal de la aplicación, y pulsa sobre "Ver más opiniones" (debe navegar un poco hacia abajo), podrá ver las reseñas de otros usuarios con nosotros.

En el caso que quiera probar más el sistema de reseñas, haga una reserva con un usuario cualquiera. A continuación, con un usuario administrador, cambie la fecha de la experiencia y la de la reserva para que estén en el pasado. Además, también debe marcar la reserva como "Confirmada" en el campo "Estado Actual". Vuelva a iniciar sesión con su usuario inicial, y deberá poder dejar una reseña sobre esa reserva. Para ir a la página de gestión de reservas de un administrador lea las instrucciones del [punto 10](#10-gestión-de-reservas-ligeras-modificaciones-respecto-al-sprint-2).



## Panel de administrador
Si inicias sesión como un usuario administrador, en la página principal de la aplicación, encontrarás un botón "Admin" en la parte superior derecha de la pantalla. Si pulsas sobre él serás redirigido al panel del administrador

### 9. **Gestión de usuarios (implementado en el Sprint 2):**
- Si pulsas sobre la tarjeta "Gestión de Usuarios", se mostrará una lista de todos los usuarios del sistema. Pulsando sobre cualquiera de los usuarios podrás acceder a los detalles del mismo.
- Puedes editar un usuario pulsando sobre el botón azul superior "Editar". Tras hacer los cambios pertinentes, podrás guardar los cambios pulsando el botón verde "Guardar" en la parte superior derecha. A su lado hay un botón gris "Cancelar" para descartar los cambios realizados.
- Puedes eliminar un usuario pulsando sobre el botón rojo inferior "Eliminar Usuario".


### 10. **Gestión de reservas (ligeras modificaciones respecto al Sprint 2):**
- Si pulsas sobre la tarjeta "Gestión de Reservas", se mostrará una lista de todos las reservas del sistema. Pulsando sobre cualquiera de las reservas podrás acceder a los detalles de la misma.
- Puedes editar una reserva modificando directamente los campos del formulario. También está la opción de añadir los datos de la experiencia que se va asignar al usuario. Para guardar los cambios, pulsa sobre el botón azul "Actualizar Reserva".
- Si volvemos al listado de reservas, podemos eliminar cualquier reserva pulsando sobre el botón rojo "Eliminar". Aparecerá una pestaña de confirmación, debemos pulsar el botón rojo "ELIMINAR" para confirmar la operación.



# 3. Requisitos potenciales para usar el sistema

1. **Acceso a Internet:**
   - Se requiere conexión a Internet para navegar por la plataforma, registrarse, seleccionar una experiencia y recibir confirmaciones.

2. **Registro de usuario obligatorio:**
   - El usuario debe crear una cuenta para poder reservar una experiencia.
   - Se requiere verificar el correo electrónico para validar la cuenta.

3. **Acceso a correo electrónico:**
   - El usuario debe proporcionar y tener acceso a un correo electrónico válido, ya que deberá confirmar su registro mediante un correo que le enviaremos. Las pistas de las experiencias, la posibilidad generar una nueva contraseña y los detalles de las experiencias se gestionarán a través del correo electrónico asociado a su cuenta.
 


# 4. Demo de la aplicación

Enlace al vídeo de la demo en formato .mp4: [\[Enlace a la demo\]](https://drive.google.com/file/d/1CVfznMEtAUXETZ83HgVxtZcD6xQV9SoD/view?usp=drive_link)
