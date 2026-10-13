# 🛡️ ALSO Microsoft Security Linux Server and Desktop Policy Templates
> A collection of Microsoft Security Linux Server and Desktop policies to help organizations accelerate secure deployments to servers with Defender for Endpoint, Defender for Servers (Defender for Cloud), Defender Business for Servers and Endpoint for Servers with Intune. 

**Works with Microsoft 365 Business Premium + Defender Suite and Microsoft 365 Business Premium + Defender Business for Servers and up**

---

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

## ✅ Supported Linux Server and Desktop Operating Systems

| Operating System | x64 (AMD64/EM64T) | ARM64 |
|-----------------|-------------------|--------|
| Red Hat Enterprise Linux | 7.2+, 8.x, 9.x, 10.x | 8.x, 9.x, 10.x |
| CentOS | 7.2+, 8.x | Not Supported |
| CentOS Stream | 8.x, 9.x, 10.x | 8.x, 9.x, 10.x |
| Ubuntu LTS | 16.04, 18.04, 20.04, 22.04, 24.04, 26.04 | 20.04, 22.04, 24.04, 26.04 |
| Ubuntu Pro | 22.04, 24.04 | 22.04, 24.04 |
| Debian | 9-13 | 11, 12, 13 |
| SUSE Linux Enterprise Server | 12.x, 15.x, 16.x | 15 (SP5, SP6), 16.x |
| openSUSE Leap | 15.6, 16.x | 15.6, 16.x |
| Oracle Linux | 7.2+, 8.x, 9.x, 10.x | 8.x, 9.x, 10.x |
| Amazon Linux | 2, 2023 | 2, 2023 |
| Fedora | 33-44 | 40-44 |
| Rocky Linux | 8.7+, 9.2+, 10.x | 8.7+, 9.2+, 10.x |
| Alma Linux | 8.4+, 9.2+, 10.x | 8.4+, 9.2+, 10.x |
| Mariner | 2 | 2 |

Source: Microsoft Learn: https://learn.microsoft.com/nb-no/defender-endpoint/mde-linux-prerequisites#supported-linux-distributions

> [!IMPORTANT]
> **⚠️ IMPORTANT: Always double check up to date information provided in source.**

### Works with following licenses for Servers 

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Defender for Business for Servers -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 + Defender for Endpoint for Servers - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

### Works with following licenses for Desktops

| Tag | Minimum Required License |
|:---:|--------------------------|
| **E5** | Microsoft 365 Business Premium + Defender Suite, Microsoft 365 E5 or Microsoft 365 E7


---

| Resource | Description |
|-----------|-------------|
| 🛡️ **[Security Information](SECURITY)** | [View Security Policy](SECURITY) |
| 📖 **[Supported Linux Server and Desktop OS](#-supported-linux-server-and-desktop-operating-systems)** | [View description](#-supported-linux-server-and-desktop-operating-systems) |
| 📖 **[Supported licenses](#works-with-following-licenses-for-servers)** | [View description](#works-with-following-licenses-for-servers) |
| 📖 **[Before importing ALSO_LINUX_SERVER_POLICIES](ALSO_LINUX_SERVER)** | [View description](#before-importing-also_linux_server_policies) |
| 📖 **[Before importing ALSO_LINUX_DESKTOP_POLICIES](#before-importing-also_linux_desktop_policies)** | [View description](#before-importing-also_linux_desktop_policies) |

---

## Before importing ALSO_LINUX_SERVER_POLICIES

## Prerequisites

Before importing **ALSO_LINUX_SERVER_POLICIES**, ensure the following prerequisites are met:

| Requirement | Details |
|------------|---------|
| Licensing | Microsoft Defender for Business (MDB), Microsoft Defender for Endpoint Server (MDES), or Defender for Servers (DfS) licensing is required. |
| Operating System | Verify that your servers meet the minimum supported operating system requirements listed above. |
| Intune | Microsoft Intune must be deployed and actively used for device management. |
| Defender Services | Microsoft Defender for Endpoint and/or Microsoft Defender for Cloud must be enabled and configured in your tenant or subscriptions and all servers needs to be onboarded to Defender with status Onboarded and Active. |
| Permissions | You must have the **Security Administrator** and **Intune Administrator**  roles assigned. |



1. Navigate to: security.microsoft.com -> Settings -> Endpoints -> Enforcement scope and toggle ON this settings. Toggle on Defender for Cloud if you are using Defender for Cloud (Linux servers in Azure or Arc onboarded Linux servers)

<img width="1687" height="1227" alt="image" src="https://github.com/user-attachments/assets/7effdd5d-9d55-46fa-bf2e-3ad2998faca5" />


2. Navigate to intune.microsoft.com -> Endpoint security > Microsoft Defender for Endpoint, and set Allow Microsoft Defender for Endpoint to enforce Endpoint Security Configurations to On.

<img width="1420" height="862" alt="image" src="https://github.com/user-attachments/assets/88068da1-754f-43d5-85ae-368c5e63b66b" />

> [!IMPORTANT]
> **⚠️IMPORTANT: Always double check official documentation here:** 

> **Source:** Microsoft Learn  
> Full documentation is available here:  
> [Microsoft Defender Security Settings Management Documentation](https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management)

## Create dynamic security group in Entra for assignments

1. Create dynamic security group to catch your Linux devices

<img width="2054" height="720" alt="image" src="https://github.com/user-attachments/assets/8ff387df-e28c-4040-8070-28981390030c" />



## Before importing ALSO_LINUX_DESKTOP_POLICIES

## Prerequisites

Before importing **ALSO_LINUX_SERVER_POLICIES**, ensure the following prerequisites are met:

| Requirement | Details |
|------------|---------|
| Licensing | Microsoft 365 Business Premium+ Defender Suite, Microsoft 365 E5 or Microsoft 365 E7|
| Operating System | Verify that your servers meet the minimum supported operating system requirements listed above. |
| Intune | Microsoft Intune must be deployed and actively used for device management. |
| Defender Services | Microsoft Defender for Business/ Endpoint must be enabled and your Linux desktop devices are enrolled into Intune. |
| Permissions | You must have the **Security Administrator** and **Intune Administrator**  roles assigned. |


---

## 📖 Naming Convention

All policy templates follow the naming format below:

```text
<ALSO>-<ImpactLevel>-<MinimumLicense>-<BaselineLevel>-<Version>-<OS>-<Main Category>-<Sub Category>-<Settings>-<Assignment>
```

### Example

```text
ALSO – LI – MDBS – Basic – v1.0– Linux – Endpoint Security - Antivirus - AV Configuration - D
```

---

## 🧩 Naming Components

| Component | Description |
|-----------|-------------|
| **ALSO** | Company providing the policy template to have a better control |
| **Impact** | Impact level of policy, low (LI), medium (MI) or high (HI) |
| **MinimumLicense** | Minimum Microsoft license required to use the policy |
| **BaselineLevel** | Baseline level of policy, Basic, Advanced |
| **Version** | Policy version, v1.0, v1.1 etc|
| **LinuxDesktop or LinuxServer** | Operating system |
| **MainCategory** | Name of main category, Device Configuration, Device Compliance etc|
| **SubCategory** | Name of sub category, MDE, AV, Disk etc|
| **Settings** | Short settings description |
| **Assignment** | Assignment scope- device (D) or user (U)|


---



## Issues? 

Open issue here: https://github.com/CoC-MS/ALSO-Microsoft-Security-Linux/issues
