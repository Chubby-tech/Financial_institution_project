# Enterprise Financial Institution Network Design and Secure Infrastructure Implementation

## Overview

This project presents the design and implementation of a secure, scalable, and highly available enterprise network infrastructure for Jubilee Financial Services Ltd (JFSL), a financial institution headquartered in Nairobi, Kenya.

The objective was to design a resilient multi-floor corporate network supporting secure communication between headquarters and an external server site while incorporating network segmentation, VoIP services, wireless connectivity, routing redundancy, NAT, Access Control Lists (ACLs), and site-to-site IPsec VPN technology.

The solution follows a hierarchical enterprise network architecture and implements security best practices to ensure confidentiality, integrity, and availability of organizational resources.

---

## Business Scenario

Jubilee Financial Services Ltd operates across two floors within its headquarters and hosts critical business services at a remote server-side location.

The organization required:

* Departmental network segmentation
* Secure access to centralized services
* Wireless connectivity for staff
* Enterprise VoIP communications
* Redundant Internet connectivity
* Secure WAN communication
* Controlled administrative access
* Scalable network architecture

The solution was designed to meet these requirements while supporting future growth and increased service demand.

---

## Network Architecture

### Headquarters Departments

#### Seventh Floor

* Human Resources (HR)
* Customer Service (CS)
* Marketing (MK)

#### Eighth Floor

* Legal Management (LM)
* Information Technology (IT)

Each department includes:

* User workstations
* IP phones
* Wireless access points
* Dedicated VLANs

### Server-Side Site

The remote data center hosts:

* DHCP Server
* DNS Server
* Email Server
* Web Server

### Internet Connectivity

The headquarters network connects to:

* Safaricom ISP
* JTL ISP

This dual-ISP design provides:

* Redundancy
* High Availability
* Internet Failover Capability
* Load Distribution

---

## Technologies Implemented

### Network Design

* Enterprise Hierarchical Design
* Redundant Architecture
* Multi-Site Network Design

### Switching Technologies

* VLAN Segmentation
* Voice VLAN Deployment
* Trunking
* Switchport Security
* Sticky MAC Address Learning

### Routing Technologies

* Inter-VLAN Routing Using SVIs
* OSPF Dynamic Routing
* Multi-Layer Switching

### Network Services

* DHCP Services
* DNS Services
* Email Services
* Web Services

### Wireless Networking

* Departmental Wireless Access Points
* Wireless User Connectivity

### Security Technologies

* SSH Secure Remote Access
* Access Control Lists (ACLs)
* Port Security
* Administrative Access Control
* Network Segmentation

### WAN Technologies

* PAT (Port Address Translation)
* NAT Overload
* Dual ISP Connectivity
* Site-to-Site IPsec VPN

### Unified Communications

* Cisco VoIP Deployment
* Voice VLANs
* Telephony Services
* IP Phone Registration

---

## Key Features

✔ Department-Based VLAN Segmentation

✔ Voice VLAN Deployment (VLAN 120)

✔ Wireless Network Integration

✔ Dynamic IP Address Allocation

✔ OSPF Dynamic Routing

✔ Layer 3 Switching

✔ Secure SSH Administration

✔ VTY Access Restrictions via ACL

✔ NAT/PAT Internet Access

✔ Dual ISP Redundancy

✔ Site-to-Site IPsec VPN

✔ Port Security with Sticky MAC Learning

✔ Enterprise VoIP Communication

✔ Remote Server-Site Integration

---

## Security Implementation

### Access Control Lists (ACLs)

ACLs were configured to:

* Restrict SSH administration access
* Control VPN traffic
* Support NAT/PAT operations
* Enforce security policies

### SSH Security

Secure remote administration was implemented on:

* Cisco Routers
* Layer 3 Switches

Only the IT Department was authorized to perform remote administrative tasks.

### Port Security

Port security was configured on server-side access switches using:

* Sticky MAC Learning
* Maximum One MAC Address
* Violation Mode Shutdown

### Site-to-Site VPN

An IPsec VPN tunnel was established between:

* Headquarters Router
* Server-Side Router

This provided encrypted communication between corporate and remote infrastructure.

---

## IP Addressing Plan

| Network Type   | Address Range    |
| -------------- | ---------------- |
| Data Network   | 192.168.20.0/24  |
| Voice Network  | 10.10.10.0/24    |
| Public Network | 190.200.100.0/24 |

Subnetting was performed to accommodate departmental requirements while maintaining scalability and efficient address utilization.

---

## Devices Used

### Routers

* Cisco 2911 Router (HQ)
* Cisco 2911 Router (Server Site)
* Cisco 2811 Voice Gateway Router

### Switching Infrastructure

* Cisco Layer 3 Switches
* Cisco Access Layer Switches

### End Devices

* PCs and Workstations
* IP Phones
* Wireless Clients
* Servers

---

## Verification and Testing

The following tests were successfully completed:

* Inter-VLAN Communication
* OSPF Neighbor Adjacency
* DHCP Address Allocation
* Wireless Connectivity
* VoIP Calling Functionality
* SSH Remote Access
* NAT/PAT Translation Verification
* ACL Validation
* VPN Tunnel Verification
* Server Accessibility
* End-to-End Network Communication

All services were tested and verified to be operating as expected.

---

## Skills Demonstrated

* Enterprise Network Design
* Layer 2 and Layer 3 Switching
* OSPF Routing
* VLAN Segmentation
* Wireless Networking
* VoIP Deployment
* ACL Implementation
* Network Security
* NAT and PAT Configuration
* Site-to-Site VPN Deployment
* Port Security
* Redundant Network Design
* Cisco Packet Tracer Simulation
* Network Troubleshooting

---

## Repository Structure

```text
JFSL-Enterprise-Network/
│
├── README.md
├── JFSL_Enterprise_Network.pkt
├── JFSL_Design_Report.pdf
├── topology.png

```

---

## Topology

Insert topology screenshot below.


---

## Author

Chibuike Obika

Enterprise Network Engineering Portfolio Project
