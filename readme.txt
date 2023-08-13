From python:3.11-slim-buster
Run pip install django
Run django-admin startproject fshm
WORKDIR /fshm
RUN python manage.py migrate
ENTRYPOINT python manage.py runserver 0.0.0.0:8000

