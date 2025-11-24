# Introduction
Example for Apache Nifi (using auto trails / revisions).

# Installation / test
- Make sure docker service is up and running
- mvn clean package
- Copy to NiFi's lib folder
  docker cp target/nifi-custom-processors-1.0.0-shaded.jar nifi:/opt/nifi/nifi-current/lib/
- Create docker network: docker network create nifi-network
- Run docker compose for database container to be available
  docker-compose up -d or docker restart nifi (if already running)

# ToDo
- Write tests
- Example for problems


