# Mount - readonly, программа

Created: Nov 18, 2020 5:18 PM

docker run --rm --mount type=bind,src=/dir_for_bind/,target=/bind/,readonly python python bind/counter.py

![Mount%20-%20readonly,%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%209647d2be09cd49e19e9a39855592b31c/Untitled.png](Mount%20-%20readonly,%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%209647d2be09cd49e19e9a39855592b31c/Untitled.png)

-rm - удалить контейнер после завршения

—mount - подлючаем директорию где лежит программа на python

readoly - не позволит контейнеру изменить содержимое и позволит только читать из неё. 

docker run -it —rm —mount type=volume,src=python_program,target=volume ubuntu bash

echo "for i in range(1,6): print(i)" > ounter.py

cat counter.py

docker run —rm —mount type=volume,src=python_program,target=/src/,readonly pythonpython /src/counter.py

Пример запуска программы с хост машины и тома. 

![Mount%20-%20readonly,%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%209647d2be09cd49e19e9a39855592b31c/Untitled%201.png](Mount%20-%20readonly,%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%209647d2be09cd49e19e9a39855592b31c/Untitled%201.png)