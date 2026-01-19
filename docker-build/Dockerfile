ARG JAVA_VERSION=21
ARG JAVA_DISTRIBUTION=temurin

FROM eclipse-${JAVA_DISTRIBUTION}:${JAVA_VERSION}-jre-alpine

WORKDIR /app

ARG JAR_FILE
COPY ${JAR_FILE} app.jar

ENTRYPOINT ["java", "-jar", "app.jar", "--spring.profiles.active=prod"]
