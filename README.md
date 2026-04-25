```markdown
# 🏢 Active Directory Lab

![Windows Server](https://img.shields.io/badge/Windows%20Server-2022-0078D4?style=flat&logo=windows&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-VE-E57000?style=flat&logo=proxmox&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat&logo=powershell&logoColor=white)
![Entra ID](https://img.shields.io/badge/Microsoft%20Entra%20ID-Hybrid%20Identity-0078D4?style=flat&logo=microsoftazure&logoColor=white)

> Hands-on Active Directory lab documenting real-world AD DS administration, GPO management,
> PowerShell automation, and hybrid identity — built on a home lab running Proxmox.

---

## 🧱 Lab Environment

| Component         | Details                                      |
|-------------------|----------------------------------------------|
| Virtualization    | Proxmox VE (hosted on physical hardware)     |
| Domain Controller | `dc-prx-01` — Windows Server 2022            |
| Domain Name       | `learnig.co.in`                              |
| IP Address        | `192.168.31.10`                              |
| Client Machine    | Windows 10/11                                |
| Hybrid Identity   | Microsoft Entra Connect 2.5.79.0             |
| Entra Tenant      | `Shanthislaboutlook.onmicrosoft.com`         |

---

## 📁 Lab Index

| # | Lab | Description | Status |
|---|-----|-------------|--------|
| 01 | [AD DS Setup & Domain Promotion](./01-AD-DS-Setup/) | Install AD DS role, promote server to DC, configure DNS | 
| 02 | [OUs & Delegation of Control](./02-OUs-Delegation/) | Design OU hierarchy, delegate admin control to specific users | 
| 03 | [Users & Groups Management](./03-Users-Groups/) | Create/manage users and groups via GUI and PowerShell | 
| 04 | [Group Policy Objects (GPOs)](./04-GPOs/) | Password policies, logon scripts, software restriction, GPO inheritance |
| 05 | [PowerShell Automation for AD](./05-PowerShell-AD/) | Bulk user creation, inactive user reports, group membership scripts
| 06 | [Troubleshooting Scenarios](./06-Troubleshooting/) | Replication failures, account lockouts, DNS issues, logon errors 
| 07 | [Hybrid Identity — Entra Connect](./07-Hybrid-Identity/) | Sync on-prem AD to Microsoft Entra ID, verified domain, SSO

---

## ⚙️ Topics Covered

- **AD DS Installation** — Deploying and promoting a Domain Controller from scratch on Windows Server 2022
- **DNS Integration** — Configuring DNS as part of AD DS, forward/reverse lookup zones, troubleshooting resolution issues
- **OU Structure** — Designing organisational units for real-world role-based administration
- **User & Group Management** — Bulk creation, group types (Security vs Distribution), nesting, and membership management
- **Group Policy (GPO)** — Implementing and troubleshooting policies across OUs including password, lockout, and desktop policies
- **PowerShell Automation** — Scripting day-to-day AD tasks using the ActiveDirectory module
- **Troubleshooting** — Real-world scenarios encountered in lab and professional environments
- **Hybrid Identity** — Extending on-premises AD to Microsoft Entra ID using Entra Connect with verified custom domain

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Windows Server 2022 | Domain Controller OS |
| Active Directory Domain Services | Core directory service |
| DNS Server | Name resolution for AD |
| Group Policy Management Console | GPO creation and linking |
| PowerShell (ActiveDirectory module) | Automation and scripting |
| Microsoft Entra Connect 2.5.79.0 | Hybrid identity sync |
| Proxmox VE | Home lab virtualisation |

---

## 🎯 Objective

To document and demonstrate practical Active Directory skills built through hands-on lab work —
aligned with real-world IT administration, Azure Administrator (AZ-104), and
Azure Security Engineer (AZ-500) certification requirements.

---

## 👨‍💻 About Me

IT professional with 5+ years of experience across desktop support, Active Directory engineering,
and systems administration.

| | |
|---|---|
| 📜 Certifications | Microsoft AZ-900 · AZ-104  | Az-500 (Inprogress)
| ☁️ Azure Labs | [azure_Learning](https://github.com/shanthirajtheetla/azure_Learning) |
| 📍 Location | Hyderabad, India |

---

## 📌 Notes

- Each lab folder contains a full step-by-step `README.md` with commands, screenshots, and outcome verification
- Labs are built using a personal home lab — no paid sandbox environment used
- Repository is continuously updated as new scenarios are explored and documented
```
