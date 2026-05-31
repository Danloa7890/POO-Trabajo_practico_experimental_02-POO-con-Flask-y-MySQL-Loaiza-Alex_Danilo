# Caso de Estudio POO con Flask y MySQL (sin ORM)

Este proyecto implementa un sistema de gestión de reservas de laboratorios universitarias utilizando una arquitectura en capas con principios SOLID en Python y una base de datos MySQL sin ORM.

## Requisitos
- Python 3.12+ o 3.13
- MySQL Server

## Instrucciones de Instalación y Ejecución

1. **Crear y activar el entorno virtual**:
   ```bash
   py -m venv .venv
   .\.venv\Scripts\activate
   ```
2. **Instalar dependencias**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Configurar el archivo `.env`**:
   Crear un archivo `.env` en la raíz con las credenciales de tu base de datos local:
   ```env
   DB_HOST=localhost
   DB_PORT=3306
   DB_USER=root
   DB_PASSWORD=tu_contraseña
   DB_NAME=local_reservas_db
   FLASK_ENV=development
   ```
4. **Inicializar y Sembrar la Base de Datos**:
   Ejecuta el script de inicialización automática en Python:
   ```bash
   python setup_db.py
   ```
5. **Ejecutar la API REST**:
   ```bash
   python run.py
   ```
6. **Ejecutar pruebas**:
   ```bash
   python test_api.py
   ```
