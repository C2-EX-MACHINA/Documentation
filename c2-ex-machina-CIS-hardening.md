<i><b>`C2-EX-MACHINA`, CIS hardening</i></b>

- Microsoft Windows Server 2022
- `Red Hat` Entreprise Linux 8

------------------------------
# Microsoft Windows Server 2022

<i><b>Resume :</i></b>

    total ;               407
    Group Policy ;        406
    REGKEY ;              1

|Index|Level|DC/MS|Action|Name|
|-|-|-|-|-|
| 1.1.1 | `(L1)` | | via GP | Ensure `Enforce password history` is set to `24 or more password(s)` [<b>Auto</b>] |
| 1.1.2 | `(L1)` | | via GP | Ensure `Maximum password age` is set to `365 or fewer days, but not 0` [<b>Auto</b>] |
| 1.1.3 | `(L1)` | | via GP | Ensure `Minimum password age` is set to `1 or more day(s)` [<b>Auto</b>]|
| 1.1.4 | `(L1)` | | via GP | Ensure `Minimum password length` is set to `14 or more character(s)` [<b>Auto</b>] |
| 1.1.5 | `(L1)` | | via GP | Ensure `Password must meet complexity requirements` is set to `Enabled` [<b>Auto</b>] |
| 1.1.6 | `(L1)` | | via GP | Ensure `Relax minimum password length limits` is set to `Enabled` [<b>Auto</b>] |
| 1.1.7 | `(L1)` | | via GP | Ensure `Store passwords using reversible encryption` is set to `Disabled` [<b>Auto</b>] |
| 1.2.1 | `(L1)` | | via GP | Ensure `Account lockout duration` is set to `15 or more minute(s)` [<b>Auto</b>] |
| 1.2.2 | `(L1)` | | via GP | Ensure `Account lockout threshold` is set to `5 or fewer invalid logon attempt(s), but not 0` [<b>Auto</b>] |
| 1.2.3 | `(L1)` | | via GP | Ensure `Reset account lockout counter after` is set to `15 or moreminute(s)` [<b>Auto</b>] |
| 2.2.1 | `(L1)` | | via GP | Ensure `Access Credential Manager as a trusted caller` is set to `No One` [<b>Auto</b>] |
| 2.2.2 | `(L1)` | DC | via GP | Ensure `Access this computer from the network` is set to `Administrators, Authenticated Users, ENTERPRISE DOMAIN CONTROLLERS` [<b>Auto</b>] |
| 2.2.3 | `(L1)` | MS | via GP | Ensure `Access this computer from the network` is set to `Administrators, Authenticated Users` [<b>Auto</b>] |
| 2.2.4 | `(L1)` | | via GP | Ensure `Act as part of the operating system` is set to `No One` [<b>Auto</b>] |
| 2.2.5 | `(L1)` | DC | via GP | Ensure `Add workstations to domain` is set to `Administrators` [<b>Auto</b>] |
| 2.2.6 | `(L1)` | | via GP | Ensure `Adjust memory quotas for a process` is set to `Administrators, LOCAL SERVICE, NETWORK SERVICE` [<b>Auto</b>] |
| 2.2.7 | `(L1)` | | via GP | Ensure `Allow log on locally` is set to `Administrators` [<b>Auto</b>] |
| 2.2.8 | `(L1)` | DC | via GP | Ensure `Allow log on through Remote Desktop Services` is set to `Administrators` [<b>Auto</b>] |
| 2.2.9 | `(L1)` | MS | via GP | Ensure `Allow log on through Remote Desktop Services` is set to `Administrators, Remote Desktop Users` [<b>Auto</b>] |
| 2.2.10 | `(L1)` | | via GP | Ensure `Back up files and directories` is set to `Administrators` [<b>Auto</b>] |
| 2.2.11 | `(L1)` | | via GP | Ensure `Change the system time` is set to `Administrators, LOCAL SERVICE` [<b>Auto</b>] |
| 2.2.12 | `(L1)` | | via GP | Ensure `Change the time zone` is set to `Administrators, LOCAL SERVICE` [<b>Auto</b>] |
| 2.2.13 | `(L1)` | | via GP | Ensure `Create a pagefile` is set to `Administrators` [<b>Auto</b>] |
| 2.2.14 | `(L1)` | | via GP | Ensure `Create a token object` is set to `No One` [<b>Auto</b>] |
| 2.2.15 | `(L1)` | | via GP | Ensure `Create global objects` is set to `Administrators, LOCAL SERVICE, NETWORK SERVICE, SERVICE` [<b>Auto</b>] |
| 2.2.16 | `(L1)` | | via GP | Ensure `Create permanent shared objects` is set to `No One` [<b>Auto</b>] |
| 2.2.17 | `(L1)` | DC | via GP | Ensure `Create symbolic links` is set to `Administrators` [<b>Auto</b>] |
| 2.2.18 | `(L1)` | MS | via GP | Ensure `Create symbolic links` is set to `Administrators, NT VIRTUAL MACHINE\Virtual Machines` [<b>Auto</b>] |
| 2.2.19 | `(L1)` | | via GP | Ensure `Debug programs` is set to `Administrators` [<b>Auto</b>] |
| 2.2.20 | `(L1)` | DC | via GP | Ensure `Deny access to this computer from the network` to include `Guests` [<b>Auto</b>] |
| 2.2.21 | `(L1)` | MS | via GP | Ensure `Deny access to this computer from the network` to include `Guests, Local account and member of Administrators group` [<b>Auto</b>] |
| 2.2.22 | `(L1)` | | via GP | Ensure `Deny log on as a batch job` to include `Guests` [<b>Auto</b>] |
| 2.2.23 | `(L1)` | | via GP | Ensure `Deny log on as a service` to include `Guests` [<b>Auto</b>] |
| 2.2.24 | `(L1)` | | via GP | Ensure `Deny log on locally` to include `Guests` [<b>Auto</b>] |
| 2.2.25 | `(L1)` | DC | via GP | Ensure `Deny log on through Remote Desktop Services` to include `Guests` [<b>Auto</b>] |
| 2.2.26 | `(L1)` | MS | via GP | Ensure `Deny log on through Remote Desktop Services` is set to `Guests, Local account` [<b>Auto</b>] |
| 2.2.27 | `(L1)` | DC | via GP | Ensure `Enable computer and user accounts to be trusted for delegation` is set to `Administrators` [<b>Auto</b>] |
| 2.2.28 | `(L1)` | MS | via GP | Ensure `Enable computer and user accounts to be trusted for delegation` is set to `No One` [<b>Auto</b>] |
| 2.2.29 | `(L1)` | | via GP | Ensure `Force shutdown from a remote system` is set to `Administrators` [<b>Auto</b>] |
| 2.2.30 | `(L1)` | | via GP | Ensure `Generate security audits` is set to `LOCAL SERVICE, NETWORK SERVICE` [<b>Auto</b>] |
| 2.2.31 | `(L1)` | DC | via GP | Ensure `Impersonate a client after authentication` is set to `Administrators, LOCAL SERVICE, NETWORK SERVICE, SERVICE` [<b>Auto</b>] |
| 2.2.32 | `(L1)` | MS | via GP | Ensure `Impersonate a client after authentication` is set to `Administrators, LOCAL SERVICE, NETWORK SERVICE, SERVICE` and (when the Web Server (IIS) Role with Web Services Role Service is installed) `IIS_IUSRS` [<b>Auto</b>] |
| 2.2.33 | `(L1)` | | via GP | Ensure `Increase scheduling priority` is set to `Administrators, Window Manager\Window Manager Group` [<b>Auto</b>] |
| 2.2.34 | `(L1)` | | via GP | Ensure `Load and unload device drivers` is set to `Administrators` [<b>Auto</b>] |
| 2.2.35 | `(L1)` | | via GP | Ensure `Lock pages in memory` is set to `No One` [<b>Auto</b>] |
| 2.2.36 | `(L2)` | DC | via GP | Ensure `Log on as a batch job` is set to `Administrators` [<b>Auto</b>] |
| 2.2.37 | `(L1)` | DC | via GP | Ensure `Manage auditing and security log` is set to`Administrators` and (when Exchange is running in the environment) `Exchange Servers` [<b>Auto</b>] |
| 2.2.38 | `(L1)` | MS | via GP | Ensure `Manage auditing and security log` is set to `Administrators` [<b>Auto</b>] |
| 2.2.39 | `(L1)` | | via GP | Ensure `Modify an object label` is set to `No One` [<b>Auto</b>] |
| 2.2.40 | `(L1)` | | via GP | Ensure `Modify firmware environment values` is set to `Administrators` [<b>Auto</b>] |
| 2.2.41 | `(L1)` | | via GP | Ensure `Perform volume maintenance tasks` is set to `Administrators` [<b>Auto</b>] |
| 2.2.42 | `(L1)` | | via GP | Ensure `Profile single process` is set to `Administrators` [<b>Auto</b>] |
| 2.2.43 | `(L1)` | | via GP | Ensure `Profile system performance` is set to `Administrators, NT SERVICE\WdiServiceHost` [<b>Auto</b>] |
| 2.2.44 | `(L1)` | | via GP | Ensure `Replace a process level token` is set to `LOCAL SERVICE, NETWORK SERVICE` [<b>Auto</b>] |
| 2.2.45 | `(L1)` | | via GP | Ensure `Restore files and directories` is set to `Administrators` [<b>Auto</b>] |
| 2.2.46 | `(L1)` | | via GP | Ensure `Shut down the system` is set to `Administrators` [<b>Auto</b>] |
| 2.2.47 | `(L1)` | DC | via GP | Ensure `Synchronize directory service data` is set to `No One` [<b>Auto</b>] |
| 2.2.48 | `(L1)` | | via GP | Ensure `Take ownership of files or other objects` is set to `Administrators` [<b>Auto</b>] |
| 2.3.1.1 | `(L1)` | MS | via GP | Ensure `Accounts: Administrator account status` is set to `Disabled` [<b>Auto</b>] |
| 2.3.1.2 | `(L1)` | | via GP | Ensure `Accounts: Block Microsoft accounts` is set to `Users can`t add or log on with Microsoft accounts` [<b>Auto</b>] |
| 2.3.1.3 | `(L1)` | MS | via GP | Ensure `Accounts: Guest account status` is set to `Disabled` [<b>Auto</b>] |
| 2.3.1.4 | `(L1)` | | via GP | Ensure `Accounts: Limit local account use of blank passwords to console logon only` is set to `Enabled` [<b>Auto</b>] |
| 2.3.1.5 | `(L1)` | | via GP | Configure `Accounts: Rename administrator account` [<b>Auto</b>] |
| 2.3.1.6 | `(L1)` | | via GP | Configure `Accounts: Rename guest account` [<b>Auto</b>] |
| 2.3.2.1 | `(L1)` | | via GP | Ensure `Audit: Force audit policy subcategory settings (Windows Vista or later) to override audit policy category settings` is set to `Enabled` [<b>Auto</b>] |
| 2.3.2.2 | `(L1)` | | via GP | Ensure `Audit: Shut down system immediately if unable to log security audits` is set to `Disabled` [<b>Auto</b>] |
| 2.3.4.1 | `(L1)` | | via GP | Ensure `Devices: Allowed to format and eject removable media` is set to `Administrators` [<b>Auto</b>] |
| 2.3.4.2 | `(L1)` | | via GP | Ensure `Devices: Prevent users from installing printer drivers` is set to `Enabled` [<b>Auto</b>] |
| 2.3.5.1 | `(L1)` | DC  | via GP | Ensure `Domain controller: Allow server operators to schedule tasks` is set to `Disabled` [<b>Auto</b>] |
| 2.3.5.2 | `(L1)` | DC | via GP | Ensure `Domain controller: Allow vulnerable Netlogon secure channel connections` is set to `Not Configured` [<b>Auto</b>] |
| 2.3.5.3 | `(L1)` | DC | via GP | Ensure `Domain controller: LDAP server channel binding token requirements` is set to `Always` [<b>Auto</b>] |
| 2.3.5.4 | `(L1)` | DC | via GP | Ensure `Domain controller: LDAP server signing requirements` is set to `Require signing` [<b>Auto</b>] |
| 2.3.5.5 | `(L1)` | DC | via GP | Ensure `Domain controller: Refuse machine account password changes` is set to `Disabled` [<b>Auto</b>] |
| 2.3.6.1 | `(L1)` | | via GP | Ensure `Domain member: Digitally encrypt or sign secure channel data (always)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.6.2 | `(L1)` | | via GP | Ensure `Domain member: Digitally encrypt secure channel data (when possible)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.6.3 | `(L1)` | | via GP | Ensure `Domain member: Digitally sign secure channel data (when possible)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.6.4 | `(L1)` | | via GP | Ensure `Domain member: Disable machine account password changes` is set to `Disabled` [<b>Auto</b>] |
| 2.3.6.5 | `(L1)` | | via GP | Ensure `Domain member: Maximum machine account password age` is set to `30 or fewer days, but not 0` [<b>Auto</b>] |
| 2.3.6.6 | `(L1)` | | via GP | Ensure `Domain member: Require strong (Windows 2000 or later) session key` is set to `Enabled` [<b>Auto</b>] |
| 2.3.7.1 | `(L1)` | | via GP | Ensure `Interactive logon: Do not require CTRL+ALT+DEL` is set to `Disabled` [<b>Auto</b>] |
| 2.3.7.2 | `(L1)` | | via GP | Ensure `Interactive logon: Don`t display last signed-in` is set to `Enabled` [<b>Auto</b>] |
| 2.3.7.3 | `(L1)` | | via GP | Ensure `Interactive logon: Machine inactivity limit` is set to `900 or fewer second(s), but not 0` [<b>Auto</b>] |
| 2.3.7.4 | `(L1)` | | via GP | Configure `Interactive logon: Message text for users attempting to log on` [<b>Auto</b>] |
| 2.3.7.5 | `(L1)` | | via GP | Configure `Interactive logon: Message title for users attempting to log on` [<b>Auto</b>] |
| 2.3.7.6 | `(L2)` | MS | via GP | Ensure `Interactive logon: Number of previous logons to cache (in case domain controller is not available)` is set to `4 or fewer logon(s)` [<b>Auto</b>] |
| 2.3.7.7 | `(L1)` | | via GP | Ensure `Interactive logon: Prompt user to change password before expiration` is set to `between 5 and 14 days` [<b>Auto</b>] |
| 2.3.7.8 | `(L1)` | MS | via GP | Ensure `Interactive logon: Require Domain Controller Authentication to unlock workstation` is set to `Enabled` [<b>Auto</b>] |
| 2.3.7.9 | `(L1)` | | via GP | Ensure `Interactive logon: Smart card removal behavior` is set to `Lock Workstation` or higher [<b>Auto</b>] |
| 2.3.8.1 | `(L1)` | | via GP | Ensure `Microsoft network client: Digitally sign communications (always)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.8.2 | `(L1)` | | via GP | Ensure `Microsoft network client: Digitally sign communications (if server agrees)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.8.3 | `(L1)` | | via GP | Ensure `Microsoft network client: Send unencrypted password to third-party SMB servers` is set to `Disabled` [<b>Auto</b>] |
| 2.3.9.1 | `(L1)` | | via GP | Ensure `Microsoft network server: Amount of idle time required before suspending session` is set to `15 or fewer minute(s)` [<b>Auto</b>] |
| 2.3.9.2 | `(L1)` | | via GP | Ensure `Microsoft network server: Digitally sign communications (always)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.9.3 | `(L1)` | | via GP | Ensure `Microsoft network server: Digitally sign communications (if client agrees)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.9.4 | `(L1)` | | via GP | Ensure `Microsoft network server: Disconnect clients when logon hours expire` is set to `Enabled` [<b>Auto</b>] |
| 2.3.9.5 | `(L1)` | MS | via GP | Ensure `Microsoft network server: Server SPN target name validation level` is set to `Accept if provided by client` or higher [<b>Auto</b>] |
| 2.3.10.1 | `(L1)` | | via GP | Ensure `Network access: Allow anonymous SID/Name translation` is set to `Disabled` [<b>Auto</b>] |
| 2.3.10.2 | `(L1)` | MS | via GP | Ensure `Network access: Do not allow anonymous enumeration of SAM accounts` is set to `Enabled` [<b>Auto</b>] |
| 2.3.10.3 | `(L1)` | MS | via GP | Ensure `Network access: Do not allow anonymous enumeration of SAM accounts and shares` is set to `Enabled` [<b>Auto</b>] |
| 2.3.10.4 | `(L2)` | | via GP | Ensure `Network access: Do not allow storage of passwords and credentials for network authentication` is set to `Enabled` [<b>Auto</b>] |
| 2.3.10.5 | `(L1)` | | via GP | Ensure `Network access: Let Everyone `permissions` apply to anonymous users` is set to `Disabled` [<b>Auto</b>] |
| 2.3.10.6 | `(L1)` | DC | via GP | Configure `Network access: Named Pipes that can be accessed anonymously` [<b>Auto</b>] |
| 2.3.10.7 | `(L1)` | MS | via GP | Configure `Network access: Named Pipes that can be accessed anonymously` [<b>Auto</b>] |
| 2.3.10.8 | `(L1)` | | via GP | Configure `Network access: Remotely accessible registry paths` is configured [<b>Auto</b>] |
| 2.3.10.9 | `(L1)` | | via GP | Configure `Network access: Remotely accessible registry paths and sub-paths` is configured [<b>Auto</b>] |
| 2.3.10.10 | `(L1)` | | via GP | Ensure `Network access: Restrict anonymous access to Named Pipes and Shares` is set to `Enabled` [<b>Auto</b>] |
| 2.3.10.11 | `(L1)` | MS | via GP | Ensure `Network access: Restrict clients allowed to make remote calls to SAM` is set to `Administrators: Remote Access: Allow` [<b>Auto</b>] |
| 2.3.10.12 | `(L1)` | | via GP | Ensure `Network access: Shares that can be accessed anonymously` is set to `None` [<b>Auto</b>] |
| 2.3.10.13 | `(L1)` | | via GP | Ensure `Network access: Sharing and security model for local accounts` is set to `Classic - local users authenticate as themselves` [<b>Auto</b>] |
| 2.3.11.1 | `(L1)` | | via GP | Ensure `Network security: Allow Local System to use computer identity for NTLM` is set to `Enabled` [<b>Auto</b>] |
| 2.3.11.2 | `(L1)` | | via GP | Ensure `Network security: Allow LocalSystem NULL session fallback` is set to `Disabled` [<b>Auto</b>] |
| 2.3.11.3 | `(L1)` | | via GP | Ensure `Network Security: Allow PKU2U authentication requests to this computer to use online identities` is set to `Disabled` [<b>Auto</b>] |
| 2.3.11.4 | `(L1)` | | via GP | Ensure `Network security: Configure encryption types allowed for Kerberos` is set to `AES128_HMAC_SHA1, AES256_HMAC_SHA1, Future encryption types` [<b>Auto</b>] |
| 2.3.11.5 | `(L1)` | | via GP | Ensure `Network security: Do not store LAN Manager hash value on next password change` is set to `Enabled` [<b>Auto</b>] |
| 2.3.11.6 | `(L1)` | | via GP | Ensure `Network security: Force logoff when logon hours expire` is set to `Enabled` [<b>Manual</b>] |
| 2.3.11.7 | `(L1)` | | via GP | Ensure `Network security: LAN Manager authentication level` is set to `Send NTLMv2 response only. Refuse LM & NTLM` [<b>Auto</b>] |
| 2.3.11.8 | `(L1)` | | via GP | Ensure `Network security: LDAP client signing requirements` is set to `Negotiate signing` or higher [<b>Auto</b>] |
| 2.3.11.9 | `(L1)` | | via GP | Ensure `Network security: Minimum session security for NTLM SSP based (including secure RPC) clients` is set to `Require NTLMv2 session security, Require 128-bit encryption` [<b>Auto</b>] |
| 2.3.11.10 | `(L1)` | | via GP | Ensure `Network security: Minimum session security for NTLM SSP based (including secure RPC) servers` is set to `Require NTLMv2 session security, Require 128-bit encryption` [<b>Auto</b>] |
| 2.3.13.1 | `(L1)` | | via GP | Ensure `Shutdown: Allow system to be shut down without having to log on` is set to `Disabled` [<b>Auto</b>] |
| 2.3.15.1 | `(L1)` | | via GP | Ensure `System objects: Require case insensitivity for non- Windows subsystems` is set to `Enabled` [<b>Auto</b>] |
| 2.3.15.2 | `(L1)` | | via GP | Ensure `System objects: Strengthen default `permissions` of internal system objects (e.g. Symbolic Links)` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.1 | `(L1)` | | via GP | Ensure `User Account Control: Admin Approval Mode for the Built-in Administrator account` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.2 | `(L1)` | | via GP | Ensure `User Account Control: Behavior of the elevation prompt for administrators in Admin Approval Mode` is set to `Prompt for consent on the secure desktop` [<b>Auto</b>] |
| 2.3.17.3 | `(L1)` | | via GP | Ensure `User Account Control: Behavior of the elevation prompt for standard users` is set to `Automatically deny elevation requests` [<b>Auto</b>] |
| 2.3.17.4 | `(L1)` | | via GP | Ensure `User Account Control: Detect application installations and prompt for elevation` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.5 | `(L1)` | | via GP | Ensure `User Account Control: Only elevate UIAccess applications that are installed in secure locations` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.6 | `(L1)` | | via GP | Ensure `User Account Control: Run all administrators in Admin Approval Mode` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.7 | `(L1)` | | via GP | Ensure `User Account Control: Switch to the secure desktop when prompting for elevation` is set to `Enabled` [<b>Auto</b>] |
| 2.3.17.8 | `(L1)` | | via GP | Ensure `User Account Control: Virtualize file and registry write failures to per-user locations` is set to `Enabled` [<b>Auto</b>] |
| 5.1 | `(L1)` | DC | via GP | Ensure `Print Spooler (Spooler)` is set to `Disabled` [<b>Auto</b>] |
| 5.2 | `(L2)` | MS | via GP | Ensure `Print Spooler (Spooler)` is set to `Disabled` [<b>Auto</b>] |
| 9.1.1 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Firewall state` is set to `On (recommended)` [<b>Auto</b>] |
| 9.1.2 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Inbound connections` is set to `Block (default)` [<b>Auto</b>] |
| 9.1.3 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Outbound connections` is set to `Allow (default)` [<b>Auto</b>] |
| 9.1.4 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Settings: Display a notification` is set to `No` [<b>Auto</b>] |
| 9.1.5 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Logging: Name` is set to `%SystemRoot%\System32\logfiles\firewall\domainfw.log` [<b>Auto</b>] |
| 9.1.6 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Logging: Size limit (KB)` is set to `16,384 KB or greater` [<b>Auto</b>] |
| 9.1.7 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Logging: Log dropped packets` is set to `Yes` [<b>Auto</b>] |
| 9.1.8 | `(L1)` | | via GP | Ensure `Windows Firewall: Domain: Logging: Log successful connections` is set to `Yes` [<b>Auto</b>] |
| 9.2.1 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Firewall state` is set to `On (recommended)` [<b>Auto</b>] |
| 9.2.2 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Inbound connections` is set to `Block (default)` [<b>Auto</b>] |
| 9.2.3 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Outbound connections` is set to `Allow (default)` [<b>Auto</b>] |
| 9.2.4 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Settings: Display a notification` is set to `No` [<b>Auto</b>] |
| 9.2.5 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Logging: Name` is set to `%SystemRoot%\System32\logfiles\firewall\privatefw.log` [<b>Auto</b>] |
| 9.2.6 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Logging: Size limit (KB)` is set to `16,384 KB or greater` [<b>Auto</b>] |
| 9.2.7 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Logging: Log dropped packets`is set to `Yes` [<b>Auto</b>] |
| 9.2.8 | `(L1)` | | via GP | Ensure `Windows Firewall: Private: Logging: Log successful connections` is set to `Yes` [<b>Auto</b>] |
| 9.3.1 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Firewall state` is set to `On (recommended)` [<b>Auto</b>] |
| 9.3.2 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Inbound connections` is set to `Block (default)` [<b>Auto</b>] |
| 9.3.3 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Outbound connections` is set to `Allow (default)` [<b>Auto</b>] |
| 9.3.4 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Settings: Display a notification` is set to `No` [<b>Auto</b>] |
| 9.3.5 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Settings: Apply local firewall rules` is set to `No` [<b>Auto</b>] |
| 9.3.6 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Settings: Apply local connection security rules` is set to `No` [<b>Auto</b>] |
| 9.3.7 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Logging: Name` is set to `%SystemRoot%\System32\logfiles\firewall\publicfw.log` [<b>Auto</b>] |
| 9.3.8 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Logging: Size limit (KB)` is set to `16,384 KB or greater` [<b>Auto</b>] |
| 9.3.9 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Logging: Log dropped packets` is set to `Yes` [<b>Auto</b>] |
| 9.3.10 | `(L1)` | | via GP | Ensure `Windows Firewall: Public: Logging: Log successful connections` is set to `Yes` [<b>Auto</b>] |
| 17.1.1 | `(L1)` | | via GP | Ensure `Audit Credential Validation` is set to `Success and Failure` [<b>Auto</b>] |
| 17.1.2 | `(L1)` | DC | via GP | Ensure `Audit Kerberos Authentication Service` is set to `Success and Failure` [<b>Auto</b>] |
| 17.1.3 | `(L1)` | DC | via GP | Ensure `Audit Kerberos Service Ticket Operations` is set to `Success and Failure` [<b>Auto</b>] |
| 17.2.1 | `(L1)` | | via GP | Ensure `Audit Application Group Management` is set to `Success and Failure` [<b>Auto</b>] |
| 17.2.2 | `(L1)` | DC | via GP | Ensure `Audit Computer Account Management` is set to include `Success` [<b>Auto</b>] |
| 17.2.3 | `(L1)` | DC | via GP | Ensure `Audit Distribution Group Management` is set to include `Success` [<b>Auto</b>] |
| 17.2.4 | `(L1)` | DC | via GP | Ensure `Audit Other Account Management Events` is set to include `Success` [<b>Auto</b>] |
| 17.2.5 | `(L1)` | | via GP | Ensure `Audit Security Group Management` is set to include `Success` [<b>Auto</b>] |
| 17.2.6 | `(L1)` | | via GP | Ensure `Audit User Account Management` is set to `Success and Failure` [<b>Auto</b>] |
| 17.3.1 | `(L1)` | | via GP | Ensure `Audit PNP Activity` is set to include `Success` [<b>Auto</b>] |
| 17.3.2 | `(L1)` | | via GP | Ensure `Audit Process Creation` is set to include `Success` [<b>Auto</b>] |
| 17.4.1 | `(L1)` | DC | via GP | Ensure `Audit Directory Service Access` is set to include `Failure` [<b>Auto</b>] |
| 17.4.2 | `(L1)` | DC | via GP | Ensure `Audit Directory Service Changes` is set to include `Success` [<b>Auto</b>] |
| 17.5.1 | `(L1)` | | via GP | Ensure `Audit Account Lockout` is set to include `Failure` [<b>Auto</b>] |
| 17.5.2 | `(L1)` | | via GP | Ensure `Audit Group Membership` is set to include `Success` [<b>Auto</b>] |
| 17.5.3 | `(L1)` | | via GP | Ensure `Audit Logoff` is set to include `Success` [<b>Auto</b>] |
| 17.5.4 | `(L1)` | | via GP | Ensure `Audit Logon` is set to `Success and Failure` [<b>Auto</b>] |
| 17.5.5 | `(L1)` | | via GP | Ensure `Audit Other Logo/Log`off Events` is set to `Success and Failure` [<b>Auto</b>] |
| 17.5.6 | `(L1)` | | via GP | Ensure `Audit Special Logon` is set to include `Success` [<b>Auto</b>] |
| 17.6.1 | `(L1)` | | via GP | Ensure `Audit Detailed File Share` is set to include `Failure` [<b>Auto</b>] |
| 17.6.2 | `(L1)` | | via GP | Ensure `Audit File Share` is set to `Success and Failure` [<b>Auto</b>] |
| 17.6.3 | `(L1)` | | via GP | Ensure `Audit Other Object Access Events` is set to `Success and Failure` [<b>Auto</b>] |
| 17.6.4 | `(L1)` | | via GP | Ensure `Audit Removable Storage` is set to `Success and Failure` [<b>Auto</b>] |
| 17.7.1 | `(L1)` | | via GP | Ensure `Audit Audit Policy Change` is set to include `Success` [<b>Auto</b>] |
| 17.7.2 | `(L1)` | | via GP | Ensure `Audit Authentication Policy Change` is set to include `Success` [<b>Auto</b>] |
| 17.7.3 | `(L1)` | | via GP | Ensure `Audit Authorization Policy Change` is set to include `Success` [<b>Auto</b>] |
| 17.7.4 | `(L1)` | | via GP | Ensure `Audit MPSSVC Rule-Level Policy Change` is set to `Success and Failure` [<b>Auto</b>] |
| 17.7.5 | `(L1)` | | via GP | Ensure `Audit Other Policy Change Events` is set to include `Failure` [<b>Auto</b>] |
| 17.8.1 | `(L1)` | | via GP | Ensure `Audit Sensitive Privilege Use` is set to `Success and `Failure` [<b>Auto</b>] |
| 17.9.1 | `(L1)` | | via GP | Ensure `Audit IPsec Driver` is set to `Success and Failure` [<b>Auto</b>] |
| 17.9.2 | `(L1)` | | via GP | Ensure `Audit Other System Events` is set to `Success and Failure` [<b>Auto</b>] |
| 17.9.3 | `(L1)` | | via GP | Ensure `Audit Security State Change` is set to include `Success` [<b>Auto</b>] |
| 17.9.4 | `(L1)` | | via GP | Ensure `Audit Security System Extension` is set to include `Success` [<b>Auto</b>] |
| 17.9.5 | `(L1)` | | via GP | Ensure `Audit System Integrity` is set to `Success and Failure` [<b>Auto</b>] |
| 18.1.1.1 | `(L1)` | | via GP | Ensure `Prevent enabling lock screen camera` is set to `Enabled` [<b>Auto</b>] |
| 18.1.1.2 | `(L1)` | | via GP | Ensure `Prevent enabling lock screen slide show` is set to `Enabled` [<b>Auto</b>] |
| 18.1.2.2 | `(L1)` | | via GP | Ensure `Allow users to enable online speech recognition services` is set to `Disabled` [<b>Auto</b>] |
| 18.1.3 | `(L2)` | | via GP | Ensure `Allow Online Tips` is set to `Disabled` [<b>Auto</b>] |
| 18.2.1 | `(L1)` | MS | check file presence | Ensure LAPS AdmPwd GPO Extension / CSE is installed [<b>Auto</b>] |
| 18.2.2 | `(L1)` | MS | via GP | Ensure `Do not allow password expiration time longer than required by policy` is set to `Enabled` [<b>Auto</b>] |
| 18.2.3 | `(L1)` | MS | via GP | Ensure `Enable Local Admin Password Management` is set to `Enabled` [<b>Auto</b>] |
| 18.2.4 | `(L1)` | MS | via GP | Ensure `Password Settings: Password Complexity` is set to `Enabled: Large letters + small letters + numbers + special characters` [<b>Auto</b>] |
| 18.2.5 | `(L1)` | MS | via GP | Ensure `Password Settings: Password Length` is set to `Enabled: 15 or more` [<b>Auto</b>] |
| 18.2.6 | `(L1)` | MS | via GP | Ensure `Password Settings: Password Age (Days)` is set to `Enabled: 30 or fewer` [<b>Auto</b>] |
| 18.3.1 | `(L1)` | MS | via GP | Ensure `Apply UAC restrictions to local accounts on network logons` is set to `Enabled` [<b>Auto</b>] |
| 18.3.2 | `(L1)` | | via GP | Ensure `Configure SMB v1 client driver` is set to `Enabled: Disable driver (recommended)` [<b>Auto</b>] |
| 18.3.3 | `(L1)` | | via GP | Ensure `Configure SMB v1 server` is set to `Disabled` [<b>Auto</b>] |
| 18.3.4 | `(L1)` | | via GP | Ensure `Enable Structured Exception Handling Overwrite Protection (SEHOP)` is set to `Enabled` [<b>Auto</b>] |
| 18.3.5 | `(L1)` | | via GP | Ensure `Limits print driver installation to Administrators` is set to `Enabled` [<b>Auto</b>] |
| 18.3.6 | `(L1)` | | via GP | Ensure `NetBT NodeType configuration` is set to `Enabled: P-node (recommended)` [<b>Auto</b>] |
| 18.3.7 | `(L1)` | | via GP | Ensure `WDigest Authentication` is set to `Disabled` [<b>Auto</b>] |
| 18.4.1 | `(L1)` | | via GP | Ensure `MSS: (AutoAdminLogon) Enable Automatic Logon (not recommended)` is set to `Disabled` [<b>Auto</b>] |
| 18.4.2 | `(L1)` | | via GP | Ensure `MSS: (DisableIPSourceRouting IPv6) IP source routing protection level (protects against packet spoofing)` is set to `Enabled: Highest protection, source routing is completely disabled` [<b>Auto</b>] |
| 18.4.3 | `(L1)` | | via GP | Ensure `MSS: (DisableIPSourceRouting) IP source routing protection level (protects against packet spoofing)` is set to `Enabled: Highest protection, source routing is completely disabled` [<b>Auto</b>] |
| 18.4.4 | `(L1)` | | via GP | Ensure `MSS: (EnableICMPRedirect) Allow ICMP redirects to override OSPF generated routes` is set to `Disabled` [<b>Auto</b>] |
| 18.4.5 | `(L2)` | | via GP | Ensure `MSS: (KeepAliveTime) How often keep-alive packets are sent in milliseconds` is set to `Enabled: 300,000 or 5 minutes (recommended)` [<b>Auto</b>] |
| 18.4.6 | `(L1)` | | via GP | Ensure `MSS: (NoNameReleaseOnDemand) Allow the computer to ignore NetBIOS name release requests except from WINS servers` is set to `Enabled` [<b>Auto</b>] |
| 18.4.7 | `(L2)` | | via GP | Ensure `MSS: (PerformRouterDiscovery) Allow IRDP to detect and configure Default Gateway addresses (could lead to DoS)` is set to `Disabled` [<b>Auto</b>] |
| 18.4.8 | `(L1)` | | via GP | Ensure `MSS: (SafeDllSearchMode) Enable Safe DLL search mode (recommended)` is set to `Enabled` [<b>Auto</b>] |
| 18.4.9 | `(L1)` | | via GP | Ensure `MSS: (ScreenSaverGracePeriod) The time in seconds before the screen saver grace period expires (0 recommended)` is set to `Enabled: 5 or fewer seconds` [<b>Auto</b>] |
| 18.4.10 | `(L2)` | | via GP | Ensure `MSS: (TcpMaxDataRetransmissions IPv6) How many times unacknowledged data is retransmitted` is set to `Enabled: 3` [<b>Auto</b>] |
| 18.4.11 | `(L2)` | | via GP | Ensure `MSS: (TcpMaxDataRetransmissions) How many times unacknowledged data is retransmitted` is set to `Enabled: 3` [<b>Auto</b>] |
| 18.4.12 | `(L1)` | | via GP | Ensure `MSS: (WarningLevel) Percentage threshold for the security event log at which the system will generate a warning` is set to `Enabled: 90% or less` [<b>Auto</b>] |
| 18.5.4.1 | `(L1)` | | via GP | Ensure `Configure DNS over HTTPS (DoH) name resolution` is set to `Enabled: Allow DoH` or higher [<b>Auto</b>] |
| 18.5.4.2 | `(L1)` | | via GP | Ensure `Turn off multicast name resolution` is set to `Enabled` [<b>Auto</b>] |
| 18.5.5.1 | `(L2)` | | via GP | Ensure `Enable Font Providers` is set to `Disabled` [<b>Auto</b>] |
| 18.5.8.1 | `(L1)` | | via GP | Ensure `Enable insecure guest logons` is set to `Disabled` [<b>Auto</b>] |
| 18.5.9.1 | `(L2)` | | via GP | Ensure `Turn on Mapper I/O \| (LLT \|DIO) driver` is set to `Disabled` [<b>Auto</b>] |
| 18.5.9.2 | `(L2)` | | via GP | Ensure `Turn on Responder (RSPNDR) driver` is set to `Disabled` [<b>Auto</b>] |
| 18.5.10.2 | `(L2)` | | via GP | Ensure `Turn off Microsoft Peer-to-Peer Networking Services` is set to `Enabled` [<b>Auto</b>] |
| 18.5.11.2 | `(L1)` | | via GP | Ensure `Prohibit installation and configuration of Network Bridge on your DNS domain network` is set to `Enabled` [<b>Auto</b>] |
| 18.5.11.3 | `(L1)` | | via GP | Ensure `Prohibit use of Internet Connection Sharing on your DNS domain network` is set to `Enabled` [<b>Auto</b>] |
| 18.5.11.4 | `(L1)` | | via GP | Ensure `Require domain users to elevate when setting a network`s location` is set to `Enabled` [<b>Auto</b>] |
| 18.5.14.1 | `(L1)` | | via GP | Ensure `Hardened UNC Paths` is set to `Enabled, with "Require Mutual Authentication" and "Require Integrity" set for all NETLOGON and SYSVOL shares` [<b>Auto</b>] |
| 18.5.19.2.1 | `(L2)` | | via REG | Disable IPv6 (Ensure TCPIP6 Parameter `DisabledComponents` is set to `0xff (255)`) [<b>Auto</b>] |
| 18.5.20.1 | `(L2)` | | via GP | Ensure `Configuration of wireless settings using Windows Connect Now` is set to `Disabled` [<b>Auto</b>] |
| 18.5.20.2 | `(L2)` | | via GP | Ensure `Prohibit access of the Windows Connect Now wizards` is set to `Enabled` [<b>Auto</b>] |
| 18.5.21.1 | `(L1)` | | via GP | Ensure `Minimize the number of simultaneous connections to the Internet or a Windows Domain` is set to `Enabled: 3 = Prevent Wi-Fi when on Ethernet` [<b>Auto</b>] |
| 18.5.21.2 | `(L2)` | MS | via GP | Ensure `Prohibit connection to non-domain networks when connected to domain authenticated network` is set to `Enabled` [<b>Auto</b>] |
| 18.6.1 | `(L1)` | | via GP | Ensure `Allow Print Spooler to accept client connections` is set to `Disabled` [<b>Auto</b>] |
| 18.6.2 | `(L1)` | | via GP | Ensure `Point and Print Restrictions: When installing drivers for a new connection` is set to `Enabled: Show warning and elevation prompt` [<b>Auto</b>] |
| 18.6.3 | `(L1)` | | via GP | Ensure `Point and Print Restrictions: When updating drivers for an existing connection` is set to `Enabled: Show warning and elevation prompt` [<b>Auto</b>] |
| 18.7.1.1 | `(L2)` | | via GP | Ensure `Turn off notifications network usage` is set to `Enabled` [<b>Auto</b>] |
| 18.8.3.1 | `(L1)` | | via GP | Ensure `Include command line in process creation events` is set to `Enabled` [<b>Auto</b>] |
| 18.8.4.1 | `(L1)` | | via GP | Ensure `Encryption Oracle Remediation` is set to `Enabled: Force Updated Clients` [<b>Auto</b>] |
| 18.8.4.2 | `(L1)` | | via GP | Ensure `Remote host allows delegation of non-exportable credentials` is set to `Enabled` [<b>Auto</b>] |
| 18.8.5.1 | `(NG)` | | via GP | Ensure `Turn On Virtualization Based Security` is set to `Enabled` [<b>Auto</b>] |
| 18.8.5.2 | `(NG)` | | via GP | Ensure `Turn On Virtualization Based Security: Select Platform Security Level` is set to `Secure Boot and DMA Protection` [<b>Auto</b>] |
| 18.8.5.3 | `(NG)` | | via GP | Ensure `Turn On Virtualization Based Security: Virtualization Based Protection of Code Integrity` is set to `Enabled with UEFI lock` [<b>Auto</b>] |
| 18.8.5.4 | `(NG)` | | via GP | Ensure `Turn On Virtualization Based Security: Require UEFI Memory Attributes Table` is set to `True (checked)` [<b>Auto</b>] |
| 18.8.5.5 | `(NG)` | MS | via GP | Ensure `Turn On Virtualization Based Security: Credential Guard Configuration` is set to `Enabled with UEFI lock` [<b>Auto</b>] |
| 18.8.5.6 | `(NG)` | DC | via GP | Ensure `Turn On Virtualization Based Security: Credential Guard Configuration` is set to `Disabled` [<b>Auto</b>] |
| 18.8.5.7 | `(NG)` | | via GP | Ensure `Turn On Virtualization Based Security: Secure Launch Configuration` is set to `Enabled` [<b>Auto</b>] |
| 18.8.7.2 | `(L1)` | | via GP | Ensure `Prevent device metadata retrieval from the Internet` is set to `Enabled` [<b>Auto</b>] |
| 18.8.14.1 | `(L1)` | | via GP | Ensure `Boot-Start Driver Initialization Policy` is set to `Enabled: Good, unknown and bad but critical` [<b>Auto</b>] |
| 18.8.21.2 | `(L1)` | | via GP | Ensure `Configure registry policy processing: Do not apply during periodic background processing` is set to `Enabled: FALSE` [<b>Auto</b>] |
| 18.8.21.3 | `(L1)` | | via GP | Ensure `Configure registry policy processing: Process even if the Group Policy objects have not changed` is set to `Enabled: TRUE` [<b>Auto</b>] |
| 18.8.21.4 | `(L1)` | | via GP | Ensure `Continue experiences on this device` is set to `Disabled` [<b>Auto</b>] |
| 18.8.21.5 | `(L1)` | | via GP | Ensure `Turn off background refresh of Group Policy` is set to `Disabled` [<b>Auto</b>] |
| 18.8.22.1.1 | `(L1)` | | via GP | Ensure `Turn off downloading of print drivers over HTTP` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.2 | `(L2)` | | via GP | Ensure `Turn off handwriting personalization data sharing` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.3 | `(L2)` | | via GP | Ensure `Turn off handwriting recognition error reporting` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.4 | `(L2)` | | via GP | Ensure `Turn off Internet Connection Wizard if URL connection is referring to Microsoft.com` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.5 | `(L1)` | | via GP | Ensure `Turn off Internet download for Web publishing and online ordering wizards` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.6 | `(L2)` | | via GP | Ensure `Turn off printing over HTTP` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.7 | `(L2)` | | via GP | Ensure `Turn off Registration if URL connection is referring to Microsoft.com` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.8 | `(L2)` | | via GP | Ensure `Turn off Search Companion content file updates` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.9 | `(L2)` | | via GP | Ensure `Turn off the "Order Prints" picture task` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.10 | `(L2)` | | via GP | Ensure `Turn off the "Publish to Web" task for files and folders` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.11 | `(L2)` | | via GP | Ensure `Turn off the Windows Messenger Customer Experience Improvement Program` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.12 | `(L2)` | | via GP | Ensure `Turn off Windows Customer Experience Improvement Program` is set to `Enabled` [<b>Auto</b>] |
| 18.8.22.1.13 | `(L2)` | | via GP | Ensure `Turn off Windows Error Reporting` is set to `Enabled` [<b>Auto</b>] |
| 18.8.25.1 | `(L2)` | | via GP | Ensure `Support device authentication using certificate` is set to `Enabled: Automatic` [<b>Auto</b>] |
| 18.8.26.1 | `(L1)` | | via GP | Ensure `Enumeration policy for external devices incompatible with Kernel DMA Protection` is set to `Enabled: Block All` [<b>Auto</b>] |
| 18.8.27.1 | `(L2)` | | via GP | Ensure `Disallow copying of user input methods to the system account for sign-in` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.1 | `(L1)` | | via GP | Ensure `Block user from showing account details on sign-in` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.2 | `(L1)` | | via GP | Ensure `Do not display network selection UI` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.3 | `(L1)` | | via GP | Ensure `Do not enumerate connected users on domain-joined computers` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.4 | `(L1)` | MS | via GP | Ensure `Enumerate local users on domain-joined computers` is set to `Disabled` [<b>Auto</b>] |
| 18.8.28.5 | `(L1)` | | via GP | Ensure `Turn off app notifications on the lock screen` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.6 | `(L1)` | | via GP | Ensure `Turn off picture password sign-in` is set to `Enabled` [<b>Auto</b>] |
| 18.8.28.7 | `(L1)` | | via GP | Ensure `Turn on convenience PIN sign-in` is set to `Disabled` [<b>Auto</b>] |
| 18.8.31.1 | `(L2)` | | via GP | Ensure `Allow Clipboard synchronization across devices` is set to `Disabled` [<b>Auto</b>] |
| 18.8.31.2 | `(L2)` | | via GP | Ensure `Allow upload of User Activities` is set to `Disabled` [<b>Auto</b>] |
| 18.8.34.6.1 | `(L2)` | | via GP | Ensure `Allow network connectivity during connected- standby (on battery)` is set to `Disabled` [<b>Auto</b>] |
| 18.8.34.6.2 | `(L2)` | | via GP | Ensure `Allow network connectivity during connected- standby (plugged in)` is set to `Disabled` [<b>Auto</b>] |
| 18.8.34.6.3 | `(L1)` | | via GP | Ensure `Require a password when a computer wakes (on battery)` is set to `Enabled` [<b>Auto</b>] |
| 18.8.34.6.4 | `(L1)` | | via GP | Ensure `Require a password when a computer wakes (plugged in)` is set to `Enabled` [<b>Auto</b>] |
| 18.8.36.1 | `(L1)` | | via GP | Ensure `Configure Offer Remote Assistance` is set to `Disabled` [<b>Auto</b>] |
| 18.8.36.2 | `(L1)` | | via GP | Ensure `Configure Solicited Remote Assistance` is set to `Disabled` [<b>Auto</b>] |
| 18.8.37.1 | `(L1)` | MS | via GP | Ensure `Enable RPC Endpoint Mapper Client Authentication` is set to `Enabled` [<b>Auto</b>] |
| 18.8.37.2 | `(L2)` | MS | via GP | Ensure `Restrict Unauthenticated RPC clients` is set to `Enabled: Authenticated` [<b>Auto</b>] |
| 18.8.40.1 | `(L1)` | DC | via GP | Ensure `Configure validation of ROCA-vulnerable WHfB keys during authentication` is set to `Enabled: Audit` or higher [<b>Auto</b>] |
| 18.8.48.5.1 | `(L2)` | | via GP | Ensure `Microsoft Support Diagnostic Tool: Turn on MSDT interactive communication with support provider` is set to `Disabled` [<b>Auto</b>] |
| 18.8.48.11.1 | `(L2)` | | via GP | Ensure `Enable/Disable PerfTrack` is set to `Disabled` [<b>Auto</b>] |
| 18.8.50.1 | `(L2)` | | via GP | Ensure `Turn off the advertising ID` is set to `Enabled` [<b>Auto</b>] |
| 18.8.53.1.1 | `(L2)` | | via GP | Ensure `Enable Windows NTP Client` is set to `Enabled` [<b>Auto</b>] |
| 18.8.53.1.2 | `(L2)` | MS | via GP | Ensure `Enable Windows NTP Server` is set to `Disabled` [<b>Auto</b>] |
| 18.9.4.1 | `(L2)` | | via GP | Ensure `Allow a Windows app to share application data between users` is set to `Disabled` [<b>Auto</b>] |
| 18.9.6.1 | `(L1)` | | via GP | Ensure `Allow Microsoft accounts to be optional` is set to `Enabled` [<b>Auto</b>] |
| 18.9.8.1 | `(L1)` | | via GP | Ensure `Disallow Autoplay for non-volume devices` is set to `Enabled` [<b>Auto</b>] |
| 18.9.8.2 | `(L1)` | | via GP | Ensure `Set the default behavior for AutoRun` is set to `Enabled: Do not execute any autorun commands` [<b>Auto</b>] |
| 18.9.8.3 | `(L1)` | | via GP | Ensure `Turn off Autoplay` is set to `Enabled: All drives` [<b>Auto</b>] |
| 18.9.10.1.1 | `(L1)` | | via GP | Ensure `Configure enhanced anti-spoofing` is set to `Enabled` [<b>Auto</b>] |
| 18.9.12.1 | `(L2)` | | via GP | Ensure `Allow Use of Camera` is set to `Disabled` [<b>Auto</b>] |
| 18.9.14.1 | `(L1)` | | via GP | Ensure `Turn off cloud consumer account state content` is set to `Enabled` [<b>Auto</b>] |
| 18.9.14.2 | `(L1)` | | via GP | Ensure `Turn off Microsoft consumer experiences` is set to `Enabled` [<b>Auto</b>] |
| 18.9.15.1 | `(L1)` | | via GP | Ensure `Require pin for pairing` is set to `Enabled: First Time` OR `Enabled: Always` [<b>Auto</b>] |
| 18.9.16.1 | `(L1)` | | via GP | Ensure `Do not display the password reveal button` is set to `Enabled` [<b>Auto</b>] |
| 18.9.16.2 | `(L1)` | | via GP | Ensure `Enumerate administrator accounts on elevation` is set to `Disabled` [<b>Auto</b>] |
| 18.9.17.1 | `(L1)` | | via GP | Ensure `Allow Diagnostic Data` is set to `Enabled: Diagnostic data off (not recommended)` or `Enabled: Send required diagnostic data` [<b>Auto</b>] |
| 18.9.17.2 | `(L2)` | | via GP | Ensure `Configure Authenticated Proxy usage for the Connected User Experience and Telemetry service` is set to `Enabled: Disable Authenticated Proxy usage` [<b>Auto</b>] |
| 18.9.17.3 | `(L1)` | | via GP | Ensure `Disable OneSettings Downloads` is set to `Enabled` [<b>Auto</b>] |
| 18.9.17.4 | `(L1)` | | via GP | Ensure `Do not show feedback notifications` is set to `Enabled` [<b>Auto</b>] |
| 18.9.17.5 | `(L1)` | | via GP | Ensure `Enable OneSettings Auditing` is set to `Enabled` [<b>Auto</b>] |
| 18.9.17.6 | `(L1)` | | via GP | Ensure `Limit Diagnostic Log Collection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.17.7 | `(L1)` | | via GP | Ensure `Limit Dump Collection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.17.8 | `(L1)` | | via GP | Ensure `Toggle user control over Insider builds` is set to `Disabled` [<b>Auto</b>] |
| 18.9.27.1.1 | `(L1)` | | via GP | Ensure `Application: Control Event Log behavior when the log file reaches its maximum size` is set to `Disabled` [<b>Auto</b>] |
| 18.9.27.1.2 | `(L1)` | | via GP | Ensure `Application: Specify the maximum log file size (KB)` is set to `Enabled: 32,768 or greater` [<b>Auto</b>] |
| 18.9.27.2.1 | `(L1)` | | via GP | Ensure `Security: Control Event Log behavior when the log file reaches its maximum size` is set to `Disabled` [<b>Auto</b>] |
| 18.9.27.2.2 | `(L1)` | | via GP | Ensure `Security: Specify the maximum log file size (KB)` is set to `Enabled: 196,608 or greater` [<b>Auto</b>] |
| 18.9.27.3.1 | `(L1)` | | via GP | Ensure `Setup: Control Event Log behavior when the log file reaches its maximum size` is set to `Disabled` [<b>Auto</b>] |
| 18.9.27.3.2 | `(L1)` | | via GP | Ensure `Setup: Specify the maximum log file size (KB)` is set to `Enabled: 32,768 or greater` [<b>Auto</b>] |
| 18.9.27.4.1 | `(L1)` | | via GP | Ensure `System: Control Event Log behavior when the log file reaches its maximum size` is set to `Disabled` [<b>Auto</b>] |
| 18.9.27.4.2 | `(L1)` | | via GP | Ensure `System: Specify the maximum log file size (KB)` is set to `Enabled: 32,768 or greater` [<b>Auto</b>] |
| 18.9.31.2 | `(L1)` | | via GP | Ensure `Turn off Data Execution Prevention for Explorer` is set to `Disabled` [<b>Auto</b>] |
| 18.9.31.3 | `(L1)` | | via GP | Ensure `Turn off heap termination on corruption` is set to `Disabled` [<b>Auto</b>] |
| 18.9.31.4 | `(L1)` | | via GP | Ensure `Turn off shell protocol protected mode` is set to `Disabled` [<b>Auto</b>] |
| 18.9.41.1 | `(L2)` | | via GP | Ensure `Turn off location` is set to `Enabled` [<b>Auto</b>] |
| 18.9.45.1 | `(L2)` | | via GP | Ensure `Allow Message Service Cloud Sync` is set to `Disabled` [<b>Auto</b>] |
| 18.9.46.1 | `(L1)` | | via GP | Ensure `Block all consumer Microsoft account user authentication` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.4.1 | `(L1)` | | via GP | Ensure `Configure local setting override for reporting to Microsoft MAPS` is set to `Disabled` [<b>Auto</b>] |
| 18.9.47.4.2 | `(L2)` | | via GP | Ensure `Join Microsoft MAPS` is set to `Disabled` [<b>Auto</b>] |
| 18.9.47.5.1.1 | `(L1)` | | via GP | Ensure `Configure Attack Surface Reduction rules` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.5.1.2 | `(L1)` | | via GP | Ensure `Configure Attack Surface Reduction rules: Set the state for each ASR rule` is configured [<b>Auto</b>] |
| 18.9.47.5.3.1 | `(L1)` | | via GP | Ensure `Prevent users and apps from accessing dangerous websites` is set to `Enabled: Block` [<b>Auto</b>] |
| 18.9.47.6.1 | `(L2)` | | via GP | Ensure `Enable file hash computation feature` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.9.1 | `(L1)` | | via GP | Ensure `Scan all downloaded files and attachments` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.9.2 | `(L1)` | | via GP | Ensure `Turn off real-time protection` is set to `Disabled` [<b>Auto</b>] |
| 18.9.47.9.3 | `(L1)` | | via GP | Ensure `Turn on behavior monitoring` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.9.4 | `(L1)` | | via GP | Ensure `Turn on script scanning` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.11.1 | `(L2)` | | via GP | Ensure `Configure Watson events` is set to `Disabled` [<b>Auto</b>] |
| 18.9.47.12.1 | `(L1)` | | via GP | Ensure `Scan removable drives` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.12.2 | `(L1)` | | via GP | Ensure `Turn on e-mail scanning` is set to `Enabled` [<b>Auto</b>] |
| 18.9.47.15 | `(L1)` | | via GP | Ensure `Configure detection for potentially unwanted applications` is set to `Enabled: Block` [<b>Auto</b>] |
| 18.9.47.16 | `(L1)` | | via GP | Ensure `Turn off Microsoft Defender AntiVirus` is set to `Disabled` [<b>Auto</b>] |
| 18.9.58.1 | `(L1)` | | via GP | Ensure `Prevent the usage of OneDrive for file storage` is set to `Enabled` [<b>Auto</b>] |
| 18.9.64.1 | `(L2)` | | via GP | Ensure `Turn off Push To Install service` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.2.2 | `(L1)` | | via GP | Ensure `Do not allow passwords to be saved` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.2.1 | `(L2)` | | via GP | Ensure `Restrict Remote Desktop Services users to a single Remote Desktop Services session` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.3.1 | `(L2)` | | via GP | Ensure `Allow UI Automation redirection` is set to `Disabled` [<b>Auto</b>] |
| 18.9.65.3.3.2 | `(L2)` | | via GP | Ensure `Do not allow COM port redirection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.3.3 | `(L1)` | | via GP | Ensure `Do not allow drive redirection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.3.4 | `(L2)` | | via GP | Ensure `Do not allow location redirection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.3.5 | `(L2)` | | via GP | Ensure `Do not allow LPT port redirection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.3.6 | `(L2)` | | via GP | Ensure `Do not allow supported Plug and Play device redirection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.9.1 | `(L1)` | | via GP | Ensure `Always prompt for password upon connection` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.9.2 | `(L1)` | | via GP | Ensure `Require secure RPC communication` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.9.3 | `(L1)` | | via GP | Ensure `Require use of specific security layer for remote (RDP) connections` is set to `Enabled: SSL` [<b>Auto</b>] |
| 18.9.65.3.9.4 | `(L1)` | | via GP | Ensure `Require user authentication for remote connections by using Network Level Authentication` is set to `Enabled` [<b>Auto</b>] |
| 18.9.65.3.9.5 | `(L1)` | | via GP | Ensure `Set client connection encryption level` is set to `Enabled: High Level` [<b>Auto</b>] |
| 18.9.65.3.10.1 | `(L2)` | | via GP | Ensure `Set time limit for active but idle Remote Desktop Services sessions` is set to `Enabled: 15 minutes or less, but not Never (0)` [<b>Auto</b>] |
| 18.9.65.3.10.2 | `(L2)` | | via GP | Ensure `Set time limit for disconnected sessions` is set to `Enabled: 1 minute` [<b>Auto</b>] |
| 18.9.65.3.11.1 | `(L1)` | | via GP | Ensure `Do not delete temp folders upon exit` is set to `Disabled` [<b>Auto</b>] |
| 18.9.65.3.11.2 | `(L1)` | | via GP | Ensure `Do not use temporary folders per session` is set to `Disabled` [<b>Auto</b>] |
| 18.9.66.1 | `(L1)` | | via GP | Ensure `Prevent downloading of enclosures` is set to `Enabled` [<b>Auto</b>] |
| 18.9.67.2 | `(L2)` | | via GP | Ensure `Allow Cloud Search` is set to `Enabled: Disable Cloud Search` [<b>Auto</b>] |
| 18.9.67.3 | `(L1)` | | via GP | Ensure `Allow indexing of encrypted files` is set to `Disabled` [<b>Auto</b>] |
| 18.9.72.1 | `(L2)` | | via GP | Ensure `Turn off KMS Client Online AVS Validation` is set to `Enabled` [<b>Auto</b>] |
| 18.9.85.1.1 | `(L1)` | | via GP | Ensure `Configure Windows Defender SmartScreen` is set to `Enabled: Warn and prevent bypass` [<b>Auto</b>] |
| 18.9.89.1 | `(L2)` | | via GP | Ensure `Allow suggested apps in Windows Ink Workspace` is set to `Disabled` [<b>Auto</b>] |
| 18.9.89.2 | `(L1)` | | via GP | Ensure `Allow Windows Ink Workspace` is set to `Enabled: On, but disallow access above lock` OR `Disabled` but not `Enabled: On` [<b>Auto</b>] |
| 18.9.90.1 | `(L1)` | | via GP | Ensure `Allow user control over installs` is set to `Disabled` [<b>Auto</b>] |
| 18.9.90.2 | `(L1)` | | via GP | Ensure `Always install with elevated privileges` is set to `Disabled` [<b>Auto</b>] |
| 18.9.90.3 | `(L2)` | | via GP | Ensure `Prevent Internet Explorer security prompt for Windows Installer scripts` is set to `Disabled` [<b>Auto</b>] |
| 18.9.91.1 | `(L1)` | | via GP | Ensure `Sign-in and lock last interactive user automatically after a restart` is set to `Disabled` [<b>Auto</b>] |
| 18.9.100.1 | `(L1)` | | via GP | Ensure `Turn on PowerShell Script Block Logging` is set to `Enabled` [<b>Auto</b>] |
| 18.9.100.2 | `(L1)` | | via GP | Ensure `Turn on PowerShell Transcription` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.1.1 | `(L1)` | | via GP | Ensure `Allow Basic authentication` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.1.2 | `(L1)` | | via GP | Ensure `Allow unencrypted traffic` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.1.3 | `(L1)` | | via GP | Ensure `Disallow Digest authentication` is set to `Enabled` [<b>Auto</b>] |
| 18.9.102.2.1 | `(L1)` | | via GP | Ensure `Allow Basic authentication` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.2.2 | `(L2)` | | via GP | Ensure `Allow remote server management through WinRM` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.2.3 | `(L1)` | | via GP | Ensure `Allow unencrypted traffic` is set to `Disabled` [<b>Auto</b>] |
| 18.9.102.2.4 | `(L1)` | | via GP | Ensure `Disallow WinRM from storing RunAs credentials` is set to `Enabled` [<b>Auto</b>] |
| 18.9.103.1 | `(L2)` | | via GP | Ensure `Allow Remote Shell Access` is set to `Disabled` [<b>Auto</b>] |
| 18.9.105.2.1 | `(L1)` | | via GP | Ensure `Prevent users from modifying settings` is set to `Enabled` [<b>Auto</b>] |
| 18.9.108.1.1 | `(L1)` | | via GP | Ensure `No auto-restart with logged on users for scheduled automatic updates installations` is set to `Disabled` [<b>Auto</b>] |
| 18.9.108.2.1 | `(L1)` | | via GP | Ensure `Configure Automatic Updates` is set to `Enabled` [<b>Auto</b>] |
| 18.9.108.2.2 | `(L1)` | | via GP | Ensure `Configure Automatic Updates: Scheduled install day` is set to `0 - Every day` [<b>Auto</b>] |
| 18.9.108.4.1 | `(L1)` | | via GP | Ensure `Manage preview builds` is set to `Disabled` [<b>Auto</b>] |
| 18.9.108.4.2 | `(L1)` | | via GP | Ensure `Select when Preview Builds and Feature Updates are received` is set to `Enabled: 180 or more days` [<b>Auto</b>] |
| 18.9.108.4.3 | `(L1)` | | via GP | Ensure `Select when Quality Updates are received` is set to `Enabled: 0 days` [<b>Auto</b>] |
| 19.1.3.1 | `(L1)` | | via GP | Ensure `Enable screen saver` is set to `Enabled` [<b>Auto</b>] |
| 19.1.3.2 | `(L1)` | | via GP | Ensure `Password protect the screen saver` is set to `Enabled` [<b>Auto</b>] |
| 19.1.3.3 | `(L1)` | | via GP | Ensure `Screen saver timeout` is set to `Enabled: 900 seconds or fewer, but not 0` [<b>Auto</b>] |
| 19.5.1.1 | `(L1)` | | via GP | Ensure `Turn off toast notifications on the lock screen` is set to `Enabled` [<b>Auto</b>] |
| 19.6.6.1.1 | `(L2)` | | via GP | Ensure `Turn off Help Experience Improvement Program` is set to `Enabled` [<b>Auto</b>] |
| 19.7.4.1 | `(L1)` | | via GP | Ensure `Do not preserve zone information in file attachments` is set to `Disabled` [<b>Auto</b>] |
| 19.7.4.2 | `(L1)` | | via GP | Ensure `Notify antivirus programs when opening attachments` is set to `Enabled` [<b>Auto</b>] |
| 19.7.8.1 | `(L1)` | | via GP | Ensure `Configure Windows spotlight on lock screen` is set to Disabled` [<b>Auto</b>] |
| 19.7.8.2 | `(L1)` | | via GP | Ensure `Do not suggest third-party content in Windows spotlight` is set to `Enabled` [<b>Auto</b>] |
| 19.7.8.3 | `(L2)` | | via GP | Ensure `Do not use diagnostic data for tailored experiences` is set to `Enabled` [<b>Auto</b>] |
| 19.7.8.4 | `(L2)` | | via GP | Ensure `Turn off all Windows spotlight features` is set to `Enabled` [<b>Auto</b>] |
| 19.7.8.5 | `(L1)` | | via GP | Ensure `Turn off Spotlight collection on Desktop` is set to `Enabled` [<b>Manual</b>] |
| 19.7.28.1 | `(L1)` | | via GP | Ensure `Prevent users from sharing files within their profile.` is set to `Enabled` [<b>Auto</b>] |
| 19.7.43.1 | `(L1)` | | via GP | Ensure `Always install with elevated privileges` is set to `Disabled` [<b>Auto</b>] |
| 19.7.47.2.1 | `(L2)` | | via GP | Ensure `Prevent Codec Download` is set to `Enabled` [<b>Auto</b>] |



------------------------------
# `Red Hat` Entreprise Linux 8

<i><b>Resume :</i></b>

    total ;               273
    auto ;                245
    manual ;              28

|Index|Level|DC/MS|Action|Name|
|-|-|-|-|-|
|<b>`1`</b>|||| <b>`Initial Setup`</b>|
|<b>`1.1`</b>|||| <b>`Filesystem Configuration`</b>|
|<b>`1.1.1`</b>|||| <b>`Disable unused filesystems`</b>|
|1.1.1.1|||| Ensure mounting of cramfs filesystems is `disabled` [<b>Auto</b>]|
|1.1.1.2|||| Ensure mounting of squashfs filesystems is `disabled` [<b>Auto</b>]|
|1.1.1.3|||| Ensure mounting of udf filesystems is `disabled` [<b>Auto</b>]|
|<b>`1.1.2`</b>|||| <b>`Configure /tmp`</b>|
|1.1.2.1|||| Ensure `/tmp` is a separate partition [<b>Auto</b>]|
|1.1.2.2|||| Ensure `nodev` option set on `/tmp` partition [<b>Auto</b>]|
|1.1.2.3|||| Ensure `noexec` option set on `/tmp` partition [<b>Auto</b>]|
|1.1.2.4|||| Ensure `nosuid` option set on `/tmp` partition [<b>Auto</b>]|
|<b>`1.1.3`</b>|||| <b>`Configure /var`</b>|
|1.1.3.1|||| Ensure separate partition exists for `/var` [<b>Auto</b>]|
|1.1.3.2|||| Ensure `nodev` option set on `/var` partition [<b>Auto</b>]|
|1.1.3.3|||| Ensure `noexec` option set on `/var` partition [<b>Auto</b>]|
|1.1.3.4|||| Ensure `nosuid` option set on `/var` partition [<b>Auto</b>]|
|<b>`1.1.4`</b>|||| <b>`Configure /var/tmp`</b>|
|1.1.4.1|||| Ensure separate partition exists for `/var/tmp` [<b>Auto</b>]|
|1.1.4.2|||| Ensure `noexec` option set on `/var/tmp` partition [<b>Auto</b>]|
|1.1.4.3|||| Ensure `nosuid` option set on `/var/tmp` partition [<b>Auto</b>]|
|1.1.4.4|||| Ensure `nodev` option set on `/var/tmp` partition [<b>Auto</b>]|
|<b>`1.1.5`</b>|||| <b>`Configure /var/log`</b>|
|1.1.5.1|||| Ensure separate partition exists for `/var/log` [<b>Auto</b>]|
|1.1.5.2|||| Ensure `nodev` option set on `/var/log` partition [<b>Auto</b>]|
|1.1.5.3|||| Ensure `noexec` option set on `/var/log` partition [<b>Auto</b>]|
|1.1.5.4|||| Ensure `nosuid` option set on `/var/log` partition [<b>Auto</b>]|
|<b>`1.1.6`</b>|||| <b>`Configure /var/log/audit`</b>|
|1.1.6.1|||| Ensure separate partition exists for `/var/log/audit` [<b>Auto</b>]|
|1.1.6.2|||| Ensure `noexec` option set on `/var/log/audit` partition [<b>Auto</b>]|
|1.1.6.3|||| Ensure `nodev` option set on `/var/log/audit` partition [<b>Auto</b>]|
|1.1.6.4|||| Ensure `nosuid` option set on `/var/log/audit` partition [<b>Auto</b>]|
|<b>`1.1.7`</b>|||| <b>`Configure /home`</b>|
|1.1.7.1|||| Ensure separate partition exists for `/home` [<b>Auto</b>]|
|1.1.7.2|||| Ensure `nodev` option set on `/home` partition [<b>Auto</b>]|
|1.1.7.3|||| Ensure `nosuid` option set on `/home` partition [<b>Auto</b>]|
|1.1.7.4|||| Ensure usrquota option set on `/home` partition [<b>Auto</b>]|
|1.1.7.5|||| Ensure grpquota option set on `/home` partition [<b>Auto</b>]|
|<b>`1.1.8`</b>|||| <b>`Configure /dev/shm`</b>|
|1.1.8.1|||| Ensure `nodev` option set on `/dev/shm` partition [<b>Auto</b>]|
|1.1.8.2|||| Ensure `noexec` option set on `/dev/shm` partition [<b>Auto</b>]|
|1.1.8.3|||| Ensure `nosuid` option set on `/dev/shm` partition [<b>Auto</b>]|
|1.1.9|||| `Disable` Automounting [<b>Auto</b>]|
|1.1.10 |||| `Disable` USB Storage [<b>Auto</b>]|
|<b>`1.2`</b>|||| <b>`Configure Software Updates`</b>|
|1.2.1|||| Ensure `Red Hat` Subscription Manager connection is configured [<b>Manual</b>]|
|1.2.2|||| Ensure `GPG keys` are configured [<b>Manual</b>]|
|1.2.3|||| Ensure `gpgcheck` is globally activated [<b>Auto</b>]|
|1.2.4|||| Ensure package manager repositories are configured [<b>Manual</b>]|
|<b>`1.3`</b>|||| <b>`Filesystem Integrity Checking`</b>|
|1.3.1|||| Ensure AIDE is `installed` [<b>Auto</b>]|
|1.3.2|||| Ensure filesystem integrity is regularly checked [<b>Auto</b>]|
|<b>`1.4`</b>|||| <b>`Secure Boot Settings`</b>|
|1.4.1|||| Ensure `bootloader` password is set [<b>Auto</b>]|
|1.4.2|||| Ensure `permissions` on `bootloader` config are configured [<b>Auto</b>]|
|1.4.3|||| Ensure authentication is required when booting into rescue mode [<b>Auto</b>]|
|<b>`1.5`</b>|||| <b>`Additional Process Hardening`</b>|
|1.5.1|||| Ensure `core dump` storage is `disabled` [<b>Auto</b>]|
|1.5.2|||| Ensure `core dump` backtraces are `disabled` [<b>Auto</b>]|
|1.5.3|||| Ensure address space layout randomization (ASLR) is enabled [<b>Auto</b>]|
|<b>`1.6`</b>|||| <b>`Mandatory Access Control`</b>|
|<b>`1.6.1`</b>|||| <b>`Configure SELinux`</b>|
|1.6.1.1|||| Ensure `SELinux` is `installed` [<b>Auto</b>]|
|1.6.1.2|||| Ensure `SELinux` is not `disabled` in `bootloader` configuration [<b>Auto</b>]|
|1.6.1.3|||| Ensure `SELinux` policy is configured [<b>Auto</b>]|
|1.6.1.4|||| Ensure the `SELinux` mode is not `disabled` [<b>Auto</b>]|
|1.6.1.5|||| Ensure the `SELinux` mode is enforcing [<b>Auto</b>]|
|1.6.1.6|||| Ensure no unconfined services exist [<b>Auto</b>]|
|1.6.1.7|||| Ensure SETroubleshoot is not `installed` [<b>Auto</b>]|
|1.6.1.8|||| Ensure the MCS Translation Service (mcstrans) is not `installed` [<b>Auto</b>]|
|<b>`1.7`</b>|||| <b>`Command Line Warning Banners`</b>|
|1.7.1|||| Ensure message of the day is configured properly [<b>Auto</b>]|
|1.7.2|||| Ensure local login warning banner is configured properly [<b>Auto</b>]|
|1.7.3|||| Ensure remote login warning banner is configured properly [<b>Auto</b>]|
|1.7.4|||| Ensure `permissions` `on /etc/motd` are configured [<b>Auto</b>]|
|1.7.5|||| Ensure `permissions` `on /etc/issue` are configured [<b>Auto</b>]|
|1.7.6|||| Ensure `permissions` on `/etc/issue`.net are configured [<b>Auto</b>]|
|<b>`1.8`</b>|||| <b>`GNOME Display Manager`</b>|
|1.8.1|||| Ensure GNOME Display Manager is removed [<b>Manual</b>]|
|1.8.2|||| Ensure GDM login banner is configured [<b>Auto</b>]|
|1.8.3|||| Ensure last logged in user display is `disabled` [<b>Auto</b>]|
|1.8.4|||| Ensure XDMCP is not enabled [<b>Auto</b>]|
|1.8.5|||| Ensure automatic mounting of removable media is `disabled` [<b>Auto</b>]|
|1.9|||| Ensure updates, patches, and additional security software are `installed` [<b>Manual</b>]|
|1.10 |||| Ensure system-wide crypto policy is not legacy [<b>Auto</b>]|
|<b>`2`</b>|||| <b>`Services`</b>|
|<b>`2.1`</b>|||| <b>`Time Synchronization`</b>|
|2.1.1|||| Ensure `time` synchronization is in use [<b>Auto</b>]|
|2.1.2|||| Ensure `chrony` is configured [<b>Auto</b>]|
|<b>`2.2`</b>|||| <b>`Special Purpose Services`</b>|
|2.2.1|||| Ensure `xinetd` is not `installed` [<b>Auto</b>]|
|2.2.2|||| Ensure `xorg-x11-server-common` is not `installed` [<b>Auto</b>]|
|2.2.3|||| Ensure `Avahi` Server is not `installed` [<b>Auto</b>]|
|2.2.4|||| Ensure `CUPS` is not `installed` [<b>Auto</b>]|
|2.2.5|||| Ensure `DHCP` Server is not `installed` [<b>Auto</b>]|
|2.2.6|||| Ensure `DNS` Server is not `installed` [<b>Auto</b>]|
|2.2.7|||| Ensure `FTP` Server is not `installed` [<b>Auto</b>]|
|2.2.8|||| Ensure `VSFTP` Server is not `installed` [<b>Auto</b>]|
|2.2.9|||| Ensure `TFTP` Server is not `installed` [<b>Auto</b>]|
|2.2.10 |||| Ensure a web server is not `installed` [<b>Auto</b>]|
|2.2.11 |||| Ensure `IMAP` and POP3 server is not `installed` [<b>Auto</b>]|
|2.2.12 |||| Ensure `Samba` is not `installed` [<b>Auto</b>]|
|2.2.13 |||| Ensure `HTTP Proxy Server` is not `installed` [<b>Auto</b>]|
|2.2.14 |||| Ensure `net-snmp` is not `installed` [<b>Auto</b>]|
|2.2.15 |||| Ensure `NIS` server is not `installed` [<b>Auto</b>]|
|2.2.16 |||| Ensure `telnet-server` is not `installed` [<b>Auto</b>]|
|2.2.17 |||| Ensure mail transfer agent is configured for local-only mode [<b>Auto</b>]|
|2.2.18 |||| Ensure `nfs-utils` is not `installed` or the nfs-server service is masked [<b>Auto</b>]|
|2.2.19 |||| Ensure `rpcbind` is not `installed` or the `rpcbind` services are masked [<b>Auto</b>]|
|2.2.20 |||| Ensure `rsync` is not `installed` or the `rsyncd` service is masked [<b>Auto</b>]|
|<b>`2.3`</b>|||| <b>`Service Clients`</b>|
|2.3.1|||| Ensure `NIS` Client is not `installed` [<b>Auto</b>]|
|2.3.2|||| Ensure `rsh` client is not `installed` [<b>Auto</b>]|
|2.3.3|||| Ensure `talk` client is not `installed` [<b>Auto</b>]|
|2.3.4|||| Ensure `telnet` client is not `installed` [<b>Auto</b>]|
|2.3.5|||| Ensure LDAP client is not `installed` [<b>Auto</b>]|
|2.3.6|||| Ensure `TFTP` client is not `installed` [<b>Auto</b>]|
|2.4|||| Ensure nonessential services are removed or masked [<b>Manual</b>]|
|<b>`3`</b>|||| <b>`Network Configuration`</b>|
|<b>`3.1`</b>|||| <b>`Disable unused network protocols and devices`</b>|
|3.1.1|||| Verify if IPv6 is enabled on the system [<b>Manual</b>]|
|3.1.2|||| Ensure SCTP is `disabled` [<b>Auto</b>]|
|3.1.3|||| Ensure DCCP is `disabled` [<b>Auto</b>]|
|3.1.4|||| Ensure wireless interfaces are `disabled` [<b>Auto</b>]|
|<b>`3.2`</b>|||| <b>`Network Parameters (Host Only)`</b>|
|3.2.1|||| Ensure IP forwarding is `disabled` [<b>Auto</b>]|
|3.2.2|||| Ensure packet redirect sending is `disabled` [<b>Auto</b>]|
|<b>`3.3`</b>|||| <b>`Network Parameters (Host and Router)`</b>|
|3.3.1|||| Ensure source routed packets are not accepted [<b>Auto</b>]|
|3.3.2|||| Ensure `ICMP` redirects are not accepted [<b>Auto</b>]|
|3.3.3|||| Ensure secure `ICMP` redirects are not accepted [<b>Auto</b>]|
|3.3.4|||| Ensure suspicious packets are logged [<b>Auto</b>]|
|3.3.5|||| Ensure broadcast `ICMP` requests are ignored [<b>Auto</b>]|
|3.3.6|||| Ensure bogus `ICMP` responses are ignored [<b>Auto</b>]|
|3.3.7|||| Ensure Reverse Path Filtering is enabled [<b>Auto</b>]|
|3.3.8|||| Ensure TCP SYN Cookies is enabled [<b>Auto</b>]|
|3.3.9|||| Ensure IPv6 router advertisements are not accepted [<b>Auto</b>]|
|<b>`3.4`</b>|||| <b>`Firewall Configuration`</b>|
|<b>`3.4.1`</b>|||| <b>`Configure firewalld`</b>|
|3.4.1.1|||| Ensure firewalld is `installed` [<b>Auto</b>]|
|3.4.1.2|||| Ensure iptables-services not `installed` with firewalld [<b>Auto</b>]|
|3.4.1.3|||| Ensure nftables either not `installed` or masked with firewalld [<b>Auto</b>]|
|3.4.1.4|||| Ensure firewalld service enabled and running [<b>Auto</b>]|
|3.4.1.5|||| Ensure firewalld default zone is set [<b>Auto</b>]|
|3.4.1.6|||| Ensure network interfaces are assigned to appropriate zone [<b>Manual</b>]|
|3.4.1.7|||| Ensure firewalld drops unnecessary services and ports [<b>Manual</b>]|
|<b>`3.4.2`</b>|||| <b>`Configure nftables`</b>|
|3.4.2.1|||| Ensure nftables is `installed` [<b>Auto</b>]|
|3.4.2.2|||| Ensure firewalld is either not `installed` or masked with nftables [<b>Auto</b>]|
|3.4.2.3|||| Ensure iptables-services not `installed` with nftables [<b>Auto</b>]|
|3.4.2.4|||| Ensure iptables are flushed with nftables [<b>Manual</b>]|
|3.4.2.5|||| Ensure an nftables table exists [<b>Auto</b>]|
|3.4.2.6|||| Ensure nftables base chains exist [<b>Auto</b>]|
|3.4.2.7|||| Ensure nftables loopback traffic is configured [<b>Auto</b>]|
|3.4.2.8|||| Ensure nftables outbound and established connections are configured [<b>Manual</b>]|
|3.4.2.9|||| Ensure nftables default deny firewall policy [<b>Auto</b>]|
|3.4.2.10|||| Ensure nftables service is enabled [<b>Auto</b>]|
|3.4.2.11|||| Ensure nftables rules are permanent [<b>Auto</b>]|
|<b>`3.4.3`</b>|||| <b>`Configure iptables`</b>|
|<b>`3.4.3.1`</b>|||| <b>`Configure iptables software`</b>|
|3.4.3.1.1 |||| Ensure iptables packages are `installed` [<b>Auto</b>]|
|3.4.3.1.2 |||| Ensure nftables is not `installed` with iptables [<b>Auto</b>]|
|3.4.3.1.3 |||| Ensure firewalld is either not `installed` or masked with iptables [<b>Auto</b>]|
|<b>`3.4.3.2`</b>|||| <b>`Configure IPv4 iptables`</b>|
|3.4.3.2.1 |||| Ensure iptables loopback traffic is configured [<b>Auto</b>]|
|3.4.3.2.2 |||| Ensure iptables outbound and established connections are configured [<b>Manual</b>]|
|3.4.3.2.3 |||| Ensure iptables rules exist for all open ports [<b>Auto</b>]|
|3.4.3.2.4 |||| Ensure iptables default deny firewall policy [<b>Auto</b>]|
|3.4.3.2.5 |||| Ensure iptables rules are saved [<b>Auto</b>]|
|3.4.3.2.6 |||| Ensure iptables is enabled and active [<b>Auto</b>]|
|<b>`3.4.3.3`</b>|||| <b>`Configure IPv6 ip6tables`</b>|
|3.4.3.3.1 |||| Ensure ip6tables loopback traffic is configured [<b>Auto</b>]|
|3.4.3.3.2 |||| Ensure ip6tables outbound and established connections are configured [<b>Manual</b>]|
|3.4.3.3.3 |||| Ensure ip6tables firewall rules exist for all open ports [<b>Auto</b>]|
|3.4.3.3.4 |||| Ensure ip6tables default deny firewall policy [<b>Auto</b>]|
|3.4.3.3.5 |||| Ensure ip6tables rules are saved [<b>Auto</b>]|
|3.4.3.3.6 |||| Ensure ip6tables is enabled and active [<b>Auto</b>]|
|<b>`4`</b>|||| <b>`Logging and Auditing`</b>|
|<b>`4.1`</b>|||| <b>`Configure System Accounting (auditd)`</b>|
|<b>`4.1.1`</b>|||| <b>`Ensure auditing is enabled`</b>|
|4.1.1.1|||| Ensure auditd is `installed` [<b>Auto</b>]|
|4.1.1.2|||| Ensure auditd service is enabled [<b>Auto</b>]|
|4.1.1.3|||| Ensure auditing for processes that start prior to auditd is enabled [<b>Auto</b>]|
|4.1.1.4|||| Ensure audit_backlog_limit is sufficient [<b>Auto</b>]|
|<b>`4.1.2`</b>|||| <b>`Configure Data Retention`</b>|
|4.1.2.1|||| Ensure audit log storage size is configured [<b>Auto</b>]|
|4.1.2.2|||| Ensure audit logs are not automatically deleted [<b>Auto</b>]|
|4.1.2.3|||| Ensure system is `disabled` when audit logs are full [<b>Auto</b>]|
|<b>`4.1.3`</b>|||| <b>`Configure auditd rules`</b>|
|4.1.3.1|||| Ensure changes to system `administration` scope (sudoers) is collected [<b>Auto</b>]|
|4.1.3.2|||| Ensure actions as another user are always logged [<b>Auto</b>]|
|4.1.3.3|||| Ensure events that modify the sudo log file are collected [<b>Auto</b>]|
|4.1.3.4|||| Ensure events that modify date and `time` information are collected [<b>Auto</b>]|
|4.1.3.5|||| Ensure events that modify the system's network environment are collected [<b>Auto</b>]|
|4.1.3.6|||| Ensure use of privileged commands are collected [<b>Auto</b>]|
|4.1.3.7|||| Ensure unsuccessful file access attempts are collected [<b>Auto</b>]|
|4.1.3.8|||| Ensure events that modify user/group information are collected [<b>Auto</b>]|
|4.1.3.9|||| Ensure discretionary access control permission modification events are collected [<b>Auto</b>]|
|4.1.3.10|||| Ensure successful file system mounts are collected [<b>Auto</b>]|
|4.1.3.11|||| Ensure session initiation information is collected [<b>Auto</b>]|
|4.1.3.12|||| Ensure login and logout events are collected [<b>Auto</b>]|
|4.1.3.13|||| Ensure file deletion events by users are collected [<b>Auto</b>]|
|4.1.3.14|||| Ensure events that modify the system's Mandatory Access Controls are collected [<b>Auto</b>]|
|4.1.3.15|||| Ensure successful and unsuccessful attempts to use the chcon command are recorded [<b>Auto</b>]|
|4.1.3.16|||| Ensure successful and unsuccessful attempts to use the setfacl command are recorded [<b>Auto</b>]|
|4.1.3.17|||| Ensure successful and unsuccessful attempts to use the chacl command are recorded [<b>Auto</b>]|
|4.1.3.18|||| Ensure successful and unsuccessful attempts to use the usermod command are recorded [<b>Auto</b>]|
|4.1.3.19|||| Ensure kernel module loading unloading and modification is collected [<b>Auto</b>]|
|4.1.3.20|||| Ensure the audit configuration is immutable [<b>Auto</b>]|
|4.1.3.21|||| Ensure the running and on disk configuration is the same [<b>Manual</b>]|
|<b>`4.2`</b>|||| <b>`Configure Logging`</b>|
|<b>`4.2.1`</b>|||| <b>`Configure rsyslog`</b>|
|4.2.1.1|||| Ensure rsyslog is `installed` [<b>Auto</b>]|
|4.2.1.2|||| Ensure rsyslog service is enabled [<b>Auto</b>]|
|4.2.1.3|||| Ensure journald is configured to send logs to rsyslog [<b>Manual</b>]|
|4.2.1.4|||| Ensure rsyslog default file `permissions` are configured [<b>Auto</b>]|
|4.2.1.5|||| Ensure logging is configured [<b>Manual</b>]|
|4.2.1.6|||| Ensure rsyslog is configured to send logs to a remote log host [<b>Manual</b>]|
|4.2.1.7|||| Ensure rsyslog is not configured to recieve logs from a remote client [<b>Auto</b>]|
|<b>`4.2.2`</b>|||| <b>`Configure journald`</b>|
|4.2.2.1|||| Ensure journald is configured to send logs to a remote log host|
|4.2.2.1.1 |||| Ensure systemd-journal-remote is `installed` [<b>Manual</b>]|
|4.2.2.1.2 |||| Ensure systemd-journal-remote is configured [<b>Manual</b>]|
|4.2.2.1.3 |||| Ensure systemd-journal-remote is enabled [<b>Manual</b>]|
|4.2.2.1.4 |||| Ensure journald is not configured to recieve logs from a remote client [<b>Auto</b>]|
|4.2.2.2|||| Ensure journald service is enabled [<b>Auto</b>]|
|4.2.2.3|||| Ensure journald is configured to compress large log files [<b>Auto</b>]|
|4.2.2.4|||| Ensure journald is configured to write logfiles to persistent disk [<b>Auto</b>]|
|4.2.2.5|||| Ensure journald is not configured to send logs to rsyslog [<b>Manual</b>]|
|4.2.2.6|||| Ensure journald log rotation is configured per site policy [<b>Manual</b>]|
|4.2.2.7|||| Ensure journald default file `permissions` configured [<b>Manual</b>]|
|4.2.3|||| Ensure `permissions` on all logfiles are configured [<b>Auto</b>]|
|4.3|||| Ensure logrotate is configured [<b>Manual</b>]|
|<b>`5`</b>|||| <b>`Access, Authentication and Authorization`</b>|
|<b>`5.1`</b>|||| <b>`Configure time-based job schedulers`</b>|
|5.1.1|||| Ensure `cron` daemon is enabled [<b>Auto</b>]|
|5.1.2|||| Ensure `permissions` on `/etc/crontab` are configured [<b>Auto</b>]|
|5.1.3|||| Ensure `permissions` on `/etc/cron.hourly` are configured [<b>Auto</b>]|
|5.1.4|||| Ensure `permissions` on `/etc/cron.daily` are configured [<b>Auto</b>]|
|5.1.5|||| Ensure `permissions` on `/etc/cron.weekly` are configured [<b>Auto</b>]|
|5.1.6|||| Ensure `permissions` on `/etc/cron.monthly` are configured [<b>Auto</b>]|
|5.1.7|||| Ensure `permissions` on `/etc/cron.d` are configured [<b>Auto</b>]|
|5.1.8|||| Ensure `cron` is restricted to authorized users [<b>Auto</b>]|
|5.1.9|||| Ensure at is restricted to authorized users [<b>Auto</b>]|
|<b>`5.2`</b>|||| <b>`Configure SSH Server`</b>|
|5.2.1|||| Ensure `permissions` on `/etc/ssh```/`ssh`d_config are configured [<b>Auto</b>]|
|5.2.2|||| Ensure `permissions` on `SSH` private host key files are configured [<b>Auto</b>]|
|5.2.3|||| Ensure `permissions` on `SSH` public host key files are configured [<b>Auto</b>]|
|5.2.4|||| Ensure `SSH` access is limited [<b>Auto</b>]|
|5.2.5|||| Ensure `SSH` LogLevel is appropriate [<b>Auto</b>]|
|5.2.6|||| Ensure `SSH` PAM is enabled [<b>Auto</b>]|
|5.2.7|||| Ensure `SSH` root login is `disabled` [<b>Auto</b>]|
|5.2.8|||| Ensure `SSH` HostbasedAuthentication is `disabled` [<b>Auto</b>]|
|5.2.9|||| Ensure `SSH` PermitEmptyPasswords is `disabled` [<b>Auto</b>]|
|5.2.10 |||| Ensure `SSH` PermitUserEnvironment is `disabled` [<b>Auto</b>]|
|5.2.11 |||| Ensure `SSH` IgnoreRhosts is enabled [<b>Auto</b>]|
|5.2.12 |||| Ensure `SSH` X11 forwarding is `disabled` [<b>Auto</b>]|
|5.2.13 |||| Ensure `SSH` AllowTcpForwarding is `disabled` [<b>Auto</b>]|
|5.2.14 |||| Ensure system-wide crypto policy is not over-ridden [<b>Auto</b>]|
|5.2.15 |||| Ensure `SSH` warning banner is configured [<b>Auto</b>]|
|5.2.16 |||| Ensure `SSH` MaxAuthTries is set to 4 or less [<b>Auto</b>]|
|5.2.17 |||| Ensure `SSH` MaxStartups is configured [<b>Auto</b>]|
|5.2.18 |||| Ensure `SSH` MaxSessions is set to 10 or less [<b>Auto</b>]|
|5.2.19 |||| Ensure `SSH` LoginGraceTime is set to one minute or less [<b>Auto</b>]|
|5.2.20 |||| Ensure `SSH` Idle Timeout Interval is configured [<b>Auto</b>]|
|<b>`5.3`</b>|||| <b>`Configure privilege escalation`</b>|
|5.3.1|||| Ensure sudo is `installed` [<b>Auto</b>]|
|5.3.2|||| Ensure sudo commands use pty [<b>Auto</b>]|
|5.3.3|||| Ensure sudo log file exists [<b>Auto</b>]|
|5.3.4|||| Ensure users must provide password for escalation [<b>Auto</b>]|
|5.3.5|||| Ensure re-authentication for privilege escalation is not `disabled` globally [<b>Auto</b>]|
|5.3.6|||| Ensure sudo authentication timeout is configured correctly [<b>Auto</b>]|
|5.3.7|||| Ensure access to the su command is restricted [<b>Auto</b>]|
|<b>`5.4`</b>|||| <b>`Configure authselect`</b>|
|5.4.1|||| Ensure custom authselect profile is used [<b>Manual</b>]|
|5.4.2|||| Ensure authselect includes with-faillock [<b>Auto</b>]|
|<b>`5.5`</b>|||| <b>`Configure PAM`</b>|
|5.5.1|||| Ensure password creation requirements are configured [<b>Auto</b>]|
|5.5.2|||| Ensure lockout for failed password attempts is configured [<b>Auto</b>]|
|5.5.3|||| Ensure password reuse is limited [<b>Auto</b>]|
|5.5.4|||| Ensure password hashing algorithm is SHA-512 [<b>Auto</b>]|
|<b>`5.6`</b>|||| <b>`User Accounts and Environment`</b>|
|<b>`5.6.1`</b>|||| <b>`Set Shadow Password Suite Parameters`</b>|
|5.6.1.1|||| Ensure password expiration is 365 days or less [<b>Auto</b>]|
|5.6.1.2|||| Ensure minimum days between password changes is 7 or more [<b>Auto</b>]|
|5.6.1.3|||| Ensure password expiration warning days is 7 or more [<b>Auto</b>]|
|5.6.1.4|||| Ensure inactive password lock is 30 days or less [<b>Auto</b>]|
|5.6.1.5|||| Ensure all users last password change date is in the past [<b>Auto</b>]|
|5.6.2|||| Ensure system accounts are secured [<b>Auto</b>]|
|5.6.3|||| Ensure default user shell timeout is 900 seconds or less [<b>Auto</b>]|
|5.6.4|||| Ensure default group for the root account is GID 0 [<b>Auto</b>]|
|5.6.5|||| Ensure default user umask is 027 or more restrictive [<b>Auto</b>]|
|<b>`6`</b>|||| <b>`System Maintenance`</b>|
|<b>`6.1`</b>|||| <b>`System File Permissions```</b>|
|6.1.1|||| Audit system file `permissions` [<b>Manual</b>]|
|6.1.2|||| Ensure sticky bit is set on all world-writable directories [<b>Auto</b>]|
|6.1.3|||| Ensure `permissions` `on /etc/passwd` are configured [<b>Auto</b>]|
|6.1.4|||| Ensure `permissions` `on /etc/shadow` are configured [<b>Auto</b>]|
|6.1.5|||| Ensure `permissions` `on /etc/group` are configured [<b>Auto</b>]|
|6.1.6|||| Ensure `permissions` `on /etc/gshadow` are configured [<b>Auto</b>]|
|6.1.7|||| Ensure `permissions` on `/etc/passwd`- are configured [<b>Auto</b>]|
|6.1.8|||| Ensure `permissions` on `/etc/shadow`- are configured [<b>Auto</b>]|
|6.1.9|||| Ensure `permissions` on `/etc/group`- are configured [<b>Auto</b>]|
|6.1.10 |||| Ensure `permissions` on `/etc/gshadow`- are configured [<b>Auto</b>]|
|6.1.11 |||| Ensure no world writable files exist [<b>Auto</b>]|
|6.1.12 |||| Ensure no unowned files or directories exist [<b>Auto</b>]|
|6.1.13 |||| Ensure no ungrouped files or directories exist [<b>Auto</b>]|
|6.1.14 |||| Audit SUID executables [<b>Manual</b>]|
|6.1.15 |||| Audit SGID executables [<b>Manual</b>]|
|<b>`6.2`</b>|||| <b>`User and Group Settings`</b>|
|6.2.1|||| Ensure password fields are not empty [<b>Auto</b>]|
|6.2.2|||| Ensure all groups `in /etc/passwd` exist `in /etc/group` [<b>Auto</b>]|
|6.2.3|||| Ensure no duplicate UIDs exist [<b>Auto</b>] |
|6.2.4|||| Ensure no duplicate GIDs exist [<b>Auto</b>] |
|6.2.5|||| Ensure no duplicate user names exist [<b>Auto</b>]|
|6.2.6|||| Ensure no duplicate group names exist [<b>Auto</b>]|
|6.2.7|||| Ensure root PATH Integrity [<b>Auto</b>]|
|6.2.8|||| Ensure root is the only UID 0 account [<b>Auto</b>]|
|6.2.9|||| Ensure all users' home directories exist [<b>Auto</b>]|
|6.2.10 |||| Ensure users own their home directories [<b>Auto</b>] |
|6.2.11 |||| Ensure users' home directories `permissions` are 750 or more restrictive [<b>Auto</b>]|
|6.2.12 |||| Ensure users' dot files are not group or world writable[<b>Auto</b>]|
|6.2.13 |||| Ensure users' .netrc Files are not group or world accessible [<b>Auto</b>]|
|6.2.14 |||| Ensure no users have .forward files [<b>Auto</b>]|
|6.2.15 |||| Ensure no users have .netrc files [<b>Auto</b>]|
|6.2.16 |||| Ensure no users have .rhosts files [<b>Auto</b>]|