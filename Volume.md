# Volume

Created: Nov 18, 2020 5:03 PM

Подключение через том. Для того, чтоб у контейнеров была общая связь. 

Тома - директории или файлы, которые существуют отдельно от контейнеров и могут быть подключены к любому из них или к нескольким. 

Том это выделенный жесткий диск. Его можно подключить к любому компьютеру и работать с ним, но при этом он не связан. С конкретной машиной. И продолжает хранить данные даже если выключиться. 

Создание Тома

![Volume%20076e90057be54604ba25a8c097c32998/Untitled.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled.png)

Список всех томов

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%201.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%201.png)

Если docker client and docker deamon находятся на одной машине, то в поле driver будет написано local

Создание контейнера и создание внутри тома файла, при выходе контейнер удаляется

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%202.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%202.png)

Создание другого контейнера и просмотр созданого файла

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%203.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%203.png)

Информация о томах храниться в недрах docker deamon

Физически она присутствует, но работать внутри неё на хост машине не принято. 

Удалить можно том которые не подключен не к одному  контейнеру

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%204.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%204.png)

После удаление контейнеров есть возможность удалить том. 

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%205.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%205.png)

Возможность удалить несколько томов. 

![Volume%20076e90057be54604ba25a8c097c32998/Untitled%206.png](Volume%20076e90057be54604ba25a8c097c32998/Untitled%206.png)