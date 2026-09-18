### Basic Docker Command

## docker start/stop/status/restart command
systemctl start/stop/status/restart docker

## pull the images in docker
docker run image-name

## view the images in docker
docker images

## view the running container in docker
docker ps

## view the exit container in docker
docker ps -a

## docker run services in detached mode 
docker run -it -d --name=add_the_name image-name

## check running process of container
docker top container-name

## container start/stop/restart/status
docker start/stop/restart/status container-name

## view container logs
docker logs container-name

## view into container
docker exec -it container-name /bin/bash

## copy file from local machine to docker container
docker cp file_address container_name:/container_folder_addess

