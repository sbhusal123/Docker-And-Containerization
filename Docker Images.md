# Docker Image
- Templates used to create Docker Containers.
- Containers are the instances of the image.
- Images are stored in the Registries.(e.g Docker Hub)


## Pull the image:
1. Goto [Public docker registry](https://hub.docker.com/).
2. Search for the required docker image and get the image name, tag.
3. Execute ``docker pull <image_name>:<tag>`` on terminal. **When tag is not provided default/stable image will be pulled**


## Image avanced commands:
- **List of Installed images:** ``docker images`` or ``docker image ls``
- **Image History:** ``docker image history <image_name>``
- **Runing untntu  image in interactive mode:** ``docker run image --name <Arbitart_name> -it <image_name>``
- **inspect the image** ``docker inspect <image_name>``
- **Remove image** ``docker image rm <image_name/id>`` or to **forecfully remove** ``docker image rm -f <image_name/id>``

> Dangling images are the images whose instance doesn't exists.





















