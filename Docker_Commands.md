### List of most widely used Docker Commands.  

 - **docker run < image >** : This command will spin up a container based on the image name provided.  
 - **docker stop < container id >** : This command will stop a running container.  
 - **docker start < container id >** : This command will start the stopped container.  
 - **docker rm** < container id >:  This will remove the stopped container.  
 - **docker images** : This will display the list of available images.  
 - **docker rmi < image name >** : This will remove the image based on the image name provided.  
 - **docker ps** : This will give us list of all the active processes.  
 - **docker ps -a** : This will give us the list of all the active and in-active processes.  
 - **docker attach < container id > :** we can login to the container and the user will be claiming the main process of the container i.e
   when the user logs out of the container , the container exits
   automatically.

  - **docker exec < container id > < process > :** This will allow us to login to the container and run a command.   e.g: *docker exec - it
   ubuntu_sample /bin/bash*


 - **docker inspect < container id > :** This will give us the details of the container in the yaml format.
 - **docker logs < container id >:** This will give us the logs of the container.

## docker run
We can also pass few parameters before running the container.  
How to do the port mapping ?  
Ans: **docker run  -p < host port >:< container port >  --name= < container name > < image name >**  
how to pass environment variables ?  
Ans: **docker run -e < env name > : < env value > < image name>**