# Agent-T
Agent T is popular TryHackMe Machine which runs on a old version of PHP and you can exploit it with just simple steps

TryhackMe Machines runs on vulnerable system.It allows us to find the structure of a machine like what type of technology it is using and how can we exploit it.

We just have to join the room and then start the Machine:

![Agent T](https://github.com/user-attachments/assets/7b162025-e363-4914-884e-7e0212574b0c)

![machine ip](https://github.com/user-attachments/assets/71a07d88-0b80-4912-a8ce-00cf04485683)




Once You Start click "Start Machine" then you have to wait for 60 seconds and then you will have your Machine's IP


 Now you have to configure you VPN which you can get from **Manage Account
< VM and VPN Setting**
and then download the Configuration file.

![how to find vpn on try](https://github.com/user-attachments/assets/75205325-6e51-4347-8c06-13e121956619)

![how to find vpn on try1](https://github.com/user-attachments/assets/3849c642-5490-4815-abbe-ed2aba9c3aae)

![how to find vpn on try2](https://github.com/user-attachments/assets/0c3cef80-f90b-4c83-98dd-612fdfb715e5)





Now we have to configure the VPN Properly:

After Downloading the VPM Configuration file run this command:

<img width="593" height="247" alt="openvpn" src="https://github.com/user-attachments/assets/67031fa5-da15-46e9-980c-ffd8cb5b8dcd" />

 ``sudo openvpn example.ovpn``

**Lets hack**

The First step is to enumerate the services and technologies our vulnerable machine is using.

For this I will use Nmap.A powerful tool for scanning

I will -A flag for Agressive Scan

command:# **sudo nmap -A IP**

According to the results.this machine is running only on port 80

**http://IP** : And this Result occurs

<img width="1918" height="1689" alt="Screenshot 2026-03-07 at 13-01-26 Admin Dashboard" src="https://github.com/user-attachments/assets/52ae1dca-c1de-44c7-ba68-463c1fc3c230" />


which is used for http and the machine is using this partucular technology "**PHP**" version '**PHP 8.1.0-dev**'

Lets check for this particular exploit online

![Exploit](https://github.com/user-attachments/assets/220d757f-8681-4cf1-a971-52a12c2f5439)

Now we have confirmed confirmed that this version is vulnerable so we will use **Exploit-DB** for this attack

If you have not instelled the Exploit-db in the kali so 
**Run** `sudo apt install exploit-db`

**To Use this**

# Usage 

**Searchploit # Version name**

**Run** `searchploit PHP 8.1.0-dev`
<img width="1853" height="780" alt="exploit-db" src="https://github.com/user-attachments/assets/cfd5888a-f51f-4c89-94ab-42fca1c7ac64" />

There are a lot of exploits here but we will use the



