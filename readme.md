# How to setup docker for ... 

## Install docker CE, docker compose
- Docker for mac: https://docs.docker.com/docker-for-mac/install/
- Docker for ubuntu: https://docs.docker.com/install/, https://docs.docker.com/compose/install/

## Check docker is already running
```
➜  ~ docker --version
Docker version 18.06.1-ce, build e68fc7a
➜  ~ docker-compose --version
docker-compose version 1.22.0, build f46880f
```

## RUN docker
### Build

```
➜  ~ docker-compose build
```
### Run

```
➜  ~ docker-compose up
```

### Run and build
```
➜  ~ docker-compose up --build
```

### Kill (down)

```
➜  ~ docker-compose down
```

## Access docker container
### Access

```
➜  ~ docker exec -it <container_name> bash
```

### Run command of docker container

```
➜  ~ docker-compose exec <name> <command>
```
ex:

```
➜  ~ docker-compose exec backend php artisan key:generate
```
