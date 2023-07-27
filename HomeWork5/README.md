HomeWork 5. Docker Compose и Docker Swarm
Создать сервис, состоящий из 2 различных контейнеров: 1 - веб, 2 - БД (compose) Задание со звездочкой - повышенной сложности..
** не обязательно
Необходимо создать 3 сервиса в каждом окружении (dev, prod, lab)
** не обязательно
По итогу на каждой ноде должно быть по 2 работающих контейнера
Выводы зафиксировать
1. Создаем директорию "compose" и переходим в неё:
mkdir compose
cd compose
2. В данной директории создаем файл "compose.yaml" и меняем его содиржимое:
nano compose.yaml

![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork5/1.jpg)

3. Создаем сервис из 2-х контейнеров (web и db)

![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork5/2.jpg)

4. Запускаем Docker Compose:
docker-compose up -d
Проверяем активность контейнера
docker-compose ps

![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork5/3.jpg)