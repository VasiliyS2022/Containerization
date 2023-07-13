Задание 2. Ограничить контейнер 256 Мб ОЗУ и проверить, что ограничение работает

Заходим в редактор nano и видим, что ограничений по памяти нет
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork2/3.jpg)

Добавляем в раздел "Conteiner specific configuration" ограничение по пямяти
lxc.cgroup2.memory.max = 256M
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork2/4.jpg)

Проверяем, что ограничение работает
free -m
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork2/5.jpg)