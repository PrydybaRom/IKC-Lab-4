# IKC-Lab-4
Network

Створення ізольованої Docker-мережі
docker network create myapp-net

Запуск контейнера бази даних MySQL
docker run -d \
  --name Mydb \
  --network=myapp-net \
  -e MYSQL_ROOT_PASSWORD=1234 \
  mysql:8

  Встановлення утиліти ping у працюючий контейнер 
  docker exec -it --user root flaskAppNet bash -c "apt-get update && apt-get install -y iputils-ping"

  
