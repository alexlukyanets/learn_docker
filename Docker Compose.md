# Docker Compose

Created: Nov 19, 2020 2:39 PM

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled.png)

docker-compose up - для страта сборки образа и запуска контейнера

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%201.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%201.png)

При изменении файлов нужно использовать с ключем —build 

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%202.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%202.png)

Удаляет все контейнеры созданные с ключем docker-compose

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%203.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%203.png)

Удаляет образы, тома, контейнеры созданные compose

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%204.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%204.png)

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%205.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%205.png)

1. Указали проксирования портов
2. Попросили отключить log сервиса в командой строке. Так, как log Selenium Server будет мешать Log - самих тестов. 
3. network_mode - host - для того, чтоб тесты и машины имели общий localhost

docker-compose up --abort-on-container-exit

Закончит работу в том случае когда хотяб один контейнер закончит работу. 

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%206.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%206.png)

Логи для теста

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%207.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%207.png)

Логи selenium server (в .yml меняем на none на local для логов

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%208.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%208.png)

Список контейнеров запущенной коммандой up

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%209.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%209.png)

Какие образы принимали участие в работе

![Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%2010.png](Docker%20Compose%2092de742fc49b4adb81b6c50cf1664ba5/Untitled%2010.png)