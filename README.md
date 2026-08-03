# Enterprise-Multi-Floor-Network-Design-using-Cisco-Packet-Tracer

A complete enterprise network designed and implemented in **Cisco Packet Tracer**, simulating a real-world three-floor hotel infrastructure. This project demonstrates how multiple departments can securely communicate using VLAN segmentation, dynamic routing, DHCP, wireless networking, and basic network security.

The goal of this project was to build a scalable and secure network where every department is logically separated while allowing seamless communication across the entire organization.

![Project Screenshot](https://github.com/srinathsamudrala/Enterprise-Multi-Floor-Network-Design-using-Cisco-Packet-Tracer/blob/main/Screenshot/Enterprise-Multi-Floor-Network-Design.png?raw=true)

---

## Project Overview

This project represents the network infrastructure of a three-floor hotel. Each floor contains multiple departments connected through dedicated switches and routers. Every department is assigned its own VLAN and subnet to improve network organization, reduce broadcast traffic, and enhance security.

The three routers are interconnected using serial links and exchange routing information through the **OSPF routing protocol**, allowing devices from different floors to communicate with each other. DHCP is configured on each router to automatically assign IP addresses to hosts, while wireless access points provide Wi-Fi connectivity for laptops, smartphones, and tablets.

To improve network security, SSH is configured for secure remote router management, and Port Security is implemented on the IT department switch using Sticky MAC Address learning.

---

# Network Architecture

The network consists of three floors, each representing different business departments.

### First Floor
- Reception
- Store
- Logistics

### Second Floor
- Finance
- Human Resources (HR)
- Sales & Marketing

### Third Floor
- Information Technology (IT)
- Administration

Each floor contains:

- One Cisco Router
- One Cisco 2960 Switch
- One Wireless Access Point
- Desktop PCs
- Network Printers
- Wireless Devices (Laptop, Tablet & Smartphone)

All three routers are connected together through Serial DCE links, forming the backbone of the enterprise network.

---

# Technologies Used

| Technology | Purpose |
|------------|---------|
| Cisco Packet Tracer | Network Simulation & Implementation |
| Cisco 2911 Routers | Routing between floors |
| Cisco 2960 Switches | VLAN and Switching |
| VLANs | Department-wise Network Segmentation |
| Router-on-a-Stick | Inter-VLAN Routing |
| IEEE 802.1Q Trunking | Carry Multiple VLANs |
| OSPF | Dynamic Routing |
| DHCP | Automatic IP Address Assignment |
| SSH | Secure Remote Router Access |
| Port Security | Restrict Unauthorized Devices |
| Sticky MAC Address | Automatically Learn Allowed Device |
| Wireless Access Points | Wi-Fi Connectivity |

---

# Network Connectivity

The enterprise network follows a hierarchical design.

- Each floor has a dedicated Layer 2 switch connecting all wired devices.
- The switch is connected to a router using a trunk link.
- Router-on-a-Stick is used to provide communication between VLANs on the same floor.
- Three routers are interconnected using Serial DCE cables.
- OSPF dynamically exchanges routing information between routers.
- Every department has its own subnet and default gateway.
- DHCP automatically assigns IP addresses to all hosts.
- Wireless Access Points provide network connectivity for mobile devices.
- All printers are connected within their respective departmental VLANs.
- SSH allows administrators to securely access routers remotely.
- Port Security protects the IT department switch by allowing only the authorized Test-PC to connect.

The final topology allows every device in the enterprise to communicate successfully while maintaining logical separation between departments.

---

# VLAN & IP Addressing

| Department | VLAN | Network |
|------------|------|----------------|
| IT | 10 | 192.168.1.0/24 |
| Admin | 20 | 192.168.2.0/24 |
| Sales | 30 | 192.168.3.0/24 |
| HR | 40 | 192.168.4.0/24 |
| Finance | 50 | 192.168.5.0/24 |
| Logistics | 60 | 192.168.6.0/24 |
| Store | 70 | 192.168.7.0/24 |
| Reception | 80 | 192.168.8.0/24 |

### Router-to-Router Networks

- 10.10.10.0/30
- 10.10.10.4/30
- 10.10.10.8/30

---

# Features Implemented

- Enterprise Multi-Floor Network Design
- Department-wise VLAN Segmentation
- Inter-VLAN Communication
- Router-on-a-Stick Configuration
- Dynamic Routing using OSPF
- DHCP Configuration for Every VLAN
- Wireless Network Connectivity
- Secure SSH Remote Login
- Port Security with Sticky MAC
- Automatic IP Address Assignment
- End-to-End Connectivity Testing
- Printer Connectivity
- Network Verification using Ping and SSH

---

# Implementation Summary

The project began by designing the physical topology of a three-floor enterprise network in Cisco Packet Tracer. Each floor was connected to its own router and switch, with all routers interconnected through serial links.

Separate VLANs were created for every department, and corresponding subnets were assigned based on the network requirements. Router-on-a-Stick was configured to enable communication between VLANs, while OSPF was implemented to dynamically advertise routes across all three routers.

DHCP services were configured on each router so that all wired and wireless devices could obtain IP addresses automatically. Wireless Access Points were deployed on every floor, allowing laptops, tablets, and smartphones to connect seamlessly.

Finally, SSH was configured on all routers to enable secure remote administration, and Port Security was implemented on the IT department switch using Sticky MAC Address learning to ensure that only the authorized Test-PC could access the secured switch port.

After completing the configuration, extensive testing was performed to verify DHCP allocation, routing, wireless connectivity, inter-VLAN communication, SSH access, and overall network functionality.

---

# Skills Demonstrated

- Enterprise Network Design
- Cisco Routing & Switching
- VLAN Configuration
- Inter-VLAN Routing
- OSPF Routing
- DHCP Configuration
- Wireless Networking
- SSH Configuration
- Network Security
- Port Security
- Enterprise Troubleshooting
- IP Address Planning
- Cisco Packet Tracer

---

# Project Outcome

This project successfully simulates a real-world enterprise network infrastructure where multiple departments operate within isolated VLANs while maintaining full communication across the organization. By implementing OSPF, DHCP, SSH, wireless networking, and switch security, the network provides scalability, efficient routing, centralized management, and secure access. The project strengthened my practical understanding of enterprise networking concepts and hands-on Cisco device configuration using Cisco Packet Tracer.

---
