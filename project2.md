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


