<div id="header" align="center">
  <img src="https://media.giphy.com/media/l41lRVmlnknDV3n9u/giphy.gif" width="100"/>
</div>

## <div align="center"> Api Yatube </div>
API для социальной сети, в которой пользователи могут делать публикации, добавлять к ним изображения, просматривать сообщения других пользователей, комментировать их, подписываться на авторов. Для возможности создания публикаций и комментирования необходима регистрация. Для аутентификации используется JWT-токен.

## Технологии
Python 3.7.9
Django 3.2.16
Django REST Framework 3.12.4
Django REST Framework simplejwt 4.7.2

## Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/mAXxtor/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции из папки проекта:

```
cd yatube_api
```

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```

## Примеры запросов к API:

Получение списка всех постов:
```
GET
http://127.0.0.1:8000/api/v1/posts/
```

Получение списка доступных сообществ:
```
GET
http://127.0.0.1:8000/api/v1/groups/
```

Получение списка комментариев к посту:
```
GET
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```

Получение списка подписок:
```
GET
http://127.0.0.1:8000/api/v1/follow/
```

### Полная документация по Api содержится в [ReDoc](http://127.0.0.1:8000/redoc/).

### Авторы
[Yandex Practicum] и [Максим Вербицкий]

[//]: #

   [Yandex Practicum]: <https://practicum.yandex.ru/>
   [Максим Вербицкий]: <https://www.facebook.com/maks.verbitskii/>
