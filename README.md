# Active Directory Lab — Shanthiraj Theetla

Hands-on Active Directory lab documenting real-world AD DS administration, OU design,
Group Policy, PowerShell automation, troubleshooting, hybrid identity, and PKI
with Active Directory Certificate Services (AD CS).

**Certifications:** AZ-900 · AZ-104  
**In progress:** AZ-500 (Azure Security Engineer)  
**Lab Domain:** learnig.co.in (Proxmox — Windows Server 2022)  
**LinkedIn:** (https://www.linkedin.com/in/shanthiraj-theetla-076a58194/)

---

## Lab Areas

| Area | Topics Covered | Status |
| --- | --- | --- |
| [01 — AD DS Setup](./01-adds-setup/) | Install AD DS role, promote to DC, DNS configuration | Active |
| [02 — OUs & Delegation](./02-ous-delegation/) | OU hierarchy design, delegation of control | Active |
| [03 — Users & Groups](./03-users-groups/) | User creation, group types, nesting, bulk management | Active |
| [04 — Group Policy](./04-gpos/) | Password policy, logon scripts, GPO inheritance, troubleshooting | Active |
| [05 — PowerShell Automation](./05-powershell-ad/) | AD cmdlets, bulk operations, inactive user reports | Active |
| [06 — Troubleshooting](./06-troubleshooting/) | Replication failures, account lockouts, DNS issues, logon errors | Active |
| [07 — Hybrid Identity](./07-hybrid-identity/) | Entra Connect setup, sync rules, verified domain, SSO | Active |
| [08 — PKI & AD CS](./08-pki-adcs/) | Install AD CS, Root CA, certificate templates, auto-enrolment, HTTPS | Active |

---

## Lab Environment

| Component | Details |
| --- | --- |
| Virtualization | Proxmox VE (running on physical hardware) |
| Domain Controller | dc-prx-01 — Windows Server 2022 |
| Domain Name | learnig.co.in |
| IP Address | 192.168.31.10 |
| Client Machine | Windows 10/11 |
| Hybrid Identity | Microsoft Entra Connect 2.5.79.0 — Password Hash Sync |
| Entra Tenant | Shanthislaboutlook.onmicrosoft.com |

---

## Hybrid Identity

On-premises Active Directory extended into Microsoft Entra ID using Entra Connect.

| Component | Details |
| --- | --- |
| On-prem DC | dc-prx-01 — Windows Server 2022, domain learnig.co.in |
| Directory Sync | Entra Connect 2.5.79.0 — Password Hash Sync confirmed |
| Synced Users | testuser@learnig.co.in and additional users synced to Entra ID |
| Entra Tenant | P2 features enabled — Conditional Access, PIM tested |

**Hybrid lab series:** Covers domain setup, Entra Connect installation, sync verification,
Conditional Access on synced users, and PIM for hybrid accounts.

---

## PKI & AD CS

Active Directory Certificate Services lab covering enterprise PKI deployment.

| Component | Details |
| --- | --- |
| CA Type | Enterprise Root CA — installed on Windows Server 2022 |
| Role | Active Directory Certificate Services (AD CS) |
| Topics | Root CA setup, certificate templates, auto-enrolment via GPO, HTTPS certs |
| AZ-500 Relevance | Certificate-based auth, NDES, integration with Azure services |

---

## Tools & Technologies

- **Administration:** ADUC, GPMC, DNS Manager, Certification Authority MMC
- **Scripting:** PowerShell — ActiveDirectory module, PKI cmdlets
- **Hybrid:** Microsoft Entra Connect, Microsoft Entra ID (P2)
- **Virtualisation:** Proxmox VE, Windows Server 2022

---

## Related Repo

Azure Administrator labs (AZ-104) covering identity, networking, compute, security, and automation:  
👉 [azure_Learning](https://github.com/Shanthiraj519/azure_Learning)
```
