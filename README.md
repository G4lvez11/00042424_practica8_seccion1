 ¿Cuál es la diferencia entre autenticación y autorización?

**Autenticación** es el proceso de verificar **quién eres**. Se realiza cuando un usuario envía sus credenciales (email y password) al servidor, y este verifica que existan en la base de datos. 

**Autorización** es el proceso de verificar **qué permisos tienes**. Después de autenticarte, el servidor verifica si tienes acceso a ciertos recursos mediante el token JWT.

 ¿Cuál es la función del token JWT en la guía?

El **JWT (JSON Web Token)** funciona como un pase de acceso temporal que cumple las siguientes funciones:

1. **Evita enviar credenciales repetidamente:** Solo te autentícas una vez durante el login, y el servidor te devuelve un token que usarás en las siguientes peticiones.

2. **Identifica al usuario:** El token contiene información del usuario encriptada (id, email, name) que el servidor puede leer sin consultar la base de datos.

3. **Tiene tiempo de expiración:** En esta guía el token expira después de 1 hora 
