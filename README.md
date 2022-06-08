# Spring Boot, Spring Data y RestApi
Minimos requisitos
- Java 11
- Maven 3.3+
- lombok
- Docker CE

Para comenzar
- Si queres utilizar esta aplicacion, clona esta aplicacion https://github.com/bullDeveloper/bull.SpringRestApi.MongoDBEmbebed.git
- Ejecutar en la raiz del proyecto, mvn clean install
- Ejecutar la clase com.bull.springboot.application.Application como una aplicacion java
- El servicio se ejecutara en localhost:8888
- La documentacion de toda la api se encuentra en http://localhost:8888/swagger-ui.html
- Los servicios publicados se encuentran desarrollados en com.bull.springboot.application.controller.ApiRestController

## To run as a container (Docker)
Construir la imagen docker (Situado en el directorio Raiz del proyecto):
```
docker build -f Dockerfile -t docker-spring-boot-api .
```

Run container:
```
docker run -p 8888:8888 docker-spring-boot-api
```
