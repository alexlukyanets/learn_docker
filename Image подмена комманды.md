# Image подмена комманды

Created: Nov 18, 2020 6:34 PM

![Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled.png](Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled.png)

Запуск с коммандой pwd

Контейнер завершил работу потому, что pwd - считается выполненой после того, как docker отобразил путь до текущей дериктории. bash - звершается после того, как мы выходим из сесии командой exit

Когда мы собираем образ, мы можем сделать любую комманду дефолтной. 

Например, хотим создать образ ubuntu так, чтоб дефолтной была комманда pwd. 

docker run -it ubuntu pwd

![Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled%201.png](Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled%201.png)

Стартуем без прописаной комманды

![Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled%202.png](Image%20%D0%BF%D0%BE%D0%B4%D0%BC%D0%B5%D0%BD%D0%B0%20%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B%20a26ba0e302d5429888dce241ca1035f9/Untitled%202.png)

Менять можно не только стартовую комманду, но и директорию с которой начеем рабоать.