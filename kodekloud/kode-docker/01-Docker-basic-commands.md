# Basic Docker Features

https://hub.docker.com

## Basic Commands 


```
$docker run nginx: Download and run the container
$docker ps: See the containers running
$docker ps -a See all containeers running and stopped
$docker stop <container-ID> or <container-NAME>: Stop a container
$docker rm <container-NAME>: Remove a container
$docker images: See all images in the local
$docker rmi <image-NAME> :Remove a image: Deleta all dependent containers to remove image :::
$docker pull: Just download the image
$docker inspect <contaner-NAME>: To see more info about containers
$docker logs <container-NAME>: to see logs
$docker run ubuntu sleep 5: Start a linux docker container and sleeps after 5 seconds
$docker exec: Execute a command in a running container
$docker exec <container-NAME> cat /etc/hosts
$docker run kodecloud/simple-webapp: This runs in the attached mode.
$docker run -d kodekloud/simple-webapp: This runs in detacched mode (BACKEND)
$docker attach <container-ID>
docker rmi -f $(docker images -a -q)

```
