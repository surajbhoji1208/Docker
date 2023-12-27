**# Docker Commands(2)**
1) Docker run commond is used to run dockr image in container
  ->cmd: sodo docker run image_name
   it first find if image is present in locally if not ther it pulls the image and run
   this command is run image but it exeted emmediatly
   to log in into container use
  ->cmd; sudo docker run -it image_name bash
2) to ckeck os details
   ->cmd: cat /etc/*release*
3) Docker ps command
    docker ps command is use show runing docker containers
     ->cmd: docker ps
    to see all the ruunnign containers which are exited and running use
    ->cmd: docker ps -a
4)to run containeer for perticular time and to run it in backrounf use
    ->cmd: docker run -d image_name sleep (time)
5) to kill or stop docker container
   ->cmd: docker stop [name_of_container/container_id]
6) to clean all the containers
   ->cmd: docker rm [cotainer_id/containr_name]
   Node: no need to provide full container id or name just need to pass few  starting latters        
         we can pass multiple ids or name to remove multiple containers
7) to see the images that we currently have
   ->cmd: docker images
   to remove images use rmi cmd
   ->cmd: docker rmi image_name 
   Note: if image is running in another container then it can not be removed at time, need to stop the container and then we can remove image
8) if we want just pull the image instead of pull and run immediatlly the use pull cmd(it pull image and stors in local system)
   ->cmd: docker pull image_name
9) to run a command inside running container
    ->cmd: docker exec image_name [commnads]
     eg: docker run centos cat /etc/*release*

#**Docker run(3)**   
