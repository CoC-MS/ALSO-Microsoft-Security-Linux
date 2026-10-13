# General prerequisites for Server and Desktop versions

## Before importing ALSO_LINUX_SERVER_POLICIES

## Prerequisites

Before importing **ALSO_LINUX_SERVER_POLICIES**, ensure the following prerequisites are met:


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

1. Ensure that you are using Intune today and that your Linux desktop devices are enrolled to Intune

How to enroll Linux Desktop to Intune 

1. On Linux desktop client, download Company portal app + Edge app

2. Download latest version from these site on Linux Desktop client https://github.com/microsoft/shell-intune-samples/tree/master/Linux/Intune%20Installer and follow instructions in readme.md file

3. Once your Linux have been enrolled to Intune, onboard it to Defender by using this guide from Learn https://learn.microsoft.com/en-us/defender-endpoint/linux-install-with-defender-deployment-tool#deployment-step-by-step-guide

4. Check results in Defender portal

5. Once Linux Desktop client are onboarded to Defender and onbaording and health state er ok, you can assign AV and compliance policies to your Linux desktop device group or All devices. 

PS: Per today there are no automated way to onboard all Linux desktop devices to Defender via Intune like Linux Server, MacOS and mobile devices, so manual approach is the only working solution.
   
