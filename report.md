# lab6-microservices


![Account Service](imagenes/accounts.png "Accounts Service")

![Web Service](imagenes/web.png "Web Service")

Both services are running and registered

![Microservices registered](imagenes/instances.png "Microservices registered")

The service registration service has the two microservices registered

![Second Accounts Service registered](imagenes/account2.png "Second Accounts Service registered")

![Second Accounts Service registered](imagenes/instances2.png "Second Accounts Service registered")

Microservice (port 4444) is also running and registered




### A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?


After killing the account service (port 2222) the web service returns "Refused Connection" because the service at port 2222 is down. After that, it ask the registration service for another account service (port 4444) and works good again.
