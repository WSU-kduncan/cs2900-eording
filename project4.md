## Investigate Container Networking 

### Docker networking modes available

host, none, and bridge 

 host: shares its network with the host machine. It is beneficial for large

containers. 


 none: Does not configure any IP for containers and does not connect to any 
other networks. 


 bridge: this is known as a link layer and can forward traffic between

network segments. It ensures networks cannot communicate with each other.


By default: BRIDGE is used for docker. 

How to run a new network container and bind a host to it: 

Run: sudo docker run 

Example: to pind port 80 to the docker container, the user can run: 

sudo docker run -p 8080:80 

which will bind the container to port 80 when it is ran. 


### Podman networking modes available 

bridge and firewall 

bridge: a link layer and can forward traffic between networks.

firewall: allows podman to open multiple needed ports automatically  

By default: BRIDGE is used for podman

How to run a new network container and bind a host to it:


sudo podman create test-network 

Then, inspect the network 

sudo podman network inspect test-network 

Here, you can make a new network then and run it to BRIDGE, by default.  
