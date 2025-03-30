# Loot
- michelle:NotMyPassword0k?
- emma:SomersetVinyl1!
- Old:HabitsAgesEnd123
- SQL:SAPassword_1998


# Overview `
.189 - proof only 
.191 - proof only 
.245 - local and proof 
.246 - local and proof 
.247 - local and proof 
.248 - local and proof 
.249 - local and proof 
.250 - NONE (WINPREP machine) 
.6 - proof only 
.7 - local and proof 
.14 - local and proof 
.15 - local and proof 
.19 - local and proof 
.20 - local and proof 
.21 - proof only 
.30 - proof only

SMB         172.16.208.14   445    WK01
SMB         172.16.208.30   445    WEBBY           
SMB         172.16.208.6    445    DC02             
SMB         172.16.208.21   445    FILES           
SMB         172.16.208.7    445    INTRANET        
SMB         172.16.208.15   445    WK02 
SMB         172.16.208.5    445    MAIL             
SMB         172.16.208.254  445    LOGIN 

AS-REP Roastable Users:
- Michelle:
	- Obtained hash with jims creds

Kerberoastable Users:
- KRBTGT
- IIS_SERVICE:
	```
	$krb5tgs$23$*iis_service$RELIA.COM$relia.com/iis_service*$c4cdd565d32427f23a31d7e5d2fd62d1$658a136dec286889e818fee8d3bb0a31d2a8afa12b164ec3c8b977ea4744c64b3554a02c98a060c6a30a5b7ef78e4100973c11513d2901e306f16d51b4cae6cfad9eb99b71c792eadcaaa9d63da310df3dbcc1bf6ec9500617d6e23096529d50777f3705fe85d98a490c4858fc2b091d0382200eac5eabed933e941a2fedff2f60bb5024489f2a25fad073299f73cb7d4b8d809244440735ce0f0834851d3a21dd4a464cfb64f622b0315c3003f5f59e6784854a7f2e2fc76eb463ed9c75425c3bb548b026298e6c5eb21125fae9330293cb27739750b157538519e93f4c78b4dfeefd0bafad82337ef98f571711d2393c0120a20bb5aa751e9761d8def5d8b6c0ed0852a5b237dbf6178bd6fcbcc2df6079724fa44075da5b996b13916c5acb65499fdf5d7c3d01b5afbd8b558bf177376eaef281622c9dab6f4c7fd87442a8165bf39c25dbfe37e6c2f34b65eb923c48bd2c213224ae6057679e88cea174820026f0b0387d9df0184c45fbba10c23cdbd727e71c5979359236e4055094c187c7d62729a3d171b07d9be9b6389397b4dbf6571c9d453fff51bc1789d555e8737d0189665de2d9fe451a7c1f6e66765011ec9bd55b585666325440309b8e4f7b42a5c2adc78c489f86d775a1b2f46f782294092d27914c0c606462819b4a0f280240bfd82d41bd61dfd87e1510623096d4128b25104987db88f59d159387e72df5e27ffa3baf5ab23dd07f18db5b9c216ec3ee2231a3bedc5bc6146da6f2769e1fed749a3b0185c85b16bef1a304612c6aeea96890d344e026d0664f334c362c0cc1cefe2417248c90f0803753babe7f7197ba910830575a9872bd5aae258a1c3ee70e0e57f9ffc7dee4071a26fcce0836f6bbee45b7eed6ff098ab192f10ec4e0d04299ad3922466b45284ddbf704b3aaeea4147167b0212e52d9575146636b68007600d143b16ae00d2c3641e08dfae5a1e7fbd81f22632639a6450bd1ce0cdaec34b375c451dad9af392a0ddf4aa123991b000f003c53757ccebe5369a4df1123f8c5a66438ec985d09bc07fed35069f52c0d0b75e28edb519dfa76b80d80e2fcfe26c3f8af879bedcd88b81cfd5fa270f2912694ddbb8a803aec1a48c745bbe6c6c3b9ff12dfb38883b7cf2d4b4b92ef2246bf561af89b1ef84164228f09098e38526207c62308a9cce1b6d47d5a4a70aea04f994d5153dd382ebbf3f436f3479b72ca733a6864bbde405c9fc7abb5eafd898348577c5eccb3bfffa615866378bc67902d5b0d9534bbd9000ef44e8e28ce5c0f3bd2d06c02fb899923452df6d45d9557424b3cb56e721702fbdfbfec8ae9ca8226543d351746cb86d85553f849977efd84ce0902be44a064
	```

- Jenny is a member of backup groups and we have the key for the "BACKUP Machine" but both machines with ssh open are asking for a password but the key wont crack and just says there is no password