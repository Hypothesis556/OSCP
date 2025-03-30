---
IP_KALI: 192.168.45.155
---
Include StrictHostKeyChecking=no fro the "WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!" error:
- ssh alfred@192.168.221.201 -i id_rsa -p 2222 -o StrictHostKeyChecking=no

Set permissions so that key is not too open:
```
chmod 400 dt_key
```
