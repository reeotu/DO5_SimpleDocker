## Part 1. Готовый докер

1) Возьми официальный докер-образ с **nginx** и выкачай его при помощи `docker pull`:

![part1](screen/screen.png)

2) Проверь наличие докер-образа через `docker images`:

![part1](screen/screen1.png)

3) Запусти докер-образ через `docker run -d [image_id|repository]`:

![part1](screen/screen2.png)

4) Проверь, что образ запустился через `docker ps`:

![part1](screen/screen3.png)

5) Посмотри информацию о контейнере через `docker inspect [container_id|container_name]`:

Размер контейнера:

![part1](screen/screen4.png)

Список замапленных портов:

![part1](screen/screen5.png)

IP контейнера:

![part1](screen/screen6.png)

6) Останови докер образ через `docker stop [container_id|container_name]`:
   Проверь, что образ остановился через `docker ps`:

![part1](screen/screen7.png)

7) Запусти докер с портами 80 и 443 в контейнере, замапленными на такие же порты на локальной машине, через команду *run*:
   Проверь, что в браузере по адресу *localhost:80* доступна стартовая страница **nginx**:

![part1](screen/screen8.png)

![part1](screen/screen9.png)

8) Перезапусти докер контейнер через `docker restart [container_id|container_name]`:

![part1](screen/screen10.png)

9) Проверь любым способом, что контейнер запустился:

![part1](screen/screen11.png)

## Part 2. Операции с контейнером