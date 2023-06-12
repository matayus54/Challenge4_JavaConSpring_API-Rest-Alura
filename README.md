# Challenge 4 | Back End | Api Rest | Foro Alura

Demostrativo de la aplicación:

https://github.com/Guipray/challenge-one-forum-alura/assets/109701399/2dcdfa9b-95dc-4978-9086-ff631eb8009

### Tecnologias utilizadas:

-  [IntelliJ](https://www.jetbrains.com/pt-br/idea/)
-  [MySql](https://www.mysql.com/)
-  [Java](https://www.java.com/pt-BR/)
-  [Spring Boot](https://start.spring.io/)
-  [Flyway Migration](https://start.spring.io/)
-  [Spring Security](https://start.spring.io/)
-  [Token JWT](https://jwt.io/)
-  [Swagger](https://swagger.io/)

## Como utilizar esse repositório

-  Descargue el código ["code"](https://github.com/matayus54/Modelo_Nuevo-Proyecto_Github/archive/refs/heads/main.zip) de GitHub
-  Ingrese a la carpeta usando su IDE preferido como IntellijIDEA o Eclipse
-  Descargue las dependencias del proyecto usando Maven
-  cree una base de datos para mysql
-  Defina las siguentes variables
-  `DB_NAME`: El nombre de la base de datos de la aplicación, ejemplo "db_forum_Alura_api"
-  `DB_USER`: El nombre de usuario de la base de datos
-  `DB_PASSWORD`: La contraseña de la base de datos
-  `JWT_SECRET`: la "contraseña/secreto" utilizada para generar y desmontar el token JWT
-  ejecutar el proyecto

## Documentación

Este proyecto utiliza Swagger para generar la documentación, al ejecutar el proyecto puede acceder
EndPoint `/swagger-ui` para ver la documentación del proyecto.

En este punto final también es posible ejecutar las funcionalidades de la API, tenga en cuenta que para esto la página requerirá
el uso de la autenticación a través del token JWT que se puede generar a través del punto final `POST /login`, que requerirá
un usuario previamente registrado en el endpoint `POST /users` o en la tabla `users` de la base de datos del proyecto.

## Puntos finales - Autenticación

-  `POST /login`: Inicia sesión en la aplicación, devuelve el token para ser utilizado en las próximas solicitudes

## Puntos finales - Usuario

-  `GET /users`: devuelve todos los usuarios
-  `GET /users/:id`: devuelve un usuario específico
-  `POST /usuarios`: crea un nuevo usuario con el nombre, email y contraseña dados
-  `PUT /users`: actualiza los datos de un usuario específico existente
-  `DELETE /users/:id`: elimina los datos de un usuario existente específico

## Puntos finales - Cursos

-  `GET /courses`: devuelve todos los cursos
-  `GET /courses/:id`: devuelve un curso específico
-  `POST /cursos`: crea un nuevo curso con el nombre y la categoría dados
-  `PUT /cursos`: actualiza los datos de un curso específico existente
-  `DELETE /courses`: elimina datos de un curso específico existente

## Criterios de valoración - Temas

-  `GET /topics`: devuelve todos los temas
-  `GET /topics/:id`: devuelve un tema específico
-  `POST /topics`: crea un nuevo tema con el título, mensaje, autor y curso informado
-  `PUT /topics`: actualiza los datos de un tema específico existente
-  `DELETE /topics`: elimina datos de un tema específico existente

## Puntos finales - Respuestas

-  `GET /respuestas`: devuelve todas las respuestas
-  `GET /respuestas/:id`: devuelve una respuesta específica
-  `POST /respuestas`: crea una nueva respuesta con el mensaje, el autor y el tema dados
-  `PUT /respuestas`: actualiza los datos de una respuesta específica existente
-  `ELIMINAR /respuestas`: eliminar datos de una respuesta específica existente
