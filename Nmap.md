---
IP_KALI: 192.168.45.155
IP_TARGET: 192.168.195.172
PORT: "80"
---
Generic:
- ~={green}nmap -A -T4 -p- <span id="IP_TARGET"/>192.168.195.172<span type="end"/>=~

UDP scan:
- ~={green}sudo nmap -sU <span id="IP_TARGET"/>192.168.195.172<span type="end"/>=~

UDP/TCP scan:
- ~={green}sudo nmap -sU -sS <span id="IP_TARGET"/>192.168.202.52
<span type="end"/>=~

Ping sweep:
- ~={yellow}NOTE: Searching for live machines using the grep command on a standard nmap output can be cumbersome. Instead, let's use Nmap's "greppable" output parameter, -oG, to save these results in a more manageable format.=~
- ~={green}nmap -v -sn 192.168.202.1-253 -oG ping-sweep.txt=~

HTTP Headers:
- ~={green}nmap --script http-headers <span id="IP_TARGET"/>192.168.202.52
<span type="end"/>=~

Script help option:
- --script-help \[SCRIPT]

Windows Test-NetConnection:
- ~={cyan}Test-NetConnection -Port <span id="PORT"/>80<span type="end"/> <span id="IP_TARGET"/>192.168.202.52
<span type="end"/>=~
- ~={cyan}1..1024 | % {echo ((New-Object Net.Sockets.TcpClient).Connect("<span id="IP_TARGET"/>192.168.202.52
<span type="end"/>", \$_)) "TCP port \$_ is open"} 2>$null=~