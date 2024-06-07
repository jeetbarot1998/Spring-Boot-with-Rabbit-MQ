
## Instructions
1. download Docker Desktop
2. on [DockerHub](https://hub.docker.com/) website, search for "rabbit mq" and check versions, i'm using the version 3.12.10-management
3. In cmd prompt, type the command ```docker pull rabbitmq: 3.12.10-management```
4. Check docker desktop images to see if docker is there.
5. run command in cmd prompt ```docker run --rm -it -p 15672:15672 -p 5672:5672 rabbitmq:3.12.10-management```
  - ***Port 15672 is for the RabbitMQ management website.***
  - ***Port 5672 is used for the RabbitMQ client connections.***

## Sending a POST Request.
http://localhost:8080/api/v1/publish

{
    "id": 1,
    "firstName": "John",
    "lastName": "Doe" 
}

## Architecture
![RabbitMQ Architecture](https://github.com/MarkVeerasingam/rabbitMQ_Tutorial/blob/master/RabbitMQ_Architecture.png)

