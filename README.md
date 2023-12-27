**# Docker Commands(2)**
1) The Docker run command is used to run a Docker image in a container
  ->cmd: sodo docker run image_name
   it first finds if an image is present locally if not it pulls the image and runs
   this command is run image but it exited immediately
   to log in to the container use
  ->cmd; sudo docker run -it image_name bash
2) to ckeck os details
   ->cmd: cat /etc/*release*
3) Docker ps command
    docker ps command is used to show running docker containers
     ->cmd: docker ps
    to see all the running containers that are exited and running use
    ->cmd: docker ps -a
4)to run containers for a particular time and to run them in the background use
    ->cmd: docker run -d image_name sleep (time)
5) to kill or stop the docker container
   ->cmd: docker stop [name_of_container/container_id]
6) to clean all the containers
   ->cmd: docker rm [cotainer_id/containr_name]
   Node: no need to provide full container ID or name just need to pass a few  starting letters        
         we can pass multiple IDs or names to remove multiple containers
7) to see the images that we currently have
   ->cmd: docker images
   to remove images use rmi cmd
   ->cmd: docker rmi image_name 
   Note: if the image is running in another container then it can not be removed at the time, we need to stop the container and then we can remove the image
8) if we want just pull the image instead of pulling and running immediately use pull cmd(it pulls the image and stores it in the local system)
   ->cmd: docker pull image_name
9) to run a command inside the running container
    ->cmd: docker exec image_name [commnads]
     eg: docker run centos cat /etc/*release*

#**Docker run(3)**  
1) docker run tag
   if we want to run a container with the specific version the use tag
   ->cmd: docker run ImageName:[version]
   
