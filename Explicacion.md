# Configuraciones de Docker Compose

## Parte 1: Drupal + MySQL

### Explicación:

-   Se define un servicio para Drupal y otro para MySQL en el archivo `docker-compose.yml`.
-   Drupal utiliza el puerto 81 del host para acceder a través del puerto 80 del contenedor.
-   Se utilizan volúmenes para persistir la información de Drupal y MySQL.
-   Drupal depende de MySQL para su funcionamiento, por lo que se especifica la dependencia.
-   Se configuran variables de entorno para que Drupal pueda conectarse a la base de datos MySQL.


## Parte 2: WordPress + MariaDB

### Explicación:

-   Se define un servicio para MariaDB y otro para WordPress en el archivo `docker-compose.yml`.
-   Se utiliza la versión 3.8 de Docker Compose para aprovechar las últimas características.
-   MariaDB y WordPress se configuran para reiniciar siempre que sea necesario.
-   Se establece la contraseña de root y se crea la base de datos para WordPress en MariaDB.
-   Se utilizan volúmenes para persistir la información de MariaDB y WordPress.
-   WordPress depende de MariaDB para su funcionamiento, por lo que se especifica la dependencia.
-   Se configuran variables de entorno para que WordPress pueda conectarse a la base de datos MariaDB.
