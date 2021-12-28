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

docker pull postgres
pgadmin4 run docker compose to test the ui


login pgadmin, choose tools->create server
    name: DiscountServer 
click connection 
    hostname: discountdb
    username: admin
    password: admin1234
Under database discountdb, find schemas->public->tables->create table
or using tools->query tool

    create table Coupon(
        ID SERIAL PRIMARY KEY NOT NUll,
        ProductName VARCHAR(24) NOT NULL,
        Description TEXT,
        Amount INT
    );

  Insert into Coupon(ProductName,Description,Amount)  Values('IPhone X','IPhone Discount', 150);
  Insert into Coupon(ProductName,Description,Amount)  Values('Samsung 10','Samsung Discount', 100);

  GRPC issue on creating on asp.net core 6 ->error: lanaguage requeired

  






