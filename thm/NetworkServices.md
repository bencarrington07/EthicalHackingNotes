# Network Services
Target Machine: $IP

## SMB

### Commands Used 
```bash
nmap --script=smb-os-discovery.nse $IP
enum4linux $IP
smbclient //$IP/profiles
mget id_rsa*
chmod 600 id_rsa
```

### Information found
|Port|State|Service|
|---|---|---|
| 22/TCP | open | ssh |
| 139/TCP | open | netbios-ssn |
| 445/TCP | open | microsoft-ds |

OS: Windows 6.1 (Samba 4.7.6-Ubuntu)
Computer Name: POLOSMB

#### Shares
- netlogon: network logon service
- __profiles__: user profiles
- print$
- ipc$

#### Suspected users
POLOSMB/None
POLOSMB/nobody
User/cactus
