# Red Social API

### Api que nos permite interactuar entre los distintos usuarios (CRUD), creando publicaciones y poder darles 'Like' y realizar comentarios.

### Dependencias utilizadas:

```java
    - "bcrypt",
    - "cors",
    - "dotenv",
    - "express":,
    - "express-rate-limit":,
    - "jsonwebtoken":,
    - "morgan",
    - "nodemailer",
    - "passport",
    - "passport-jwt",
    - "pg",
    - "pg-hstore",
    - "sequelize",
    - "uuid"
```

#### Instalar Dependencias:

```java
npm install
```

#### Configurar Variables de entorno:

```javascript
PORT =
HOST =
JWT_SECRET =
DB_HOST =
DB_USER =
DB_PASSWORD =
DB_NAME =
DB_PORT =
MAIL_PASS =
```

#### Iniciar Proyecto:

```java
npm run dev
```

### Rutas

- /auth

```javascript
  - /login -> Login con las credenciales del usuario para autenticar
```

- /posts

```javascript
  - /me -> Mis propias publicaciones
  - /user/:id -> Publicaciones de usuarios en particular
  - /:id -> Una publicación en especifico
  - /:id/comments -> Los comentarios de una publicación en especifico
  - /:id/likes -> Los likes de una publicación en especifico
```

- /users

```javascript
  - /me -> Mi informacion de usuario
  - /:id -> Un usuario en especifico
  - /:id/follow
```

- /follows

```javascript
  - /:id
```

- /followers

```javascript
  - /:id
```

### Controllers Posts

```javascript
- [x] findAllPosts
- [x] findPostById
- [x] createPost
- [x] updatePost
- [x] removePost
```

### Services Posts

```javascript
- [ ] getAllPosts
- [ ] getPostById
- [ ] postNewPost
- [ ] patchPost
- [ ] deletePost
```
