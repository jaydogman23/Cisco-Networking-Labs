# 🔐 Cisco Port Security Lab

## 📌 Overview
This lab demonstrates how **Cisco Switch Port Security** is used to control access to switch interfaces by limiting and securing MAC addresses. The lab explores different violation modes and shows how switches respond to unauthorized devices.
This lab focuses on enforcing Layer 2 security controls to prevent unauthorized device access and MAC flooding attacks.
The lab was designed and tested using **Cisco Packet Tracer** with **Cisco 2960 switches** and aligns with **CCNA-level networking and security concepts**.

---

## 🎯 Learning Objectives
- Configure port security on access ports
- Limit the number of MAC addresses allowed on a port
- Use **sticky MAC address learning**
- Compare **shutdown** and **restrict** violation modes
- Observe and recover from **err-disabled** states
- Verify port security using IOS commands

---

## 🧰 Lab Environment
- Cisco Packet Tracer
- Cisco 2960-24TT switches
- FastEthernet interfaces
- Copper crossover cables
- Access mode interfaces only

---

## 🔒 Scenario 1: Port Security (Maximum 4 MAC Addresses – Shutdown Mode)

### Configuration
```bash
interface fa0/1
 switchport mode access
 switchport port-security
 switchport port-security maximum 4
 switchport port-security violation shutdown
