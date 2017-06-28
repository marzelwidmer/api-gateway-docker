#FROM java:8
#VOLUME /tmp
#ADD api-gateway.jar app.jar
#RUN bash -c 'touch /app.jar'
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]



#FROM frolvlad/alpine-oraclejdk8:slim
#VOLUME /tmp
#ADD api-gateway.jar app.jar
#RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]



#FROM frolvlad/alpine-oraclejdk8:slim
##FROM dockerfile/java:oracle-java8
#MAINTAINER marzelwidmer@gmail.com
#EXPOSE 8080
#VOLUME /tmp
#ADD api-gateway.jar api-gateway.jar
#RUN sh -c 'touch /api-gateway.jar'
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /api-gateway.jar" ]

FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD api-gateway.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
