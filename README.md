### API YaMDb

### Описание
Проект YaMDb собирает отзывы пользователей на произведения. Произведения делятся на категории: «Книги», «Фильмы», «Музыка». Список категорий может быть расширен администратором (например, можно добавить категорию «Изобразительное искусство» или «Ювелирка»).

### Технологии
Python 3.7
Django 2.2.16

## **Как запустить проект:**
Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/ArtemWhiter/api_yamdb
cd api_yamdb
```
Cоздать и активировать виртуальное окружение:
```
python3 -m venv env
source env/bin/activate
```
Установить зависимости из файла requirements.txt:
```
python3 -m pip install --upgrade pip
pip install -r requirements.txt
```
Для Win отдельно установить
```
pip install wheel
```


Выполнить миграции:

```
python3 manage.py migrate
```
Запустить проект:
```
python3 manage.py runserver
```


### Примеры запросов API

Получение списка всех категорий [POST]
```
http://127.0.0.1:8000/api/v1/categories/
```

Получение списка всех жанров [POST]
```
http://127.0.0.1:8000/api/v1/genres/
```

Удаление произведения [DELETE]
```
http://127.0.0.1:8000/api/v1/titles/{titles_id}/
```