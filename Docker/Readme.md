## Docker  
программное обеспечение для автоматизации развёртывания и управления приложениями в среде виртуализации 
на уровне операционной системы; позволяет «упаковать» приложение со всем его окружением и зависимостями в контейнер, 
а также предоставляет среду по управлению контейнерами.  
____  

![](https://github.com/Dv-nn/Python--Cheat-Sheet/blob/main/Docker/img/Docker%20(1).jpg)   

____    
![](https://github.com/Dv-nn/Python--Cheat-Sheet/blob/main/Docker/img/doker1.JPG)   
____  
![](https://github.com/Dv-nn/Python--Cheat-Sheet/blob/main/Docker/img/doker2.JPG)   
____  
![](https://github.com/Dv-nn/Python--Cheat-Sheet/blob/main/Docker/img/изображение_2025-08-19_091904405.png)  
  *Образ (или Docker-образ)* — это шаблон или "слепок", на основе которого создаются контейнеры.   
Он содержит все необходимые компоненты для запуска приложения, включая операционную систему, приложения,   
библиотеки и зависимости. Образ — это как фотография или чертёж, на основе которого можно создать множество контейнеров. 
Образы большинства используемых в it инструментов уже созданы их разработчиками. Лежат они в официальном репозитории Docker по адресу https://hub.docker.com/ 
  *Docker-файл* — это текстовый документ, который содержит инструкции, описывающие, как создать нужный Docker-образ.     
Docker-файл помогает автоматизировать создание образов, описывая весь процесс в виде последовательности шагов.    

____ 
*Шпаргалка по основным командам Docker*  
1. Установка Docker  
docker --version: Проверка установленной версии Docker  
2. Управление образами (Images)  
docker pull <image>: Загрузка образа из Docker Hub (следующий шаг об этом)  
docker buildx build -t <image_name> <path>: Сборка образа из Dockerfile  
docker images: Просмотр списка локально сохраненных образов  
docker rmi <image>: Удаление образа   
docker exec <container id or name> <command> - Выполняет команду в существующем контейнере на докер хосте
 
4. Управление контейнерами  
docker run <options> <image>: Запуск нового контейнера  
docker ps: Просмотр списка запущенных контейнеров  
docker ps -a: Просмотр списка всех контейнеров вообще  
docker stop <container>: Остановка запущенного контейнера  
docker start <container>: Запуск остановленного контейнера  
docker restart <container>: Перезапуск контейнера  
docker rm <container>: Удаление остановленного контейнера
docker run -d <container name> - Запускает контейнер в фоновом режиме    
docker attach <container id or name> - Прикрепляет существующий контейнер к терминалу  
6. Работа с томами (Volumes)  
docker volume create <volume>: Создание тома  
docker volume ls: Просмотр списка томов  
docker volume inspect <volume>: Просмотр деталей тома  
docker volume rm <volume>: Удаление тома  
7. Работа с сетями (Networks)  
docker network create <network>: Создание сети  
docker network ls: Просмотр списка сетей  
docker network inspect <network>: Просмотр деталей сети  
docker network rm <network>: Удаление сети  
8. Полезные команды  
docker exec -it <container> <command>: Выполнение команды в запущенном контейнере  
docker logs <container>: Просмотр логов контейнера  
docker inspect <container_or_image>: Просмотр деталей контейнера или образа  
docker compose up: Запуск всех сервисов, определенных в docker-compose.yml  
docker compose stop: Остановка  всех контейнеров, сетей и томов, созданных docker compose up  
docker compose down: Остановка  всех контейнеров, сетей и томов, созданных docker compose up И УДАЛЕНИЕ ИХ

*Ctrl + C* - Выход из контейнера, если он прикреплён к терминалу    

Docker Hub — центральный публичный реестр Docker, предоставляющий доступ к миллионам готовых образов и возможность публиковать собственные образы  
____  


