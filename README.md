# 🚀 Docker WordPress + Nginx + MariaDB + Adminer

![Docker Logo](https://www.docker.com/app/uploads/2023/08/logo-guide-logos-1.svg)

Este proyecto levanta un entorno completo de **WordPress** utilizando **Docker Compose**, ideal para desarrollo local o pruebas rápidas.

##  Contenido de los Servicios

- **WordPress (PHP-FPM 8.2)**  
  Ejecuta WordPress con PHP-FPM 8.2. Los archivos del sitio se guardan en: `./wp-data`.

- **Nginx (stable)**  
  Servidor frontend que expone WordPress en **[http://localhost:8080](http://localhost:8080)**. Usa configuración personalizada (`./nginx/default.conf`).

- **MariaDB (10.6)**  
  Base de datos para WordPress, con datos persistentes en el volumen `db_data`.  

  ⚠️ **Importante**: debes configurar tus propios valores de conexión en el archivo `docker-compose.yml`.  
  Los que vienen son solo de ejemplo:  
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
