### Проект YATUBE_API:

Yatube API - это платформа для блогов, предоставляющая пользователям возможность регистрироваться, создавать, редактировать, удалять собственные посты и комментарии, а также подписываться на других пользователей и отслеживать их публикации.

### Технологии:

Python
SQLite3
Django REST Framework

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram.git
```

```
cd kittygram
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

### Пример запроса и ответа:

Открыть сервис для тестирования API - Postman,в строке ввода ввести:

```
POST http://127.0.0.1:8000/api/v1/posts/
```

Под строкой ввода выбрать разделы Body, Row и тип запроса JSON, а делее в поле ниже ввести:

```
{
    "text": "Hello world!"
}
```

Если все сделано корректно, то в поле ответа должно венуться:

```
{
"id": 0,
"author": "string",
"text": "Hello world!",
"pub_date": "current date",
"image": "string",
"group": 0
}
```

### Документация:

http://127.0.0.1:8000/redoc/

### Автор:
Автор: Nikita Blokhin
GitHub: github.com/bignikkk