# temario-de-app-web
# Propósito de Aprendizaje 1: Comprender los fundamentos del desarrollo de aplicaciones web

---

## 1. Introducción al desarrollo web
<img width="364" height="178" alt="image" src="https://github.com/user-attachments/assets/86e73d4f-0cdf-4388-84a9-a1029760225d" />

El **desarrollo web** consiste en la creación y mantenimiento de sitios o aplicaciones accesibles a través de navegadores. Su propósito es permitir la interacción entre usuarios y sistemas, brindando información, servicios y experiencias digitales.

### Historia y evolución del desarrollo web

- **Década de 1990:** El nacimiento de la web (World Wide Web) se atribuye a Tim Berners-Lee. Surge HTML como lenguaje de marcado, y los sitios eran principalmente estáticos (solo texto e imágenes).
- **Años 2000:** Aparecen tecnologías como JavaScript y CSS, que permiten interactividad y estilos. Surge el desarrollo dinámico con lenguajes como PHP, ASP y bases de datos como MySQL.
- **Años 2010:** Emergen frameworks y librerías (jQuery, Angular, React, Vue), promoviendo el desarrollo de aplicaciones de una sola página (SPA).
- **Actualidad:** La web moderna incorpora aplicaciones progresivas (PWA), APIs, servicios en la nube y mayor énfasis en la experiencia de usuario y seguridad.

### Tipos de aplicaciones web

- **Estáticas:** El contenido no cambia; suelen ser páginas informativas. Ejemplo: portafolios, sitios de presentación.
- **Dinámicas:** El contenido se genera en función de la interacción del usuario o datos almacenados. Ejemplo: foros, tiendas en línea.
- **SPA (Single Page Application):** Toda la aplicación se carga en una sola página, y la navegación es gestionada por JavaScript, mejorando la experiencia (ejemplo: Gmail).
- **PWA (Progressive Web App):** Aplicaciones web que ofrecen funcionalidades como notificaciones, trabajo offline y acceso desde la pantalla de inicio del dispositivo, acercándose a la experiencia de una app nativa.

---

## 2. Arquitectura de aplicaciones web

### Cliente-Servidor

- **Cliente:** El navegador del usuario, que solicita recursos y muestra la información.
- **Servidor:** Computadora que almacena, procesa y envía la información solicitada por el cliente.

### Arquitectura de tres capas

1. **Presentación:** Interfaz con la que interactúa el usuario (HTML, CSS, JS).
2. **Lógica de negocio:** Procesa las reglas y operaciones de la aplicación (PHP, JavaScript, Python).
3. **Datos:** Almacena la información que utiliza la aplicación (base de datos como MySQL).

Esta separación facilita el mantenimiento, escalabilidad y pruebas de la aplicación.

### REST y API-first design

- **REST (Representational State Transfer):** Arquitectura para el diseño de servicios web. Permite que los sistemas se comuniquen usando HTTP y recursos identificados por URLs.
- **API-first design:** Se diseña la API antes de implementar el resto de la aplicación, asegurando que otros sistemas puedan interactuar fácilmente y que el desarrollo sea más ágil y escalable.

---

## 3. Lenguajes y tecnologías fundamentales

- **HTML (HyperText Markup Language):** Estructura el contenido de las páginas web.
- **CSS (Cascading Style Sheets):** Permite definir el estilo y la presentación visual de los elementos HTML.
- **JavaScript:** Lenguaje de programación que añade interactividad y lógica a las páginas web (validaciones, animaciones, peticiones a servidores).
- **PHP:** Lenguaje de programación orientado a la web, ejecutado en el servidor, usado para crear páginas dinámicas y gestionar datos.
- **MySQL:** Sistema de gestión de bases de datos relacional. Permite almacenar, consultar y modificar datos utilizados por las aplicaciones.

---

## 4. Control de versiones

### Git y GitHub

- **Git:** Sistema de control de versiones distribuido que permite registrar los cambios realizados a los archivos de un proyecto, facilitando la colaboración y el seguimiento de la evolución del código.
- **GitHub:** Plataforma que hospeda repositorios Git en la nube, permitiendo compartir, colaborar y gestionar proyectos, además de facilitar la integración con otros servicios.

### Flujo de trabajo con ramas

- **Branching (ramificación):** Crear una nueva rama permite trabajar en una característica o corrección sin afectar la versión principal. Ejemplo: rama `feature/login`.
- **Merge (fusión):** Una vez terminados los cambios en una rama, se pueden combinar (merge) con la rama principal (`main` o `master`).
- **Pull requests (solicitudes de extracción):** Proceso mediante el cual se solicita que los cambios realizados en una rama sean revisados y fusionados en la rama principal. Permite la revisión colaborativa y asegura la calidad del código.

---

**Conclusión:**  
Comprender estos fundamentos permite construir aplicaciones web modernas, funcionales y mantenibles, además de facilitar el trabajo en equipo y la integración de nuevas tecnologías.

# Propósito de Aprendizaje 2: Desarrollar componentes y funcionalidades de una aplicación web

---

## 1. Diseño e implementación del frontend

El **frontend** es la parte de la aplicación web con la que interactúa el usuario. Su desarrollo implica diseñar la interfaz y construir la lógica que se ejecuta en el navegador.

### Maquetación / Wireframe / Mockup

- **Wireframe:** Esquema básico y funcional de la interfaz, normalmente dibujado en papel o software especializado. Define la estructura y ubicación de los elementos principales.
- **Mockup:** Prototipo visual más detallado, muestra colores, tipografía y diseño final pero sin interactividad.
- **Maquetación:** Proceso de convertir el diseño (mockup) en código HTML, CSS y JavaScript. Se crean los componentes visuales y la estructura de la página web.

### API

El frontend se comunica con el backend mediante **APIs** (Interfaz de Programación de Aplicaciones). A través de llamadas HTTP (fetch, axios), el frontend solicita datos, envía información y recibe respuestas para actualizar la interfaz dinámicamente.

---

## 2. Diseño e implementación del backend

El **backend** es la lógica y procesamiento que ocurre en el servidor, invisible para el usuario pero esencial para el funcionamiento de la aplicación.

### Servidor

El servidor ejecuta el código que procesa las solicitudes del cliente, accede a bases de datos y envía respuestas. Puede estar construido con tecnologías como Node.js, PHP, Python (Django/Flask), Java (Spring), etc.

### Manejo de peticiones y respuestas HTTP

- El backend recibe **peticiones HTTP** (GET, POST, PUT, DELETE, etc.) desde el frontend o servicios externos.
- Procesa la solicitud, realiza operaciones (consultar, guardar, modificar datos) y envía una **respuesta HTTP** con el resultado (datos, mensajes de estado, etc.).

### Conexión a bases de datos

El backend debe conectarse a una base de datos para almacenar y recuperar información. Ejemplos de sistemas de bases de datos:

- **MySQL/PostgreSQL:** Bases de datos relacionales, estructuran datos en tablas relacionadas.
- **MongoDB:** Base de datos NoSQL orientada a documentos, almacena información en formato JSON/BSON.

---

## 3. Bases de datos

### Modelado de datos y relaciones

El **modelado de datos** implica definir las entidades (por ejemplo, usuarios, productos) y cómo se relacionan entre sí (uno a uno, uno a muchos, muchos a muchos). En bases de datos relacionales, esto se traduce en tablas y claves foráneas.

### ORM (Object Relational Mapping)

Un **ORM** es una herramienta que permite trabajar con bases de datos usando objetos en el lenguaje de programación del backend. Ejemplo: Sequelize (Node.js), SQLAlchemy (Python), Doctrine (PHP).

- Facilita consultas, inserciones y actualizaciones sin escribir SQL directamente.
- Permite mapear modelos de datos a tablas de la base de datos.

### CRUD desde el backend

**CRUD** significa **Create, Read, Update, Delete** (Crear, Leer, Actualizar, Eliminar). El backend implementa estas operaciones para que el frontend pueda gestionar datos a través de la API.

Ejemplo de endpoints:
- **POST /usuarios** → Crear usuario
- **GET /usuarios** → Leer usuarios
- **PUT /usuarios/:id** → Actualizar usuario
- **DELETE /usuarios/:id** → Eliminar usuario

---

## 4. Seguridad básica en aplicaciones web

La seguridad protege la aplicación y los datos de los usuarios frente a amenazas y errores.

### Validación de formularios

- Validar los datos ingresados por el usuario tanto en el frontend como en el backend.
- Prevenir ataques como la inyección de código o envío de datos maliciosos.

### Autenticación y autorización

- **Autenticación:** Verifica la identidad del usuario (login con usuario y contraseña, tokens, OAuth).
- **Autorización:** Determina qué acciones puede realizar el usuario según sus permisos o roles (administrador, usuario normal).

---

**Conclusión:**  
El desarrollo de componentes y funcionalidades de una aplicación web requiere coordinar el diseño visual, la lógica del servidor, la gestión de datos y la seguridad para crear aplicaciones robustas y eficientes.

# Propósito de Aprendizaje 3: Implementar y desplegar una aplicación web funcional

---

## 1. Integración de frontend y backend

La integración consiste en conectar la interfaz de usuario con la lógica de negocio y los datos, logrando una aplicación web completa y funcional.

### Interfaz de usuario Frontend

El **frontend** es el punto de interacción de los usuarios con la aplicación. Utiliza tecnologías como HTML, CSS y JavaScript (o frameworks como React, Vue, Angular) para construir páginas interactivas, formularios y componentes visuales.

### Manejo de API

La comunicación entre frontend y backend se realiza mediante **APIs (Application Programming Interface)**. El frontend envía **solicitudes HTTP** (fetch, axios) a los endpoints del backend y recibe **respuestas** con datos o confirmaciones de operaciones.

Por ejemplo, un formulario de registro en el frontend envía los datos a una API del backend, que los valida, almacena y responde con el resultado.

### Proceso de Solicitud y Respuesta de Backend

El **backend** recibe las solicitudes del frontend, procesa la lógica (validaciones, operaciones con bases de datos), y envía una **respuesta** (éxito, error, datos solicitados) al frontend. Este ciclo permite la interacción dinámica y la actualización de la interfaz según las acciones del usuario.

---

## 2. Almacenamiento en Servidor

El almacenamiento y la publicación de la aplicación requieren servidores y servicios especializados.

### Tipos de servidores

- **Servidores dedicados:** Hardware exclusivo para una o varias aplicaciones, ofrece mayor control y rendimiento.
- **Servidores compartidos:** Varios sitios comparten los recursos del servidor; es más económico pero con menos recursos.
- **Servidores virtuales (VPS):** Particiones virtuales de un servidor físico, ofrecen flexibilidad y escalabilidad.

### Servidores y servicios de hosting

- **Hosting tradicional:** Empresas que proveen espacio en servidores para alojar sitios web (ejemplo: Bluehost, Hostgator).
- **Hosting en la nube:** Servicios escalables y flexibles (ejemplo: AWS, Google Cloud, Azure) que permiten desplegar aplicaciones en infraestructura gestionada.

### Proveedores de Servicios de Almacenamiento

Proveedores populares de almacenamiento y hosting incluyen:
- **Amazon Web Services (AWS):** Ofrece EC2 (servidores virtuales), S3 (almacenamiento de archivos), RDS (bases de datos).
- **Google Cloud Platform:** Instancias de servidor, almacenamiento, bases de datos.
- **Microsoft Azure:** Servicios similares a AWS y Google Cloud.
- **Heroku:** Despliegue sencillo de aplicaciones web, ideal para proyectos pequeños y medianos.
- **Vercel/Netlify:** Especializados en aplicaciones frontend y JAMstack.

---

## 3. Optimización y rendimiento

La optimización asegura que la aplicación funcione rápido, de manera eficiente y con bajo consumo de recursos.

### Optimización de recursos (imágenes, scripts)

- **Imágenes:** Reducir tamaño y formato, usar lazy loading para cargar solo las necesarias.
- **Scripts:** Minimizar y agrupar archivos JavaScript y CSS, cargar scripts de manera asíncrona.
- **Caching:** Almacenar recursos en el navegador para reducir solicitudes repetidas.

### Despliegue de aplicaciones web

El **despliegue** consiste en publicar la aplicación en un servidor o servicio de hosting, haciéndola accesible para los usuarios. Implica transferir archivos, configurar servicios y asegurar que la aplicación esté lista para producción.

### CI/CD básico

- **Integración Continua (CI):** Automatización de pruebas y verificación de cambios en el código antes de integrarlos.
- **Despliegue Continuo (CD):** Automatización del proceso de publicación de la aplicación al servidor tras cada cambio exitoso.
- Herramientas populares: GitHub Actions, GitLab CI, Jenkins.

### Documentación del proyecto

Documentar el proyecto facilita su uso, mantenimiento y colaboración. Incluye:
- **README:** Explicaciones de la funcionalidad, instrucciones de instalación y uso.
- **Comentarios en el código:** Ayudan a entender la lógica y el propósito de funciones y módulos.
- **Guía de despliegue y configuración:** Pasos para instalar, ejecutar y desplegar la aplicación.

---

**Conclusión:**  
Implementar y desplegar una aplicación web funcional requiere conectar todas sus partes (frontend, backend, almacenamiento), asegurar su rendimiento y documentar el proceso, logrando un producto listo para el usuario final y para el trabajo colaborativo.
