# Integrated Network Systems: Smart Transportation & Enterprise NAT Analysis

This repository contains a comprehensive two-part network infrastructure project designed for the **Fall 2025 Open Ended Lab (CS260L)**. The system demonstrates advanced skills in network segmentation, access control, and dynamic NAT translations.

## 🚦 Task 1: Smart Transportation Segmentation & Control
Designed for a metropolitan transport authority to manage a city-wide smart infrastructure.

### Core Implementation
- **VLAN Segmentation:** Organizes devices into logical roles: Traffic Control (VLAN 10), Surveillance (VLAN 20), Payment (VLAN 30), Emergency (VLAN 40), and Management (VLAN 99).
- **Inter-Segment Routing:** Controlled communication between segments using sub-interfaces and inter-VLAN routing.
- **Emergency Bypass Protocol:** A specialized metric where emergency override traffic is prioritized and bypasses standard authentication loops.
- **Access Control:** Implemented ACLs to verify allowed and denied traffic paths, ensuring critical subsystems remain isolated from unauthorized access.

### Diagnostics & Validation
- **Broadcast Containment:** Verified effectiveness of VLANs in isolating broadcast traffic.
- **Traffic Isolation:** Monitoring success/failure counts across control zones.
- **Topology Map:**
![Smart Transportation Map](Screenshot%202026-02-02%20144835.png)

---

## 🏦 Task 2: Enterprise Internet Access & NAT Analysis
An international financial services simulation connecting multiple global branches to a Public Cloud.

### Core Implementation
- **Inside/Outside Addressing:** Clear separation of internal private branch roles and external public network roles.
- **NAT with Overload (PAT):** Configured Dynamic NAT with Overload to support concurrent traffic from multiple branches using a single Public IP (200.1.1.2).
- **Enterprise Edge:** A Border Router manages the translation table and maintains session integrity under peak loads.
- **Cloud Integration:** End-to-end connectivity verified from Branch LANs to the Public Cloud Server (8.8.8.8).

### Performance Metrics
- **NAT Translation Tables:** Monitoring active port utilization and translation efficiency.
- **Scalability Analysis:** Evaluated behavior under concurrent traffic loads from Branch 1, 2, and 3.
- **Topology Map:**
![Enterprise Edge Map](Screenshot%202026-02-02%20150627.png)

---

## 🛠️ Technical Specifications & Deliverables
- **Software:** Cisco Packet Tracer (v8.2+)
- **Configurations Included:** VLAN Trunking (802.1Q), OSPF/Static Routing, Access Control Lists (ACLs), and NAT Overload.
- **Verification:**
![Connectivity Proof](Screenshot%202026-02-02%20145042.png)

## 📂 Files in this Repository
- `OEL.pkt`: The full integrated simulation file covering both Task 1 and Task 2.
- `README.md`: Detailed project analysis and technical summary.
