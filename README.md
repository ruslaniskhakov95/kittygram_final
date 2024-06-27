#  Проект Kittygram

Приложение для публикации и просмотра фото котят. Требует аутентификации для доступа к функционалу.

## Технологии
- Python 3.9
- Django
- Nginx
- Gunicorn
- Docker

## Развертывание на сервере
- Скачайте/скопируйте файл dcoker-compose.production.yml
- Заполните файл .env (требуются переменные: POSTGRES_USER, POSTGRES_PASSWORD,
POSTGRES_DB, DB_HOST, DB_PORT, SECRET_KEY, HOST_IP, HOST_DOMAIN)
- Настройте внешний nginx на проксирование запросов к домену kittygram на порт 9000 контейнера.
- Создайте Docker compose.