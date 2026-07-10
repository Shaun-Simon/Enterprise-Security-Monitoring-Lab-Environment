# Security Hardening

## Overview

This section documents security improvements applied to the Active Directory environment to establish a stronger enterprise security baseline.

The objective was to move beyond a default Windows deployment and introduce security controls commonly implemented within organisational environments.

---

# Hardening Objectives

The security hardening phase focuses on:

- `Reducing account compromise risk`
- `Improving visibility into user activity`
- `Establishing secure authentication controls`
- `Preparing endpoints for security monitoring`

---

# Implemented Security Controls

## Authentication Security

Implemented:

- `Minimum password requirements`
- `Password complexity enforcement`
- `Password history`
- `Maximum password age`
- `Account lockout protection`

These controls help reduce the effectiveness of password-based attacks.

---

## Security Auditing

Enabled auditing for:

- `Successful authentication`
- `Failed authentication`
- `Account management activity`
- `Privileged operations`

These events provide valuable telemetry for future SOC monitoring.

---

## Group Policy Security Baseline

Security configurations were deployed centrally through Group Policy Objects (GPOs).

This demonstrates how enterprise administrators can enforce security requirements across multiple endpoints.

---

# Security Monitoring Preparation

The hardening phase created the foundation required for later monitoring activities.

The enabled auditing configuration allows the following in order:

- `User Activity`
- `Windows Security Events`
- `SIEM Collection`
- `Security Investigation`

---

# Documentation

Further implementation details can be found in:

- `group-policy-baseline.md`
