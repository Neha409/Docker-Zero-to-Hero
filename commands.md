# Docker Commands

Some of the most commonly used docker commands are 

### docker images

Lists docker images on the host machine.

### docker build

Builds image from Dockerfile.

### docker run

Runs a Docker container. 

There are many arguments which you can pass to this command for example,

`docker run -d` -> Run container in background and print container ID
`docker run -p` -> Port mapping
docker run -d --name login nginx:latest --give the name of the container
use `docker run --help` to look into more arguments.

### docker ps

Lists running containers on the host machine.
✅ See all containers (running + stopped)
docker ps -a
Look at the STATUS column:

Up ... → running 🟢

Exited (...) → stopped 🔴

Created → never started

### docker stop

Stops running container.

### docker start

Starts a stopped container.

### docker rm

Removes a stopped container.

### docker rmi

Removes an image from the host machine.

### docker pull

Downloads an image from the configured registry.

### docker push

Uploads an image to the configured registry.

### docker exec
docker exec -it <containerNAme> /bin/bash --login to the container

Run a command in a running container.

### docker network

Manage Docker networks such as creating and removing networks, and connecting containers to networks.

docker network create secure-netowrk --create the network

Attach the network to the existing container
docker network connect my_network finace

Removing a network (if needed)
docker network disconnect my_network finace


List the network
docker network ls

### docker inspect 
to get complete info about the container 
docker inspect <containername>

