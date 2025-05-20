# CMPE-451 Network Engineering - Skill-Based Project

This repository contains the final submission files for the **Skill-Based Experiment Design Project** completed for the **CMPE-451: Network Engineering - I** course at **Kadir Has University**, Spring 2025.

## 👥 Team Members
- **Samet Tok (Computer Engineering)**
- **Mohamed Ayhem Jlassi (Computer Engineering)**

## 📄 Project Description

The objective of this project was to design, implement, and test a large-scale network topology simulating two separate company LANs connected via a WAN link. Each company was assigned to a student who was responsible for the design and configuration of their own company network using **Cisco Packet Tracer**.

Each network includes:
- 1 Router (Cisco 2911)
- 2 Switches (Cisco 2960)
- 1 Wireless Access Point
- Multiple wired and wireless end devices
- Subnets created using **Variable Length Subnet Masking (VLSM)**

The two company networks are connected via a point-to-point **WAN link** and use **RIPv2 (Routing Information Protocol)** for dynamic routing and inter-network communication.

> Samet's network uses VLANs 11–14 mapped to floors, implemented with **trunking and router-on-a-stick** configuration. Ayhem’s network has a different structure (explained in the project report).

## 📦 Contents of the Repository

| File Name | Description |
|----------|-------------|
| `CMPE451-Skill-Based-Project-Final.pdf` | Official project announcement and instructions |
| `Experiment_Design_Report.docx` | Full report including topology, addressing, configuration, and test results |
| `Final_Topology.pkt` | Cisco Packet Tracer file with complete network setup |
| `Samet_R1_config.rtf` | Running configuration of Samet's router |
| `Samet_S1_config.rtf` | Running configuration of Samet's first switch |
| `Samet_S2_config.rtf` | Running configuration of Samet's second switch |
| `Ayham_S1_config.rtf` | Running configuration of Ayhem's first switch |
| `Ayham_S2_config.rtf` | Running configuration of Ayhem's second switch |

> 🔐 All devices were secured with hostnames, login banners, and passwords (`Samet` or `Ayhem` depending on the owner).

## 🛠️ Key Technologies Used
- Cisco Packet Tracer (Simulation)
- VLANs & Inter-VLAN Routing
- RIPv2 Routing Protocol
- VLSM (Variable Length Subnet Masking)
- Trunking (802.1Q)
- Static IP configuration
- Access Point & wireless clients

## ✅ Testing and Verification

The following tests were performed and documented in the report:
- End-to-end **ping** between all wired and wireless hosts
- **Traceroute** (`tracert`) across the WAN
- Inter-VLAN communication using **router-on-a-stick**
- Configuration validation using `show` commands (e.g., `show ip route`, `show interfaces trunk`, etc.)

> All test results confirmed full connectivity and correct configuration across both networks.

## 📁 How to Use

1. Open the `.pkt` file using **Cisco Packet Tracer 8.2+**
2. Inspect router and switch configurations via CLI (`show running-config`)
3. Check connectivity using simulation tools (`ping`, `tracert`)
4. Refer to the `.docx` report for detailed documentation

## 📚 References
- Cisco NetAcad: CCNA Modules
- CMPE-451 Course Materials
- [Cisco Documentation](https://www.cisco.com/)

---

