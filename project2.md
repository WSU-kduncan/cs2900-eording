## Container Technologies 

Container Platform 1: Docker

Container Platform 2: Podman 

## How to Install 

Docker: 

1. sudo apt-get install updates (to make sure there are no outgoing updates needed)

2. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

3. echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

4. sudo apt-get install docker.io 

5. Tested docker using sudo docker run hello-world which was a success 

Podman 

1. sudo apt-get -y update

2. apt-get install curl wget gnupg2 -y

3. source /etc/os-release
sh -c "echo 'deb http://download.opensuse.org/repositories/devel:/kubic:/libcontainers:/stable/xUbuntu_${VERSION_ID}/ /' > /etc/apt/sources.list.d/devel:kubic:libcontainers:stable.list"

4. wget -nv https://download.opensuse.org/repositories/devel:kubic:libcontainers:stable/xUbuntu_${VERSION_ID}/Release.key -O- |sudo apt-key add -

5. sudo apt-get update -qq -y

6. sudo apt-get -qq -yes install podman 

7. to verify podman was actually installed, I ran podman --version

## Pulling a Container Image

1. For docker, I did the following command to pull the image 

sudo docker pull hello-world

2. To view the images I have I did the following command: 

sudo docker images 

There I saw my hello-world image and information such as when it was last updated, the size of it etc. 

3. To pull an image in podman I did the following command: 

sudo podman run hello-world 

This then gave me another message from docker 


## Running a container 

1. Definition of running in detached mode: -d = the container will start and run

without the users interaction with the container or image. This is helper to 

users because there is no interaction needed between them and the container. 

They ultimately run on defaults within the container. 

2. Definition of running and entering shell: keeping the STDIN open and allocating sudo 

Running in shell allows commands to be executed in one location and in one script. 


3.Initalizing the container means the minimum processes are being placed on 

the container. Essentially, it is running in "zombie" mode. This ensures

the usual responsibilites are being ran. 

4. Running a container allows the user to control what the container is doing 

and what commands are being run. 

5. The main difference is initializing the container is running it in more of

a dormat mode than actually running the container.  
