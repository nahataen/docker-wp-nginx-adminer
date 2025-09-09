# 🚀 Docker WordPress + Nginx + MariaDB + Adminer

![Docker Logo](./docker-logo.png)

Este proyecto levanta un entorno completo de **WordPress** utilizando **Docker Compose**, ideal para desarrollo local o pruebas rápidas.

##  Contenido de los Servicios

- **WordPress (PHP-FPM 8.2)**  
  Ejecuta WordPress con PHP-FPM 8.2. Los archivos del sitio se guardan en: `./wp-data`.

- **Nginx (stable)**  
  Servidor frontend que expone WordPress en **[http://localhost:8080](http://localhost:8080)**. Usa configuración personalizada (`./nginx/default.conf`).

- **MariaDB (10.6)**  
  Base de datos para WordPress, con datos persistentes en el volumen `db_data`.  
  - Usuario: `wpuser`  
  - Contraseña: `wppass`  
  - Base de datos: `wpdb`  
  - Root: `rootpass`

- **Adminer**  
  Interfaz web para gestionar la base de datos en **[http://localhost:8081](http://localhost:8081)**. Usa tema CSS personalizado (`./adminer-theme/adminer.css`).

## ▶ Cómo usarlo

1. Clona el repositorio:
   ```bash
   git clone https://github.com/nahataen/docker-wp-nginx-adminer.git
   cd docker-wp-nginx-adminer
