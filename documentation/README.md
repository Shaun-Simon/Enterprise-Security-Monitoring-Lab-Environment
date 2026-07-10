# Enterprise Security Monitoring Lab Enviornment

## Overview

This project aims to demonstrates the planning, design and deployment of an enterprise style Windows based security monitoring environment using virtualised infrastructure, Active Directory, Group Policy, Sysmon and linux based Wazuh SIEM.

The objective and overall aim of this project was to simulate a small enterprise environment where identity management, endpoint security controls and security monitoring could be implemented using commonly used industry technologies.

The entire environment was built within a Physical Proxmox virtualisation cluster (homelab) and designed to replicate the workflow of a real world IT and Security Operations environment.

---

# Project Objectives

- Build and manage a virtualised enterprise style environment
- Deploy Active Directory Domain Services
- Implement centralised identity management
- Configure Group Policy security controls
- Deploy endpoint monitoring using Sysmon
- Implement centralised security monitoring using the Wazuh SIEM tool
- Analyse Windows security telemetry
- Create a foundation for future detection engineering and incident response exercises

---

# Architecture Overview

The environment consists of:

| System | Role | IP Address |
|---|---|---|
| DC01 | Windows Server 2022 Domain Controller & DNS Server | 192.168.0.200 |
| CLIENT01 | Windows 11 Pro Workstation | 192.168.0.201 |
| CLIENT02 | Windows 11 Pro Workstation | 192.168.0.202 |
| CLIENT03 | Windows 11 Pro Workstation | 192.168.0.203 |
| SOC01 | Wazuh SIEM Monitoring Server | 192.168.0.210 |

---

# Technology Used

## Infrastructure

- Proxmox Virtual Environment 
- Virtual Machines
- Virtual Networking

## Identity & Administrative

- Windows Server 2022
- Active Directory Domain Services
- DNS
- Group Policy Objects

## Endpoint Security

- Sysmon ingestion
- Windows Event Logging

## Security Monitoring

- Wazuh SIEM
- Wazuh Agents
- Security Event Analysis

---

# Project Architecture in order
- Active Directory
- Windows Endpoints
- Sysmon Telemetry
- Wazuh Agents
- Wazuh SIEM Dashboard


---

# Current Implementation Timeline 

Completed:

✅ Proxmox enterprise-style environment deployment  
✅ Windows Server domain controller deployment  
✅ Active Directory domain configuration  
✅ DNS configuration  
✅ Domain joined Windows endpoints  
✅ Organisational Unit structure  
✅ User and security group management  
✅ Group Policy security controls  
✅ Sysmon endpoint telemetry collection  
✅ Wazuh SIEM deployment  
✅ Windows endpoint monitoring integration  

---

# Future Development

Planned enhancements:

- Security incident simulation
- Detection engineering
- Brute force attack scenarios
- Privilege escalation investigations
- Suspicious PowerShell analysis
- Custom Wazuh detection rules
- MITRE ATT&CK mapping

---

# Documentation

Detailed implementation documentation can be found below:

- [Infrastructure Deployment](documentation/01-infrastructure/)
- [Active Directory Deployment](documentation/02-active-directory/)
- [Security Hardening](documentation/03-security-hardening/)
- [Endpoint Monitoring](documentation/04-endpoint-monitoring/)
- [SIEM Deployment](documentation/05-siem-deployment/)
- [Detection Engineering](documentation/06-detection-engineering/)
