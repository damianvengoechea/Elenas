# Prueba Qa

## Setup

1. Hacer fork de este repositorio en Gitlab
2. clonea el repo forkeado localmente
3. Instala python3
4. Dentro de la carpeta `qaback` crea un entrono python virtual `python3 -m venv .venv`
5. Activa el entorno segun tu sistema operativo
6. Instala las dependencias `pip3 install -r requirements.txt`

### Correr

Corre el servidor con `python manage.py runserver`
Corre las pruebas con `python manage.py test`

## Tarea

La carpeta mysite contiente un projecto python basico.
El file “.gitlab-ci.yml” contiene la specification de GitlabCI que corre las pruebas de django.

Agrega al menos una prueba de la vista `http://127.0.0.1:8000/polls/1/` con una herramienta de prueba end-to-end (Selenium, Cypress etc).

Opcional:
Corre tu prueba como parte de una tarea en gitlabCI.
