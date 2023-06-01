# lab08
1) Создаем директории server и client
2) В директории server создаем файлы: `nano server.cpp` и `nano Dockerfile`
```
docker build
docker ps -  для просмотра активных контейнеров. Находим ID контейнера и копируем
docker inspect <ID_container> - вывод содержимого контейнера. Здесь находим IP_Adress контейнера по типу : "172.17.0.2"
```
3) В директории client создаем файлы: `nano client.cpp` и `nano Dockerfile`
4) Создаем файл docker-compose.yml

`docker-compose build` - сборка docker-compose

`docker-compose up` - запуск контейнера
```
[+] Running 2/2
 ✔ Network tp-lab08_app-network  Created                                   0.0s 
 ✔ Container tp-lab08-server-1   Created                                   0.1s 
 ✔ Container tp-lab08-client-1   Created                                   0.1s 
Attaching to tp-lab08-client-1, tp-lab08-server-1
tp-lab08-server-1  | Server listening on port 1223
```
Для выхода и завершения работы сервера нажать CTRL + C

5) Создаем директорию .github/workflows
6) В ней прописываем CI.yml
```
git add -A
git commit -m "commit"   
git push origin main
```
