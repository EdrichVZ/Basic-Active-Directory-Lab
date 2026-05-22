# Basic-Active-Directory-Lab

## Overview
This project documents the creation of a Windows Active Directory home lab environment using VirtualBox, Windows Server 2022, and Windows 10/11.

## Objectives
- Learn Active Directory fundamentals
- Practice enterprise user management
- Configure Group Policy
- Simulate enterprise infrastructure
- Develop hands-on IT and cybersecurity skills

## Virtualization Platform

Installed Oracle VirtualBox to host the virtual lab environment.

Purpose:
- Isolate the lab from the host system
- Simulate enterprise infrastructure
- Allow safe testing and rollback
- (see Screenshots/virtualbox-installed.png)

## Operating Systems Used

- Windows Server 2022 Evaluation
- Windows 10/11 Pro

These systems were used to simulate a domain controller and enterprise workstation environment.

## Lab Organization

Created dedicated folders for:
- ISOs
- Virtual Machines
- Screenshots
- Documentation

This keeps the lab organized and easier to maintain.

## Domain Controller VM

Created a Windows Server 2022 virtual machine named DC01.

Purpose
This virtual machine will function as:
- Active Directory Domain Controller
- DNS Server
- Centralized authentication server
  
Specifications:
- 8GB RAM
- 4 CPU cores
- 50GB storage
- (see Screenshots/domain_controller_VM-setup.png)
- (see Screenshots/domain_controller_VM-hardware.png)

Install of Windows Server 2022 on DC01-VM succesfull.
- (see Screenshots/DC01_VM-OS-install.png)
- (see Screenshots/DC01_VM-Server-Manager

Internal network called LABNET setup for DC01 VM.
- (see Screenshots/domain_controller_VM-network.png)

PW = DC01@12345

## Server Configuration

Configured the Windows Server virtual machine prior to Active Directory installation.

Tasks Completed
- Renamed the server to DC01
- Configured a static IP address
- Configured local DNS settings
- Verified basic network connectivity
- (see Screenshots/DC01_VM-Renamed.png)
- (see Screenshots/DC01_VM-OS-install.png)
- (see Screenshots/DC01_VM-Network-Verifying.png)

Network Configuration
- IP Address: 192.168.10.10
- Subnet Mask: 255.255.255.0
- DNS Server: 192.168.10.10

Purpose
Static addressing ensures the Domain Controller remains consistently reachable by clients and domain services.

## Active Directory Domain Services Installation

Installed the Active Directory Domain Services (AD DS) role and promoted DC01 to a Domain Controller.
- (see Screenshots/DC01_VM-Promoting to Domain Controller.png)

Domain Information
- Domain Name: basic.local
- NetBIOS Name: basic
- (see Screenshots/DC01_VM-basic-domain-created.png)

Services Installed
- Active Directory Domain Services
- DNS Server

Purpose
Active Directory provides centralized identity management, authentication, and administrative control within enterprise environments.

Outcome
Successfully created the basic.local Active Directory domain.
- (see Screenshots/DC01_VM-AD-installed.png)
