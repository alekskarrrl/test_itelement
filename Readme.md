## Структура каталогов проекта

./dags - каталог для DAG
./data - исходные данные
./postgres/init/init.sql -  ddl для задания, выполняются при инициализации postgres


Dockerfile - образ apache/airflow:2.6.2 + установка openpyxl
docker-compose.yml - сервисы AF + postgres в качестве хранилища

Запуск контейнеров:

`docker-compose up -d`

`docker-compose up airflow-init`


Для работы Дага в AF нужно добавить подключение:

![img.png](img.png)



