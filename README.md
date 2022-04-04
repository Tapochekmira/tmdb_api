# Фильмы с www.themoviedb.org

Скрипт нужен для скачивания информации о фильмах с [сайта](https://www.themoviedb.org/), через его API. Поиска информации о фильме в скаченной БД.

## Полный запуск
- Создать БД из филтмов скачанных с [сайта](https://www.themoviedb.org/), запустив файл make_own_db.py 
- Найти нужный фильма запустив search_in_db.py 


## Файл hello_api_TMDB.py

Проверяет подключение к API [сайта](https://www.themoviedb.org/) через получение бюджета фильма по его номеру зашитому в `movie_number`, в данный момент [фильм](https://www.themoviedb.org/movie/215-saw-ii).

### Как пользоваться
При запуске надо указать ключ API.
```
py hello_api_TMDB.py
API_KEY
```

## Файл tmdb_helpers.py

Содержит вспомогательные функции для работы с API, получает ключ API, делает запросы к API.

### Как пользоваться
Нет исполняемых файлов

## Файл own_db_helpers.py

Содержит функцию для считывания информации из БД. 

### Как пользоваться
Нет исполняемых файлов

## Файл search_in_db.py 

Запрашивает дерикторию БД и фильм для поиска. После чего выполняет поиск фильма в БД. Выводит все фильмы с названием, содержащим введенное название фильма.

### Как пользоваться
При запуске надо указать путь к БД, включа название БД\
```
py search_in_db.py 
PATH_TO_DB
FILM_NAME
```

## Файл make_own_db.py 

Создает базу данных(`.json` файл) из 1000 фильмов скаченных с [сайта](https://www.themoviedb.org/). При помощи API этого [сайта](https://www.themoviedb.org/).

### Как пользоваться
При запуске надо указать ключ API
```
py make_own_db.py 
API_KEY
```

## Файл find_similar.py

Находит в базе данных фильмы по введенному названию. И выдает из них фильмы с лучшим рейтингом. 

### Как пользоваться
При запуске надо указать ключ API
```
py find_similar.py
API_KEY
FILM_NAME
```
