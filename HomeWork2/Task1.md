Задание 1. Запустить контейнер с ubuntu, используя механизм LXC

Создаем контейнер "test1":
lxc-create -n test1 -t ubuntu
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork2/1.jpg)

Контейнер успешно создан, на экране показано сообщение
Запускаем контейнер
lxc-stast -n test1
Заходим в наш контейнер
lxc-attach -n test1
Командой free -m проверяем количество памяти
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork2/2.jpg)