### О проекте: 

**Учебный проект для демонстрации запуска компонентов системы (Django, Nginx и Postgresql) в контейнерах с использованием docker-compose.
Так же реализован простой API  возвращающий список фильмов и позволяющий получить информацию об одном фильме.**

**Используемые технологии:**

- django
- uwsgi
- psycopg

### Как развернуть проект:

Склонируйте проект

```
git clone https://github.com/VladimirNagibin/new_admin_panel_sprint_2
```

Перейдите в рабочую папку
```
cd new_admin_panel_sprint_2/docker_compose/simple_project/
```

Создайте файл .env 
```
touch .env
```

Заполните файл .env по шаблону .env.example

Запустите приложение
```
sudo docker compose up
```

После запуска и загрузки тестовых данных админка будет доступна по адресу http://localhost/admin/. 
Логин: admin, пароль: 123123.

### Запросы к API:

- Получение списка всех кинопроизведений - GET запрос на эндпоинт: /api/v1/movies/
- Информация об одном фильме - GET запрос на эндпоинт: /api/v1/movies/{id}

____

**Владимир Нагибин** 

Github: [@VladimirNagibin](https://github.com/VladimirNagibin/)