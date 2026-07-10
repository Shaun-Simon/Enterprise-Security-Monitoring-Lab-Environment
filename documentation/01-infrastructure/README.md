# Infrastructure

## Overview

This section documents the underlying infrastructure used to build the enterprise security monitoring environment.

The project was developed using a self-hosted Proxmox virtualisation environment consisting of multiple physical nodes, allowing the deployment of isolated virtual machines for Active Directory, endpoints, monitoring systems and security testing.

The infrastructure provides the foundation required to simulate a small enterprise environment where identity management, endpoint security and SOC monitoring workflows can be implemented.

---

# Infrastructure Components

## Virtualisation Platform

The environment is hosted using:

- Proxmox Virtual Environment
- Virtual machines
- Virtual networking
- Managed switching infrastructure

Proxmox provides the ability to deploy, manage and test multiple operating systems while maintaining separation between different systems and roles.

---

# Lab Architecture

The environment consists of:

| System | Role |
|:------|:-----|
| `DC01` | Windows Server Domain Controller |
| `CLIENT01` | Windows Enterprise Endpoint |
| `CLIENT02` | Windows Enterprise Endpoint |
| `CLIENT03` | Windows Enterprise Endpoint |
| `SOC01` | Wazuh Security Monitoring Server |

---

# Network Design

The environment uses a dedicated private network range:

```
192.168.0.0/24
```

Core systems:

| Hostname | IP Address | Purpose |
|:---------|:-----------|:--------|
| `DC01` | `192.168.0.200` | Active Directory Domain Controller |
| `CLIENT01` | `192.168.0.201` | Domain Endpoint |
| `CLIENT02` | `192.168.0.202` | Domain Endpoint |
| `CLIENT03` | `192.168.0.203` | Domain Endpoint |
| `SOC01` | `192.168.0.210` | Security Monitoring Platform |

---

# Infrastructure Objectives

The infrastructure was designed to provide:

- Realistic enterprise-style deployment
- Network segmentation
- Safe security testing environment
- Ability to deploy multiple security tools
- Repeatable project development platform

---

# Documentation

Detailed infrastructure deployment information can be found in:

- `proxmox-environment.md`

This includes:

- Proxmox configuration
- Virtual machine deployment
- Network configuration
- Initial operating system installation
