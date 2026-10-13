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
