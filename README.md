# TrackTower

TrackTower es una plataforma completa para la gestión eficiente de listas de reproducción de música. Con tecnologías modernas como Java, Spring Boot, Angular y JWT, TrackTower ofrece una experiencia robusta y segura para los amantes de la música que desean crear y organizar sus propias colecciones de canciones.

![TrackTower Demo](link a una imagen o GIF demostrativo del proyecto)

## Detalles Técnicos para Colaboradores

### Tecnologías Utilizadas:

- **Java:** El backend del proyecto está desarrollado en Java utilizando el framework Spring Boot.
- **Maven:** Se utiliza Maven como sistema de gestión de dependencias y para la construcción del proyecto.
- **Spring Boot:** Se emplea Spring Boot para la creación de la aplicación web y la configuración del servidor.
- **Spring Data JPA:** Para la capa de persistencia, se utiliza Spring Data JPA para interactuar con la base de datos.
- **H2 Database:** La base de datos en memoria H2 se utiliza para el almacenamiento de los datos en tiempo de ejecución.
- **JWT (JSON Web Token):** Se implementa JWT para la autenticación y autorización de los usuarios.
- **Angular:** Para el frontend, se utiliza Angular como framework de desarrollo web.
- **HttpClient:** Angular HttpClient se utiliza para realizar solicitudes HTTP al backend y consumir la API REST.

### Estructura del Proyecto:

- **Backend (`tracktower-api`):**
  - **Modelo:** Las entidades JPA (`Playlist` y `Song`) se encuentran en el paquete `com.example.playlistapi.model`.
  - **Repositorios:** Los repositorios JPA (`PlaylistRepository`) se encuentran en el paquete `com.example.playlistapi.repository`.
  - **Controladores:** Los controladores REST (`PlaylistController`) se encuentran en el paquete `com.example.playlistapi.controller`.
  - **Seguridad:** La configuración de seguridad con JWT se encuentra en el paquete `com.example.playlistapi.security`.
  - **Pruebas Unitarias:** Las pruebas unitarias para los controladores se encuentran en el directorio `src/test/java`.

- **Frontend (`tracktower-app`):**
  - **Servicios:** El servicio Angular para interactuar con la API REST se encuentra en el directorio `src/app/services`.
  - **Componentes:** Los componentes Angular (`playlist-list` y `playlist-create`) se encuentran en el directorio `src/app/components`.
  - **Enrutamiento:** La configuración de las rutas de la aplicación se encuentra en el archivo `src/app/app-routing.module.ts`.
  - **Interfaz de Usuario:** Las plantillas HTML y estilos CSS se encuentran en los archivos `.html` y `.css` respectivamente.

### Configuración del Entorno de Desarrollo:

- **IDE Recomendado:** Se recomienda utilizar un IDE compatible con Java y Angular, como IntelliJ IDEA o Visual Studio Code.
- **Dependencias:** Asegúrate de tener instaladas las dependencias necesarias como Maven, Node.js y Angular CLI.
- **Base de Datos:** La aplicación utiliza una base de datos H2 en memoria. No se requiere configuración adicional.
- **Variables de Entorno:** Configura las variables de entorno necesarias, como la clave secreta para JWT.

### Ejecución y Pruebas:

- **Backend:** Para ejecutar el servidor backend, utiliza el comando `mvn spring-boot:run`.
- **Frontend:** Para ejecutar el servidor frontend, utiliza el comando `ng serve`. La aplicación estará disponible en `http://localhost:4200`.
- **Pruebas:** Utiliza herramientas como Postman para probar los endpoints de la API REST. Para ejecutar las pruebas unitarias, utiliza el comando `mvn test`.

### Colaboración y Contribución:

- Si deseas contribuir al proyecto, asegúrate de seguir las pautas de contribución y abrir un pull request con tus cambios.
- Si tienes alguna pregunta o problema, no dudes en abrir un issue en el repositorio del proyecto.
