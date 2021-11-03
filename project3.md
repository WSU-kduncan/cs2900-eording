## Investigate Available Mounts: 

1. Docker - volume and bind mounts

2. Podman - bind, volume, image, tmpfs, and devpts   

Docker bind: Allows a file or folder to run in a running container to see and

identify changes. 

Docker Volume: Stores data but does not have to be in a specified location. 

Creating Volume: docker volume create (volume_name). This is to persist data. 

Creating Bind: Create a folder and then run the docker program but add -d\.

The preferred method for docker is volume.

Podman bind: podman run -d 

Podman mounts: podman mount [container] 

All mounts have equal importance in podman

## Investigate building images for the container engine  
