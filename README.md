# docker_projects

Projects using Docker

## comandos

### crear un contenedor

- docker run hello-world
- docker run -it ubuntu

### crear imagen y agregar un nombre y un comando personalizado

- docker run --it --name alwaysup -d ubuntu tail -f /dev/null

### correr shell

- docker exec -it alwaysup bash

### Inspeccionar id del contenedor

- docker inspect --format '{{.State.Pid}}' alwaysup

### detener contenedor

-docker stop alwaysup

### ver procesos

- docker ps -a

### Inspect container

- docker inspect #id_container || name_container

### delete container

- docker rm name container

#### delete all containers

- docker container prune
