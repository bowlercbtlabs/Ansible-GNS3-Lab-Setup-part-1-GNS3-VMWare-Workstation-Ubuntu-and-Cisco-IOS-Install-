*******
Step By Step Guide:
*******

1) Download and install VMWare Workstation:

https://www.techspot.com/downloads/1969-vmware-player.html

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/cf63d16c-8c2e-4a42-8c0a-5908c2d9c620)


2) Download and install Ubuntu:

https://ubuntu.com/download/desktop

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/096d8b3c-f2aa-4f50-9732-c323d3e3801e)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/b5cc7614-f3b2-4f82-936d-b6ed9010dd31)

- Add a 2nd interface to the ubuntu server, this will be for the connection inside GNS3:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/4bd830d8-3312-4842-972c-912aeb51f30c)

- power on the Ubuntu Server, run updates and enable the interfaces:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/75b68185-1178-46fa-bbfa-0002f7e4f945)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/5fb41204-e733-4255-91a3-7f6580bfa25b)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/6533a833-d587-473f-83a1-31d619d9c164)


3) Download and install GNS3

https://www.gns3.com/software/download

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/f24983a9-96c7-4d31-97cd-79dee999fcec)


4) Download the Cisco appliance file:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/17765234-e40f-47e4-9b11-8831e789a5d8)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/bb4ca286-e928-4782-985e-b34ca3c59e9c)

https://www.gns3.com/marketplace/featured/cisco-3725


5) Download the Cisco Image:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/579277d4-911b-434a-b529-819b9cc27fd4)


5) Open GNS3 and Create a new project:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/688dbc39-7ef1-4118-bfe5-7e728fc54e2f)


- load the IOS image into GNS3 via 'new template' then select 'install appliance from the GNS3 server':

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/6fa9ee55-3429-4c32-be06-de9421456fa8)

  - from dropdown select the appliance type "router/firewall" etc... then select the model type 
  - click 'install'

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/98675839-52ff-4b65-b1c3-1483c97948f0)


  - then select 'install the device on your local computer'

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/a24a182f-850d-4cc2-865d-44b8aecce22e)

  - then import and select the appropriate version and file and select next

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/dfca6faf-9203-4a99-82c6-0172c8996159)

  - when asked to install the new device select 'yes'

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/8544ffa3-6595-4c70-ba29-9ce71715fae7)

  - you should now see the device added to GNS3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/0f96b214-5ab4-4917-bf81-381f2fc1230e)

  - add the new router into gns3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/6d53cdeb-8774-4b15-a9fd-18cf6156a0e7)


5) Add the Ubuntu device to GNS3:

- Enable the GNS3 VM under Edit > Preferences

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/8f96d797-6f0c-47bb-85df-0663d8ffc17e)

- Select the Ubuntu Server

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/7a8acca7-8567-46b1-8095-f8be4c357583)

- Under VMware Preferences
  - check the 'block network traffic originating from the host OS'
  - click the 'configure' box under vmnet2 to vmnet19 options. this will allow GNS3 to automatically configure the vmnet interfaces

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/c7fb1e94-63d6-4b95-9af1-fee6bc8fa15e)


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
