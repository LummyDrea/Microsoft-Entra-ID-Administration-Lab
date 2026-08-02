# Microsoft Entra ID Administration Lab

## Overview

This project demonstrates hands-on administration of **Microsoft Entra ID (formerly Azure Active Directory)** in a Microsoft 365 cloud environment. The lab focuses on identity and access management (IAM) tasks commonly performed by IT Support Specialists, Microsoft 365 Administrators, and Junior Systems Administrators.

The project covers user administration, group management, administrative role assignments, Multi-Factor Authentication (MFA), password management, audit logging, sign-in monitoring, enterprise applications, and app registrations.

---

## Lab Objectives

- Create and manage Microsoft Entra ID users
- Configure user properties
- Create Security Groups
- Configure Dynamic Membership Rules
- Assign Microsoft Entra administrative roles
- Reset user passwords
- Configure Multi-Factor Authentication (MFA)
- Register authentication methods
- Monitor Sign-in Logs
- Review Audit Logs
- Explore Enterprise Applications
- Explore App Registrations
- Review Tenant Configuration

---

# Lab Environment

| Component | Details |
|-----------|----------|
| Platform | Microsoft Entra Admin Center |
| Tenant | Ayodeji Solutions |
| Primary Domain | AyodejiSolutions.onmicrosoft.com |
| License | Microsoft Entra ID Premium P2 |
| Authentication | Password + Microsoft Authenticator |
| Browser | Microsoft Edge |

---
## Microsoft Entra ID Admin Center Homepage
#
<img width="1898" height="911" alt="Screenshot 2026-08-02 102525" src="https://github.com/user-attachments/assets/321a966c-484b-4e44-a0bd-09c10cf80a41" />



---
# Technologies Used

- Microsoft Entra ID
- Microsoft 365 Admin Center
- Microsoft Authenticator
- Microsoft Graph
- Enterprise Applications
- App Registrations
- Security Groups
- Dynamic Membership Rules
- Multi-Factor Authentication
- Identity & Access Management (IAM)

---

# Lab Tasks

## 1. User Administration

Created multiple users representing different departments within an organisation.

Departments included:

- IT
- Human Resources
- Sales
- Marketing
- Finance

### Users Created

| Name | Job Title | Department |
|------|-----------|------------|
| Ayodeji Awe | IT Admin | IT |
| Alice Johnson | IT Support Technician | IT |
| Donald Jacob | IT Support Technician | IT |
| John Truden | IT Support Technician | IT |
| Bob Smith | Sales Executive | Sales |
| David Wilson | Sales Executive | Sales |
| Charles Baker | Sales Executive | Sales |
| Charlie Brown | Marketing Officer | Marketing |
| Chris Evan | Marketing Officer | Marketing |
| Emma Davis | Accountant | Finance Department |
| Adefunke Talabi | HR Officer | Human Resources |
| Tyler Smith | HR Officer | Human Resources |
| Wade Johnson | HR Officer | Human Resources |

---

## 2. Password Management

Performed password administration tasks including:

- Reset user passwords
- Generated temporary passwords
- Forced password change at first sign-in
- Verified successful password update

Example:

- Alice Johnson password reset
- Temporary password generated
- User required to change password during first sign-in

---

## 3. Multi-Factor Authentication (MFA)

Configured Microsoft Entra authentication methods.

Tasks completed:

- Registered Microsoft Authenticator
- Set Microsoft Authenticator as the default authentication method
- Enabled MFA for selected users
- Verified successful MFA authentication

---

## 4. Administrative Roles

Assigned Microsoft Entra administrative roles.

Example:

**Helpdesk Administrator**

Role capabilities:

- Reset passwords
- Support end users
- Perform delegated identity administration

Verified role assignment from the **Assigned Roles** blade.

---

## 5. Security Groups

Created a Security Group.

| Setting | Value |
|---------|-------|
| Group Name | HR Department |
| Group Type | Security |
| Membership Type | Dynamic User |
| Microsoft Entra Roles Assignable | Yes |

---

## 6. Dynamic Membership Rules

Configured automatic user membership based on user attributes.

### Rule

```text
(user.department -eq "Human Resources") and (user.jobTitle -eq "HR Officer")
```

This automatically adds users whose:

- Department = Human Resources
- Job Title = HR Officer

Validated the rule before saving.

---

## 7. Sign-in Monitoring

Reviewed Microsoft Entra Sign-in Logs.

Information monitored included:

- Interactive Sign-ins
- Non-interactive Sign-ins
- Authentication Status
- Request ID
- Correlation ID
- IP Address
- MFA Status
- Authentication Requirement
- Applications Accessed

Observed both successful and interrupted authentication events.

---

## 8. Audit Logs

Reviewed Microsoft Entra Audit Logs.

Activities monitored included:

- Password Changes
- Password Reset Attempts
- User Updates
- Authentication Registration
- Security Information Registration
- Token Refresh Updates

Observed both successful and failed administrative operations.

---

## 9. Enterprise Applications

Explored Enterprise Applications.

Example reviewed:

**Google Cloud / G Suite Connector by Microsoft**

Examined:

- Application Properties
- Single Sign-On (SSO)
- Provisioning
- Permissions
- Security Settings
- Sign-on URL
- Owners
- Roles

---

## 10. App Registrations

Reviewed Microsoft Entra App Registration configuration.

Examined:

- Application (Client) ID
- Object ID
- Directory (Tenant) ID
- Redirect URIs
- API Permissions
- Certificates & Secrets
- Branding
- Authentication Settings

---

## 11. Tenant Configuration

Reviewed tenant information including:

- Default Domain
- Custom Domain Names
- Tenant Overview
- Microsoft Entra Connect
- Identity Secure Score
- Tenant Status

---

# Screenshots

| Screenshot | Description |
|------------|-------------|
| 01 | Microsoft Entra Dashboard |
| 02 | All Users |
| 03 | User Properties |
| 04 | Password Reset |
| 05 | MFA Configuration |
| 06 | Assigned Roles |
| 07 | Create Security Group |
| 08 | Dynamic Membership Rule |
| 09 | Rule Validation |
| 10 | Audit Logs |
| 11 | Sign-in Logs |
| 12 | Enterprise Application |
| 13 | App Registration |
| 14 | Custom Domain |
| 15 | Tenant Overview |

---

# Skills Demonstrated

- Microsoft Entra ID Administration
- Identity & Access Management (IAM)
- Microsoft 365 Administration
- User Lifecycle Management
- Role-Based Access Control (RBAC)
- Dynamic Security Groups
- Password Administration
- Multi-Factor Authentication (MFA)
- Microsoft Authenticator
- Enterprise Application Management
- App Registration Management
- Identity Monitoring
- Audit Log Analysis
- Sign-in Monitoring
- Cloud Identity Administration

---

# Project Structure

```text
Microsoft-Entra-ID-Administration-Lab
│
├── README.md
│
├── Screenshots
│   ├── 01-Entra-Dashboard.png
│   ├── 02-Users.png
│   ├── 03-User-Properties.png
│   ├── 04-Password-Reset.png
│   ├── 05-MFA-Configuration.png
│   ├── 06-Assigned-Roles.png
│   ├── 07-Create-Security-Group.png
│   ├── 08-Dynamic-Membership-Rule.png
│   ├── 09-Rule-Validation.png
│   ├── 10-Audit-Logs.png
│   ├── 11-Signin-Logs.png
│   ├── 12-Enterprise-Application.png
│   ├── 13-App-Registration.png
│   ├── 14-Custom-Domain.png
│   └── 15-Tenant-Overview.png
│
└── Documentation.pdf
```

---

# Key Learning Outcomes

This lab provided practical experience managing cloud identities using Microsoft Entra ID. It strengthened skills in identity administration, user management, authentication, role delegation, dynamic group membership, enterprise applications, security monitoring, and cloud-based identity governance.

The project demonstrates real-world administrative tasks commonly performed by IT Support Specialists, Microsoft 365 Administrators, and Junior Systems Administrators.

---

# Author

**Ayodeji Olumide Awe**

**CompTIA Security+ Certified**

**IT Support | Microsoft 365 | Microsoft Entra ID | Active Directory | Windows Administration | Cybersecurity**
