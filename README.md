# Active Directory Home Lab

## Overview

This project demonstrates the deployment and configuration of a Windows Server 2022 Active Directory environment using VirtualBox. The lab includes creating Organizational Units (OUs), domain users, security groups, shared folders, NTFS permissions, and connecting a Windows 11 client to the domain to verify authentication and network file access.

---

# Technologies Used

- Windows Server 2022
- Windows 11
- Active Directory Domain Services (AD DS)
- DNS
- NTFS Permissions
- SMB File Sharing
- VirtualBox

---

# Skills Demonstrated

- Active Directory Administration
- Organizational Unit (OU) Management
- User & Group Management
- Security Group Configuration
- Role-Based Access Control (RBAC)
- NTFS Permissions
- Shared Folder Configuration
- Domain Joining
- Network File Sharing
- Windows Server Administration

---

# Lab Environment

| Component | Description |
|-----------|-------------|
| Hypervisor | VirtualBox |
| Server | Windows Server 2022 |
| Client | Windows 11 |
| Services | Active Directory Domain Services, DNS |
| Network | Internal Network |
| Authentication | Active Directory Domain |

---

# Project Walkthrough

## 1. Created Active Directory Environment

Configured a Windows Server 2022 virtual machine and promoted it to a Domain Controller.

![image alt](<img width="1012" height="762" alt="image" src="https://github.com/user-attachments/assets/0f068501-e23c-485b-9779-551fc794c7f9" />)



---

## 2. Created Organizational Units (OUs)

Created departmental Organizational Units to organize users and resources.

Departments:

- IT
- HR
- Finance
- Sales

**Screenshot**

![OUs](screenshots/02-organizational-units.png)

---

## 3. Created Domain Users

Created multiple Active Directory user accounts for each department.

**Screenshot**

![Users](screenshots/03-users.png)

---

## 4. Created Security Groups

Configured security groups for department-based access control.

Examples:

- IT_Admins
- IT_Users
- HR_Admins
- HR_Users
- Finance_Admins
- Finance_Users
- Sales_Admins
- Sales_Users

**Screenshot**

![Groups](screenshots/04-security-groups.png)

---

## 5. Assigned Users to Security Groups

Added users to the appropriate Active Directory security groups.

**Screenshot**

![Group Membership](screenshots/05-group-membership.png)

---

## 6. Configured Shared Folder Permissions

Created departmental shared folders and configured NTFS permissions using security groups.

**Screenshot**

![Permissions](screenshots/06-ntfs-permissions.png)

---

## 7. Joined Windows 11 Client to the Domain

Successfully joined a Windows 11 workstation to the Active Directory domain.

**Screenshot**

![Domain Join](screenshots/07-domain-joined-client.png)

---

## 8. Accessed Shared Network Resources

Verified access to the shared folder from the Windows 11 domain client using the network share.

Example:

```
\\192.168.1.32\Company Data\IT
```

**Screenshot**

![Network Share](screenshots/08-network-share.png)

---

## 9. Verified File Access

Successfully opened files stored on the Windows Server from the Windows 11 client.

**Screenshot**

![Shared File](screenshots/09-opened-file.png)

---

# Key Takeaways

During this lab I learned how to:

- Deploy Active Directory Domain Services
- Create Organizational Units
- Create domain users
- Create and manage security groups
- Configure NTFS permissions
- Configure SMB shared folders
- Join Windows clients to a domain
- Authenticate users through Active Directory
- Access shared resources across the network
- Troubleshoot Active Directory networking issues

---

# Future Improvements

- Configure Group Policy Objects (GPOs)
- Implement password policies
- Configure folder redirection
- Automate administration with PowerShell
- Add roaming profiles
- Integrate Microsoft Defender or Microsoft Sentinel

---

# Screenshots

```
screenshots/
│
├── 01-domain-controller.png
├── 02-organizational-units.png
├── 03-users.png
├── 04-security-groups.png
├── 05-group-membership.png
├── 06-ntfs-permissions.png
├── 07-domain-joined-client.png
├── 08-network-share.png
└── 09-opened-file.png
```

---
