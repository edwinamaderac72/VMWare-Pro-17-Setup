# Windows Server Lab

## Overview
A home lab with 2 Domain Controllers, DNS, DHCP, and a Windows 11 domain-joined client.

## Network Topology
![Network Diagram](diagrams/Network_Diagram.JPG)

## Screenshots
### Active Directory Structure
Domain Controllers
![Domain Controllers](screenshots/2.jpg)
Users
![Users](screenshots/3.jpg)
Computers
![Computers](screenshots/4.jpg)
GPO for User
![GPO](screenshots/7GPO.jpg)
#### Windows 11 Client
![Client](screenshots/6Client.jpg)

### DHCP Pool
![DHCP](screenshots/5DHCP.jpg)
### DNS Pool
![DNS](screenshots/5DNS.jpg)

### GPO for Firewall and general config
Configs
![Configs](screenshots/Configs.jpg)
Firewall
![Firewall](configs/firewal/firewall.md)

## Technologies Used
- VMWare Workstation Pro 17
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS Server
- DHCP Server
- Windows 11 Client

## Troubleshooting 
 * Solve DNS not showing on Win11 Client

## Future changes
* Stop using Administrator user
* Add another client
* Push more GPO's
