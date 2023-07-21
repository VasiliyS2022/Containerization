HomeWork 4. Dockerfile и слои
Задание: необходимо создать Dockerfile, основанный на любом образе (вы в праве выбрать самостоятельно). В него необходимо поместить приложение, написанное на любом известном вам языке программирования (Python, Java, C, С#, C++). При запуске контейнера должно запускаться самостоятельно написанное приложение.
1. Создаем директорию "dockerfiles_hw_4"
mkdir dockerfiles_hw_4
2. В данной директории создаем файл "Task_1" и меняем его содиржимое (в данном случае написана программа на языке Python)
nano Task_1
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork4/1.jpg)
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork4/2.jpg)
3. В данной директории создаем файл "Dockerfile" на основе образа alpine:latest и меняем его содиржимое
nano Dockerfile
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork4/3.jpg)
4. Собираем наш образ под названием "images_task_4" и запускаем контейнер
docker build -t images_task_4 .
docker run -it images_task_4
![](https://github.com/VasiliyS2022/Containerization/blob/master/HomeWork4/4.jpg)
Программа запускается, запрашивает число и выдает результат.