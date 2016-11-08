# Asistentul Cetateanului

## Docker Development environment

### Initial build

To set up the Postgres user password, at first run you need to give the desired password to the compose command as an environment variable
    
    POSTGRES_PASSWORD=mytestpwd ./compose.sh up

### How to use? 

Create and start all docker containers (configured in _docker-compose.yml_)

    ./compose.sh up

Create and start a single docker container (configured in _docker-compose.yml_)

    ./compose.sh up <containername>

Show the logs of a container.

    ./compose.sh logs <containername>

Stop, delete, pull, build or list all containers

    ./compose.sh stop
    ./compose.sh rm
    ./compose.sh pull
    ./compose.sh build
    ./compose.sh ps