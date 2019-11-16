# Docker 
- Tool designed to make it easier to create, deploy, and run applications by using containers.
- Tool that is designed to benefit both developers and system administrators.
- A part of many DevOps (developers + operations) toolchains.

## 1. Docker: Architecture:
- Follows client server architecture.

![Docker Architecture](https://geekflare.com/wp-content/uploads/2019/09/docker-architecture.png)

### Docker Client:
- User directly interacts with this component by runing commands.
- When commands are executed, client sends them to daemon which carries the proper operation for command executed.
- Uses Docker API.

### Docker Registries:
- Location where the Docker images are stored.
- Can be public docker registry([docker hub](https://hub.docker.com/)) or private docker registry.
- When **pull command** is executed, required docker image is pulled from the configured registry.
- When **push command** is executed, docker image is stored on configured registry.


- 

