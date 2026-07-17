# Active Directory Home Lab - Progress Log

## Day 1 Progress

### Completed

✅ Created Windows Server 2022 virtual machine  
- Installed Windows Server 2022 Evaluation Edition in Oracle VirtualBox
- Configured VM resources (CPU, RAM, networking)

✅ Configured Network Settings
- Assigned a static IP address to the Windows Server VM
- Configured subnet mask
- Configured DNS to point to the future Domain Controller

Why:
A Domain Controller requires a consistent IP address because network services such as DNS and Active Directory rely on stable addressing.

✅ Installed Active Directory Domain Services
- Added the AD DS server role
- Began Domain Controller promotion

### In Progress

🔄 Promoting Windows Server 2022 to a Domain Controller

Configuration:
- Domain: cyberlab.local
- NetBIOS Name: CYBERLAB
- DNS Server: Enabled
- Global Catalog: Enabled

### Concepts Learned

## Active Directory
Active Directory provides centralized identity and access management for Windows environments.

Key functions:
- User authentication
- Computer management
- Security policies
- Permission management

## Domain Controllers
A Domain Controller is a server running Active Directory Domain Services that manages:
- User accounts
- Computer accounts
- Authentication requests
- Group Policy

## DNS in Active Directory
DNS allows domain computers to locate services by translating names into IP addresses.

Example:

DC01.cyberlab.local → 192.168.x.x

## Networking Concepts Practiced

- Static IP addressing
- Subnet masks

  ## Future Lab Expansion

Planned:

- Add Windows 11 client VM
- Join client to the domain
- Create users and groups
- Configure Organizational Units
- Implement Group Policy Objects
- Create file shares and permissions
- Perform security auditing
- Test common Active Directory attack techniques in a controlled environment
- DNS configuration
- Virtual networking
- Client/server architecture
