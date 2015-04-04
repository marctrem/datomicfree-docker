FROM dockerfile/java:oracle-java8
MAINTAINER marcandre.tr@gmail.com

RUN ["mkdir", "-p", "/app/datomic-free"]
RUN ["mkdir", "/datomic-data"]

WORKDIR /app/datomic-free

ADD datomic-free/datomic-transactor-free-0.9.5153.jar ./
ADD datomic-free/bin bin/
ADD datomic-free/lib lib/
ADD config.properties ./



CMD ["./bin/transactor", "config.properties"]