# ContenedorIAW

Usuarios actualmeente existentes (usuario - contraseña): 

user - user
admin - admin

Para arrancar el contenedor:
(Los siguientes puertos y nombre del contenedor pueden ser modificados, pero han de ser posibles)

sudo docker run -it -d --name proyecto -p 8080:80 -p 3316:3306 algargon99/proyecto_iaw

Para poder ser visualizada, en un navegador web escribimos lo siguiente:
(El puerto será el indicado en el anterior comando)

localhost:8080

La página web esta creada en base a una librería, en la que se permiten el servicio de venta para los usuarios,
además de el control total de esta siendo el usuario "admin".

El usuario podrá ver los libros que hay disponibles y la opción de comprarlos. 
También tiene la opción de ver los datos de los pedidos que ha hecho.

El admin tiene la opción de manipular los datos de toda la base de datos, incluyenbdo esto:

· Ver, crear, eliminar y modificar todos los datos de todos los usuarios, pedidos, empleados y libros.
· Comprar sus propios libros

Ambos pueden ver los datos actuales de su perfil.
