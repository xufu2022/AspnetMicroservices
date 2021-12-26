# installation

docker pull mongo
be aware envirnoment settings

docker pull mongoclient/mongoclient
docker run -d -p 3000:3000 mongoclient/mongoclient

http://localhost:3000

docker pull redis
docker run -d -p 6379:6379 --name aspnetrun-redis redis

docker logs -f aspnetrun-redis
docker exec -it aspnetrun-redis /bin/bash

    redis-cli
    ping
    set key value
    get key
    set name mehet
    get name

docker pull portainer/portainer (skip to code directly)

update docker compose and override file, navigate to http://localhost:9000/

