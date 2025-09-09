# 🚀 Docker WordPress + Nginx + MariaDB + Adminer

Este proyecto levanta un entorno completo de **WordPress** utilizando **Docker Compose**, ideal para desarrollo local o pruebas rápidas.  

## 📦 Servicios incluidos

- **WordPress (php8.2-fpm)**  
  Ejecuta WordPress con PHP-FPM 8.2. Los archivos del sitio se almacenan en `./wp-data`.  

- **Nginx (stable)**  
  Servidor web que expone WordPress en [http://localhost:8080](http://localhost:8080).  
  Usa la configuración personalizada en `./nginx/default.conf`.  

- **MariaDB (10.6)**  
  Base de datos para WordPress. Los datos se guardan en un volumen persistente `db_data`.  

  - Usuario: ``  
  - Contraseña: ``  
  - Base de datos: ``  
  - Root: ``  

- **Adminer**  
  Herramienta ligera para administrar la base de datos vía web, accesible en [http://localhost:8081](http://localhost:8081).  
  Usa un tema CSS personalizado desde `./adminer-theme/adminer.css`.  

## ▶️ Cómo usarlo

1. Clona este repositorio:  
   ```bash
   git clone https://github.com/nahataen/docker-wp-nginx-adminer.git
   cd docker-wp-nginx-adminer
