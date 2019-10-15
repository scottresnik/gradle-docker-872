FROM openjdk:8-jdk-alpine

ENV SPRING_OUTPUT_ANSI_ENABLED=ALWAYS \
    S_SLEEP=0 \
    JAVA_OPTS=""

CMD echo "The application will start in ${S_SLEEP}s..." && \
    sleep ${S_SLEEP} && \
    java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app.war

ADD *.war /app.war
