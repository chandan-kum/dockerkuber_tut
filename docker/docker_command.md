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

## jenkins container run with mount volume 
 docker run -d --name=jenkins --restart=unless-stopped -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock -e TZ=Asia/Kolkata jenkins/jenkins:lts
## only install docker cli in jenkins
 chmod 666 /var/run/docker.sock

curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh

## go into docker container with root user
docker exec -it -u root container id/name /bin/bash

