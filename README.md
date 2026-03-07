# Agent-T
Agent T is popular TryHackMe Machine which runs on a old version of PHP and you can exploit it with just simple steps

TryhackMe Machines runs on vulnerable system.It allows us to find the structure of a machine like what type of technology it is using and how can we exploit it.

We just have to join the room and then start the Machine:

![Agent T](https://github.com/user-attachments/assets/7b162025-e363-4914-884e-7e0212574b0c)


Once You Start click "Start Machine" then you have to wait for 60 seconds and then you will have your Machine's IP


 Now you have to configure you VPN which you can get from **Manage Account
< VM and VPN Setting**
and then download the Configuration file.
![how to find vpn on try](https://github.com/user-attachments/assets/75205325-6e51-4347-8c06-13e121956619)
![how to find vpn on try1](https://github.com/user-attachments/assets/3849c642-5490-4815-abbe-ed2aba9c3aae)
![how to find vpn on try2](https://github.com/user-attachments/assets/0c3cef80-f90b-4c83-98dd-612fdfb715e5)

Now we have to configure the VPN Properly:

**Lets hack**

The First step is to enumerate the services and technologies our vulnerable machine is using.

For this I will use Nmap.A powerful tool for scanning

I will -A flag for Agressive Scan
command:# sudo nmap -A IP
According to the results.this machine is running only on port 80 which is used for http
and the machine is using this partucular technology "**PHP**" version 

