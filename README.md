- docker-compose build
- docker-compose up
- winpty docker exec -it d07f23243261 sh [to navigate an image]
- [Remove all images] docker rm $(docker ps -a -q)
- Create an image ( docker build -t [imagename] . )
- docker build -t logstashtest . [Build image from Dockerfile]

- elasticsearch-2.4.6
- kibana-5.6.10
- logstash-6.3.1

# .env

- ELASTIC_VERSION=2.4.6
- KIBANA_VERSION=5.6.10
- LOGSTASH_VERSION=6.3.1
- ES_JVM_HEAP=1024m