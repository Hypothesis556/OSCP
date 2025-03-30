---
IP_KALI: 192.168.45.155
IP_TARGET: 192.168.122.52
WORDLIST: 
PORT: "80"
---
Using gobuster:
- gobuster dir -u http://<span id="IP_TARGET"/>192.168.122.52<span type="end"/>:<span id="PORT"/>80<span type="end"/>/ -w /usr/share/wordlists/dirb/common.txt -x pdf,txt,html,aspx,php
Feroxbuster:
- feroxbuster --url http://<span id="IP_TARGET"/>192.168.122.52<span type="end"/>/ -x php -w /usr/share/seclists/Discovery/Web-Content/raft-large-files.txt