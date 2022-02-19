# Network Services
Target Machine: 10.10.246.182

## SMB

### Commands Used 
```bash
nmap --script=smb-os-discovery.nse 10.10.246.182
enum4linux 10.10.246.182
```

### Information found
|Port|State|Service|
|---|---|---|
| 22/TCP | open | ssh |
| 139/TCP | open | netbios-ssn |
| 445/TCP | open | microsoft-ds |

OS: Windows 6.1 (Samba 4.7.6-Ubuntu)
Computer Name: POLOSMB
