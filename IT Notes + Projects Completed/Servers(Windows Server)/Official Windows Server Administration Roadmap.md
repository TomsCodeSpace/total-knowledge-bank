# Official Windows Server Administration: Five-Belt Learning & Project Roadmap

# Windows Server Administration: Five-Belt Learning & Project Roadmap

**Technical Knowledge Bank & Project Portfolio**

## Overview

This roadmap organizes Windows Server administration into five progressive skill levels, moving from foundational server configuration to enterprise infrastructure design, automation, security, and recovery.

Each belt combines technical concepts with hands-on labs, practical projects, troubleshooting exercises, and documented verification. The objective is to develop repeatable administrative skills and demonstrate them through a portfolio of reproducible lab environments.

### Learning Progression

| Belt | Level | Primary Focus |
| --- | --- | --- |
| White | Beginner | Server fundamentals and initial configuration |
| Yellow | Beginner–Intermediate | IT support operations and domain administration |
| Red | Intermediate | Systems troubleshooting and root-cause analysis |
| Brown | Advanced | Infrastructure, security, automation, and recovery |
| Black | Expert-Level Projects | Infrastructure engineering and architecture |

*Belt levels represent learning milestones, not formal industry certifications or a substitute for professional experience.*

---

# Recommended Lab Environment

Most projects can be completed using virtual machines, allowing infrastructure to be built, tested, broken, restored, and documented without dedicated physical servers.

### Core Lab Components

- **Hypervisor:** Hyper-V, VMware Workstation, or VirtualBox, depending on host and guest compatibility.
- **Server operating system:** A supported Windows Server evaluation installation.
- **Client operating system:** A compatible Windows client installation with appropriate licensing.
- **Administration tools:** Server Manager, Windows Admin Center, PowerShell, Event Viewer, and Windows networking utilities.
- **Documentation tools:** GitHub Markdown, network diagrams, screenshots, test results, and incident reports.

### Recommended Starting Configuration

Begin with one Windows Server virtual machine and one Windows client. Expand the environment as project complexity increases.

Use isolated virtual networks for experiments involving Active Directory, DNS, DHCP, firewall configuration, and security testing. Take known-good snapshots before introducing deliberate faults.

---

# Belt 1 — White Belt: Windows Server Fundamentals

**Level:** Beginner

**Focus:** Understand, configure, and observe.

### Objective

Establish a foundation in Windows Server installation, basic administration, networking, maintenance, and system verification before introducing domain infrastructure.

### Practical Project Topics

1. **Windows Server Installation**
    - Install a Windows Server evaluation image.
    - Compare Desktop Experience and Server Core.
    - Complete initial configuration and administrator setup.
    - Document installation settings and system requirements.
2. **Server Manager and Server Roles**
    - Navigate Server Manager.
    - Install and remove roles and features.
    - Inspect installed roles and services.
    - Use `Get-WindowsFeature` in PowerShell.
3. Computer Identity and Initial Configuration
4. Local Users and Groups
5. Local File Systems and Storage
6. Basic Network Configuration
7. Remote Server Access
8. Services and Processes
9. Event Logs and Basic Monitoring
10. Windows Update and Maintenance
11. Basic Windows Firewall Administration
12. Server Documentation and Verification

### Capstone Project: Standalone Server Setup

Build a Windows Server virtual machine, configure its network settings, create local accounts, install a server role, configure firewall rules, and document the resulting configuration.

**Completion criteria:**

- Server configuration is documented.
- Required services and network settings are verified.
- A client can reach the intended service.
- Access controls and firewall rules are tested.
- Evidence of successful operation is included in the project report.

---

# Belt 2 — Yellow Belt: IT Support Operations

**Level:** Beginner–Intermediate

**Focus:** Manage users, devices, and shared resources.

### Objective

Develop the practical skills required to support users, administer domain-connected computers, manage shared resources, and perform routine Windows infrastructure tasks.

### Practical Project Topics

1. **Active Directory Domain Services (AD DS)**
    - Install the AD DS role.
    - Promote a server to domain controller.
    - Create a lab domain.
    - Understand domain and forest concepts.
    - Verify basic domain-controller health.
2. Organizational Units (OUs)
3. Domain User Account Administration
4. Security Groups and Access Management
5. Windows Client Domain Joining
6. Shared Folders and Server Message Block (SMB)
7. File-Server Administration
8. Print Services
9. Group Policy Fundamentals
10. DNS Administration
11. DHCP Administration
12. Remote IT Support
13. Software and Configuration Deployment
14. Account and Device Lifecycle Management
15. Support Tickets and Standard Operating Procedures

### Capstone Project: Small Business Domain

Build a fictional business environment with three departments, a domain controller, two or more Windows client virtual machines, user accounts, security groups, shared folders, DNS, DHCP, and basic Group Policy.

**Completion criteria:**

- Domain clients successfully join and authenticate.
- Users and groups reflect the organizational structure.
- Shared-folder permissions enforce the intended access boundaries.
- Basic domain policies apply as expected.
- Administrative procedures and verification results are documented.

---

# Belt 3 — Red Belt: Systems and Network Troubleshooting

**Level:** Intermediate

**Focus:** Diagnose failures and establish root causes.

### Objective

Develop a systematic troubleshooting methodology that uses observable evidence, appropriate diagnostic tools, controlled testing, and documented corrective actions.

### Practical Project Topics

1. **DNS Failure Diagnosis**
    - Introduce incorrect client DNS settings in an isolated lab.
    - Diagnose missing or incorrect DNS records.
    - Investigate DNS suffix and name-resolution problems.
    - Inspect the DNS client cache.
    - Document the path from initial symptom to root cause.
2. DHCP Failure Diagnosis
3. Active Directory Health and Replication Checks
4. Group Policy Troubleshooting
5. Authentication and Account Failures
6. Permissions and Resource-Access Failures
7. Network Connectivity and Firewall Troubleshooting
8. Service Failures and Resource Exhaustion
9. File-Server Incidents
10. PowerShell-Based Troubleshooting
11. Patch and Update Failures
12. Remote Management Failures
13. Backup and Restore Troubleshooting
14. Performance and Capacity Monitoring
15. Incident Response and Root-Cause Analysis

### Capstone Project: Broken Office Infrastructure

Start with a functioning domain environment and introduce controlled faults, such as incorrect DNS settings, a faulty DHCP option, an incorrectly configured Group Policy Object, or an inappropriate folder permission.

For each incident, document:

- Initial symptoms and user impact
- Diagnostic commands and investigation steps
- Collected evidence
- Confirmed root cause
- Corrective action
- Post-repair verification
- Preventive recommendations

**Completion criteria:** Demonstrate the successful diagnosis and resolution of multiple independent incidents without relying solely on trial and error.

Retain a known-good snapshot and introduce faults only within the isolated lab.

---

# Belt 4 — Brown Belt: Infrastructure, Security, and Cloud

**Level:** Advanced

**Focus:** Secure, maintain, automate, and recover multi-server environments.

### Objective

Move beyond individual support tickets into infrastructure administration, security hardening, automation, resilience, and operational recovery.

### Practical Project Topics

1. **Multi-Server Architecture**
    - Separate domain controllers, file servers, and application services.
    - Maintain a server inventory.
    - Plan IP addressing, DNS dependencies, and naming conventions.
    - Document service dependencies and trust boundaries.
2. Multiple Domain Controllers and Replication
3. Active Directory Organizational Design
4. Group Policy Security Baselines
5. Windows Server Security Hardening
6. Windows LAPS and Local Administrator Management
7. PowerShell Administration Automation
8. PowerShell Remoting and Delegated Administration
9. Windows Server Backup and Recovery
10. Storage Spaces and Advanced Storage
11. File-Server Resource Management
12. Hyper-V Virtualization
13. Remote Access and Administrative Boundaries
14. Active Directory Certificate Services and PKI Fundamentals
15. Hybrid Identity and Cloud Integration
16. Monitoring, Logging, and Operational Health

### Capstone Project: Secure and Recoverable Small Business

Create a multi-server environment with redundant domain services where feasible, file sharing, security policies, automated account administration, centralized monitoring, and tested backups.

**Completion criteria:**

- Server roles and dependencies are documented.
- Redundancy and replication are tested where implemented.
- Administrative access follows least-privilege principles.
- Repetitive administrative tasks are automated and validated.
- Backup and recovery procedures are demonstrated.
- A security review identifies risks and recommended improvements.

---

# Belt 5 — Black Belt: Infrastructure Engineering and Architecture

**Level:** Expert-Level Projects

**Focus:** Design, automate, validate, and operate complete systems.

### Objective

Integrate Windows Server administration with resilient architecture, infrastructure automation, security engineering, operational standards, and enterprise-style change management.

Some projects may require additional virtual machines, licensing, hardware, or specialized infrastructure. Design documents, automation scripts, and validation plans remain valuable deliverables when full deployment is impractical.

### Practical Project Topics

1. **Enterprise Infrastructure Design**
    - Design a multi-site organization with multiple departments.
    - Plan IP addressing, DNS, DHCP, and routing dependencies.
    - Define domain and OU architecture.
    - Design identity, server, and management boundaries.
    - Produce an architecture diagram and implementation plan.
2. Active Directory Disaster Recovery
3. High Availability and Fault Tolerance
4. Advanced Group Policy and Configuration Control
5. Infrastructure Automation and Desired State
6. Automated Server Provisioning
7. Privileged Access and Identity Security
8. Security Auditing and Incident Investigation
9. Centralized Monitoring and Alerting
10. Backup Architecture and Disaster Recovery
11. Patch Management and Release Engineering
12. Multi-Site and Branch-Office Infrastructure
13. Hybrid Infrastructure Architecture
14. Infrastructure Monitoring as Code
15. Configuration Drift and Compliance
16. Enterprise Capstone and Technical Handover

### Capstone Project: Enterprise-Style Windows Infrastructure

Design and deploy a small but complete environment featuring separate server roles, Active Directory, managed Windows clients, secure access controls, automated configuration, monitoring, and recovery testing.

**Completion criteria:**

- Architecture and implementation decisions are documented.
- Identity, network, and administrative boundaries are defined.
- Configuration and operational checks are repeatable.
- Security controls and monitoring are validated.
- Controlled failure and recovery scenarios are demonstrated.
- The final handover includes diagrams, operating procedures, known limitations, and future improvements.

---

# Standard Notes’ Documentation Framework

Every project should use a consistent documentation structure so that another administrator can understand the objective, reproduce the configuration, and verify the results.

## 1. Big Picture Ideas

**Purpose:** Understand why the technology exists.

Explain its purpose, business value, place in the infrastructure, and the problems it solves.

*Example: Why organizations use Windows Server and Active Directory.*

## 2. Core Concepts

**Purpose:** Understand the components and how they work.

Define terminology, system components, processes, protocols, commands, configuration options, and dependencies.

*Example: Domain controllers, organizational units, DNS records, security groups, and Group Policy Objects.*

## 3. Text-Based Mind Maps

**Purpose:** Visualize relationships and dependencies.

Represent system components, information flows, decision paths, and troubleshooting sequences in a readable text-based format.

*Example: Client → DNS lookup → Domain Controller discovery → Authentication → Resource authorization.*

## 4. Initial Setup Guides

**Purpose:** Build a repeatable configuration.

Include prerequisites, equipment, network diagrams, numbered setup instructions, configuration commands, expected outputs, and verification tests.

*Example: Install AD DS, promote a server to a domain controller, configure DNS, and join a Windows client to the domain.*

## 5. Sample Tickets Solved

**Purpose:** Demonstrate practical diagnosis and resolution.

Simulate realistic IT support requests with symptoms, investigation steps, evidence, root cause, corrective actions, and verification.

*Example: An employee can sign in successfully but cannot access a department shared folder.*

## 6. Practical Projects and Capstones

**Purpose:** Demonstrate applied technical ability.

Include objectives, prerequisites, initial configuration, implementation steps, screenshots, test results, and completion criteria.

## 7. Security, Validation, and Recovery

**Purpose:** Establish that configurations are secure, functional, and recoverable.

Record permission tests, security checks, backup verification, recovery exercises, and relevant limitations.

---

# Portfolio Quality Standard

A project is considered complete when it contains:

- A clear objective and scope
- Prerequisites and lab requirements
- A documented topology or configuration diagram, where applicable
- Reproducible implementation instructions
- Relevant commands and configuration details
- Verification steps and supporting evidence
- Troubleshooting notes or a tested failure scenario
- Security considerations and known limitations
- A concise summary of results and lessons learned

## Guiding Principle

**Build it. Understand it. Break it safely. Diagnose it. Restore it. Document it.**

The objective is not simply to collect completed labs, but to develop a reusable technical knowledge base and demonstrate the ability to configure, administer, troubleshoot, secure, and maintain Windows infrastructure.