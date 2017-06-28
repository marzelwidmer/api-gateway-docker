#FROM frolvlad/alpine-oraclejdk8:slim
#VOLUME /tmp
#ADD api-gateway.jar app.jar
#RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]


# Using rpi image with java 8
FROM hypriot/rpi-java

# Build number hard-coded so far
ADD api-gateway.jar app.jar

EXPOSE 80
CMD ["java", "-jar", "app.jar"]
