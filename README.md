Spring Cloud configuration server:

Configuration server created and updated with filesystem/git/Vault repository in bootsrap.yml (for Vault created secret wih VaultUI).

Implement URI endpoint to connect licensing service to the configuration service.

Checking multiple API endpoints like HTTP GET http://localhost:8071/licensing-service/dev or GET http://localhost:8071/licensing-service/
default to get properties files details (from configuration server). Endpoint API GET http://localhost:8080/actuator/env to get the configuration information about the service including all properties and endpoints the service is booted with. Using tools like cURL or Postman to check all the API endpoints.

PostgresSQL database installed and configured with password encrypted (bootstrap.yml updated and encryption through endpoint: POST http://localhost:8071/encrypt).

License service updated: created service layer for the REST controller, implemented CRUD interface repository with Spring data JPA. Entities classes updated for tables creation for postgressql database.

