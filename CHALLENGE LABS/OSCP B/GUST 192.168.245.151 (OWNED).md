# LOOT:
# NMAP:
```
Nmap scan report for 192.168.245.151
Host is up (0.023s latency).
Not shown: 65532 filtered tcp ports (no-response)
PORT     STATE SERVICE          VERSION
80/tcp   open  http             Microsoft IIS httpd 10.0
|_http-title: IIS Windows
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-server-header: Microsoft-IIS/10.0
3389/tcp open  ms-wbt-server    Microsoft Terminal Services
| ssl-cert: Subject: commonName=OSCP
| Not valid before: 2025-02-11T20:59:08
|_Not valid after:  2025-08-13T20:59:08
| rdp-ntlm-info: 
|   Target_Name: OSCP
|   NetBIOS_Domain_Name: OSCP
|   NetBIOS_Computer_Name: OSCP
|   DNS_Domain_Name: OSCP
|   DNS_Computer_Name: OSCP
|   Product_Version: 10.0.19041
|_  System_Time: 2025-02-20T16:32:31+00:00
|_ssl-date: 2025-02-20T16:32:44+00:00; -2s from scanner time.
8021/tcp open  freeswitch-event FreeSWITCH mod_event_socket
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows XP (89%)
OS CPE: cpe:/o:microsoft:windows_xp::sp3
Aggressive OS guesses: Microsoft Windows XP SP3 (89%)
No exact OS matches for host (test conditions non-ideal).
Network Distance: 4 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: mean: -2s, deviation: 0s, median: -2s

TRACEROUTE (using port 3389/tcp)
HOP RTT      ADDRESS
-   Hops 1-3 are the same as for 192.168.245.150
4   23.03 ms 192.168.245.151

Post-scan script results:
| clock-skew: 
|   -2s: 
|     192.168.245.151
|_    192.168.245.147
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Feb 20 11:32:47 2025 -- 4 IP addresses (4 hosts up) scanned in 277.13 seconds
```
# ENUMERATION:
- weird open port not available externally: 
	- TCP    192.168.245.151:56978  172.202.163.200:https  SYN_SENT
- PS history file: C:\Users\chris\AppData\Roaming\Microsoft\Windows\PowerShell\PSReadLine\ConsoleHost_history.txt
- Possible DLL Hijacking folder: C:\Program Files\FreeSWITCH (chris [AllAccess])
- C:\Program Files\Kite(chris [WriteData/CreateFiles])

# COAS:
# LOG:
- Got limited command execution using freeswitch exploit
- Got reverse shell using port 4445 and powershell b64 shell combined with freeswitch exploit
- Got root by using "Unquoted Service Paths" which was really just replacing the KiteService.exe with a reverse shell