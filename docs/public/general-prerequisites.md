# General prerequisites

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
