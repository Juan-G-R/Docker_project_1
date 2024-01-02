
FROM openjdk:21-jdk-slim


WORKDIR /usr/src/app


COPY src ./src


COPY gson-2.10.1.jar ./


RUN javac -d ./out -cp .:gson-2.10.1.jar src/main/*.java src/components/*.java


CMD ["java", "-cp", "./out:gson-2.10.1.jar", "main.Main"]
