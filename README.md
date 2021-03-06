# API для тестового задания. Фронтенд

Этот репозиторий содержит сервер с JSON-файлом, который играет роль базы данных в [тестовом задании для фронтенд-разработчиков](https://github.com/itrevolution-perm/test-task-frontend).

Вам нужно создать свою локальную копию и работать с ней через API.

## Как работать

Склонировать репозиторий

    git clone https://github.com/itrevolution-perm/json-server-distances.git

Установить зависимости

    npm install

Запустить сервер

    npm start

## Пример JSON-файла

```json
{
  "walking": [
    {
      "id": 1,
      "date": "2019-07-24T09:24:06.364Z",
      "distance": 12500
    },
    {
      "id": 2,
      "date": "2019-07-24T09:25:44.252Z",
      "distance": 7500
    },
    {
      "id": 3,
      "date": "2019-07-24T09:35:06.654Z",
      "distance": 21000
    }
  ]
}
```

## API

Для выполнения задания вам достаточно запрашивать записи, добавлять, обновлять и удалять их.

```
GET     /walking           Получить список прогулок
GET     /walking/[id]      Получить прогулку по ее id
POST    /walking/          Добавить запись о новой прогулке
PUT     /walking/[id]      Обновить запись о существующей прогулке
DELETE  /walking/[id]      Удалить запись о прогулке
```

Подробнее о пакете json-server можно узнать [в документации](https://github.com/typicode/json-server/).
