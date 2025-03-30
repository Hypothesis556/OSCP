```
Nmap scan report for 172.16.208.21
Host is up (0.015s latency).
Not shown: 65530 filtered tcp ports (no-response)
PORT      STATE SERVICE       VERSION
135/tcp   open  msrpc         Microsoft Windows RPC
139/tcp   open  netbios-ssn?
445/tcp   open  microsoft-ds?
49665/tcp open  unknown
49666/tcp open  tcpwrapped
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port139-TCP:V=7.94SVN%I=7%D=2/6%Time=67A54315%P=x86_64-pc-linux-gnu%r(G
SF:etRequest,5,"\x83\0\0\x01\x8f");
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Aggressive OS guesses: Cisco SG 500 switch (94%), Oki B711 printer (91%), Oki B930 printer (91%), 3Com SuperStack 3 Switch 3870 (91%), Samsung CLP-310N or CLX-3175RW, or Xerox Phaser 6110 printer (90%), Dell PowerEdge 2650 server Embedded Remote Access (ERA) (90%), Dell Remote Access Controller 4 (DRAC 4) (90%), Samsung CLX-3160FN printer (90%), Cisco SF300 or SG300 switch (89%), Cisco SG200 or SG300 switch (89%)
No exact OS matches for host (test conditions non-ideal).
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_nbstat: NetBIOS name: FILES, NetBIOS user: <unknown>, NetBIOS MAC: 00:50:56:86:18:5d (VMware)
|_smb2-time: Protocol negotiation failed (SMB2)
```

Loot:
- unknown:vau!XCKjNQBv2$
- john:YouWillNeverTakeMyTractor!1922
Log:
- Got smb access with mountuser credentials (DRtajyCwcbWvH/9)
Enumeration:
- PowerShell_transcript.FILES.35fvmr5q.20221019013308.txt:
	- Appears to be PS transcript run by admin
	- There is a file on admins desktop called Process Hacker 2.lnk
- PowerShell_transcript.FILES.9_DjDa0f.20221019132304.txt:
	- Found Administrator password: vau!XCKjNQBv2$
- UserExpire - Copy - Copy.ps1:
	- Got password for john