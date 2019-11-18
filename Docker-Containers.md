# Docker container
- Running instances of the docker image.
- [Readmore ....](https://github.com/sbhusal123/Docker-And-Containerization/blob/master/Introduction%20to%20Virtualization%20and%20Containerization%20.md#ii-container)

# Lifecycle Of Docker Container
![COntainer Life cycle](https://github.com/sbhusal123/Docker-And-Containerization/blob/master/images/IMG_20191117_143259.jpg?raw=true)

# Container Commands

## Create a container from an image:
- Create a container out of an image:``docker run <image_name>``
    - Name of the container is provided by default.
- Creating a container with specific name: ``docker run --name <name>``
- **Create container with specific name run in interactive mode:** ``docker run -it --name <container_name> <image_name>``

## List of containers:
- ``docker ps``  runing containers.
- ``docker ps -a`` list of all containers and their status(stopped, running, paused,...)

## Stopping, Starting containers:
- **Stop containers:** ``docker stop <container_id/name>``
- **Start container:** ``docker stop <container_id/name>``

## Additional Commands:
**Status Of Container:**(cpu,m/m usage) ``docker stats <container>``

**Attach terminal to container:** ``docker attach <container>``. Before attaching container must be runing/started.

**Remove container:** ``docker rm <container_name>``
















