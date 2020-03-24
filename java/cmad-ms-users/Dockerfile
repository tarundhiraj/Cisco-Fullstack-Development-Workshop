  FROM maven:3.6.1-jdk-8-slim
  WORKDIR /app
  COPY .  .
  RUN mvn package && \
      mv target/cmad-user-service.jar /run/users.jar && \
      rm -rf /app/*
  EXPOSE 8081
  CMD java  -jar /run/users.jar
