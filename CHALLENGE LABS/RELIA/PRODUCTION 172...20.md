```
Nmap scan report for 172.16.201.20
Host is up (0.015s latency).
Not shown: 65533 filtered tcp ports (no-response)
PORT      STATE SERVICE VERSION
22/tcp    open  ssh     OpenSSH 7.9 (FreeBSD 20200214; protocol 2.0)
| ssh-hostkey: 
|   2048 33:4a:77:87:5b:88:f4:f1:f3:bb:75:7b:ec:9e:21:31 (RSA)
|_  256 c8:3a:f1:c9:e1:9c:31:2d:9d:26:df:c7:c5:21:d8:e3 (ECDSA)
33060/tcp open  mysqlx?
| fingerprint-strings: 
|   DNSStatusRequestTCP, LDAPSearchReq, NotesRPC, SSLSessionReq, TLSSessionReq, X11Probe, afp: 
|     Invalid message"
|     HY000
|   LDAPBindReq: 
|     *Parse error unserializing protobuf message"
|     HY000
|   oracle-tns: 
|     Invalid message-frame."
|_    HY000
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing a closed TCP port so results incomplete
No OS matches for host
Service Info: OS: FreeBSD; CPE: cpe:/o:freebsd:freebsd

```
Loot:
- mountuser:DRtajyCwcbWvH/9
Log:
- Able to access via ssh with id_rsa from WK02 but still need password
- Able to ssh in with andrews creds taken from 19
Enumeration:
```
╔══════════╣ Analyzing Keyring Files (limit 70)
drwxr-xr-x  2 root  wheel  512 Dec  6  2018 /usr/ports/security/py-plone.keyring

╔══════════╣ Analyzing SSH Files (limit 70)                                 
-rw-r--r--  1 root  wheel  177 Oct 31  2022 /etc/ssh/ssh_host_ecdsa_key.pub
-rw-r--r--  1 root  wheel  97 Oct 31  2022 /etc/ssh/ssh_host_ed25519_key.pub
-rw-r--r--  1 root  wheel  397 Oct 31  2022 /etc/ssh/ssh_host_rsa_key.pub
-rw-r--r--  1 root  wheel  104 Dec  6  2018 /usr/ports/security/signify/files/openbsd-62-base.pub
-rw-r--r--  1 root  wheel  104 Dec  6  2018 /usr/ports/security/signify/files/openbsd-63-base.pub
-rw-r--r--  1 root  wheel  104 Dec  6  2018 /usr/ports/security/signify/files/openbsd-64-base.pub

╔══════════╣ Backup folders
drwxr-x---  2 root  wheel  512 Dec  6  2018 /var/backups

╔══════════╣ Searching tables inside readable .db/.sql/.sqlite files (limit 100)
Found /etc/login.conf.db: Berkeley DB 1.85 (Hash, version 2, native byte-order)                                                      
Found /etc/mail/aliases.db: regular file, no read permission
Found /etc/pwd.db: Berkeley DB 1.85 (Hash, version 2, big-endian)
Found /etc/spwd.db: regular file, no read permission
Found /var/db/pkg/local.sqlite: SQLite 3.x database, user version 36, last written using SQLite version 3038005
Found /var/db/services.db: Berkeley DB 1.85 (Hash, version 2, native byte-order
```
