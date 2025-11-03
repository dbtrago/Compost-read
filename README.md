<p align="center">
  <a href="https://camporegenerativo.edu.co/imagenes/sponsors/compostometro.png">
    <img src="https://camporegenerativo.edu.co/imagenes/sponsors/compostometro.png" alt="Compost" width="400"/>
  </a>
</p>


<p align="center">
  <a href="https://laravel.com/"><img src="https://img.shields.io/badge/Laravel-12.x-red?style=&logo=laravel" alt="Laravel"></a> <a href="https://www.php.net/"><img src="https://img.shields.io/badge/PHP-8.2-blue?style=&logo=php" alt="PHP"></a> <a href="https://www.mysql.com/"><img src="https://img.shields.io/badge/MySQL-8-orange?style=&logo=mysql" alt="MySQL"></a> <a href="https://getbootstrap.com/"><img src="https://img.shields.io/badge/Bootstrap-5-purple?style=&logo=bootstrap" alt="Bootstrap"></a> <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/TailwindCSS-3.x-teal?style=&logo=tailwindcss" alt="TailwindCSS"></a>
</p>


# 🌱 Compostómetro - Campo Regenerativo

> Plataforma web desarrollada en **Laravel 12** para la **Alianza Sostenibilidad Productiva en el Campo (ASOPROCAM - Quindío)**.  **landing page institucional** y  **calculadora de compostaje** que automatiza el cálculo de mezclas óptimas para cultivos, contribuyendo a la sostenibilidad y regeneración del campo.

🔗 Sitio oficial: [camporegenerativo.edu.co](https://camporegenerativo.edu.co)  
🔗 Proyecto Compostómetro: [camporegenerativo.edu.co/compostometro](https://camporegenerativo.edu.co/compostometro)

---

## 📖 Descripción

Este repositorio contiene dos componentes principales:

### 🌍 Landing page - Campo Regenerativo
Sitio informativo que presenta los objetivos, proyectos, equipo y recursos de la alianza ASOPROCAM - Quindío.  
Incluye secciones como: página principal, proyectos, sobre nosotros, multimedia y contacto.

### 🧮 Compostómetro
Calculadora web que permite a los agricultores generar mezclas de compost óptimas.  

- Evalúa la relación **Carbono/Nitrógeno (C/N)** y genera un puntaje entre **0 y 60**.  
- Rango óptimo: **25 a 35**.  
- Funcionalidades principales: guardar cálculos, exportarlos, marcarlos como favoritos.  
- Panel administrativo con gráficas:
  - Cantidad de cálculos por mes.  
  - Cantidad de kilos procesados por mes.  
- Módulos de gestión (CRUDs): **Materiales, Fincas y Personas**.  

---

## ✨ Características principales

### 🔐 Autenticación y seguridad
- Login de usuarios con validación de credenciales.  
- Recuperación de contraseñas mediante documento de identidad y token enviado por correo.  
- Restauración de contraseña desde el panel de administración.  

### 📦 Módulos principales
- **Materiales**: gestión de insumos (nombre común, nombre científico, valores C/N, tipo).  
- **Fincas**: administración de fincas con ubicación, hectáreas, altitud, propietario y asignación de personal.  
- **Personas**: registro de datos básicos (nombre, cédula, contacto, rol en finca) y creación de claves personalizadas.  
- **Calculadora de compost**: ingreso de ingredientes, cálculo de mezcla, exportación de resultados como imagen, histórico de cálculos y favoritos.  

### 📊 Reportes
- Cálculos realizados por mes.  
- Cantidad de kilos procesados.  

### 💻 Interfaz
- Responsive, compatible con dispositivos móviles y escritorio.  
- Basada en **Bootstrap** y **Tailwind CSS**.  

---

## 🛠️ Tecnologías utilizadas

- **Backend**: Laravel 12 + PHP 8.2  
- **Base de datos**: MySQL 8+  
- **Frontend**: Blade templates, Bootstrap, Tailwind CSS  
- **Autenticación**: Laravel Sanctum  
- **Diseño gráfico**: Corel Draw, GIMP (para edición de imágenes)  

---

## 📋 Modelo relacional

El sistema utiliza un modelo de base de datos en MySQL que incluye tablas para usuarios, fincas, materiales, cálculos históricos y relaciones entre personas y fincas:

<p align="center">
  <a href="https://camporegenerativo.edu.co/Modelo_Relacional_Compostometro.png">
    <img src="https://camporegenerativo.edu.co/Modelo_Relacional_Compostometro.png" alt="Compost" width="400"/>
  </a>
</p>

---

## 📑 Requisitos previos

Para ejecutar y mantener este proyecto se recomienda contar con:

- PHP 8.2+  
- Composer 2.5+  
- MySQL 8+  
- Node.js 18+ (para manejo de assets)  

---

## ⚙️ Instalación y despliegue

Sigue estos pasos para clonar e instalar el sistema desde GitHub:

```bash
# 1. Clonar el repositorio
git clone https://github.com/dbtrago/Compost.git
cd Compost

# 2. Instalar dependencias de PHP con Composer
composer install

# 3. Crear el archivo de entorno
cp .env.example .env

# 4. Configurar conexión a la base de datos en el archivo .env
Ejemplo:
# DB_CONNECTION=mysql
# DB_HOST=127.0.0.1
# DB_PORT=3306
# DB_DATABASE=compostometro
# DB_USERNAME=root
# DB_PASSWORD=secret

# 5. Iniciar el servidor de desarrollo
php artisan serve
```

## 📂 Estructura del proyecto

- `/app` → Lógica principal (modelos, controladores).  
- `/routes` → Definición de rutas (web y API).  
- `/database` → Migraciones y seeders.  
- `/resources` → Vistas Blade, CSS y JS.  
- `/public` → Archivos accesibles públicamente.  
- `/config` → Archivos de configuración del sistema.  

---

## 📚 Manuales de uso

- [Manual de Usuario - Compostómetro (PDF)](https://camporegenerativo.edu.co/Manual_de_usuario.pdf)  
- [Manual del Administrador - Compostómetro (PDF)](https://camporegenerativo.edu.co/Manual_de_administrador.pdf) 

---

## 👥 Autores

Proyecto desarrollado en la **Universidad La Gran Colombia, seccional Armenia**, en el marco de un proyecto de regalías.  

**Autores (orden alfabético):**
- Anderson Fonseca López — sisacademico@ugca.edu.co  
- Daniel Esteban Buitrago Lozano — proyectosddt@ugca.edu.co  
- Fernando Jaime Escobar Botero — fescobar@ugca.edu.co  
- Jonny Andres Restrepo Gallego — soporteredes@ugca.edu.co  
- Juan Diego Rosero Ríos — jrosero@ugca.edu.co  

---

## ⚖️ Licencia y derechos de autor

Este proyecto fue desarrollado como parte de la **Alianza Sostenibilidad Productiva en el Campo (ASOPROCAM - Quindío)**, en convenio con la **Universidad La Gran Colombia** y financiado por el **Sistema General de Regalías (SGR)**, con apoyo de MinCiencias y la Gobernación del Quindío.  

📌 **Todos los derechos reservados** a sus autores y entidades participantes.  
No está permitida su reproducción o distribución sin autorización expresa.  
