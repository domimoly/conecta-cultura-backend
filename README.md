CREATE DATABASE conecta_cultura
  CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

CREATE USER 'conecta_app'@'localhost'
  IDENTIFIED BY 'CAMBIAR_CLAVE';

GRANT ALL PRIVILEGES ON conecta_cultura.*
  TO 'conecta_app'@'localhost';
FLUSH PRIVILEGES;

### -----

http://localhost:8082/swagger-ui/index.html#/actividad-controller/crear
