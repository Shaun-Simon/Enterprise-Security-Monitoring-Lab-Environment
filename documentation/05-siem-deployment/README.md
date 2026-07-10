# SIEM Monitoring

This section documents the deployment and configuration of a centralised Security Information and Event Management (SIEM) platform.

The objective of this phase was to collect, analyse, and investigate security telemetry generated from the Windows enterprise environment.

## Contents

- Wazuh SIEM deployment
- Endpoint agent configuration
- Windows event collection
- Sysmon telemetry ingestion
- Security dashboard creation
- Detection validation

## Architecture
Active Directory Environment
DC01
- CLIENT01
- CLIENT02
- CLIENT03

Endpoint Monitoring
Windows Endpoints
- Sysmon Telemetry
- Wazuh Agents
- Security Monitoring Infrastructure
SOC01
- Wazuh Manager
- Security Dashboard
 
Wazuh provides centralised visibility into authentication activity, endpoint behaviour, and security events across the simulated enterprise environment.
