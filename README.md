# Описание

Проект Yamdb, предназначенный для запуска через Docker. Проект YaMDb собирает отзывы пользователей на произведения. Сами произведения в YaMDb не хранятся, здесь нельзя посмотреть фильм или послушать музыку.

По адресу http://localhost/redoc/ подключена документация. 

## Технологии

1. Python 3.9
2. Django 3.2
3. gunicorn 20.1.0
4. psycopg2-binary 2.9.6

## Как развернуть проект через докер

1. Во время работы Docker'а перейти в директорию, где расположен docker-compose.yaml (.../infra_sp2/infra/docker-compose.yaml)
2. Ввести команду ```docker-compose up```
3. docker-compose exec web python manage.py migrate
4. docker-compose exec web python manage.py createsuperuser
5. docker-compose exec web python manage.py collectstatic --no-input

## Шаблон наполнения env-файла

```
DB_ENGINE=...
DB_NAME=...
POSTGRES_USER=...
POSTGRES_PASSWORD=...
DB_HOST=... 
DB_PORT=...
```

## Автор

[Олег Призов](https://github.com/OlegPrizov)
