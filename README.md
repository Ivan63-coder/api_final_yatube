# Yatube
— это платформа для блогов. Возможность зарегистрироваться, создать, отредактировать или удалить собственный пост, прокомментировать пост другого автора и подписаться на него.

# Как запустить проект:
## Клонировать репозиторий и перейти в него в командной строке:
_git clone https://github.com/yandex-praktikum/kittygram.git_

_cd kittygram_

## Cоздать и активировать виртуальное окружение:
_python -m venv env_

_source venv/Scripts/activate_

## Установить зависимости из файла requirements.txt:
_python -m pip install --upgrade pip_

_pip install -r requirements.txt_

## Выполнить миграции:
_python3 manage.py migrate_

## Запустить проект:
_python3 manage.py runserver_

# Примеры работы с API:
_api/v1/posts/_ (GET, POST): получаем список всех постов или создаём новый пост.

_api/v1/posts/{post_id}/_ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост по id.

_api/v1/groups/_ (GET): получаем список всех групп.

_api/v1/groups/{group_id}/_ (GET): получаем информацию о группе по id.

_api/v1/posts/{post_id}/comments/_ (GET, POST): получаем список всех комментариев поста с id=post_id или создаём новый, указав id поста, который хотим прокомментировать.

_api/v1/posts/{post_id}/comments/{comment_id}/_ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий по id у поста с id=post_id

# Используемые технологии:
Python 3.9
Django 3.2.20
Django REST Framework 3.12.4
SQLite3

## Об авторе:
профиль на GitHub: https://github.com/Ivan63-coder/
