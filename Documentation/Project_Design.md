# Project Design Document

## Project Title

Design and Implementation of a Secure Multi-Institute Campus Network Using Cisco Packet Tracer and Windows Server 2022

## Overview

This project aims to design and implement a secure campus network for three institutes operating within a campus.

The institutes include:

* Institute of Business Studies (IBS)
* Craft Engineering Institute (CEI)
* Textile Training Institute (TTI)

## Objectives

* Design a scalable Campus Area Network (CAN)
* Implement VLAN segmentation
* Provide centralized services using Windows Server 2022
* Improve security through network policies and access control
* Demonstrate practical networking and system administration skills

## Core Services

* Active Directory Domain Services
* DNS
* DHCP
* File Services
* IIS Web Services
* Group Policy Management

## Expected Capacity

Approximately 2,300 devices across the campus.

## Technologies

* Cisco Packet Tracer
* Windows Server 2022
* Oracle VM VirtualBox
* GitHub
* Parrot OS

## Proposed Topology

Internet → Router → Core Switch → Institute Distribution Switches → Department Access Switches → End Devices

Centralized services will be hosted on a Windows Server 2022 virtual machine connected through the Server VLAN.
