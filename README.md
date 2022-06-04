# project-microservice-eureka

````
1.Create jar file
mvn clean install -Dmaven.test.skip

2.Run app with mvn
mvn spring-boot:run

3.Create docker image
docker build . -t mini2/eureka

4.Docker run
docker run --network=backend -p 8761:8761 mini2/eureka

5. Push images to docker hub
docker login

docker tag mini2/eureka:latest subo8/mini2-eureka:latest
docker push subo8/mini2-eureka:latest
````