#Express-Mongodb exercise

Ejercicio de websockets con Express y Mongodb para ISIS3710 de Uniandes.

Para correrlo se debe ejecutar npm start.

Luego, en el navegador entrar a localhost:3000. Se puede entrar al tiempo desde varias pestañas o máquinas. En la página se pueden intercambiar mensaje usando un nombre de usuario. Por otro lado, la api que tiene el proyecto es la siguiente:

GET /chat/api/messages/ Responde con un JSON dde todos los mensajes que se han enviado.

GET /chat/api/messages/tp Responde con el JSON del mensaje con timestamp (tp) específico.

POST /chat/api/messages/ Se envía un JSON para enviar un mensaje al chat. El JSON debe tener el siguiente formato: { "message": "Mensaje a enviar", "author": "Autor del mensaje" } Responde con el mensaje enviado y su timestamp asignado.

PUT /chat/api/messages/tp Se envía un JSON para actualizar el mensaje con timestamp (tp) específico. El JSON debe tener el siguiente formato: { "message": "Mensaje a enviar", "author": "Autor del mensaje" } Responde con el mensaje actualizado y su timestamp asignado.

DELETE /chat/api/messages/tp Se borra el mensaje con el timestamp (tp) especificado. Responde con el JSON del mensaje borrado.

Restricciones: Para crear y actualizar por API los mensajes deben seguir las siguientes restricciones: -Todos los campos (message, author) son requeridos -El mensaje no puede tener menos de 5 caracteres -El autor debe tener un nombre y un apellido separados por un espacio.
