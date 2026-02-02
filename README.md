# Integrated Network Systems: Smart Transportation & Enterprise NAT Analysis

This repository contains a comprehensive two-part network infrastructure project designed for the **Fall 2025 Open Ended Lab (CS260L)**. The system demonstrates advanced skills in network segmentation, access control, and dynamic NAT translations.

---

## 🚦 Task 1: Smart Transportation Segmentation & Control
Designed for a metropolitan transport authority to manage a city-wide smart infrastructure.

### Core Implementation
* **VLAN Segmentation**: Organizes devices into logical roles: Traffic Control (VLAN 10), Surveillance (VLAN 20), Payment (VLAN 30), Emergency (VLAN 40), and Management (VLAN 99).
* **Inter-Segment Routing**: Controlled communication between segments using sub-interfaces and inter-VLAN routing.
* **Emergency Bypass Protocol**: A specialized metric where emergency override traffic is prioritized and bypasses standard authentication loops.

### Task 1 Design (Topology)
![Smart Transportation Map](Screenshot%202026-02-02%20144835.png)

### Diagnostic Output 1: Task 1 Verification
* **Verified**: Success counts across control zones and broadcast containment effectiveness.
* **Verified**: Allowed and denied traffic paths through Access Control Lists (ACLs).
![Task 1 Success Ping](Screenshot%202026-02-02%20145042.png)

---

## 🏦 Task 2: Enterprise Internet Access & NAT Analysis
An international financial services simulation connecting multiple global branches to a Public Cloud.

### Core Implementation
* **Dynamic NAT with Overload (PAT)**: Implemented to allow multiple internal hosts from Branch LANs to access external services (8.8.8.8) using a single Public IP (200.1.1.2).
* **Session Integrity**: Managed through a Border Router to maintain transaction success counts and prevent translation conflicts.

### Task 2 Design (Topology)
![Enterprise Edge Map](Screenshot%202026-02-02%20150627.png)

### Diagnostic Output 2: Task 2 Verification
* **Verified**: NAT translation efficiency and successful connectivity from Branch LANs to the Public Cloud.
![Task 2 Success Ping](Screenshot%202026-02-02%20150748.png)

---

## 📂 Repository Contents
* `OEL.pkt`: The full integrated simulation file covering both Task 1 and Task 2.
* `README.md`: Detailed project analysis and technical summary.
