FROM registry.cn-hangzhou.aliyuncs.com/dockerhub_mirror/java:1.8-full

WORKDIR /pig-register

ARG JAR_FILE=target/pig-register.jar

COPY ${JAR_FILE} app.jar

EXPOSE 8848

ENV TZ=Asia/Shanghai JAVA_OPTS="-Xms128m -Xmx256m -Djava.security.egd=file:/dev/./urandom"

CMD sleep 30; java $JAVA_OPTS -jar app.jar
