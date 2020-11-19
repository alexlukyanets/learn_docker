# Container - attach, detach

Created: Nov 18, 2020 2:12 PM

При запуске контейнеров не обязательно к нему подключаться. 

Чтоб не переходить в контейнер каждый раз при подлкючении существет флаг для комманды Run -d: - detached. Он запускает контейнер, но не пехеодит внутрь него. 

![Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled.png](Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled.png)

Переводит в терминал host машины. 

it - обьедененные ключи 

-i - Позволяет увидеть все, что будет выводить контейнер

-t - Позволяет сделать так, чтоб все команды вводимые с терминала, были восприняты как комманды для контейнера. 

docker container ls

![Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%201.png](Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%201.png)

Для того, чтоб войти в контейнер. 

![Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%202.png](Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%202.png)

Для того, чтоб выйти без остановки контейнера (спец команды нет). 

![Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%203.png](Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%203.png)

docker stop для остановки контейнера. 

Для того, чтоб удалить все оставшиеся контейнеры комманда 

![Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%204.png](Container%20-%20attach,%20detach%20e233c77d577040c09316d820b16f1fe9/Untitled%204.png)

После выполнение выдается список удаленных контейнеров, а также количество освобожденного места. 

Запущенные контейнеры не будут удалены.