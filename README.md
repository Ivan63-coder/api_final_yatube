# Yatube 
— это платформа для блогов. Возможность зарегистрироваться, создать, отредактировать или удалить собственный пост, прокомментировать пост другого автора и подписаться на него.

# Как запустить проект:
## Клонировать репозиторий и перейти в него в командной строке:

_ _git clone https://github.com/yandex-praktikum/kittygram.git_ _

_ _cd kittygram_ _

## Cоздать и активировать виртуальное окружение:

_ _python -m venv env_ _

_ _source venv/Scripts/activate_ _

## Установить зависимости из файла requirements.txt:

_ _python -m pip install --upgrade pip_ _

_ _pip install -r requirements.txt_ _

## Выполнить миграции:

_ _python3 manage.py migrate_ _

## Запустить проект:

_ _python3 manage.py runserver_ _

# Примеры работы с API:

_ _api/v1/posts/_ _ (GET, POST): получаем список всех постов или создаём новый пост.

_ _api/v1/posts/{post_id}/_ _ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост по id.

_ _api/v1/groups/_ _ (GET): получаем список всех групп.

_ _api/v1/groups/{group_id}/_ _ (GET): получаем информацию о группе по id.

_ _api/v1/posts/{post_id}/comments/_ _ (GET, POST): получаем список всех комментариев поста с id=post_id или создаём новый, указав id поста, который хотим прокомментировать.

_ _api/v1/posts/{post_id}/comments/{comment_id}/_ _ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий по id у поста с id=post_id
