# App Cactus API

## Descripción

**App Cactus API** es un servicio backend desarrollado en **Node.js** con **Express.js**, que proporciona endpoints para la gestión de usuarios y productos. La API permite registrar usuarios, iniciar sesión, gestionar perfiles, CRUD y listar productos.

## URL para pruebas en producción

- Para las pruebas en producción utilizar la siguiente URL: https://app-cactus-api.onrender.com

## Tecnologías Utilizadas

- **Node.js**: Entorno de ejecución para JavaScript.
- **Express.js**: Framework para crear la API REST.
- **MongoDB**: Base de datos NoSQL para almacenar datos de usuarios y productos.
- **JWT**: Autenticación y generación de tokens de sesión.
- **Swagger**: Documentación de la API.

## Requisitos Previos

1. **Node.js** instalado (v16 o superior).
2. **MongoDB Atlas** o servidor local de MongoDB.
3. **Cuenta de Render.com** o servidor de despliegue compatible.

## Instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/usuario/app-cactus-api.git
   ```

2. Navega al directorio del proyecto:

   ```bash
   cd app-cactus-api
   ```

3. Instala las dependencias:

   ```bash
   npm install
   ```

4. Configura las variables de entorno creando un archivo **.env** en la raíz del proyecto:

   ```env
   PORT=3000
   MONGO_URI=mongodb+srv://<usuario>:<password>@cluster.mongodb.net/app-cactus-api
   JWT_SECRET=tu_clave_secreta
   ```

## Scripts Disponibles

- **Iniciar el servidor en desarrollo:**

  ```bash
  npm run dev
  ```

- **Compilar y ejecutar en producción:**

  ```bash
  npm start
  ```

## Endpoints Principales

### Autenticación

- **POST** `/api/usuarios/register`: Registro de usuarios.
- **POST** `/api/usuarios/login`: Inicio de sesión.

### Gestión de Usuarios

- **GET** `/api/usuarios/me`: Obtener datos del usuario autenticado.
- **PUT** `/api/usuarios/:id`: Actualizar perfil.
- **DELETE** `/api/usuarios/:id`: Eliminar cuenta.

### Productos

- **GET** `/api/productos`: Listar todos los productos.
- **GET** `/api/productos/:id`: Detalle de un producto.

### Compras

- **POST** `/api/compras`: Procesar compras con PayPal.

## Documentación de la API

Accede a la documentación generada automáticamente por **Swagger** en:

```
http://localhost:3000/api-docs
```

## Despliegue

Despliega la API en servicios como **Render.com**, **Heroku** o **AWS** siguiendo estas instrucciones:

1. Configura las variables de entorno en la plataforma de despliegue.
2. Define el comando de inicio: `npm start`.

## Contribución

1. Crea un fork del repositorio.
2. Crea una nueva rama:
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```
3. Realiza tus cambios y confirma los commits.
4. Envía una solicitud de extracción (Pull Request).

## Licencia

Este proyecto está bajo la **Licencia MIT**.

---

