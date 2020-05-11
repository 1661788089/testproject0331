FROM openjdk:8-slim

VOLUME /tmp

RUN mkdir -p /data/docker_files

ADD helloworld-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT eval exec "java -Djava.security.egd=file:/dev/./urandom -Dspring.profiles.active=$REGISTRY_PROFILE $OPTS -jar /app.jar"
