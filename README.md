# Dockerfile для сборки PostgreSQL, адаптированного для 1С.


Версия PG: 9.6.10 

Сделано на основе замечательных [docker-postgresql](https://hub.docker.com/r/rsyuzyov/docker-postgresql-pro-1c/)

# Использование
Под linux (bash):
```bash
docker volume create --name pg-data
docker volume create --name pg-run
docker run --name postgresql --restart always \
 -v pg-data:/var/lib/postgresql -v pg-run:/run/postgresql \
 -d savilovoa/docker-postgresql-pro-1c
```

Подключение:
- сервер: сервер или ip, на котором запущен Docker
- порт: 5432
- пользователь: postgresql
- пароль: пустой


# Ссылки

