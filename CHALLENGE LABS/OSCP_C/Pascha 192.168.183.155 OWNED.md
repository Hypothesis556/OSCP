# LOOT:
# NMAP:
```
Nmap scan report for 192.168.183.155
Host is up (0.023s latency).
Not shown: 65531 filtered tcp ports (no-response)
PORT      STATE SERVICE VERSION
80/tcp    open  http    Microsoft IIS httpd 10.0
|_http-title: IIS Windows
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/10.0
9099/tcp  open  unknown
| fingerprint-strings: 
|   FourOhFourRequest, GetRequest: 
|     HTTP/1.0 200 OK 
|     Server: Mobile Mouse Server 
|     Content-Type: text/html 
|     Content-Length: 321
|_    <HTML><HEAD><TITLE>Success!</TITLE><meta name="viewport" content="width=device-width,user-scalable=no" /></HEAD><BODY BGCOLOR=#000000><br><br><p style="font:12pt arial,geneva,sans-serif; text-align:center; color:green; font-weight:bold;" >The server running on "OSCP" was able to receive your request.</p></BODY></HTML>
9999/tcp  open  abyss?
35913/tcp open  unknown
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port9099-TCP:V=7.94SVN%I=7%D=2/23%Time=67BB3F38%P=x86_64-pc-linux-gnu%r
SF:(GetRequest,1A2,"HTTP/1\.0\x20200\x20OK\x20\r\nServer:\x20Mobile\x20Mou
SF:se\x20Server\x20\r\nContent-Type:\x20text/html\x20\r\nContent-Length:\x
SF:20321\r\n\r\n<HTML><HEAD><TITLE>Success!</TITLE><meta\x20name=\"viewpor
SF:t\"\x20content=\"width=device-width,user-scalable=no\"\x20/></HEAD><BOD
SF:Y\x20BGCOLOR=#000000><br><br><p\x20style=\"font:12pt\x20arial,geneva,sa
SF:ns-serif;\x20text-align:center;\x20color:green;\x20font-weight:bold;\"\
SF:x20>The\x20server\x20running\x20on\x20\"OSCP\"\x20was\x20able\x20to\x20
SF:receive\x20your\x20request\.</p></BODY></HTML>\r\n")%r(FourOhFourReques
SF:t,1A2,"HTTP/1\.0\x20200\x20OK\x20\r\nServer:\x20Mobile\x20Mouse\x20Serv
SF:er\x20\r\nContent-Type:\x20text/html\x20\r\nContent-Length:\x20321\r\n\
SF:r\n<HTML><HEAD><TITLE>Success!</TITLE><meta\x20name=\"viewport\"\x20con
SF:tent=\"width=device-width,user-scalable=no\"\x20/></HEAD><BODY\x20BGCOL
SF:OR=#000000><br><br><p\x20style=\"font:12pt\x20arial,geneva,sans-serif;\
SF:x20text-align:center;\x20color:green;\x20font-weight:bold;\"\x20>The\x2
SF:0server\x20running\x20on\x20\"OSCP\"\x20was\x20able\x20to\x20receive\x2
SF:0your\x20request\.</p></BODY></HTML>\r\n");
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows XP (87%)
OS CPE: cpe:/o:microsoft:windows_xp::sp3
Aggressive OS guesses: Microsoft Windows XP SP3 (87%)
No exact OS matches for host (test conditions non-ideal).
Network Distance: 4 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

TRACEROUTE (using port 80/tcp)
HOP RTT      ADDRESS
-   Hops 1-3 are the same as for 192.168.183.156
4   21.71 ms 192.168.183.155
```
# ENUMERATION:
```
YOU CAN MODIFY THIS SERVICE: AllAccess
    File Permissions: Users [WriteData/CreateFiles]
    Possible DLL Hijacking in binary folder: C:\Program Files\MilleGPG5 (Users [WriteData/CreateFiles])
```
```
LOOKS LIKE YOU CAN MODIFY OR START/STOP SOME SERVICE/s:
    GPGOrchestrator: AllAccess
```
```
C:\Program Files\MilleGPG5
```
# COAS:
# LOG:
- Got revshell as tim using https://github.com/blue0x1/mobilemouse-exploit?tab=readme-ov-file
- Got root rev shell by hijacking the service binary for GPGOrchestrator
- 