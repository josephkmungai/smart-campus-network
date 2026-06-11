# Campus Capacity and VLAN Plan

## Project Overview

This project aims to design and implement a secure Multi-Institute Campus Area Network (CAN) for a Campus consisting of:

- Institute of Business Studies (IBS)
- Craft Engineering Institute (CEI)
- Textile Training Institute (TTI)

The network will support approximately 2,500 users and devices while providing centralized services through Windows Server 2022.

---

# Institute of Business Studies (IBS)

## Departments

1. Administration
2. Accounting & Finance
3. Human Resource Management
4. Information Communication Technology (ICT)
5. Student Labs

## Estimated Capacity

| Department | Estimated Devices |
|------------|------------------|
| Administration | 50 |
| Accounting & Finance | 80 |
| Human Resource Management | 70 |
| ICT | 100 |
| Student Labs | 700 |

### Total Capacity

Approximately 1000 Devices

## VLAN Allocation

| VLAN ID | Department |
|----------|-----------|
| 110 | Administration |
| 120 | Accounting & Finance |
| 130 | Human Resource Management |
| 140 | ICT |
| 150 | Student Labs |

---

# Craft Engineering Institute (CEI)

## Departments

1. Administration
2. Mechanical Engineering
3. Electrical Engineering
4. Building & Construction
5. Student Labs

## Estimated Capacity

| Department | Estimated Devices |
|------------|------------------|
| Administration | 40 |
| Mechanical Engineering | 120 |
| Electrical Engineering | 120 |
| Building & Construction | 70 |
| Student Labs | 450 |

### Total Capacity

Approximately 800 Devices

## VLAN Allocation

| VLAN ID | Department |
|----------|-----------|
| 210 | Administration |
| 220 | Mechanical Engineering |
| 230 | Electrical Engineering |
| 240 | Building & Construction |
| 250 | Student Labs |

---

# Textile Training Institute (TTI)

## Departments

1. Administration
2. Textile Production
3. Garment Design & Fashion
4. Quality Control & Inspection
5. Student Labs

## Estimated Capacity

| Department | Estimated Devices |
|------------|------------------|
| Administration | 30 |
| Textile Production | 120 |
| Garment Design & Fashion | 100 |
| Quality Control & Inspection | 50 |
| Student Labs | 400 |

### Total Capacity

Approximately 700 Devices

## VLAN Allocation

| VLAN ID | Department |
|----------|-----------|
| 310 | Administration |
| 320 | Textile Production |
| 330 | Garment Design & Fashion |
| 340 | Quality Control & Inspection |
| 350 | Student Labs |

---

# Shared Campus Services

## Data Center and Campus Services

| VLAN ID | Service |
|----------|---------|
| 400 | Server VLAN |
| 410 | ICT Operations |
| 420 | Guest WiFi |
| 499 | Network Management |

---

# Centralized Windows Server 2022 Infrastructure

The entire campus will utilize a centralized Windows Server 2022 infrastructure located in the campus Data Center.

The server will provide:

- Active Directory Domain Services (AD DS)
- Domain Name System (DNS)
- Dynamic Host Configuration Protocol (DHCP)
- File Services
- Internet Information Services (IIS)
- Group Policy Management

Proposed Domain Name:

smartcampus.com

---

# Security Objectives

The network will implement:

- VLAN Segmentation
- Access Control Lists (ACLs)
- Secure Device Management using SSH
- Password Policies
- Account Lockout Policies
- Network Monitoring
- Principle of Least Privilege
- Defense in Depth

---

# Expected Benefits

## Academic Benefits

- Improved access to learning resources
- Reliable connectivity for students and staff
- Centralized management of users and devices

## Business Benefits

- Reduced operational costs
- Easier network management
- Improved scalability
- Better resource utilization

## Security Benefits

- Reduced attack surface
- Better access control
- Improved monitoring and auditing
- Protection of sensitive departmental data

---

# Technologies Used

- Cisco Packet Tracer
- Windows Server 2022
- Oracle VM VirtualBox
- GitHub
- Parrot OS
- Active Directory
- DNS
- DHCP
- IIS
- VLANs
- OSPF
- ACLs

---

