# pymongo-api

## Как запустить

Запускаем mongodb и приложение

```shell
docker compose up -d
```

Инициализируем сервер конфигурации

```shell
./scripts/mongo-confif-init.sh
```

Инициализируем шарды

```shell
./scripts/mongo-shards-init.sh
```

Инициализируем роутер

```shell
./scripts/mongo-router-init.sh
```

Наполняем базу тестовыми данными

```shell
./scripts/mongo-load-test-data.sh
```

## Как проверить

### Если вы запускаете проект на локальной машине

Откройте в браузере http://localhost:8080

### Если вы запускаете проект на предоставленной виртуальной машине

Узнать белый ip виртуальной машины

```shell
curl --silent http://ifconfig.me
```

Откройте в браузере http://<ip виртуальной машины>:8080

## Доступные эндпоинты

Список доступных эндпоинтов, swagger http://<ip виртуальной машины>:8080/docs