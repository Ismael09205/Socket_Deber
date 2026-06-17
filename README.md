# Proyecto WebSocket

Aplicación de mensajería en tiempo real con Node.js, Express y Socket.IO.

## Descripción

Este proyecto ofrece un chat básico con registro de usuarios, mensajes globales y mensajes privados. El servidor mantiene la lista de usuarios conectados y administra las comunicaciones en tiempo real.

## Características

- Registro de usuario con nombre
- Lista de usuarios conectados
- Mensajes globales a todos los clientes
- Mensajes privados entre usuarios
- Indicadores de conexión y desconexión

## Estructura del proyecto

- `server.js`: servidor de Node.js que usa Express y Socket.IO.
- `package.json`: dependencias y script de inicio.
- `public/index.html`: interfaz cliente en el navegador.

## Requisitos

- Node.js instalado (versión compatible con Express 5 y Socket.IO 4)

## Instalación


```bash
npm server.js
```

## Uso

1. Iniciar el servidor:

```bash
npm start
```

2. Abrir el navegador en:

```text
http://localhost:3000
```

3. Registrar un nombre de usuario.
4. Enviar mensajes globales o privados a otros usuarios.

## Flujo de funcionamiento

- Al conectarse, el servidor agrega al usuario a un arreglo de `usuarios`.
- El cliente envía el nombre con el evento `registrar`.
- Los mensajes globales se emiten con `mensaje-global`.
- Los mensajes privados se envían con `mensaje-privado` a un `destinoId` específico.
- Cuando un usuario se desconecta, se actualiza la lista y se notifica a todos.

## Dependencias

- `express`
- `socket.io`

## Notas

- El proyecto sirve archivos estáticos desde `public/`.
- El ID de socket se utiliza para identificar usuarios y enviar mensajes privados.

## Capturas de pantalla

<img width="1569" height="768" alt="image" src="https://github.com/user-attachments/assets/11b4f6dd-8eea-46c8-8edb-c6d1e9027f9f" />


<img width="1569" height="775" alt="image" src="https://github.com/user-attachments/assets/09baf8e3-8472-46db-b9ee-ad3c355aecf1" />


<img width="1583" height="777" alt="image" src="https://github.com/user-attachments/assets/dfad9f00-92ff-4519-a167-3f6015e54cb2" />

## Integrantes

- Edwin Chusin
- Joel Acosta
- Ismael Narvaez




