# SuperHosting
1. Tendremos 2 máquinas con distintos servicios cada una:
	-Batman: ldap, mysql
	-Robin: apache2, dns, phpmyadmin, cliente ldap, ftp, monsta ftp
Crear un usuario virtual en ldap donde se guarda su nombre usuario, contraseña y directorio home.
También se creará un usuario y una base de datos para este usuario.
Para el servicio de apache2 crearemos un virtualhost para cada usuario donde indicaremos en el DocumentRoot y el ServerName 
Para el nombre de dominio tendremos que crear una zona.

2. Para comprobar la existencia de un usuario lo podremos hacer mediante el servidor ldap fijandonos en el uid.
Para ver si esta dado de alta en un determinado nombre de dominio lo haremos mediante un atributo en ldap.

3. A  la hora de crear el directorio home del usuario para que pueda acceder por ftp este estará en el directorio indicado en el DocumentRoot en el virtualhost de este usuario.

4. En la resolución directa de la zona de nuestro usuario tendremos que tener 3 nombre: www, ftp y mysql

Tendremos la posibilidad de dar de baja y de dar de alta a los usuarios guardados en el ldap. Nuestro servidor tendrá la posibilidad albergar páginas
estáticas y páginas dinámicas mediante php. Cada usuario tendrá sus zonas www, ftp y mysql. Se creará el directorio personal del usuario y también
se hará referencia en el ldap y en este directorio se guardará su DocumentRoot.


Roles:
Dani: Desarrollo
Misa: Sistema
Vargax: Coordiandor y Supervisión
