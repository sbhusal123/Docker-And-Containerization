# Docker Images
- Images are templates used to create Docker containers.
- Container is a running instance of image.
- Stored in the registries.

# Docker Basic Commands

## i. Basic Commands

| Command | Description |
|-------------------------|------------------------------------------------------------------------------|
| docker -version | shows the client and server version of docker |
| docker -v | Shows the version of docker |
| docker -info  | Shows: - No of images running, paused and stopped - Server Version, e.t.c |
| docker --help | Shows the list of available commands and options  docker [OPTIONS] COMMAND |
| docker [COMMAND] --help | Shows the description of command and available  options and flags. |
| docker login | Allows logging in to docker registry.  Need to create account at docker hub. |


## ii. Images Command:
| Command  | Description |
|----------------------------------|-------------------------------------|
| docker images | Shows the list of all the images.  |
| docker pull <image> | Pulls the <image> from the registry |
| docker rmi <image_name/image_id> | Removes the image.(Not a container) |

## iii. Containers Command:
| Command  | Description |
|------------------------------|------------------------------------------------------------------------------|
| docker ps | Shows the containers. |
| docker run <image/image id> | Runs the container inside the image. |
| docker run -it <image/name>  | Runs the docker container in interactive mode.(only if  terminal is present) |
| docker start <container> | Starts stopped container |
| docker stop <container> | Stops runing container. |
  
## iv. Docker System Command:

| Command  | Description |
|---------------------|-----------------------------------------------------------------|
| docker stats | Display a live stream of container(s) resource usage statistics |
| docker system df | Show docker disk usage |
| docker system prune | Remove unused data. Warning!!! |
