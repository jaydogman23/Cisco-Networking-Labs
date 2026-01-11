# OSPF & DHCP Enterprise Routing Lab

## Overview
This lab simulates a small enterprise network using Cisco Packet Tracer. It demonstrates dynamic routing with OSPF, centralized DHCP services, secure switch access, and best-practice subnetting.

---

## Topology Summary
- 2 Routers running OSPF Area 0
- 2 Access Switches
- Centralized DHCP Server
- /30 Point-to-Point WAN link
- SSH-only device management
- Port security on access ports

---

## Technologies Demonstrated
- OSPF (Area 0)
- /30 Point-to-Point Subnetting
- DHCP with IP Helper Address
- Port Security (Sticky MAC, Restrict Mode)
- SSH-only VTY access
- Local authentication & exec-timeout

---

## IP Addressing

| Network | Purpose |
|-------|--------|
| 192.168.10.0/24 | LAN 1 |
| 192.168.20.0/24 | LAN 2 |
| 10.0.0.0/30 | Router-to-Router Link |

---

## Verification Commands
```bash
show ip ospf neighbor
show ip route ospf
show ip dhcp binding
show port-security interface fa0/2
