# Модельный CDN

Данный репозиторий содержит описание модельного CDN.

## Сборка и запуск

Для запуска воспользуйтесь `docker-compose`.

Сборка: `docker-compose build`

Запуск: `docker-compose up`

## Архитектура

* 2 веб-сервера, отдающие какие-то файлы (`image1.svg` и `image2.svg`)
* точка выбора на основе геолокации - geoDNS сервер (см. [example.com.json](router/example.com.json))
* 2 клиента, 1 соответствует Европе, 1 Северной Америке (см. адреса в [docker-compose.yml](docker-compose.yml))
