Yatube
— это платформа для блогов. Возможность зарегистрироваться, создать, отредактировать или удалить собственный пост, прокомментировать пост другого автора и подписаться на него.

Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:
_ git clone https://github.com/yandex-praktikum/kittygram.git _

_ cd kittygram _

Cоздать и активировать виртуальное окружение:
_ python -m venv env _

_ source venv/Scripts/activate _

Установить зависимости из файла requirements.txt:
_ python -m pip install --upgrade pip _

_ pip install -r requirements.txt _

Выполнить миграции:
_ python3 manage.py migrate _

Запустить проект:
_ python3 manage.py runserver _

Примеры работы с API:
_ api/v1/posts/ _ (GET, POST): получаем список всех постов или создаём новый пост.

_ api/v1/posts/{post_id}/ _ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост по id.

_ api/v1/groups/ _ (GET): получаем список всех групп.

_ api/v1/groups/{group_id}/ _ (GET): получаем информацию о группе по id.

_ api/v1/posts/{post_id}/comments/ _ (GET, POST): получаем список всех комментариев поста с id=post_id или создаём новый, указав id поста, который хотим прокомментировать.

_ api/v1/posts/{post_id}/comments/{comment_id}/ _ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий по id у поста с id=post_id
