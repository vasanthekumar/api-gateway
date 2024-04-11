# api-gateway
This is a Api gateway application build with Spring boot.

## Prerequisites
- Java 17 or higher
- Maven 5.7.43

## Dependency
The API gateway application relies on Config Server, Eureka server.

## Configuration
The Api gateway application config server can be configured using boostrap properties.
~`spring.cloud.config.uri`: The config server url eg: http://localhost:8191

The Api gateway application can be configured using properties in the cloud config server.
https://github.com/vasanthekumar/cloud-country-service-config-store.git
~`server.port`: The port number on which the Api gateway listens for incoming requests.
~`eureka.client.register-with-eureka`:Indicates whether the server should register with Eureka server.
~`eureka.client.fetch-registry`: Indicates whether the server should fetch the registry information from Eureka server.
~`spring.cloud.gateway.discovery.locator.enabled`:
~`spring.cloud.gateway.discovery.locator.lower-case-service-id`:

## Running the Application

To run the Config server application locally, follow these steps:

1. Clone this repository to your local machine:
   https://github.com/vasanthekumar/api-gateway.git
2. Navigate to the project directory:
   cd api-gateway
3. Build the application using Maven
   mvn clean install
4. Run the application:
   java -jar api-gateway-0.0.1-SNAPSHOT.jar
5. Access the Config server dashboard in your web browser:
   http://localhost:8083/

