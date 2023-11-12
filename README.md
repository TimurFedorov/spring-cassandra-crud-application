docker-compose up

docker ps
docker exec -it {CONTAINER_ID} bash
cqlsh

create keyspace mykeyspace with replication={'class':'SimpleStrategy', 'replication_factor':1};
use mykeyspace;
CREATE TABLE demo1(id int PRIMARY KEY, rate decimal, madeAt date, symbol text);
