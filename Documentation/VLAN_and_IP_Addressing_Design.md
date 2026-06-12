# Smart Campus Network Project

## VLAN and IP Addressing Design

### Project Overview

This presents the VLAN and IP addressing design for a Smart Campus consisting of three institutes:

1. Institute of Business Studies (IBS)
2. Craft Engineering Institute (CEI)
3. Textile Training Institute (TTI)

The network is designed using a hierarchical model, VLAN segmentation, VLSM addressing, and centralized Windows Server 2022 services.

---

# Campus Address Space

Campus Network Block:

10.10.0.0/16

Reasons for selecting 10.10.0.0/16:

* Supports up to 65,534 hosts.
* Allows future expansion.
* Simplifies network management.
* Provides sufficient address space for all institutes, servers, guest networks, and future growth.

---

# VLAN Design

## Institute of Business Studies (IBS)

| VLAN ID | VLAN Name    | Network Address | Purpose                         |
| ------- | ------------ | --------------- | ------------------------------- |
| 110     | IBS_ADMIN    | 10.10.10.0/26   | Administration Department       |
| 120     | IBS_FINANCE  | 10.10.11.0/25   | Accounting & Finance Department |
| 130     | IBS_HR       | 10.10.12.0/25   | Human Resource Department       |
| 140     | IBS_ICT      | 10.10.13.0/25   | ICT Department                  |
| 150     | IBS_STUDENTS | 10.10.14.0/22   | Student Computer Laboratories   |

---

## Craft Engineering Institute (CEI)

| VLAN ID | VLAN Name        | Network Address | Purpose                            |
| ------- | ---------------- | --------------- | ---------------------------------- |
| 210     | CEI_ADMIN        | 10.10.20.0/26   | Administration Department          |
| 220     | CEI_MECHANICAL   | 10.10.21.0/25   | Mechanical Engineering Department  |
| 230     | CEI_ELECTRICAL   | 10.10.22.0/25   | Electrical Engineering Department  |
| 240     | CEI_CONSTRUCTION | 10.10.23.0/25   | Building & Construction Department |
| 250     | CEI_STUDENTS     | 10.10.24.0/23   | Student Computer Laboratories      |

---

## Textile Training Institute (TTI)

| VLAN ID | VLAN Name    | Network Address | Purpose                       |
| ------- | ------------ | --------------- | ----------------------------- |
| 310     | TTI_ADMIN    | 10.10.30.0/27   | Administration Department     |
| 320     | TTI_TEXTILE  | 10.10.31.0/25   | Textile Production Department |
| 330     | TTI_GARMENT  | 10.10.32.0/25   | Garment Design Department     |
| 340     | TTI_QC       | 10.10.33.0/26   | Quality Control Department    |
| 350     | TTI_STUDENTS | 10.10.34.0/23   | Student Computer Laboratories |

---

# Shared Campus Services

| VLAN ID | VLAN Name          | Network Address | Purpose                                      |
| ------- | ------------------ | --------------- | -------------------------------------------- |
| 400     | SERVER_FARM        | 10.10.200.0/24  | Windows Server and Core Services             |
| 410     | ICT_OPERATIONS     | 10.10.201.0/24  | ICT Support Team                             |
| 420     | GUEST_WIFI         | 10.10.210.0/23  | Visitor Internet Access                      |
| 499     | NETWORK_MANAGEMENT | 10.10.250.0/24  | Switches, Routers, and Management Interfaces |

---

# Windows Server 2022

Server VLAN:

VLAN 400

Server IP Address:

10.10.200.10

Domain Name:

smartcampus.com

Services to be Implemented:

* Active Directory Domain Services (AD DS)
* DNS Server
* DHCP Server
* File and Storage Services
* Group Policy Management
* IIS Web Services

---

# Design Principles

The network design follows the following principles:

1. Scalability

   * Supports future growth of students and staff.

2. Security

   * Departments are isolated using VLANs.
   * Access control can be implemented between VLANs.

3. Manageability

   * Structured VLAN numbering scheme.
   * Institute-based IP addressing plan.

4. High Availability

   * Centralized server infrastructure.
   * Efficient routing and switching architecture.

5. Enterprise Best Practices

   * Hierarchical network model.
   * VLAN segmentation.
   * VLSM-based IP allocation.
   * Centralized identity and access management.

---

# Implementation Phases

Phase 1:

* VLAN Creation
* Switch Configuration
* Trunk Configuration

Phase 2:

* Inter-VLAN Routing
* DHCP Deployment

Phase 3:

* Windows Server 2022 Deployment
* Active Directory Configuration
* DNS Configuration

Phase 4:

* Security Hardening
* ACL Implementation
* Monitoring and Logging

Phase 5:

* Documentation and Final Testing

---

Author: Cyb3rJay_netlabs

Project: Smart Campus Network Infrastructure Design

Domain: smartcampus.com
