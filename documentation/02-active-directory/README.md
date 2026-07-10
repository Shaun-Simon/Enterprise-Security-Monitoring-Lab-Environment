# Active Directory

## Overview

This section documents the deployment and configuration of a Windows Active Directory environment designed to simulate enterprise identity management.

Active Directory provides the foundation of the environment by managing:

- User identities
- Computer accounts
- Authentication
- Security groups
- Organisational structure
- Group Policy management

The deployment simulates how organisations centrally manage users, devices and security policies.

---

# Active Directory Architecture

The environment uses:

| Component | Purpose |
|:----------|:--------|
| `DC01` | Windows Server Domain Controller |
| `corp.local` | Active Directory Domain |
| `CLIENT01`-`03` | Domain-joined Windows endpoints |

---

# Implemented Features

## Domain Services

Configured:

- Active Directory Domain Services
- DNS Services
- Domain Controller promotion
- Domain authentication

---

## Identity Management

Implemented:

- User accounts
- Security groups
- Department structure
- Role-based access control

Example departments:

- `IT`
- `HR`
- `Finance`

---

## Group Policy Management

Configured centralised security controls including:

- `Password policies`
- `Account lockout policies`
- `Security auditing`
- `Endpoint configuration policies`

Group Policy allows administrators to enforce security settings across multiple systems from a central location.

---

# Security Objectives

The Active Directory environment provides the identity layer for later security monitoring activities.

It enables:

- `Authentication monitoring`
- `Account activity tracking`
- `Privileged access monitoring`
- `Security event collection`

---

# Documentation

Detailed implementation documentation:

- `domain-controller-deployment.md`
- `identity-management.md`
- `group-policy-baseline.md`
