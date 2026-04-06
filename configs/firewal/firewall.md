# Firewall GPO — MAHOGANY.LOCAL
> **GPO:** Firewall  
> **Domain:** MAHOGANY.LOCAL  
> **Owner:** MAHOGANY\Domain Admins  
> **Created:** 3/11/2026  
> **Modified:** 3/11/2026  
> **Status:** Enabled
---
## Computer Configuration
### Windows Firewall with Advanced Security
#### Global Settings
| Policy | Setting |
|--------|--------|
| Policy version | 2.31 |
| Disable stateful FTP | Not Configured |
| Disable stateful PPTP | Not Configured |
| IPsec exempt | Not Configured |
| IPsec through NAT | Not Configured |
| Preshared key encoding | Not Configured |
| SA idle time | Not Configured |
| Strong CRL check | Not Configured |

#### Domain Profile Settings
| Policy | Setting |
|--------|--------|
| Firewall state | Off |
| Inbound connections | Allow |
| Outbound connections | Allow |
| Apply local firewall rules | Not Configured |
| Apply local connection security rules | Not Configured |
| Display notifications | Not Configured |
| Allow unicast responses | Not Configured |
| Log dropped packets | Not Configured |
| Log successful connections | Not Configured |
| Log file path | Not Configured |
| Log file maximum size (KB) | Not Configured |

#### Inbound Rules

**Active Directory Domain Services**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| Active Directory Domain Controller - Secure LDAP for Global Catalog (TCP-In) | TCP | 3269Remote | Inbound rule for the Active Directory Domain Controller service to allow remote Secure Global Catalog traffic. [TCP 3269] |
| Active Directory Domain Controller - NetBIOS name resolution (UDP-In) | UDP | 138Remote | Inbound rule for the Active Directory Domain Controller service to allow NetBIOS name resolution. [UDP 138] |
| Active Directory Domain Controller (RPC-EPMAP) | TCP | RPC | Inbound rule for the RPCSS service to allow RPC/TCP traffic to the Active Directory Domain Controller service. |
| Active Directory Domain Controller - W32Time (NTP-UDP-In) | UDP | 123Remote | Inbound rule for the Active Directory Domain Controller service to allow NTP traffic for the Windows Time service. [UDP 123] |
| Active Directory Domain Controller -  Echo Request (ICMPv6-In) | ICMPv6 | AnyRemote | Inbound rule for the Active Directory Domain Controller service to allow Echo requests (ping). |
| Active Directory Domain Controller - LDAP (UDP-In) | UDP | 389Remote | Inbound rule for the Active Directory Domain Controller service to allow remote LDAP traffic. [UDP 389] |
| Active Directory Domain Controller - LDAP (TCP-In) | TCP | 389Remote | Inbound rule for the Active Directory Domain Controller service to allow remote LDAP traffic. [TCP 389] |
| Active Directory Domain Controller (RPC) | TCP | Dynamic | Inbound rule to allow remote RPC/TCP access to the Active Directory Domain Controller service. |
| Active Directory Domain Controller - SAM/LSA (NP-UDP-In) | UDP | 445Remote | Inbound rule for the Active Directory Domain Controller service to be remotely managed over Named Pipes. [UDP 445] |
| Active Directory Domain Controller - SAM/LSA (NP-TCP-In) | TCP | 445Remote | Inbound rule for the Active Directory Domain Controller service to be remotely managed over Named Pipes. [TCP 445] |
| Active Directory Domain Controller - LDAP for Global Catalog (TCP-In) | TCP | 3268Remote | Inbound rule for the Active Directory Domain Controller service to allow remote Global Catalog traffic. [TCP 3268] |
| Active Directory Domain Controller - Secure LDAP (TCP-In) | TCP | 636Remote | Inbound rule for the Active Directory Domain Controller service to allow remote Secure LDAP traffic. [TCP 636] |
| Active Directory Domain Controller -  Echo Request (ICMPv4-In) | ICMPv4 | AnyRemote | Inbound rule for the Active Directory Domain Controller service to allow Echo requests (ping). |

**DHCP Server**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| DHCP Server v6 (UDP-In) | UDP | 546Remote | An inbound rule to allow traffic so that rogue detection works in V6. [UDP 546] |
| DHCP Server v4 (UDP-In) | UDP | 68Remote | An inbound rule to allow traffic so that rogue detection works in V4. [UDP 68] |
| DHCP Server v4 (UDP-In) | UDP | 67Remote | An inbound rule to allow traffic to the IPv4 Dynamic Host Control Protocol Server. [UDP 67] |
| DHCP Server v6 (UDP-In) | UDP | 547Remote | An inbound rule to allow traffic to the IPv6 Dynamic Host Control Protocol Server. [UDP 547] |

**DNS Service**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| DNS (UDP, Incoming) | UDP | 53Remote | Inbound rule to allow remote UDP access to the DNS service. |
| RPC (TCP, Incoming) | TCP | Dynamic | Inbound rule to allow remote RPC/TCP access to the DNS service. |
| RPC Endpoint Mapper (TCP, Incoming) | TCP | RPC | Inbound rule for the RPCSS service to allow RPC/TCP traffic to the DNS Service. |
| DNS (TCP, Incoming) | TCP | 53Remote | Inbound rule to allow remote TCP access to the DNS service. |

**File and Printer Sharing**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| File and Printer Sharing (LLMNR-UDP-In) | UDP | 5355Remote | Inbound rule for File and Printer Sharing to allow Link Local Multicast Name Resolution. [UDP 5355] |
| File and Printer Sharing (NB-Datagram-In) | UDP | 138Remote | Inbound rule for File and Printer Sharing to allow NetBIOS Datagram transmission and reception. [UDP 138] |
| File and Printer Sharing (Echo Request - ICMPv6-In) | ICMPv6 | AnyRemote | Echo Request messages are sent as ping requests to other nodes. |
| File and Printer Sharing (SMB-In) | TCP | 445Remote | Inbound rule for File and Printer Sharing to allow Server Message Block transmission and reception via Named Pipes. [TCP 445] |
| File and Printer Sharing (Echo Request - ICMPv4-In) | ICMPv4 | AnyRemote | Echo Request messages are sent as ping requests to other nodes. |
| File and Printer Sharing (NB-Session-In) | TCP | 139Remote | Inbound rule for File and Printer Sharing to allow NetBIOS Session Service connections. [TCP 139] |
| File and Printer Sharing (Spooler Service - RPC-EPMAP) | TCP | RPC | Inbound rule for the RPCSS service to allow RPC/TCP traffic for the Spooler Service. |
| File and Printer Sharing (NB-Name-In) | UDP | 137Remote | Inbound rule for File and Printer Sharing to allow NetBIOS Name Resolution. [UDP 137] |
| File and Printer Sharing (Spooler Service - RPC) | TCP | Dynamic | Inbound rule for File and Printer Sharing to allow the Print Spooler Service to communicate via TCP/RPC. |

**Windows Management Instrumentation (WMI)**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| Windows Management Instrumentation (DCOM-In) | TCP | 135Remote | Inbound rule to allow DCOM traffic for remote Windows Management Instrumentation. [TCP 135] |
| Windows Management Instrumentation (WMI-In) | TCP | AnyRemote | Inbound rule to allow WMI traffic for remote Windows Management Instrumentation. [TCP] |
| Windows Management Instrumentation (ASync-In) | TCP | AnyRemote | Inbound rule to allow Asynchronous WMI traffic for remote Windows Management Instrumentation. [TCP] |

**Other**

| Rule Name | Protocol | Port | Description |
|-----------|----------|------|-------------|
| Ping | ICMPv4 | AnyRemote |  |

#### Outbound Rules

**Active Directory Domain Services**

| Rule Name | Protocol | Remote Port | Description |
|-----------|----------|-------------|-------------|
| Active Directory Domain Controller (UDP-Out) | UDP | AnyICMP | Outbound rule for the Active Directory Domain Controller service. [UDP] |
| Active Directory Domain Controller -  Echo Request (ICMPv4-Out) | ICMPv4 | AnyICMP | Outbound rule for the Active Directory Domain Controller service to allow Echo requests (ping). |
| Active Directory Domain Controller -  Echo Request (ICMPv6-Out) | ICMPv6 | AnyICMP | Outbound rule for the Active Directory Domain Controller service to allow Echo requests (ping). |
| Active Directory Domain Controller (TCP-Out) | TCP | AnyICMP | Outbound rule for the Active Directory Domain Controller service. [TCP] |

**File and Printer Sharing**

| Rule Name | Protocol | Remote Port | Description |
|-----------|----------|-------------|-------------|
| File and Printer Sharing (LLMNR-UDP-Out) | UDP | 5355ICMP | Outbound rule for File and Printer Sharing to allow Link Local Multicast Name Resolution. [UDP 5355] |
| File and Printer Sharing (NB-Name-Out) | UDP | 137ICMP | Outbound rule for File and Printer Sharing to allow NetBIOS Name Resolution. [UDP 137] |
| File and Printer Sharing (NB-Datagram-Out) | UDP | 138ICMP | Outbound rule for File and Printer Sharing to allow NetBIOS Datagram transmission and reception. [UDP 138] |
| File and Printer Sharing (Echo Request - ICMPv6-Out) | ICMPv6 | AnyICMP | Echo Request messages are sent as ping requests to other nodes. |
| File and Printer Sharing (NB-Session-Out) | TCP | 139ICMP | Outbound rule for File and Printer Sharing to allow NetBIOS Session Service connections. [TCP 139] |
| File and Printer Sharing (SMB-Out) | TCP | 445ICMP | Outbound rule for File and Printer Sharing to allow Server Message Block transmission and reception via Named Pipes. [TCP 445] |
| File and Printer Sharing (Echo Request - ICMPv4-Out) | ICMPv4 | AnyICMP | Echo Request messages are sent as ping requests to other nodes. |

**DNS Service**

| Rule Name | Protocol | Remote Port | Description |
|-----------|----------|-------------|-------------|
| All Outgoing (UDP) | UDP | AnyICMP | Outbound rule to allow all UDP traffic from the DNS service. |
| All Outgoing (TCP) | TCP | AnyICMP | Outbound rule to allow all TCP traffic from the DNS service. |

**Windows Management Instrumentation (WMI)**

| Rule Name | Protocol | Remote Port | Description |
|-----------|----------|-------------|-------------|
| Windows Management Instrumentation (WMI-Out) | TCP | AnyICMP | Outbound rule to allow WMI traffic for remote Windows Management Instrumentation. [TCP] |

#### Connection Security Settings
No connection security rules defined.

### Administrative Templates
#### Network > Windows Defender Firewall > Domain Profile

| Policy | Setting |
|--------|--------|
| Windows Defender Firewall: Protect all network connections | Disabled |

---
## User Configuration
No settings defined.
