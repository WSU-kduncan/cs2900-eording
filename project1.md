## Part 1 



1. Host OS I chose: Linux - Ubuntu 64bit 

2. Disk Space Reservered: 2G. I am not allowing to expand because I do not want it to take over my actual OS and slow down my system. 

3. I am going to be creating a virtual disk so I have a hard copy of it in my files

4. Not allowing 3D alleration 

5. Guest Additions should be included! It makes it easier! 

I went and downloaded the VirtualBox Guest Additions ISO, went to my storage

 of my whole machine and added it as a disk.

 From there, I went on my actual VM and under devices, I selected "insert cd/disk". It then prompted me to run and install Guest Additions. 

 The ISO package was then installed

 Then, I went to my VM's view settings and enabled full screen mode.

I installed Ubuntu on my VM. I went and downloaded the ISO for it and then once

I open my VM for the first time, it was ready to be installed. If I want it detached

I simply just remove it from my disk in the VM settings.  

 
## Part 2

1. Yes, with the guest additions installed, it is possible to see folders

from guest to host and vice versa. This is achieved by going to devices

in your VM and then selecting shared folders and picking the folders

which you wish to share. 

2. When creating a snapshot, it stored wherever I was when I shut my machine down. 

I was on the login screen when I created the snapshot and when I turned the 

machine back on, it brough me back to the lock screen I left it at. 

When creating a snapshot, it does not take up usually anymore than

100MB, but the more information you are saving, the more Ram it will take.

3. With a template, it is more a copy image of the VM that includes the disks,

virtual devices, and settings. It takes up about 10 GB depending on how big

the VM is and what is all stored.

4. It is possible to share the guest to the outside world through a bridged network. 

That allows the IP address open to anyone, meaning they can access whatever they

want. 


## Part 3 

1. I am going to pick on bridged networking. I configured this by going

to my VM's network settings and going to adapter 2 and enabling bridged 

networking. Because my networks are bridged, I am able to get to the apache

site from my main OS.    
