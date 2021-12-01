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


### Podman networking modes available 

bridge and firewall 

bridge: a link layer and can forward traffic between networks.

firewall: allows podman to open multiple needed ports automatically  


