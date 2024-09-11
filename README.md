## API для тестового задания для фронтенд-разработчиков

Этот репозиторий содержит сервер с JSON-файлом, играющий роль базы данных.

Вам необходимо создать свою локальную копию и работать с ней через API.

### Как действовать

Склонировать репозиторий

`git clone https://github.com/it-albion/api-for-test-task.git`


Установить зависимости

`npm install`


Запустить сервер

`npm start`

### Пример JSON-файла

```
{
    "patients": [
      {
        "id": "89983486-1342-45b3-a38f-b6cc52439070",
        "name": "Николай",
        "surname": "Скоморохин",
        "patronymic": null,
        "birthday": "2004-10-03",
        "marital_status": null,
        "gender": "MALE",
        "snils": null,
        "reason_no_snils": "-",
        "series_number_policy": "1223 125725",
        "author_id": "6dc89f2a-4c09-4228-950a-2120cc7403d9",
        "date_first_reception": "2023-10-30 15:43:44.109"
      },
      ...
  ]
}
```

### API

Для выполнения задания вам достаточно запрашивать записи, добавлять, обновлять их.

```
GET     /patients          Получить список пациентов
GET     /patient/[id]      Получить пациента по его id
POST    /patient/          Добавить запись о новом пациенте
PUT     /patient/[id]      Обновить запись о существующем пациенте
```

Подробнее о пакете json-server можно узнать [в документации](https://https://github.com/typicode/json-server/).
