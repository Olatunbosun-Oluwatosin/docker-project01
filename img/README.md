## Docker Project 

### _Prepping the Server for Docker Installation_ 
![](./1.%20prepping-docker.png)

This is a debian Ubuntu system and the necessary commands to get the server up-to-date for docker installation.
"sudo apt-get update" was initiated.

### _Docker Installation_
![](./2.%20docker-installed.png)
As provided in the project manual, the required command for docker to run was initiated. This can be seen in the image above.

### _Docker initiated_
![](./3.%20docker-installation-active.png)
To confirm that docker is running on the Ubuntu server, command "sudo systemctl status docker" was ran and came back with "Active(running)".

### _Building docker image_
![](./4.%20docker-run-hello-world.png)
The command "docker run hello-world" is a Docker command used to run a container from the "hello-world" image.

### _Build docker image(nginx)_
![](./6.%20docker-run-nginx.png)
"nginx" ia a popular open-source web server software that can be run as a container using docker. With the command "docker run nginx", this pull the latest nginx image from Docker Hub and create a new container from the nginx image.

### _docker images_
![](./7.%20docker-images-available.png)

The command "docker images" lists all the Docker images on my local system as seen in the image above.

### _docker stop command_
![](./8.%20docker-stop-command.png)
The Docker stop command is used to stop a running container.
"docker stop <container_id> or <container_name>". In my case, "docker stop mynginx" was used.

### _docker pull command_
![](./9.%20docker-pull-command.png)
The Docker pull command is used to download a Docker image from a registry(such as Docker Hub) to a local system. As in my case, "docker pull ubuntu" was used.

### _docker search command_
![](./10.%20docker-search-command.png)
The Docker 4search command is used to search for docker images in Docker Hub or other registries.

### _dockerfile_
![](./11.%20dockerfile.png)
A Dockerfile is a text file that contains instructions for building a Docker image. It specifices the bsae image, commands to run, and other settings required to create a Docker image. 

### _html file content_
![](./12.%20index-file-content.png)

At this stage, the local html file was copied to the nginx default public directory. The content of the file is " echo Welcome to Darey.io" as seen in the image above.

### _dockerfile build command_ 
![](./13.%20dockerfile-build-image.png)

This command "_docker build -t dockerfile ._" builds a Docker image from the instructions in the Dockerfile located in the specified context directory.

### _dockerfile run command_
![](./14.%20docker-run-with-dockerfile.png)
This command tells Docker to:
Run a container from the image built
Map port 8080 on the host machine to port 80 in the container.

### _docker container_
![](./15.%20docker-container-started.png)
The command _"docker ps -a"_ is used to list both running containers and non-running containers while _"docker start container-id"_ is used to start a container.

### _Homepage_
![](./16.%20page-with-content.png)
The content of the page from the html file which is to _"echo Welcome to Darey.io"_.


### _docker push_
![](./17.%20docker-login-push-command.png)
To log in to Docker with the username tosyeno as seen in the image above, the following command was used "docker login -u tosyeno" and followed by the Password prompt. 
Then "docker push tosyeno/my-nginx:1.0" command is used to push the image to the Docker Hub rePository under the above account. 

### _docker hub_
![](./18.%20image-dockerhub-repo.png)
The image was successfully push to Docker Hub repository and this can be seen in the image above.

Thank you
