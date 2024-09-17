# credit-cards-service

The service service is coded in Java and makes use of Controller, Service, Client architecture.
It makes use of WebClient for external api calls.
For deployment I would make use of Kubernetes, with a service such as Rancher as a UI for container.management.

Improvements can be made by making use of global exception handler pattern, creating custom exceptions, and possibly custom messages for a front-end if required. An error Error code (i.e single digit) can be assigned to custom exceptions to group error types into buckets.

Bash script
Format:
.start.sh {port} {base-url} {csCards-endpoint} {scoredCards-endpoint}
e.g:
./start.sh 8080 https://app.clearscore.com/api/global/backend-tech-test /v1/cards /v2/creditcards
