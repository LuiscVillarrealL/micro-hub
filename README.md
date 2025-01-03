# micro-hub
This project is a multi-service architecture built using Spring Boot and Docker.


## Repositories

- **[api-gateway](https://github.com/LuiscVillarrealL/micro-api-gateway):** The API gateway for routing and authentication. Also contains Observability stack configuration (Prometheus, Grafana, Loki)
- **[product-service](https://github.com/LuiscVillarrealL/micro-product-service):** Manages product data.
- **[order-service](https://github.com/LuiscVillarrealL/order-service):** Handles customer orders and transactions.
- **[notification-service](https://github.com/LuiscVillarrealL/notification-service):** Sends order email notifications to users using kafka.
- **[inventory-service](https://github.com/LuiscVillarrealL/micro-inventory-service):** Saves, checks items in inventory.


## Architecture

Here's an overview of the architecture:

![Architecture Diagram](https://github.com/LuiscVillarrealL/micro-hub/blob/main/Media/Arquitecture.drawio.png)


## General Information
- Resilience4j: Used for implementing circuit breakers to ensure fault tolerance and resilience.
- Spring Web (RestTemplate/WebClient): Handles synchronous REST API calls between microservices.
- Swagger/OpenAPI: Provides API documentation for easier understanding and integration.
- Flyway: Manages database schema creation and version control.
- Keycloak: Handles authentication and authorization across services.
- Grafana: Analytics & monitoring

## TODO
- Add frontend with angular (WIP)
- Add more tests
- Join in kubernetes
- Add checkstyle and sonarlint
- Add instructions to deploy
- More swagger information


