
[![Lint](https://github.com/nichegosebe/test/workflows/lint/badge.svg)](https://github.com/nichegosebe/test/actions)

# Carprice test app

## Установка

`yarn install`

## Запуск

`yarn dev`

## Запуск отдельно api и web-server

`yarn dev:api` запуск локального сервера на localhost:3000

`yarn dev:web` запуск dev сервера webpack на localhost:8080

## Методы API

GET: `/api/filterAuctions?search=''` возвращает список аукционов, отфильтрованных по get-параметру `search`

GET: `/api/auction/:auctionId` возвращает информацию об отдельном аукционе, дополненную пробегом авто

## Настройка

Конфигурация приложени задается переменными в файле ./client/builder/env/dev.json

Внутри приложения переменные доступны через `process.env.CONFIG`

`IMAGES_BASEPATH` путь к локальному серверу с изображениями

`API_BASEPATH` путь к api endpoints

`POLLING_INTERVAL` интервал по умолчанию для запросов (20сек)

## UI kit

В проекте подключен и преднастроен [material-ui](https://mui.com/), будет большим плюсом, если он будет использован. 
