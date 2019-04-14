FROM eviles/alpine-oracle-jdk8
VOLUME /tmp
ADD demo2-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]