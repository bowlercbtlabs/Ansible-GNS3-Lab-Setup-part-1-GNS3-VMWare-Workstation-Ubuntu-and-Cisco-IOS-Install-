*******
Step By Step Guide:
*******

1) Download and install VMWare Workstation:

https://www.techspot.com/downloads/1969-vmware-player.html

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/cf63d16c-8c2e-4a42-8c0a-5908c2d9c620)


2) Download and install Ubuntu:

https://ubuntu.com/download/desktop

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/096d8b3c-f2aa-4f50-9732-c323d3e3801e)

- Open VMware and 'create new virtual machine':

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/868893c4-f7ba-47c2-b395-2270a4b07ef2)

- Point install to the Ubuntu ISO image you downloaded:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/11c42298-f008-468f-bb24-42d504c8a96b)

- Complete the VM wizard:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/9a5f30a8-fbf0-4740-aae2-1d359cd34fa7)

Name the VM and select the install location:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/49336152-7d7d-4958-8b99-214a9adb6663)

Select the default disk options:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/70f4ddd5-3b58-43d3-b56a-13cc2104f5e7)

Click finish:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/efc94da3-dc3a-4391-ad67-44039e54b527)

Once the setup comes up, run through the default settings, then add a user account and computer name shown below:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/3dabedfb-9342-47d6-864b-cc2a1b07e87f)

Installation will begin:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/35e17b50-0e6e-46dc-83e8-f0c70259e55d)

Reboot the Ubuntu server when installation has completed:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/2f01a3df-c250-4db5-b95b-0b22cca293be)

- you should see the new Ubuntu VM inside VMWare, lets go to the settings and add a 2nd interface to the ubuntu server, this will be for the connection inside GNS3:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/cc87a12b-572e-4331-987a-ea0124575df1)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/43a25cb7-c44b-4332-ab25-9bbf3ed9fb3a)


![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/4bd830d8-3312-4842-972c-912aeb51f30c)

- power on the Ubuntu Server, open a terminal connection, login with your credentials you created in previous steps, run system updates and enable the interfaces:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/6a50f9a9-4203-47ca-a177-4670e71068b4)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/75b68185-1178-46fa-bbfa-0002f7e4f945)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/87e3c3ad-765c-4c58-92b7-ccf4276b73cd)


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

- Add the Ubuntu Server to GNS3:

Edit > Preferences > VMWare > VMWare VMs > New

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/7b29db5f-e8c8-455c-9400-324ab04fa83b)

Select the Ubuntu VM and click finish:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/da42bea8-376a-41f4-bd81-d16727be57da)

You will now see the Ubuntu VM inside GNS3:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/bbc9ad45-7d35-46dc-b544-5253b455d12f)

Drag it over to the working area of the project:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/b7fda016-a6d1-451a-8519-8f48b8a91ccb)

Configure the Ubuntu Server to show the 2 interfaces:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/d3fb4823-b9f8-4b12-a795-18127259f9c6)

Click on network tab, select 'allow GNS3 to override non custom vmware adapter and change network adapters to 2:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/ae65235d-27bf-4068-a8e8-2069c29e9976)


6) Add the ethernet switch into GNS3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/527e5711-1d02-4eb5-ad11-4646f1645119)


  - Add the 2nd port on the Ubuntu server to the switch (created in step 3)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/8921e6b4-e6e4-4cff-ab8b-cbf2f49d9f43)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/7ec9d914-4714-4ab1-b883-efe0be08f38b)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/c842cf61-77a1-4af9-a37b-b0ff609701c0)

  - Add the 1st port on the router to the switch

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/c8dd6740-b876-48b6-ba15-5de1413603a9)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/e82f252b-de12-497c-b212-c19d29bd1831)


7) power up the Ubuntu Server

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/ff245f54-722e-4dc5-9fe0-046b3113ceaf)

- The Ubuntu server link will go green in GNS3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/144f03dc-4d16-41ea-945d-6cb34b0a1d7e)



9) power up the Router

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/ee57b4be-fda0-4653-81ad-06b96d8c7ec5)

- The Router link will go green in GNS3

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/5fb4a6e1-7f11-40e9-8735-6ddbcdc094de)

10) Console into the router and assign it an IP address on the same subnet as the Ubuntu Server (192.168.158.0/24)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/f3925433-eb41-4d8a-853f-24c9859509a9)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/f27dcf6b-267e-44f4-8d1c-2fcd450273f8)

- Ping from the router to the ubuntu server (192.168.158.128)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/dcd30e67-d365-46a9-b114-f057c152efe3)

- Ping from the ubuntu server to the router (192.168.158.200)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/d447e599-edcc-4340-bb8a-67cc58809daf)

- We now have reachability between the Ubuntu server and the router

10) Enable SSH on the Routers:


ip domain name bowlercbtlabs
crypto key generate rsa 2048
ip ssh version 2
username steve privilege 15 password 0 password

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/e57d1ef5-857d-4e4a-b793-f869d538448e)


line vty 0 4
 login local
 transport input ssh

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/2830e458-c3e0-4325-8df5-b6babd7af457)


11) Enable SSH on the Ubuntu server and modify the etc/ssh/ssh_config file to allow older version of ssh to work to connect to the Cisco routers:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/b34f77f6-f2cf-4cbd-b436-943150735ccc)

- install VIM:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/100b890b-200a-45e0-a355-2919a55481a2)

vim /etc/ssh/ssh_config (add following lines to end of file):

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/2746139c-8f88-4aa1-a54b-7d2ac976f4a4)

KexAlgorithms diffie-hellman-group1-sha1,curve25519-sha256@libssh.org,ecdh-sha2-nistp256,ecdh-sha2-nistp384,ecdh-sha2-nistp521,diffie-hellman-group-exchange-sha256,diffie-hellman-group14-sha1

HostKeyAlgorithms +ssh-rsa

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/6311bd98-d3b0-4d01-8c16-ae9c866ac022)


12) Try to now ssh (using the username/password created earlier) from Ubuntu server to the router:

ubuntu# ssh steve@192.168.158.200

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/fd06ec59-983d-4d84-8f26-23cc9ea20877)

13) Now add 2 more routers to the GNS3 project, connect them to the switch, power them up, add the ssh configuration and give them IP addresses on the same subnet (192.168.158.0/24)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/0181c1bf-6926-4c78-a502-88540e4da01f)

- Once completed, ping the new routers from the ubuntu server:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/242acc48-a1ba-49fc-9b95-a204f0fc6e7d)

- try to ssh to the new routers:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/e0296b7e-80a7-41d3-bb08-381ea99702bc)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/7b4213ee-d23a-41f7-80d2-9e2e03d5db5b)

- Here is what the final network topology will look like (your subnet may be different):

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/5fe7a8bc-1ca0-47e9-804e-0fad986b58d1)


*** NOTE ***

If at any time you are experiencing high CPU utilization on your computer when adding routers you can manually set the idle-pc timeout value, select the option with the (*) to get the best CPU performance as shown below:

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/a0b6f2ae-e989-47df-9b46-f286c7894d4e)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/615352a3-d9c3-4540-bcb1-b9ed8195f2e1)

![image](https://github.com/bowlercbtlabs/Ansible-GNS3-Lab-Setup-part-1-GNS3-VMWare-Workstation-Ubuntu-and-Cisco-IOS-Install-/assets/120626722/67097b5f-0f1f-4973-85ed-b3254b6928ea)


14) Once we have reachability via ssh we can now start installing and creating ansible playbooks to push to our GNS3 clients, We will do this in Ansible GNS3 Lab Setup part 2
