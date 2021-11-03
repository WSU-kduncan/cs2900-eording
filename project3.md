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

1. For docker - dockerfiles are used to build images 

The command: docker build PATH URL

The path is where the container lives or the URL is another thing to insert

if this is coming from somewhere specific. 

How to write this: 

1. From whatever registery you are using

2. Copy from the build directory you are working in (some kind of .txt, .md file)

3. Run the new image that was built from the dockerfile 

Sometimes, running updates is necessary as well for everything to be

build correctly.

2. For podman - must install buildah for images to be created 

To install buildah: sudo apt get install buildah

Using buildah simply replaces docker build commands with buildah bud -t [image name]

3. Again running is the same as docker 

From - whatever application is being used or the original path 

May choose to copy from another file or directory

Run using podman run buildah version  
