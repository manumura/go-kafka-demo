# go-kafka-example

Thanks to <https://medium.com/swlh/apache-kafka-with-golang-227f9f2eb818>

curl --location --request POST '0.0.0.0:3000/api/v1/comments' \
--header 'Content-Type: application/json' \
--data-raw '{ "text":"nice boy" }'

curl --location --request POST '0.0.0.0:3000/api/v1/comments' \
--header 'Content-Type: application/json' \
--data-raw '{ "text":"keep up the good work" }'

## Kafka

docker compose up

docker exec -it zookeeper bash
./bin/zkCli.sh
create /kafka-manager/mutex ""
create /kafka-manager/mutex/locks ""
create /kafka-manager/mutex/leases ""
