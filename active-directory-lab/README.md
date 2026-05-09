# Hospital Active Directory Security Architecture and Access Control Implementation

## Project Overview

This project involved designing and implementing a secure Active Directory environment for a simulated healthcare organisation using Windows Server 2022.

The healthcare environment was selected to simulate the security and access control requirements associated with protecting sensitive operational and patient-related information.

The project focused on centralized identity and access management (IAM), role-based access control (RBAC), Group Policy enforcement, authentication security, and recovery planning aligned with enterprise cybersecurity principles.

---

## Environment

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- Windows 11 Client Systems
- Virtualized UTM Lab Environment

---

## Organizational Structure

The following departments were configured within Active Directory Organizational Units (OUs):

- Cybersecurity Department
- Network Management Department
- Cloud Services Department
- Software Development Department
- Desk Support Department
- IT Infrastructure Support
- Data Management and Analytics
- Telecommunications

Each department was organized using Organizational Units (OUs) within Active Directory.

---

## Security Implementation

### Identity and Access Management

- Created domain users and department-specific security groups
- Structured Organizational Units (OUs) for administrative separation
- Implemented account lifecycle management by disabling former employee accounts
- Configured restricted guest accounts for temporary access scenarios
- Applied centralized account management policies

### Access Enforcement and Group Policy

- Integrated Windows 11 client systems into the Active Directory domain environment
- Restricted access to:
  - Command Prompt
  - Registry Editor
  - Control Panel
- Configured login notification banners
- Applied security restrictions using Group Policy

### Role-Based Access Control and Least Privilege

- Configured department-specific shared folders
- Restricted cross-department access
- Applied role-based access permissions
- Implemented least privilege principles

### Authentication Security

- Configured domain-based authentication through Active Directory
- Implemented account lockout policies after repeated failed login attempts
- Applied automatic device locking after inactivity
- Researched MFA and CAPTCHA integration limitations within standard AD environments

### Backup and Recovery Planning

- Planned Active Directory system state backups
- Planned encrypted database backup strategies
- Configured mapped backup storage locations conceptually
- Reviewed recovery and business continuity planning procedures

---

## Key Security Concepts Demonstrated

- Active Directory Administration
- Windows Server 2022 Administration
- Group Policy Management
- User and Group Management
- Role-Based Access Control (RBAC)
- Identity and Access Management (IAM)
- Authentication and Access Security
- Shared Folder Permission Management
- Windows Endpoint Security Configuration
- Backup and Recovery Planning
- Security Policy Enforcement

---

## Lab Constraints and Limitations

Some advanced configurations such as encrypted MS-SQL backups and full Windows Server backup implementation were partially constrained by virtualized lab environment storage limitations within the UTM environment.

Despite these constraints, the security design, configuration planning, and implementation methodology were analysed and documented as part of the project.

Additionally, CAPTCHA and advanced MFA functionality were researched conceptually but not fully implemented because standard Active Directory environments do not natively provide CAPTCHA-based authentication without additional third-party services or cloud-based identity solutions.

---

## Screenshots and Evidence

Relevant configuration screenshots, access control examples, Group Policy settings, and Active Directory structures are included within the project folders.

---

## Disclaimer

This project was developed within a controlled educational lab environment for learning and portfolio purposes.
