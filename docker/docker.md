### Basics

```jsx
//build docker image w/ tag // . is build context
docker build -t <image>:<tag> .

//run docker image on port, with -it specifying interactive mode
docker run -p <exposed port>:<exposed port from container> -it <image>:<tag>

//list docker images
docker images

//list docker containers
docker ps

//remove dangling images and containers
docker image prune
docker container prune

//remove all unused, not just dangling.. add -f to not be prompted for confirmation (force)
docker image prune -a
docker container prune -a

//get bash shell in the container 
docker exec -it <container name> /bin/bash

//execute specified command in the container
docker exec -it <container name> <command>
```