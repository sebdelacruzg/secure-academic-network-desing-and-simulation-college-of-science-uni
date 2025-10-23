# Design and simulation of a secure academic network for the College of Science using Cisco Packet Tracer

Design, simulation, and documentation of a hierarchical network architecture for an academic environment (College of Science) using VLANs, ACLs, and a router-on-a-stick approach in Cisco Packet Tracer.

This repository serves as a **portfolio project** and *case study* demonstrating the design and implementation of a secure, scalable, and modern network for a medium-sized academic institution.

---

## 🎯 Project Objectives

- **Design** a hierarchical, secure, and scalable network for the College of Science scenario.  
- **Segment** the network into logical broadcast domains (VLANs) to separate traffic for Students, Faculty, Administration, Labs, and Servers.  
- **Implement** inter-VLAN routing (using the *router-on-a-stick* method) to allow controlled communication between VLANs.  
- **Configure** essential network services such as DHCP (for dynamic IP assignment) and NAT (for Internet access).  
- **Apply** security policies using Access Control Lists (ACLs) to filter and control traffic between VLANs.  
- **Validate** the entire design through comprehensive connectivity and security testing.
  
---

## 🛠️ Key Features Implemented

- **Hierarchical topology:** Based on Cisco’s three-layer model (Core, Distribution, Access).  
- **VLSM (Variable Length Subnet Mask):** Used the `172.16.0.0/16` base network for efficient IP allocation.  
- **VLANs:** Created 6 VLANs for traffic segmentation:  
  - `VLAN 10`: Administration  
  - `VLAN 20`: Faculty (Teachers)  
  - `VLAN 30`: Students  
  - `VLAN 40`: Laboratories (Rooms 1–5)  
  - `VLAN 50`: Servers  
  - `VLAN 99`: Network Management (Native VLAN)  
- **Inter-VLAN routing:** Configured on the main router to allow controlled communication between VLANs.  
- **DHCP server:** The router dynamically assigns IPs to user VLANs.  
- **ACLs (Access Control Lists):** Enforced to secure network segments (e.g., Students VLAN cannot access Administration or Server VLANs).  
- **NAT (Network Address Translation):** Configured so the entire internal network can access the Internet securely.

---
