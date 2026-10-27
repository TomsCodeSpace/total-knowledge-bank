# Official Windows Active Directory: Five-Belt Learning & Project Roadmap

**Technical Knowledge Bank & Project Portfolio**

## Overview

This roadmap organizes Windows Active Directory into five progressive skill levels, advancing from foundational identity management to enterprise administration, security engineering, and directory infrastructure architecture.

Each belt combines technical concepts with hands-on projects, troubleshooting scenarios, administrative procedures, and documented verification. The goal is to build a practical, reusable knowledge base that demonstrates skills relevant to Help Desk, IT Specialist, Desktop Support, and Systems Administrator roles.

### Learning progression

| Belt | Difficulty | Primary focus |
| --- | --- | --- |
| White | Beginner | Identity management fundamentals and initial domain deployment |
| Blue | Beginner–Intermediate | User, device, and resource administration |
| Purple | Intermediate | Authentication troubleshooting and administrative automation |
| Brown | Advanced | Enterprise administration, replication, and operational management |
| Black | Expert-Level Projects | Directory architecture, security engineering, and disaster recovery |

*Belt levels represent practical learning milestones, not formal industry certifications.*

---

# Belt 1 — White Belt: Active Directory Foundations

**Focus:** Understand identity management and build a functioning domain environment.

### Objective

Develop a foundational understanding of Active Directory Domain Services (AD DS), its core components, and the dependencies required for domain-based authentication.

### Practical project topics

1. Active Directory Domain Services fundamentals
2. Domains, forests, trees, and domain controllers
3. Windows Server installation and initial configuration
4. Virtual machines and isolated lab networking
5. DNS fundamentals and domain name resolution
6. Installing AD DS and promoting a server to a domain controller
7. Creating and inspecting a domain
8. Joining a Windows client to a domain
9. Active Directory Users and Computers (ADUC)
10. Domain authentication fundamentals

### Capstone project: Single-Domain Lab

Build a functioning domain environment with one domain controller, one Windows client, and a test user.

**Completion criteria:**

- AD DS is installed and configured.
- The client successfully joins the domain.
- The test user can authenticate using a domain account.
- DNS configuration and domain connectivity are verified.
- The topology, configuration, and test results are documented.

---

# Belt 2 — Blue Belt: User & Device Administration

**Focus:** Manage identities, computers, permissions, and organizational resources.

### Objective

Develop the practical skills needed to perform routine identity and access administration in a small-business environment.

### Practical project topics

1. Creating, modifying, disabling, and deleting user accounts
2. Organizational Units (OUs) and directory organization
3. Security groups and distribution groups
4. Group-based permissions and role separation
5. Password resets, account lockouts, and account status
6. Joining, renaming, moving, and removing domain computers
7. Group Policy Objects (GPOs): creation, linking, and basic settings
8. Shared folders and NTFS permissions
9. Domain-based resource access
10. Account and access request documentation

### Capstone project: Small-Business Identity Management

Build a fictional business directory containing multiple departments, user accounts, security groups, and shared folders with department-specific access restrictions.

**Completion criteria:**

- Accounts and groups follow a consistent naming convention.
- Users are assigned appropriate group memberships.
- Access to shared folders follows least-privilege principles.
- Basic Group Policy settings are applied and verified.
- Sample onboarding, access-change, and offboarding requests are documented.

---

# Belt 3 — Purple Belt: Troubleshooting & Automation

**Focus:** Diagnose directory failures, establish root causes, and automate routine administration.

### Objective

Develop a repeatable troubleshooting process for authentication, DNS, Group Policy, permissions, and domain connectivity issues.

### Practical project topics

1. Domain sign-in and authentication failures
2. DNS misconfiguration and domain discovery failures
3. Group Policy troubleshooting using `gpupdate` and `gpresult`
4. Account lockouts, expired passwords, and disabled accounts
5. Secure channel and domain trust troubleshooting
6. Time synchronization and Kerberos fundamentals
7. Event Viewer and relevant Windows logs
8. PowerShell administration of users, groups, and computers
9. Bulk account operations and input validation
10. Permissions troubleshooting and least-privilege verification
11. Domain-controller health checks
12. Basic backup, recovery, and rollback procedures

### Capstone project: Broken-Domain Troubleshooting Lab

Build a working domain, introduce five controlled faults, and resolve them using a documented diagnostic process.

Potential scenarios include incorrect DNS settings, failed Group Policy application, account lockouts, incorrect group membership, and shared-folder access failures.

**Completion criteria:**

- Each fault produces a reproducible symptom.
- Diagnostic commands and relevant logs are recorded.
- The root cause is distinguished from the initial symptom.
- Each fix is validated with a post-repair test.
- Prevention recommendations are included in the incident report.

All deliberate faults must remain within an isolated lab environment.

---

# Belt 4 — Brown Belt: Enterprise Administration

**Focus:** Manage larger directory environments and enforce organizational standards.

### Objective

Progress from individual account administration to managing directory health, delegated administration, replication, automation, and operational recovery.

### Practical project topics

1. Advanced Group Policy design, inheritance, and precedence
2. Group Policy security filtering and delegation
3. Active Directory replication and health checks
4. Additional domain controllers and redundancy
5. Active Directory Sites and Services
6. Organizational access models and delegated administration
7. PowerShell automation for onboarding and offboarding
8. Service accounts and managed service accounts
9. Active Directory backup and recovery concepts
10. Monitoring, auditing, and directory health
11. Directory permissions and administrative boundaries
12. Hybrid identity fundamentals, Microsoft Entra ID, and directory synchronization

### Capstone project: Multi-Department Directory Environment

Design a multi-department business environment with redundant domain controllers where feasible, standardized workstation policies, delegated administration, and scripted employee onboarding.

**Completion criteria:**

- Directory structure reflects the organization's needs.
- Replication and domain-controller health are verified where applicable.
- Administrative responsibilities are appropriately delegated.
- Account lifecycle tasks are automated and tested.
- Recovery procedures and monitoring checks are documented.
- A technical handover explains the architecture and operational procedures.

---

# Belt 5 — Black Belt: Architecture, Security & Recovery

**Focus:** Design, harden, recover, and evaluate directory infrastructure.

### Objective

Integrate Active Directory administration with security engineering, enterprise architecture, disaster recovery, and long-term operational planning.

### Practical project topics

1. Forests, domains, trusts, and multi-domain architecture
2. Active Directory security architecture and attack paths
3. Privileged access management and administrative tiering
4. Kerberos security, delegation risks, and authentication hardening
5. Windows security baselines and advanced auditing
6. Domain-controller protection and secure administration
7. Disaster recovery planning and recovery testing
8. Replication failures and complex directory diagnostics
9. Directory migrations and domain consolidation concepts
10. Hybrid identity security and access lifecycle design
11. Infrastructure documentation, monitoring, and operational standards
12. Security assessment and remediation planning

### Capstone project: Enterprise Active Directory Architecture

Produce an enterprise-style Active Directory deployment plan, threat assessment, security-hardening checklist, disaster recovery procedure, and demonstrated recovery test in an isolated lab.

**Completion criteria:**

- Architecture decisions and security boundaries are documented.
- Privileged access and administrative roles are defined.
- Security controls are tested against documented requirements.
- Recovery objectives and procedures are established.
- A controlled recovery exercise demonstrates the documented process.
- Final deliverables include diagrams, test results, risks, and recommendations.

---

# Standard Notes’ Documentation Framework

Every belt uses the same documentation structure to keep the knowledge base consistent, navigable, and useful to both technical reviewers and future colleagues.

| Section | Purpose |
| --- | --- |
| **Big Picture Ideas** | Explain the role of identity, authentication, authorization, and directory services within an organization. |
| **Core Concepts** | Define technologies, protocols, components, and administrative principles. |
| **Text-Based Mindmaps** | Visualize dependencies, authentication flows, and troubleshooting decision paths. |
| **Initial Setup Guides** | Provide repeatable lab construction instructions, configuration steps, and verification tests. |
| **Sample Tickets Solved** | Demonstrate realistic Help Desk and systems administration investigations. |
| **Sample Projects Completed** | Showcase working configurations with objectives, implementation steps, and evidence. |
| **Scripts & Automation** | Store tested PowerShell commands, reusable scripts, prerequisites, and expected outputs. |
| **Security & Recovery** | Document access controls, hardening, backup, recovery, and validation procedures. |

---

# Project Completion Standard

Every completed project should include:

- [ ]  Clear objective and scope
- [ ]  Prerequisites and lab requirements
- [ ]  Relevant topology or architecture diagram
- [ ]  Reproducible implementation instructions
- [ ]  Configuration details and commands
- [ ]  Verification steps and supporting evidence
- [ ]  Troubleshooting scenario or diagnostic notes
- [ ]  Security considerations and known limitations
- [ ]  Results, lessons learned, and recommended next steps

## Guiding principle

**Build it. Understand it. Administer it. Break it safely. Diagnose it. Secure it. Recover it. Document it.**

The purpose of this roadmap is to develop a practical Active Directory knowledge bank that demonstrates not only familiarity with directory services, but also the ability to configure, administer, troubleshoot, automate, and maintain identity infrastructure.
