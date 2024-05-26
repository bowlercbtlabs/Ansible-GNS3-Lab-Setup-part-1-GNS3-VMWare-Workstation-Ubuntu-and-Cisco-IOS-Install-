*******
Step By Step Guide:
*******

1) Download and install VMWare Workstation:

https://www.techspot.com/downloads/1969-vmware-player.html

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/cf63d16c-8c2e-4a42-8c0a-5908c2d9c620)


2) Download and install Ubuntu:

https://ubuntu.com/download/desktop

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/096d8b3c-f2aa-4f50-9732-c323d3e3801e)

- Add a 2nd interface to the ubuntu server, this will be for the connection inside GNS3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/4bd830d8-3312-4842-972c-912aeb51f30c)


3) Download GNS3

https://www.gns3.com/software/download

- Create a new project

4) Download and install the Cisco Image in GNS3:

https://www.gns3.com/marketplace/featured/cisco-3725

- download the IOS image
- load the IOS image into GNS3 via 'new template' > 
  - then select 'install appliance from the GNS3 server' 
  - from dropdown select the appliance type "router/firewall" etc... then select the model type 
  - click 'install'
  - then select 'install the device on your local computer'
  - then import and select the appropriate version and file and select next
  - when asked to install the new device select 'yes'
  - you should now see the device added to GNS3 
  - add the new router into gns3

5) Add the Ubuntu device to GNS3:

- Enable the GNS3 VM under Edit > Preferences
- Select the Ubuntu Server
- Under VMware Preferences
  - check the 'block network traffic originating from the host OS'
  - click the 'configure' box under vmnet2 to vmnet19 options. this will allow GNS3 to automatically configure the vmnet interfaces

6) Add the switch into GNS3
  - Add the 2nd port on the Ubuntu server to the switch (created in step 3)
  - Add the 1st port on the routers to the switch

7) power up the router/routers and ping between them

8) power up the Ubuntu Server VM inside GNS3 and test ping reachability to the routers

9) Enable SSH on the Routers:

ip domain name bowlercbtlabs
crytpo key generate-rsa 
ip ssh version 2
username steve privilege 15 password 0 password
line vty 0 4
 login local
 transport input ssh

10) Modify the etc/ssh/ssh_config file on the Ubuntu server to allow older version of ssh to work to connect to the Cisco routers:

sudo vi /etc/ssh/ssh_config (add following lines to end of file):

KexAlgorithms diffie-hellman-group1-sha1,curve25519-sha256@libssh.org,ecdh-sha2-nistp256,ecdh-sha2-nistp384,ecdh-sha2-nistp521,diffie-hellman-group-exchange-sha256,diffie-hellman-group14-sha1
HostKeyAlgorithms +ssh-rsa

11) Try to now ssh from Ubuntu server to the routers:

ubuntu# ping 192.168.158.200 
ubuntu# ssh steve@192.168.158.200

12) Once we have reachability via ssh we can now start installing and creating ansible playbooks to push to our GNS3 clients, We will do this in Ansible GNS3 Lab Setup part 2
