## Описание
- TODO-сервис: Реализует CRUD-операции для списка задач с хранением данных в SQLite
- Сервис сокращения URL: Позволяет создавать короткие ссылки для длинных URL

## Запуск сервисов локально

Для начала скоипровать проект себе на компьютер:
```bash
git clone git@github.com:DorianGrayPicture/mentor_seminar_final_project.git
```

### Запуск Short URL-сервиса

1. Собрать проект (находясь в директории short-url-app):
```bash
docker build -t short-url-app .
```

2. Запустить контейнер:
```bash
docker run -d -p 8000:8000 -v short-url-db:/app/data short-url-app:latest
```

3. Перейти по ссылке:
```url
http://0.0.0.0:8000
```
### Запуск TODO-Сервиса

1. Собрать проект (находясь в директории todo-app):
```bash
docker build -t todo-app .
```

2. Запустить контейнер:
```bash
docker run -d -p 8000:8000 -v todo-db:/app/data todo-appp:latest
```

3. Перейти по ссылке:
```url
http://0.0.0.0:8000
```