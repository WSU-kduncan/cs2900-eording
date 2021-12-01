## Investigate Container Networking 

# Docker networking modes available

host, none, and bridge 

host: shares its network with the host machine. It is beneficial for large

containers. 


none: Does not configure any IP for containers and does not connect to any other

networks. 


bridge: this is known as a link layer and can forward traffic between

network segments. It ensures networks cannot communicate with each other. 
