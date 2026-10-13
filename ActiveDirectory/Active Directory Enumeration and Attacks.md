# Active Directory Enumeration and Attacks

Connection details:
Found at https://academy.hackthebox.com/app/module/143/section/1262

Important directories:
- C:\Tools
- /opt
- ~

Things referenced to look up:
1. d3ad0ne rule in Hashcat
2. SCF files
3. Responder, Bloodhound, Rubeus
4. SMB Null Session
5. enum4Linux
6. Pass-the-ticket
7. Use the Kerbrute tool to attempt to enumerate valid usernames (userenum feature)
8. DomainPasswordSpray (powershell tool that automatically removes usernames from target list that are close to being locked out)
9. 
10. SPNs, Kerberoasting, TGS Tickets, TGT Tickets

### 1. Introduction
This module introduces AD enumeration and attack techniques in modern and legacy enterprise environments. We will cover:
- Core principles surrounding AD
- Enumeration tools such as Bloodhound and Kerbrute
- Attack TTPs such as taking advantage of SMB Null sessions, Password spraying, ACL attacks, attacking domain trusts, and more.

In this module, we will cover:

- Foundational AD knowledge
- AD enumeration principles
- External Reconnaissance
- Internal enumeration and footprinting
- Lateral movement
- Enumerating and Exploiting Trusts
- Password spraying
- LLMNR/NBT-NS Poisoning
- Gaining privileged access
- Using native tools to perform actions
- Kerberoasting
- Performing ACL Attacks
- AD hardening principles

### 2. AD Historical Info
AD was officially implemented in 2000 with the release of Windows Server 2000. It has been incrementally improved over the years as new Windows Server OS versions release. 

- AD is based on the protocols x.500 and LDAP.
- AD has many possible services, and was originally built for the purpose of making information easy to find/access. This makes it a bit of a behemoth to manage and harden.
- Enterprises regularly get exposed to vulnerabilities, just by misconfiguring services or permissions.
- Enumeration of AD can be done using native tools (Sysinternals, WMI, DNS, many others).
-  Many open-source tools are available to facilitate enumerating and attacking Active Directory. To be most effective, it is important to understand how to do it manually.
-  
