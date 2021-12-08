<h1 align="center">  🛒 &nbsp; App de compras 🛒 </h1>

> Construido con el Stack MERN (MongoDB, Express, React and Node).

## 📜 &nbsp; Tabla de conceptos

- [Principales características](#--main-features)
- [Tecnologías](#--technologies)
- [Conceptos clave](#--key-concepts)
- [Diagrama UML](#--uml-diagram)
- [Configuración](#--setup)
- [ENV](#-ENV)

## 🚩 &nbsp; Principales características

> Esta aplicación se creó para rastrear el estado del pedido desde que el cliente lo colocó
> una vez enviado, el vendedor lo marca como enviado y luego el remitente lo marca como entregado.

#### Metodología del proyecto

- ** Sistema de registro e inicio de sesión **
  - Todo el mundo está registrado como cliente.
  - Los clientes pueden postularse para ser vendedores. [Imagen] (https://imgur.com/a0Jcmtf)
  - Remitente solo creado por el administrador.
  - Los administradores pueden crear otros administradores.
- **Ciclo de vida del producto**
  - Un vendedor agrega un producto.
  - Un cliente pide algunos productos, el número de existencias disminuye.
  - El cliente rastrea el estado del pedido desde que se realiza. [Imagen] (https://imgur.com/9DqrnjF)
  - Depende de la dirección proporcionada por el cliente, el remitente del área recibe una notificación. [Imagen] (https://imgur.com/Q2zWau2)
  - El vendedor del producto recibe una notificación sobre el pedido. [Imagen] (https://imgur.com/2ZnjDLA)
  - El remitente elige el producto, el vendedor lo marca como enviado.
  - El remitente entrega el pedido y lo marca como entregado.
  - El cliente puede querer devolverlo (por hacer).
- **Otras facilidades**
  - Los usuarios pueden editar la información de su cuenta. [Imagen] (https://imgur.com/gAaF4rm)
  - Los usuarios pueden rastrear el estado de su pedido. [Imagen] (https://imgur.com/9DqrnjF)
  - Los usuarios pueden agregar, eliminar o editar direcciones. [Imagen] (https://imgur.com/YUWHMko)
  - Los usuarios pueden tener una lista de deseos con cualquier cantidad de productos. [Imagen] (https://imgur.com/XVBMsAB)

#### Funciones de los usuarios - [Imagen del panel] (https://imgur.com/hn5QKlp)

- **Cliente**
  - Registrarse e iniciar sesión.
  - Cambiar la cuenta al vendedor. [Imagen] (https://imgur.com/a0Jcmtf)
  - Orden de compra de cualquier cantidad de productos.
  - Estado de la orden de seguimiento. [Imagen] (https://imgur.com/9DqrnjF)
  - Orden de devolución (Pendiente).
- ** Vendedor ** -> todo lo anterior más.
  - Agregar y editar sus propios productos.
  - Recibir notificaciones de los nuevos pedidos que realice el cliente (solo sus productos).
  - Marcar los pedidos que hacen los clientes como enviados cuando el Remitente los reciba.
- ** Remitente ** -> todo lo anterior más
  - Recibir notificaciones de pedidos (Según la dirección del cliente facilitada).
  - Envíe los pedidos a la dirección del cliente y marque el pedido como Entregado.
- ** Admin ** -> todo lo anterior más
  - Agregar, editar y eliminar categorías.
  - Agregar, editar y eliminar cualquier producto.
  - Crear otros administradores.
  - Cree remitentes y agregue un área de remitente de la que será responsable.
  - Restrinja a cualquier usuario de todos los permisos.

## 💹 &nbsp; Tecnologías

> El proyecto es creado con:

#### Backend

- Express
- Mongoose
- Json Web Token
- bcryptjs

#### Frontend

- React JS
- Redux (Manejo de estado)
- React-router (Enrutado)
- Axios (http requests)
- React Bootstrap
- React-toastify (Mensajes de error y éxito)
- Formik (Validaciones)
- Yup (Validación del lado del cliente)
- Sass

## 💡 &nbsp; Conceptos clave

- MVC (Modelo-Vista-Controlador)
- Operaciones CRUD
- Autenticación
- Encriptado de contraseñas
- Images handling using multer
- Programación orientada a objetos

## 📈 &nbsp; Diagrama UML

![Diagrama UML ](https://i.imgur.com/vGa9f8e.jpg)

## 💻 &nbsp; Configuración

Para que este proyecto funcione, installe localmente con npm:

```
$ cd inventory-application
$ npm install (install backend dependencies)
$ cd views
$ npm install (install frontend dependencies)
$ cd ..
$ npm run server (for Node server side development)
$ npm run client (for React client side development)
$ npm run dev (for both client and server side)
```

## &nbsp; ENV

- PORT=
- DB_URI=
- JWT_SECRET=
- CLOUDINARY_CLOUD_NAME=
- CLOUDINARY_API_KEY=
- CLOUDINARY_API_ESCRET=
