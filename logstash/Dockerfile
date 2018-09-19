

# https://github.com/elastic/logstash-docker

FROM docker.elastic.co/logstash/logstash:6.3.1

RUN logstash-plugin install logstash-input-jdbc
RUN logstash-plugin install logstash-filter-aggregate
RUN logstash-plugin install logstash-output-elasticsearch

RUN rm -f /usr/share/logstash/pipeline/logstash.conf
ADD pipeline/ /usr/share/logstash/pipeline/

#USER root
#COPY mysql-connector-java-5.1.44-bin.jar /
#COPY migrate_db.conf/

CMD ["-f", "/usr/share/logstash/pipeline/logstash.conf"]


