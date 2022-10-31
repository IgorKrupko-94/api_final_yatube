<<<<<<< HEAD
Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

git clone https://github.com/yandex-praktikum/kittygram.git
cd kittygram
Cоздать и активировать виртуальное окружение:

python3 -m venv env
source env/bin/activate
Установить зависимости из файла requirements.txt:

python3 -m pip install --upgrade pip
pip install -r requirements.txt
Выполнить миграции:

python3 manage.py migrate
Запустить проект:

python3 manage.py runserver
=======
# API_FINAL_YATUBE
##### Данный проект создан для работы с социальной сетью Yatube, где реализованы следующие функции:
- просмотр всех постов
- создание поста
- комментирование постов
- создание подписок на других пользователей

## Запуск проекта в dev-режиме
Клонировать репозиторий и перейти в него в командной строке:

``` git clone git@github.com:IgorKrupko-94/yatube_project.git ```

``` cd api_final_yatube ```

Установите и активируйте виртуальное окружение c учетом версии Python 3.7 (выбираем python не ниже 3.7):

``` py -3.7 -m venv venv ```

``` venv/Scripts/activate ```

``` python -m pip install --upgrade pip ```

Затем нужно установить все зависимости из файла requirements.txt:

``` pip install -r requirements.txt ```

Выполняем миграции:

``` python manage.py migrate ```

Запускаем проект:

``` python manage.py runserver ```

### Примеры работы с API для всех пользователей
###### Для неавторизованных пользователей работа с API доступна в режиме чтения, что-либо изменить или создать не получится.
GET api/v1/posts/ - получить список всех публикаций.
При указании параметров limit и offset выдача должна работать с пагинацией
GET api/v1/posts/{id}/ - получение публикации по id

GET api/v1/groups/ - получение списка доступных сообществ
GET api/v1/groups/{id}/ - получение информации о сообществе по id

GET api/v1/{post_id}/comments/ - получение всех комментариев к публикации
GET api/v1/{post_id}/comments/{id}/ - Получение комментария к публикации по id

#### Все остальные примеры запросов доступны в документации

# Author
## Igor Krupko
>>>>>>> 929676f6e42e5c54a258d67b1cf929ca86663a83
