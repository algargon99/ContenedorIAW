# ContenedorIAW

Usuarios actualmente existentes de la página web (usuario - contraseña): 

- user - user
- admin - admin

Usuarios actualmente existentes de la base de datos (usuario - contraseña): 

- root - 123456
- user - 2asirtriana

Para arrancar el contenedor:
(Los siguientes puertos y nombre del contenedor pueden ser modificados, pero han de ser posibles)

**sudo docker run -it -d --name proyecto -p 8080:80 -p 3316:3306 algargon99/proyecto_iaw**

Si quisieramos entrar en el contenedor:

**sudo docker exec -it proyecto /bin/bash**

Para iniciar el contenedor:

**sudo docker start proyecto**

Para para y borrar el contenedor, respectivamente:

**sudo docker stop proyecto**
**sudo docker rm proyecto**

Para poder ser visualizada, en un navegador web escribimos lo siguiente:
(El puerto será el indicado en el anterior comando)

**localhost:8080**

La página web esta creada en base a una librería, en la que se permiten el servicio de venta para los usuarios,
además de el control total de esta siendo el usuario "admin".

El usuario podrá ver los libros que hay disponibles y la opción de comprarlos. 
También tiene la opción de ver los datos de los pedidos que ha hecho.

El admin tiene la opción de manipular los datos de toda la base de datos, incluyenbdo esto:

- Ver, crear, eliminar y modificar todos los datos de todos los usuarios, pedidos, empleados y libros.
- Comprar sus propios libros

Ambos pueden ver los datos actuales de su perfil.

La estructura de la base de datos es:

![alt text](https://raw.githubusercontent.com/algargon99/PROYECTO_IAW_GARCIA_GONZALEZ/master/imagenes/Base_de_datos.png)
