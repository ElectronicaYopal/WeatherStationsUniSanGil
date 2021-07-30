# MariaDB: Aplicativo para guardar los datos.

Software de codigo abierto para manejo de bases de datos relacionales.

## Instalación

Seguir los siguiente pasos para instalar en sistemas Debian, información más detallada aquí: https://www.digitalocean.com/community/tutorials/how-to-install-mariadb-on-ubuntu-20-04-es

```bash
sudo apt update
sudo apt install mariadb-server
sudo mysql_secure_installation
```

## Añadir usuario a base de datos

- Ingresar a MariaDB
```bash
sudo mariadb
```
- Dentro crear usuario y garantizar sus permisos
```bash
CREATE USER 'weewx'@'localhost' IDENTIFIED BY 'weewx';
GRANT select, update, create, delete, insert, alter, drop ON weewx.* TO weewx@localhost;
```
para salidr de MariaDB digite: *exit* y presione [Enter]
