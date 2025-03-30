```
2>/dev/null: redirecout error to dev null
ls &                                 # will background the LS command (you'll have a ready prompt) but will show standard output and standard error
ls > /dev/null &                     # will do LS in background showing only standard error
ls > /dev/null 2>&1 &                # will execute the LS command discarding any output        
ls > ls_output.txt &                 # will background LS and store the output in ls_output.txt while error still on video
ls > ls_output.txt 2>ls_error.log &  # will put LS output in ls_output.txt and errors in ls_error.log
ls > ls_output_all.txt 2>&1 &        # will put both LS standard error and standard output to same output_all.txt
```

Find files and directories with certain name:
```
find / -name "[NAME]*" 
```

See which shell you are using:
```
echo "$SHELL"
```

Capture ping requests:
```
sudo tcpdump -i tun0 icmp and icmp[icmptype]=icmp-echo
```

Read doas.conf file:
```
cat /etc/doas.conf
```

Add a user to a group wtih doas permisison:
```
doas usermod -aG groupname username
```

Drop into root shell if you have doas permission:
```
doas csh
```
```
doas /bin/bash
```