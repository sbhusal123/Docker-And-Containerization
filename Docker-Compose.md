# Docker Compose
- Tool for defining and runing multi-container docker applications.
- Uses YAML files to configure services(**docker-compose.yml**)

## Creating docker-compose files

```yml
version: "3"
services:
    web:
      image: nginx
      ports:
      - 9090:80
    database:
      image: redis    
```

#### Description:

1. ``version: 3`` Use docker-compose version 3.  [Docker Compose version Compatibility](https://docs.docker.com/compose/compose-file/)
2. ``services:`` Defines a list of services below the line. 

```yml
  web:
    image: nginx
    ports:
    - 9090:80
```
- *Creates a **service** named **web** by using **image nginx***
- *Map the port **9090** from container to port **80** on host OS.*

```yml
database:
  image: redis
```
*Creates a **service** named database by using **redis** image.*

**Runing docker-compose file:** ``docker-compose up`` or ``docker-compose up -d`` to run in detached mode(in background).

**Stopping app:** ``docker-compose down``

**Scalling services:** ``docker-compose up -d --scale <service-name>:<no_of_instances>``






