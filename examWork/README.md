# Докер контейнеры

- PostgreSQL database
- Django application)
- load balancer

# Струкура проекта

    django-rest-skeleton/
    |---src                                     
    |   |---drs                                 
    |   |   |---settings.py
    |   |   |---urls.py
    |   |   |---wsgi.py
    |   |---files
    |   |   |---tempaltes                       
    |   |   |   |---index.html
    |   |   |---media                           
    |   |   |   |---.gitignore
    |   |   |   |---placeholder.png
    |   |   |   |---README.md
    |   |   |---static
    |   |   |   |---placeholder.png
    |   |   |---README.md
    |   |---manage.py
    |---.gitignore
    |---.dockerignore
    |---Dockerfile
    |---docker-compose.yml
    |---requirements.txt
    |---README.md

# Установка и запуск

## Клонировать репозиторий
git clone https://github.com/AkmaralKakhar/exam_work.git
##Перейти на директорию проекта

cd exam_work

## Запустить докер контейнеры


    docker-compose build

    # 1: run 1 instance of web
    docker-compose up

    # 2:
    docker-compose up --scale web=2
    

## Запустить на локальной машине

    pip install -r requirements.txt
    cd src
    python manage.py runserver

