# Tools of the Trade

The Tools used for Attacking AD (Common Ones) And only some of them.

- `PowerView/SharpView:`
    
    <aside>
    💡
    
    Acts as a Tool that is made for AD Recon, it can give us similar Infos to bloodhound. And it can also replace various net* commands.
    
    </aside>
    
    [PowerView:](Tools%20of%20the%20Trade%20152357aeddc080ecb6efd3bc4484f520/PowerView%20166357aeddc08015ac46e48110874580.md)
    
- `Bloodhound` / `.py`
    
    <aside>
    💡
    
    Bloodhound is a GUI Based tool, used to map the AD Enviroment and give a detailed Visualised Image about Domains, Groups, links and relationships between forests, nodes or other groups, including attack vectors.
    
    </aside>
    
    <aside>
    💡
    
    The .py Version is based on the Impacket toolkit.
    
    It supports most Bloodhound utils, can also be run from a non domain joined AttackBox
    
    </aside>
    
- `Sharphound`
    
    <aside>
    💡
    
    Gathers various data about the AD, same thing like Bloodhound but minus the Visualisation aspect.
    
    </aside>
    
- `Responder`
    
    <aside>
    💡
    
    Responder is purpose-built, it is used to poison `LLMNR, NBT-NS and MDNS`
    
    </aside>
    
- `Inveigh.ps1`
    
    <aside>
    💡
    
    Similar to responder, writtein in PS and is used to also perform various network spoofing and poisoning attacks.
    
    </aside>
    
    <aside>
    💡
    
    REST IS SHOWN AS A SLIDESHOW DUE TO AMOUNT:
    
    </aside>
    
    | [C# Inveigh (InveighZero)](https://github.com/Kevin-Robertson/Inveigh/tree/master/Inveigh) | The C# version of Inveigh with a semi-interactive console for interacting with captured data such as username and password hashes. |
    | --- | --- |
    | [rpcinfo](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/rpcinfo) | The rpcinfo utility is used to query the status of an RPC program or enumerate the list of available RPC services on a remote host. The "-p" option is used to specify the target host. For example the command "rpcinfo -p 10.0.0.1" will return a list of all the RPC services available on the remote host, along with their program number, version number, and protocol. Note that this command must be run with sufficient privileges. |
    | [`rpcclient`](https://www.samba.org/samba/docs/current/man-html/rpcclient.1.html) | A part of the Samba suite on Linux distributions that can be used to perform a variety of Active Directory `enumeration tasks via the remote RPC service.` |
    | [`CrackMapExec (CME)`](https://github.com/byt3bl33d3r/CrackMapExec) | CME is an enumeration, attack, and post-exploitation toolkit which can help us greatly in enumeration and performing attacks with the data we gather. CME attempts to `"live off the land" and abuse built-in AD features and protocols like SMB, WMI, WinRM, and MSSQL.` |
    | [Rubeus](https://github.com/GhostPack/Rubeus) | Rubeus is a C# tool built for Kerberos Abuse. |
    | [GetUserSPNs.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/GetUserSPNs.py) | `Another Impacket module geared towards finding Service Principal names tied to normal users.` |
    | [Hashcat](https://hashcat.net/hashcat/) | A great hash cracking and password recovery tool. |
    | [`enum4linux`](https://github.com/CiscoCXSecurity/enum4linux) | A tool for enumerating information from Windows and Samba systems. |
    | [enum4linux-ng](https://github.com/cddmp/enum4linux-ng) | A rework of the original Enum4linux tool that works a bit differently. |
    | [`ldapsearch`](https://linux.die.net/man/1/ldapsearch) | Built-in interface for interacting with the LDAP protocol. |
    | [windapsearch](https://github.com/ropnop/windapsearch) | A Python script used to enumerate AD users, groups, and computers using LDAP queries. Useful for automating custom LDAP queries. |
    | [`DomainPasswordSpray.ps1`](https://github.com/dafthack/DomainPasswordSpray) | `DomainPasswordSpray is a tool written in PowerShell to perform a password spray attack against users of a domain`. |
    | [LAPSToolkit](https://github.com/leoloobeek/LAPSToolkit) | The toolkit includes functions written in PowerShell that leverage PowerView to audit and attack Active Directory environments that have deployed Microsoft's Local Administrator Password Solution (LAPS). |
    | [smbmap](https://github.com/ShawnDEvans/smbmap) | SMB share enumeration across a domain. |
    | [psexec.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/psexec.py) | Part of the Impacket toolkit, it provides us with Psexec-like functionality in the form of a semi-interactive shell. |
    | [wmiexec.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/wmiexec.py) | Part of the Impacket toolkit, it provides the capability of command execution over WMI. |
    | [Snaffler](https://github.com/SnaffCon/Snaffler) | Useful for finding information (such as credentials) in Active Directory on computers with accessible file shares. |
    | [`smbserver.py`](https://github.com/SecureAuthCorp/impacket/blob/master/examples/smbserver.py) | Simple SMB server execution for interaction with Windows hosts. `Easy way to transfer files within a network.` |
    | [setspn.exe](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/cc731241(v=ws.11)) | Adds, reads, modifies and deletes the Service Principal Names (SPN) directory property for an Active Directory service account. |
    | [`Mimikatz`](https://github.com/ParrotSec/mimikatz) | `Performs many functions. Notably, pass-the-hash attacks, extracting plaintext passwords, and Kerberos ticket extraction from memory on a host.` |
    | [`secretsdump.py`](https://github.com/SecureAuthCorp/impacket/blob/master/examples/secretsdump.py) | Remotely dump SAM and LSA secrets from a host. |
    | [`evil-winrm`](https://github.com/Hackplayers/evil-winrm) | `Provides us with an interactive shell on a host over the WinRM protocol.` |
    | [mssqlclient.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/mssqlclient.py) | Part of the Impacket toolkit, it provides the ability to interact with MSSQL databases. |
    | [noPac.py](https://github.com/Ridter/noPac) | Exploit combo using CVE-2021-42278 and CVE-2021-42287 to impersonate DA from standard domain user. |
    | [rpcdump.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/rpcdump.py) | Part of the Impacket toolset, RPC endpoint mapper. |
    | [CVE-2021-1675.py](https://github.com/cube0x0/CVE-2021-1675/blob/main/CVE-2021-1675.py) | `Printnightmare PoC in py`thon. |
    | [ntlmrelayx.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/ntlmrelayx.py) | Part of the Impacket toolset, it performs SMB relay attacks. |
    | [PetitPotam.py](https://github.com/topotam/PetitPotam) | PoC tool for CVE-2021-36942 to coerce Windows hosts to authenticate to other machines via MS-EFSRPC EfsRpcOpenFileRaw or other functions. |
    | [gettgtpkinit.py](https://github.com/dirkjanm/PKINITtools/blob/master/gettgtpkinit.py) | Tool for manipulating certificates and TGTs. |
    | [getnthash.py](https://github.com/dirkjanm/PKINITtools/blob/master/getnthash.py) | This tool will use an existing TGT to request a PAC for the current user using U2U. |
    | [adidnsdump](https://github.com/dirkjanm/adidnsdump) | A tool for enumerating and dumping DNS records from a domain. Similar to performing a DNS Zone transfer. |
    | [gpp-decrypt](https://github.com/t0thkr1s/gpp-decrypt) | Extracts usernames and passwords from Group Policy preferences files. |
    | [GetNPUsers.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/GetNPUsers.py) | Part of the Impacket toolkit. Used to perform the ASREPRoasting attack to list and obtain AS-REP hashes for users with the 'Do not require Kerberos preauthentication' set. These hashes are then fed into a tool such as Hashcat for attempts at offline password cracking. |
    | [`lookupsid.py`](https://github.com/SecureAuthCorp/impacket/blob/master/examples/lookupsid.py) | `SID bruteforcing tool.` |
    | [ticketer.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/ticketer.py) | A tool for creation and customization of TGT/TGS tickets. It can be used for Golden Ticket creation, child to parent trust attacks, etc. |
    | [raiseChild.py](https://github.com/SecureAuthCorp/impacket/blob/master/examples/raiseChild.py) | Part of the Impacket toolkit, It is a tool for automated child to parent domain privilege escalation. |
    | [Active Directory Explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/adexplorer) | Active Directory Explorer (AD Explorer) is an AD viewer and editor. It can be used to navigate an AD database and view object properties and attributes. It can also be used to save a snapshot of an AD database for offline analysis. When an AD snapshot is loaded, it can be explored as a live version of the database. It can also be used to compare two AD database snapshots to see changes in objects, attributes, and security permissions. |
    | [PingCastle](https://www.pingcastle.com/documentation/) | Used for auditing the security level of an AD environment based on a risk assessment and maturity framework (based on [CMMI](https://en.wikipedia.org/wiki/Capability_Maturity_Model_Integration) adapted to AD security). |
    | [Group3r](https://github.com/Group3r/Group3r) | `Group3r is useful for auditing and finding security misconfigurations in AD Group Policy Objects (GPO).` |
    | [ADRecon](https://github.com/adrecon/ADRecon) | A tool used to extract various data from a target AD environment. The data can be output in Microsoft Excel format with summary views and analysis to assist with analysis and paint a picture of the environment's overall security state. |