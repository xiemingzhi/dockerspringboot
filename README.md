# What am I?

Spring Boot project with Docker image.

Install JDK8.
Install Maven.
Build project.

```
cmd
git clone https://github.com/xiemingzhi/dockerspringboot
cd dockerspringboot
mvn package -DskipTests
```

Build docker image.
Run container.

```
open Docker Quickstart Terminal
docker build --build-arg JAR_FILE=target/springangularjsproject-0.0.1-SNAPSHOT.jar -t sample-app .
docker run -p 8080:8080 -t sample-app --name dockerspringboot
```
open browser: http://192.168.99.100:8080/

To stop and remove

```
docker stop dockerspringboot
docker rm dockerspringboot
docker rmi sample-app
```
