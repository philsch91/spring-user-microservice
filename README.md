# User Microservice

Microservice for Service Engineering

## Build and Run 

1. `mvn package`
2. `docker build -t se/user-service .`
3. `docker tag se/user-service rabbitcarrental.azurecr.io/se/user-service:latest`
4. `docker login rabbitcarrental.azurecr.io`
5. `docker push rabbitcarrental.azurecr.io/se/user-service:latest`
6. `docker logout rabbitcarrental.azurecr.io`
7. `docker run -p 3333:3333 se/user-service`
