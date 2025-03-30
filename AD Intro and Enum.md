- LegmanTeamBenzoin!!
- LDAP path prototype:
	```
	LDAP://HostName[:PortNumber][/DistinguishedName]
	```
- The _Hostname_ can be a computer name, IP address or a domain name
- The primary domain contrller is the DC that holds the most updated information and this is the DC that should be used in the query
- To find the PDC, we need to find the DC holding the [[PdcRoleOwner]] property
- The [[Distinguished Name]] (DN) is a name that uniquely identifies an object in AD, including the domain itself (e.g. CN=Stephanie,CN=Users,DC=corp,DC=com)
- The [[Common Name]] (CN) specifies the identifier of an object in the domain
- [[Domain Component]] represents the top of an LDAP tree and in this case we refer to it as the Distinguished Name of the domain itself
- A script to get the PdcRoleOwnder propery:
```
function LDAPSearch {
    param (
        [string]$LDAPQuery
    )

    $PDC = [System.DirectoryServices.ActiveDirectory.Domain]::GetCurrentDomain().PdcRoleOwner.Name
    $DistinguishedName = ([adsi]'').distinguishedName

    $DirectoryEntry = New-Object System.DirectoryServices.DirectoryEntry("LDAP://$PDC/$DistinguishedName")

    $DirectorySearcher = New-Object System.DirectoryServices.DirectorySearcher($DirectoryEntry, $LDAPQuery)

    return $DirectorySearcher.FindAll()

}
```

- Bypass execution policy
```
powershell -ep bypass
```

- Import function
```
Import-Module .\function.ps1
```
- [[SAM-Account-Type]] attribute
	- This attribute contains information about every account type object (e.g. SAM_NORMAL_USER_ACCOUNT 0x30000000)
- To enumerate every group available in the domain and also display the user members, we can pipe the output into a new variable and use a foreach loop that will print each property for a group. This allows us to select specific attributes we are interested in.
```
foreach ($group in $(LDAPSearch -LDAPQuery "(objectCategory=group)")) {
$group.properties | select {$_.cn}, {$_.member}
}
```

```
$dirsearcher = New-Object System.DirectoryServices.DirectorySearcher($direntry)
$dirsearcher.filter="name=michelle"
$result = $dirsearcher.FindAll()

Foreach($obj in $result)
{
    Foreach($prop in $obj.Properties)
    {
        $prop
    }

    Write-Host "-------------------------------"
}
```
