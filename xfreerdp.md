---
IP_KALI: 192.168.45.155
IP_TARGET: 192.168.195.174
USER: dave4
PASSWD: passwords.txt
DOMAIN: oscp.exam
---
xfreerdp +clipboard /d:<span id="DOMAIN"/>oscp.exam<span type="end"/> /u:<span id="USER"/>dave4<span type="end"/> /p:<span id="PASSWD"/>passwords.txt<span type="end"/> /v:<span id="IP_TARGET"/>192.168.195.174<span type="end"/> +drive:/home/kali

Enable RDP:
```
reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server" /v fDenyTSConnections /t REG_DWORD /d 0 /f
```

```
netsh advfirewall firewall set rule group="remote desktop" new enable=Yes
```

```
net localgroup "Remote Desktop Users" Administrator /add
```