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

### Con docker / docker-compose

En la subcarpeta de `qaback`

`docker build --tag prueba .`

`docker run --publish 8000:8000 --name p prueba python manage.py runserver 0.0.0.0:8000`

Para correr cualcuier otro commando, como pruebas:

`docker run --publish 8000:8000 --name p prueba python manage.py test`

## Tarea

La carpeta mysite contiente un projecto python basico.
El file “.gitlab-ci.yml” contiene la specification de GitlabCI que corre las pruebas de django.

Agrega al menos 3 scripts de pruebas de la vista `http://127.0.0.1:8000/polls/1/` con una herramienta de prueba end-to-end (Selenium, Cypress etc).

(Punto opcional). Agrega 1 script de prueba móvil libre (la que quieras)

Opcional:
Corre tu prueba como parte de una tarea en gitlabCI.

```

```
