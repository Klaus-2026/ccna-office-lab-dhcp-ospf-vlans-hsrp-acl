# ccna-office-lab-dhcp-ospf-vlans-hsrp-acl
## Overview
Office Network with 6-Vlan, OSPF, DHCP, HSRP, ACLs, Wifi
## Topology
![Topology and Objectives.png](https://github.com/Klaus-2026/ccna-office-lab-dhcp-ospf-vlans-hsrp-acl/blob/main/Topology%20and%20Objectives.png)
## Features
Vlans: Mgmt(10), MKG(20), HR(30), IT(40), RTL(50), Guest_Wifi(60)

OSPF: ID 1 Area 0 with network 20.20.20.0/24 and Router A as default-information originate

DHCP: Router A -> Vlan 10 - 40; Router B -> Vlan 50 & 60

HSRP: Router A primary for Vlan 10 - 40 and secondary for Vlan 50 & 60; Router B primary for 50 & 60 and secondary for Vlan 10 - 40; Virtual IP 192.168.#vlan.254

ACL: Preventing any form of connection between Vlan 60 and FTP server
