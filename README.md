🌟 ForoHub 🌟
# ![Badge-Spring](https://github.com/user-attachments/assets/65298ec3-048b-4166-ab66-70929be32f48)

¡Bienvenido a ForoHub! Esta API te permite realizar diversas solicitudes REST:

* Iniciar sesión
* Registrar un tópico
* Actualizar un tópico
* Eliminar un tópico
* Listar tópicos

## 🚀 Servidores

La API se despliega localmente en:
* Base URL: http://localhost:8080

## 🔐 Autorización

La API requiere autorización mediante tokens JWT para acceder a ciertas funciones.

## ✅ Tecnologías Utilizadas

- Java (versión 17 en adelante)
- Maven (Initializr utiliza la versión 4)
- Spring Boot
- MySQL
- JWT (JSON Web Tokens)

### Dependencias
Al crear el proyecto con Spring Initializr, se utilizaron las siguientes dependencias:

- Lombok
- Spring Web
- Spring Boot DevTools
- Spring Data JPA
- Flyway Migration
- MySQL Driver
- Validation
- Spring Security

## 🌟 Endpoints

### Tópicos (`topico-controller`)

- **Actualizar un tópico**
   - `PUT /topico/actualizar`
   - Body: `DatosActualizarTopico`

- **Crear un nuevo tópico**
   - `POST /topico`
   - Body: `DatosRegistroTopico`

- **Listar todos los tópicos**
   - `GET /topico/listar`
   - Respuesta: `List<PageDatosListadoTopico>`

- **Dar de alta un tópico**
   - `GET /topico/alta/{id}`

- **Eliminar un tópico (lógico)**
   - `DELETE /topico/eliminar/{id}`
 

### Autenticación (`autenticacion-controller`)

- **Iniciar sesión (login)**
   - `POST /login`
   - Body: `DatosAutenticacionUsuario`
   - Respuesta: `DatosJWTtoken`

### Diagrama de la base de datos MySQL:
![image](https://github.com/user-attachments/assets/7ec6c4b6-632b-4ccc-bcd8-c69e3c428d2f)
