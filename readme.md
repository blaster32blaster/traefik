# Docker for local Development

## 1 : Install and configure Docker for your operating system

Navigate to Docker - <https://docs.docker.com/docker-for-windows/install/>

## 2 : Create Docker Networks

    - run command : docker create network traefik_webgateway 
    - run command : docker create network internal 
    - this is to allow the containers to communicate, if this gets removed, recreate it.

## 3 : Clone Docker Traefik Repository

### Clone and start traefik

    - git clone https://github.com/blaster32blaster/traefik
    - cd into Traefik directory
    - docker-compose up / docker-compose up -d

## 4 : Setup Docker for Repositories

    - if docker-compose.yml is missing in root directory, it must be created before docker will work
    - if docker-compose.yml is in place -
      - navigate to repo
      - run command : docker-compose up / docker-compose up -d

## 5 : setup something to resolve host names

    this should work as long as the repositiories are named *.localhost

## 6 : @Todo

    -   add ssl here and to other repos
    -   internal network should not be external
    -   THIS IS VERY MUCH A WIP, the traefik portion works fine for local development, but all the supporting features still need work.  not for production

## Thanks

    - thanks to https://github.com/vegasbrianc for his great work on traefik with prometheus. His hard work gave me a good starting point, allowing for me to adapt his work to traefik 2.0
