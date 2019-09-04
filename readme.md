# Docker for local Development

## 1 : Install and configure Docker for Windows

Navigate to Docker - https://docs.docker.com/docker-for-windows/install/

## 2 : Clone Docker Traefik Repository

    ### Clone and start traefik

    - git clone https://github.com/blaster32blaster/traefik
    - cd into Traefik directory
    - docker-compose up / docker-compose up -d

## 3 : Create Docker Network

   run command : docker create network traefik_webgateway - this is to allow the containers to communicate, if this gets removed, recreate it.

## 3 : Setup Docker for Repositories

    navigate to repo, run command : docker-compose up

## 4 : TBA - setup something to resolve host names

    this should work as long as the repositiories are named *.localhost

## 5 : @Todo

    -   add ssl here and to other repos
    -   work out the Oracle database requirements
