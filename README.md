# Computer Networks - Open Ended Lab (OEL)

This repository contains a comprehensive network design featuring automated routing and a specialized **Emergency Traffic Protocol** created in Cisco Packet Tracer.

## 🌐 Network Topology
![Topology Map](Screenshot%202026-02-02%20144835.png)

## 🛠️ Project Details
* **Simulation Tool:** Cisco Packet Tracer
* **Routing Logic:** Configured Dynamic Routing to ensure high availability across the enterprise infrastructure.
* **Key Implementation:** **Emergency Bypass Policy.** I implemented logic where emergency-related traffic bypasses standard verification gateways to ensure zero-latency communication.
* **File Included:** `OEL.pkt` (Executable simulation file)

## 🛡️ Emergency Protocol Logic
In this design, I simulated a scenario where **Emergency Services** do not require the standard payment/authentication handshake.
* **Traffic Prioritization:** Emergency data is tagged with higher priority to ensure immediate delivery.
* **Access Control:** Standard "Pings" (ICMP) from the payment gateway are bypassed for emergency nodes to prevent bottlenecks.
* **Zero-Halt Access:** Designed to ensure that in an emergency state, the network does not "ping" or wait for payment verification before allowing data flow.

## 📸 Verification & Testing
![Ping Test](Screenshot%202026-02-02%20145042.png)
* **Standard Mode:** Verified connectivity between User and Payment Gateway.
* **Emergency Mode:** Verified that Emergency Nodes access the Server directly, bypassing the authentication loop.
