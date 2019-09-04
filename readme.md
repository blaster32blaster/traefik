# Docker for local Development

## 1 : Install and configure Docker for Windows

Navigate to Docker - https://docs.docker.com/docker-for-windows/install/

## 2 : Clone Docker Traefik Repository

### Clone and start traefik

    - git clone https://github.com/blaster32blaster/traefik
    - cd into Traefik directory
    - docker-compose up / docker-compose up -d

## 3 : Create Docker Network

    - run command : docker create network traefik_webgateway 
    - this is to allow the containers to communicate, if this gets removed, recreate it.

## 4 : Setup Docker for Repositories

    - if docker-compose.yml is missing in root directory, it must be created before docker will work
    - if docker-compose.yml is in place -
      - navigate to repo
      - run command : docker-compose up / docker-compose up -d

## 5 : setup something to resolve host names

    this should work as long as the repositiories are named *.localhost

## 6 : @Todo

    -   add ssl here and to other repos
    -   work out the Oracle database requirements
