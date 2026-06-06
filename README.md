<div align="center">

# 🖥️ MCSA Windows Server Lab Project

**A fully configured Windows Server 2022 enterprise environment — built from scratch**

![Windows Server](https://img.shields.io/badge/Windows_Server-2022-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active_Directory-ITI.LOCAL-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white)
![IIS](https://img.shields.io/badge/IIS-Web_Server-5C2D91?style=for-the-badge&logo=microsoft&logoColor=white)
![ITI](https://img.shields.io/badge/ITI-Intake_46-E30613?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

</div>

---

## 🗺️ Infrastructure Architecture

<!-- ضع صورة الـ Architecture هنا -->
![Architecture](https://github.com/OmarHesham249/MCSA-project/blob/main/Project%20Architecture.png)

---

## 👥 Team

| Name |
|------|
| **Mohamed Morsi Saad** |
| **Ahmed Kamel** |
| **Omar Hesham** |
| **Marwan Tarek** |

> ITI Intensive Program — System Administration Track — Intake 46

---

## 📋 Project Overview

This project simulates a real-world enterprise Windows Server environment using **VMware Workstation** and **Windows Server 2022**. The infrastructure spans a multi-domain Active Directory forest with full role deployment including DHCP, DNS, GPO, IIS, FTP, and WDS.

---

## 🏗️ Domain Structure

```
Forest Root: ITI.LOCAL
├── DC1  (Primary DC — AD DS, DHCP, DNS)         IP: 10.80.64.79
├── DC2  (Secondary DC — Global Catalog)
├── DC3  (RODC — Read-Only Domain Controller)
├── Alex.ITI.LOCAL       (Child Domain — Alexandria Branch)
│   └── DC4              IP: 10.80.64.142
└── Ismaliya.ITI.LOCAL   (Child Domain — Ismailia Branch)
    └── Isamaliya  (DC + DHCP + DNS + WDS)        IP: 10.80.64.187
```

---

## ✅ What We Built

| # | Feature | Details |
|---|---------|---------|
| 1 | **AD Forest** | ITI.LOCAL root + 2 child domains (Alex & Ismaliya) |
| 2 | **Domain Controllers** | DC1 (PDC), DC2 (GC), DC3 (RODC) |
| 3 | **Organizational Units** | HR, IT, Finance, Sales, users-ftp |
| 4 | **Bulk User Creation** | PowerShell CSV script — 30+ users across all OUs |
| 5 | **DHCP** | Scopes on DC1 & Ismaliya server with PXE (060) option |
| 6 | **Group Policy (GPO)** | USB block · Control Panel disable · Forced wallpaper |
| 7 | **IIS + FTP** | web1.com · web2.com · FTP site hosted on DC5 |
| 8 | **WDS** | Network OS deployment via PXE boot |
| 9 | **RDP** | Remote management across all domain machines |

---

## 🛠️ Technologies Used

![Windows Server](https://img.shields.io/badge/Windows_Server_2022-0078D4?style=flat-square&logo=windows&logoColor=white)
![VMware](https://img.shields.io/badge/VMware_Workstation-607078?style=flat-square&logo=vmware&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active_Directory-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![IIS](https://img.shields.io/badge/IIS-5C2D91?style=flat-square&logo=microsoft&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![DNS](https://img.shields.io/badge/DNS_Server-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![DHCP](https://img.shields.io/badge/DHCP_Server-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![GPO](https://img.shields.io/badge/Group_Policy-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![WDS](https://img.shields.io/badge/WDS-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![RDP](https://img.shields.io/badge/Remote_Desktop-0078D4?style=flat-square&logo=microsoft&logoColor=white)


---


<div align="center">

Made with 💙 by the MCSA Team — **ITI, Intake 46**

</div>
