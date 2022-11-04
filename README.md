# CortexXDR-Profiles
Ready to import Cortex XDR profiles:
|os|[Agent Settings](#agent-settings)|[Malware Protection](#malware-protection)|[Exploit Protection](#exploit-protection)|[Restriction Profile](#restriction-profile)|
|-------|---------------------------|-------------------------------|-------------------------------|--------------------------------|
|**Win**|[INT] Windows AgentSettings|[INT] Windows MalwareProtection|[INT] Windows ExploitProtection|[INT] Windows RestrictionProfile|
|**mac**|[INT] macOS AgentSettings|[INT] macOS MalwareProtection|[INT] macOS ExploitProtection|*default - nothing to change*|
|***nix**|[INT] Linux AgentSettings|[INT] Linux MalwareProtection|[INT] Linux ExploitProtection|*default - nothing to change*|

## Agent Settings
- [x] **Agent Auto-Upgrade** [Windows|macOS|Linux]
- [x] **Monitor and Collect enhanced application logs** [Windows|macOS|Linux]
- - *[Endpoint data collected by Cortex XDR](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-pro-admin/endpoint-security/customizable-agent-settings/endpoint-data-collected-by-cortex-xdr)*
- [x] **Agent Operation :: _Kernel_** [Linux] 
- - *[Options: (User Space|Kernel)](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-pro-admin/endpoint-security/customizable-agent-settings/add-agent-settings-profile#id17AHKE0N00P_id8dc924cc-2be3-4b26-895e-30e59bc443ce)*
- [x] **Compliance Collection** [Linux] 
- - *[Based on CIS benchmarks. (Missing documentation for this feature)](https://live.paloaltonetworks.com/t5/cortex-xdr-discussions/compliance-dashboard/td-p/517226)*
- [ ] **Network Scan** [Windows|macOS|Linux] 
- - *[Depends on 'Network Location Configuration'](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-pro-admin/endpoint-security/customizable-agent-settings/add-agent-settings-profile#id17AHKE0N00P_id8dc924cc-2be3-4b26-895e-30e59bc443ce)*

## Malware Protection
- [x] **Quarantine Malicious Files**:
- - [x] **Executable and DLL files** [Windows]
- - [x] **Global Behavioral Threat Protection Rules: _built-in OS executables and common administration utilities_** [Windows]
- - [x] **Credential Gathering Protection: _processes trying to access/steal passwords_** [Windows]
- - [x] **Anti Webshell Protection: _processes dropping malicious webshells_** [Windows]
- - [x] **Ransomware Protection: _encryption based activity_** [Windows]
- - [x] **Mach-O Files** [macOS]
- - [x] **ELF Files** [Linux]
- - [x] **Local File Threat: _malicious non-ELF files, such as scripts_** [Linux]
- - *[Manage Quarantined Files](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-pro-admin/investigation-and-response/investigate-files/manage-quarantined-files)*
- [x] **Endpoint Scanning: _Weekly, Sunday 00:00_** [Windows|macOS|Linux]
- - [x] **Scan Removable drives** [Windows|Linux]
- - *[Scan Endpoint for Malware](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-prevent-admin/investigation-and-response/investigate-endpoints/scan-endpoint-for-malware)*

## Exploit Protection
- [x] **Exploit Protection for Additional Processes**
- **Windows**
- - _msedge.exe_
- **macOS**
- - _nothing yet_
- **Linux**
- - _nothing yet_

## Restriction Settings
- [x] **Network Location Files :: _Notify_** [Windows]
- [x] **Removable Media Files :: _Notify_** [Windows]
- [x] **Optical Drive Files :: _Notify_** [Windows]
- *[Restriction Profile Settings](https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-pro-admin/endpoint-security/endpoint-security-profiles/add-restrictions-profile#id17CUM0O0EJH_id2ccede29-5c5c-4429-85e4-aa40fbea5215)*
