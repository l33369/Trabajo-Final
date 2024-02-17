# Trabajo-Final

# Crear un repositorio en GitHub (asegúrate de tener instalado Git y haber iniciado sesión en tu cuenta)
git init

# Agregar todos los archivos al repositorio
git add .

# Realizar el primer commit
git commit -m "Primer commit: Configuración inicial del proyecto Django"

# Crear un repositorio en GitHub (reemplaza 'nombre-repositorio' con el nombre que desees)
# Asegúrate de haber creado un repositorio vacío en GitHub antes de ejecutar este comando
git remote add origin https://github.com/tu-usuario/nombre-repositorio.git

# Enviar el código al repositorio de GitHub
git push -u origin master

# Configurar el entorno virtual para el proyecto Django
python -m venv venv

# Activar el entorno virtual (en Windows)
venv\Scripts\activate

# Instalar Django
pip install django

# Crear un proyecto Django (reemplaza 'nombreproyecto' con el nombre que desees)
django-admin startproject nombreproyecto

# Cambiarse al directorio del proyecto Django
cd nombreproyecto

# Crear una aplicación Django dentro del proyecto (reemplaza 'nombreapp' con el nombre que desees)
python manage.py startapp nombreapp

# Configurar el archivo settings.py para usar SQLite3 como base de datos
# Agrega la siguiente línea a DATABASES en settings.py:
# 'ENGINE': 'django.db.backends.sqlite3',
# 'NAME': BASE_DIR / "db.sqlite3",

# Realizar migraciones
python manage.py makemigrations
python manage.py migrate

# Agregar la aplicación al archivo settings.py
# Agrega 'nombreapp' a la lista de 'INSTALLED_APPS'

# Crear un README.md con las instrucciones para levantar el proyecto en ambiente local

# Crear el archivo .gitignore para ignorar archivos y carpetas innecesarios
# Puedes usar https://www.toptal.com/developers/gitignore y seleccionar Python y Django

# Hacer commit de los cambios
git add .
git commit -m "Configuración inicial del proyecto Django con SQLite3"

# Enviar los cambios al repositorio de GitHub
git push origin master
