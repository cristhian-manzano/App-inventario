<h1 align="center">  馃洅 &nbsp; App de compras 馃洅 </h1>

> Construido con el Stack MERN (MongoDB, Express, React and Node).

## 馃摐 &nbsp; Tabla de conceptos

- [Principales caracter铆sticas](#--main-features)
- [Tecnolog铆as](#--technologies)
- [Conceptos clave](#--key-concepts)
- [Diagrama UML](#--uml-diagram)
- [Configuraci贸n](#--setup)
- [ENV](#-ENV)

## 馃毄 &nbsp; Principales caracter铆sticas

> Esta aplicaci贸n se cre贸 para rastrear el estado del pedido desde que el cliente lo coloc贸
> una vez enviado, el vendedor lo marca como enviado y luego el remitente lo marca como entregado.

#### Metodolog铆a del proyecto

- ** Sistema de registro e inicio de sesi贸n **
  - Todo el mundo est谩 registrado como cliente.
  - Los clientes pueden postularse para ser vendedores. [Imagen] (https://imgur.com/a0Jcmtf)
  - Remitente solo creado por el administrador.
  - Los administradores pueden crear otros administradores.
- **Ciclo de vida del producto**
  - Un vendedor agrega un producto.
  - Un cliente pide algunos productos, el n煤mero de existencias disminuye.
  - El cliente rastrea el estado del pedido desde que se realiza. [Imagen] (https://imgur.com/9DqrnjF)
  - Depende de la direcci贸n proporcionada por el cliente, el remitente del 谩rea recibe una notificaci贸n. [Imagen] (https://imgur.com/Q2zWau2)
  - El vendedor del producto recibe una notificaci贸n sobre el pedido. [Imagen] (https://imgur.com/2ZnjDLA)
  - El remitente elige el producto, el vendedor lo marca como enviado.
  - El remitente entrega el pedido y lo marca como entregado.
  - El cliente puede querer devolverlo (por hacer).
- **Otras facilidades**
  - Los usuarios pueden editar la informaci贸n de su cuenta. [Imagen] (https://imgur.com/gAaF4rm)
  - Los usuarios pueden rastrear el estado de su pedido. [Imagen] (https://imgur.com/9DqrnjF)
  - Los usuarios pueden agregar, eliminar o editar direcciones. [Imagen] (https://imgur.com/YUWHMko)
  - Los usuarios pueden tener una lista de deseos con cualquier cantidad de productos. [Imagen] (https://imgur.com/XVBMsAB)

#### Funciones de los usuarios - [Imagen del panel] (https://imgur.com/hn5QKlp)

- **Cliente**
  - Registrarse e iniciar sesi贸n.
  - Cambiar la cuenta al vendedor. [Imagen] (https://imgur.com/a0Jcmtf)
  - Orden de compra de cualquier cantidad de productos.
  - Estado de la orden de seguimiento. [Imagen] (https://imgur.com/9DqrnjF)
  - Orden de devoluci贸n (Pendiente).
- ** Vendedor ** -> todo lo anterior m谩s.
  - Agregar y editar sus propios productos.
  - Recibir notificaciones de los nuevos pedidos que realice el cliente (solo sus productos).
  - Marcar los pedidos que hacen los clientes como enviados cuando el Remitente los reciba.
- ** Remitente ** -> todo lo anterior m谩s
  - Recibir notificaciones de pedidos (Seg煤n la direcci贸n del cliente facilitada).
  - Env铆e los pedidos a la direcci贸n del cliente y marque el pedido como Entregado.
- ** Admin ** -> todo lo anterior m谩s
  - Agregar, editar y eliminar categor铆as.
  - Agregar, editar y eliminar cualquier producto.
  - Crear otros administradores.
  - Cree remitentes y agregue un 谩rea de remitente de la que ser谩 responsable.
  - Restrinja a cualquier usuario de todos los permisos.

## 馃捁 &nbsp; Tecnolog铆as

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
- React-toastify (Mensajes de error y 茅xito)
- Formik (Validaciones)
- Yup (Validaci贸n del lado del cliente)
- Sass

## 馃挕 &nbsp; Conceptos clave

- MVC (Modelo-Vista-Controlador)
- Operaciones CRUD
- Autenticaci贸n
- Encriptado de contrase帽as
- Images handling using multer
- Programaci贸n orientada a objetos

## 馃搱 &nbsp; Diagrama UML

![Diagrama UML ](https://i.imgur.com/vGa9f8e.jpg)

## 馃捇 &nbsp; Configuraci贸n

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
