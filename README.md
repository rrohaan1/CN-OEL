# Integrated Network Systems: Smart Transportation & Enterprise NAT Analysis

This repository contains a comprehensive two-part network infrastructure project designed for the **Fall 2025 Open Ended Lab (CS260L)**. The system demonstrates advanced skills in network segmentation, access control, and dynamic NAT translations for the BSCY program.

## 🚦 Task 1: Smart Transportation Segmentation & Control
Designed for a metropolitan transport authority to manage city-wide smart infrastructure with logical isolation.

### Core Implementation
- **VLAN Segmentation:** Organized devices into operational roles including Traffic Control (VLAN 10), Surveillance (VLAN 20), Payment (VLAN 30), Emergency (VLAN 40), and Management (VLAN 99).
- **Emergency Override Performance:** Implemented a specialized priority protocol where emergency traffic bypasses standard authentication loops for zero-latency communication.
- **Topology Map:**
![Smart Transportation Map](Screenshot%202026-02-02%20144835.png)

---

## 🏦 Task 2: Enterprise Internet Access & NAT Analysis
A sophisticated enterprise internet access system connecting multiple global branches to a Public Cloud using NAT analysis.

### Core Implementation
- **Dynamic NAT with Overload (PAT):** Implemented to allow multiple internal hosts from Branch LANs to access external services (8.8.8.8) using a single Public IP (200.1.1.2).
- **Session Integrity:** Managed through a Border Router to maintain transaction success counts and prevent translation conflicts.
- **Topology Map:**
![Enterprise Edge Map](Screenshot%202026-02-02%20150627.png)

---

## ✅ Diagnostics & Verification (Lab Deliverables)
Per the lab requirements, the following diagnostic outputs verify inter-segment communication, broadcast containment, and NAT translation success.

### Diagnostic Output 1: Task 1 Verification
Verifies allowed and denied traffic paths across the smart transportation zones.
![Task 1 Ping Verification](Screenshot%202026-02-02%20145042.png)

### Diagnostic Output 2: Task 2 Verification
Verifies translation efficiency and connectivity from Branch LANs to the Public Cloud.
![Task 2 Ping Verification](Screenshot%202026-02-02%20150748.png)

---

## 📂 Repository Contents
- **OEL.pkt:** The complete integrated Cisco Packet Tracer simulation file.
- **Screenshots/:** Full-screen diagnostic and configuration summaries as required by the lab.
