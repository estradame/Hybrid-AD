# Enterprise-Grade Hybrid Active Directory Environment with Azure Integration 

[![Azure](https://img.shields.io/badge/Azure-0089D6?logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com)
[![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?logo=powershell&logoColor=white)](https://learn.microsoft.com/en-us/powershell/)
[![Active Directory](https://img.shields.io/badge/Active_Directory-0078D4?logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)

Demonstrating the implementation of a hybrid Active Directory environment that integrates on-premises Active Directory with Azure Active Directory (Entra ID), featuring security hardening & PowerShell automation. ![Hybrid-AD](https://learn.microsoft.com/en-us/entra/identity/devices/media/concept-hybrid-join/azure-ad-hybrid-joined-device.png)

---

## **Overview**  
| Phase | Description | Key Tools |  
|-------|-------------|-----------|  
| [Lab Setup](docs/Lab-Setup.md) | Built a hybrid lab with on-prem AD + Azure AD | VirtualBox, Windows Server 2022, Azure VPN Gateway |  
| [Hybrid Identity](docs/Hybrid-Identity.md) | Synced users/groups via Azure AD Connect | PowerShell, Microsoft Entra Connect |  
| [Security & Compliance](docs/Security-Compliance.md) | Enforced MFA, GPOs, and Conditional Access | GPO, Azure MFA |  
| [Automation](docs/Automation-Lifecycle.md) | Scripted user lifecycle management | PowerShell, Graph API |  

---

## **Features Deployed**  
- **Hybrid Identity Sync:** Seamless SSO between on-prem AD and Azure AD.  
- **Security Hardening:** Disabled legacy protocols, enforced MFA, and deployed GPOs.  
- **Automated User Lifecycle:** PowerShell scripts for onboarding/offboarding users.  

---

## **Screenshots**  
| Azure AD Connect Sync | Conditional Access Policy |  
|-----------------------|---------------------------|  
| ![Sync Health](docs/screenshots/sync-health.png) | ![Conditional Access](docs/screenshots/conditional-access.png) |  

---

## **Repository Structure**  
```bash
Hybrid-AD/  
├── docs/         # Detailed phase documentation  
├── scripts/      # PowerShell automation scripts  
├── diagrams/     # Architecture diagrams  
└── backups/      # GPO backups and configs  
```

---


## **License**  
MIT License - Feel free to adapt this project for your learning!
