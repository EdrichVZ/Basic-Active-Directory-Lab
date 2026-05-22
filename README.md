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

Specifications:
- 8GB RAM
- 4 CPU cores
- 50GB storage
- (see Screenshots/domain_controller_VM-setup.png)
- (see Screenshots/domain_controller_VM-hardware.png)

Internal network called LABNET setup for DC01 VM.
- (see Screenshots/domain_controller_VM-network.png)
