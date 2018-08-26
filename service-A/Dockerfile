FROM java:8-jdk

FROM index.alauda.cn/demo100/piggyjava 
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/service-a.jar /app/
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app/service-a.jar", "--spring.profiles.active=docker"]

EXPOSE 8080
