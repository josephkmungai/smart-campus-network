# Smart Campus Network Project

# Physical and Logical Topology Design

## Project Information

Project Name: Smart Campus Network Infrastructure Design

Domain Name: smartcampus.com

Author: Joseph_net_labs

---

# 1. Project Objective

The objective of this phase is to design a realistic enterprise Campus Area Network (CAN) connecting three institutes within a single campus while providing centralized network services using Windows Server 2022.

The design must provide:

* Scalability
* Security
* High Performance
* Centralized Management
* Future Expansion Capability

---

# 2. Institutes Within the Campus

The campus consists of:

## Institute of Business Studies (IBS)

Departments:

* Administration
* Accounting & Finance
* Human Resource Management
* ICT Department
* Student Computer Laboratories

---

## Craft Engineering Institute (CEI)

Departments:

* Administration
* Mechanical Engineering
* Electrical Engineering
* Building & Construction
* Student Computer Laboratories

---

## Textile Training Institute (TTI)

Departments:

* Administration
* Textile Production
* Garment Design
* Quality Control
* Student Computer Laboratories

---

# 3. Network Design Model

The Smart Campus Network follows the Enterprise Hierarchical Network Design Model.

The design contains three layers:

## Core Layer

Provides the backbone of the entire campus network.

Responsibilities:

* Inter-VLAN Routing
* Routing Between Institutes
* High-Speed Switching
* Connectivity to Internet Router
* Connectivity to Server Farm

---

## Distribution Layer

Acts as the aggregation point between Access and Core Layers.

Responsibilities:

* VLAN Aggregation
* Policy Enforcement
* Traffic Control
* Network Expansion

---

## Access Layer

Provides connectivity for end devices.

Examples:

* Computers
* Printers
* Access Points
* Student Lab PCs
* Administrative Workstations

---

# 4. Physical Topology

```
                       INTERNET
                           |
                      2911 Router
                           |
                3560 Layer 3 Core Switch
                           |
    -------------------------------------------------
    |                       |                       |
    |                       |                       |
```

IBS Distribution      CEI Distribution      TTI Distribution
Switch                Switch               Switch
|                     |                    |
----------------      ----------------    ----------------
|              |      |              |    |              |
IBS Access 1  IBS Access 2 CEI Access 1 CEI Access 2 TTI Access 1 TTI Access 2
|              |      |              |    |              |
Users          Users   Users          Users Users        Users

```
                           |
                     Server Switch
                           |
                Windows Server 2022
```

---

# 5. Device Selection

## Internet Router

Device:

Cisco 2911 Router

Quantity:

1

Purpose:

* Internet Connectivity
* NAT Services
* External Routing

Reason for Selection:

The Cisco 2911 Router is commonly used in Packet Tracer and supports enterprise routing features suitable for campus environments.

---

## Core Layer Device

Device:

Cisco 3560 Multilayer Switch

Quantity:

1

Purpose:

* Inter-VLAN Routing
* Campus Backbone
* Default Gateway Services

Reason for Selection:

A Layer 3 switch supports routing and switching simultaneously, making it ideal as the campus core device.

---

## Distribution Layer Devices

Device:

Cisco 2960-48TT Switch

Quantity:

3

Allocation:

* 1 for IBS
* 1 for CEI
* 1 for TTI

Purpose:

* Aggregate Access Switches
* Forward Traffic to Core Layer

Reason for Selection:

Provides a realistic enterprise structure and simplifies future expansion.

---

## Access Layer Devices

Device:

Cisco 2960-48TT Switch

Quantity:

6

Allocation:

### IBS

* IBS Access Switch 1
* IBS Access Switch 2

### CEI

* CEI Access Switch 1
* CEI Access Switch 2

### TTI

* TTI Access Switch 1
* TTI Access Switch 2

Purpose:

* Connect End Users
* Connect Departmental Devices

Reason for Selection:

48-port switches support larger numbers of users while reducing the total number of switches required.

---

## Server Network

Device:

Cisco 2960-48TT Switch

Quantity:

1

Purpose:

Dedicated connectivity for server infrastructure.

Reason for Selection:

Separates server traffic from user traffic and reflects real enterprise practice.

---

## Windows Server 2022

Quantity:

1 Virtual Machine

IP Address:

10.10.200.10

Domain:

smartcampus.com

Services:

* Active Directory Domain Services (AD DS)
* DNS
* DHCP
* File Services
* Group Policy
* IIS Web Services

Reason for Selection:

Centralized management reduces infrastructure complexity while providing enterprise functionality.

---

# 6. Final Device Inventory

| Device                                | Quantity |
| ------------------------------------- | -------- |
| Cisco 2911 Router                     | 1        |
| Cisco 3560 Multilayer Switch          | 1        |
| Cisco 2960-48TT Distribution Switches | 3        |
| Cisco 2960-48TT Access Switches       | 6        |
| Cisco 2960-48TT Server Switch         | 1        |
| Windows Server 2022 VM                | 1        |

Total Major Devices:

13

---

# 7. Security Considerations

The topology supports:

* VLAN Segmentation
* Department Isolation
* ACL Implementation
* Centralized Authentication
* Least Privilege Access
* Management VLAN
* Guest Network Separation

---

# 8. Business Considerations

The design supports:

* Growth of Student Population
* Future Departments
* Additional Institutes
* Additional Servers
* Reduced Administration Costs
* Centralized Service Management

---

# 9. Future Expansion

The topology reserves capacity for:

* Wireless Access Points
* CCTV Systems
* VoIP Infrastructure
* Linux Servers
* Backup Servers
* Monitoring Servers
* Additional Academic Departments

---

# 10. Conclusion

The Smart Campus Network uses an enterprise hierarchical architecture consisting of:

* 1 Router
* 1 Core Layer 3 Switch
* 3 Distribution Switches
* 6 Access Switches
* 1 Server Switch
* 1 Windows Server 2022 Virtual Machine

The design provides scalability, security, centralized management, and realistic enterprise implementation suitable for academic learning, networking practice, cybersecurity integration, and portfolio development.

Version: 1.0
