# YaCut

Сервис для укорачивания ссылок.

## Используемые технологии

- Python
- Flask
- SQLAlchemy

## Ключевые возможности

- Генерация коротких ссылок и связь их с исходными ссылками
- Переадресация на исходный адрес при обращении к коротким ссылкам

## API проекта

- /api/id/ - POST-запрос на создание короткой ссылки

```
{
  "url": "string",
  "custom_id": "string"
}
```

- /api/id/<short_id/ - GET-запрос на получение оригинальной ссылки по указанному идентификатору

```
{
  "url": "string"
}
```


### Порядок запуска

Клонировать репозиторий и перейти в него в командной строке:

```
git clone 
```

```
cd yacut
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

* Если у вас Linux/MacOS

    ```
    source venv/bin/activate
    ```

* Если у вас windows

    ```
    source venv/scripts/activate
    ```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```
