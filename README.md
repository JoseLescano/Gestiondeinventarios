# Plataforma de Gestión de Ventas y Productos

Este repositorio contiene el código fuente de una plataforma web diseñada para gestionar productos, ventas y usuarios. La aplicación está construida utilizando Node.js, Express.js, MongoDB, y Tailwind CSS, y está pensada para servir tanto a vendedores como a compradores, ofreciendo una experiencia de usuario intuitiva y segura.

## Video: 
https://youtu.be/sg8d5tUO0s4

## Informe:
https://drive.google.com/file/d/1Bxl6KWTiHNvX36I6K-wsG3qnEr7jcT5M/view?usp=sharing

## Figma
https://www.figma.com/design/JUtB1k4HYJJwgqc5CDFh9Q/Wireframes?node-id=2-41&t=QWgkL0m53NVz8idT-1 


## Características Principales

- **Gestión de Inventarios:** Permite a los vendedores agregar, editar y eliminar productos con facilidad.
- **Sistema de Autenticación:** Autenticación segura mediante JSON Web Tokens (JWT) y roles específicos para compradores, vendedores y administradores.
- **Interfaz Intuitiva:** Uso de Tailwind CSS para una experiencia de usuario fluida y responsiva.
- **Favoritos y Compras:** Los compradores pueden agregar productos a favoritos y realizar compras fácilmente.
- **Análisis de Ventas:** Estadísticas detalladas para vendedores, incluyendo productos más vendidos y clientes únicos.

## Tecnologías Utilizadas

- **Backend:** Node.js, Express.js, MongoDB
- **Frontend:** HTML5, Tailwind CSS, JavaScript
- **Autenticación y Seguridad:** JSON Web Tokens (JWT), bcrypt.js
- **Cargas de Archivos:** multer para la gestión de imágenes

## Instalación

Sigue los siguientes pasos para instalar y configurar el proyecto en tu máquina local:

1. Clona el repositorio:
   
   git clone [URL_DEL_REPOSITORIO]

2. Navega al directorio del proyecto:
   
   cd [NOMBRE_DEL_DIRECTORIO]

3. Instala las dependencias necesarias:
   
   npm install

4. Configura las variables de entorno creando un archivo `.env` en la raíz del proyecto con el siguiente contenido:
   
   PORT=3000
   MONGODB_URI=mongodb://localhost:27017/nombreDeTuBaseDeDatos
   JWT_SECRET=tuClaveSecreta

5. Inicia el servidor:
   
   node app.js

6. Abre tu navegador web y accede a la aplicación en http://localhost:3000.

## Estructura del Proyecto

- **models/**: Contiene los esquemas de datos para usuarios, productos, favoritos y compras.
- **routes/**: Define las rutas de la API y los controladores para manejar las solicitudes.
- **middleware/**: Contiene funciones de autenticación y autorización.
- **uploads/**: Almacena las imágenes de los productos cargados.
- **public/**: Archivos estáticos accesibles para el frontend.

## Uso

### Registro e Inicio de Sesión
- Los usuarios pueden registrarse como compradores, vendedores o administradores.
- Autenticación segura mediante JWT para proteger las rutas de la aplicación.

### Gestión de Productos (Para Vendedores)
- Los vendedores pueden agregar nuevos productos, editar detalles existentes y gestionar su inventario a través del panel de control.

### Favoritos y Compras (Para Compradores)
- Los compradores pueden añadir productos a sus favoritos y proceder a la compra de manera sencilla.

### Estadísticas y Análisis de Ventas (Para Vendedores)
- Los vendedores tienen acceso a estadísticas detalladas que les permiten analizar el rendimiento de sus ventas.

## Contribuciones

Las contribuciones son bienvenidas. Siéntete libre de abrir un issue o enviar un pull request con mejoras y correcciones. Por favor, asegúrate de seguir las mejores prácticas y proporcionar una descripción clara de los cambios que realizas.

## Problemas y Soluciones Comunes

- **Problema de Conexión con MongoDB:** Verifica que el URI de la base de datos esté configurado correctamente en el archivo `.env`.
- **Errores de Autenticación:** Asegúrate de que el JWT_SECRET esté configurado correctamente y que los tokens no estén expirados.
