# 🛡️ ALSO Microsoft Security Linux Server and Desktop Policy Templates
> A collection of Microsoft Security Linux Server and Desktop policies to help organizations accelerate secure deployments to servers with Defender for Endpoint, Defender for Servers (Defender for Cloud), Defender Business for Servers and Endpoint for Servers with Intune. 

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

---

<a id="getting-started"></a>
## 🚀 Getting started

1. ✅ Review [General prerequisites for Desktop og Server versions](docs/public/general-prerequisites.md) and [Linux requirements for Desktop and Servers](docs/public/linux-prerequisites.md).
2. 📂 [Download the repository ZIP](https://github.com/CoC-MS/ALSO-Microsoft-Security-Linux/archive/refs/heads/main.zip) and extract it.
3. 📥 [How to import](docs/public/how-to-import.md).
4. 🚀 Pilot reviewed policies, check policy deployment reports and user impact, then expand in stages.

For controlled rollouts, we recommend using Microsoft's [deployment plans](https://learn.microsoft.com/en-us/intune/device-management/deployments/overview). This Intune feature is currently in public preview.

**Issues?** [Open an issue](https://github.com/CoC-MS/ALSO-Microsoft-Security-Linux/issues).

> [!WARNING]
> All issues are public; do not include sensitive information.

### Quick navigation

| Section | What you will find |
| --- | --- |
| [Getting started](#getting-started) | Prerequisites, download, import, and staged rollout. |
| [Linux Server and Desktop licensing guide](#linux-server-and-desktop-licensing-guide) | License compatibility and limitations. |
| [Documentation](#documentation) | Links to supporting guides and the repository license. |

---

<a id="linux-server-and-desktop-licensing-guide"></a>
## Linux Server and Desktop licensing guide

### Works with following licenses for Servers 

| Tag | Minimum Required License |
| --- | --- |
| **MDBS** | Microsoft 365 Business Premium + Defender for Business for Servers -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3, F3 or Microsoft 365 E5 and E7 + Defender for Endpoint for Servers - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Any of those above + Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

### Works with following licenses for Desktops

| Tag | Minimum Required License |
| --- | --- |
| **E5** | Microsoft 365 Business Premium + Defender Suite
| **E5** | Microsoft 365 E5 
| **E5** | Microsoft 365 E7
| **E5** | Microsoft 365 E3 + Defender Suite
| **E5** | Microsoft 365 F3/F1 + Defender Suite FLW


<a id="documentation"></a>
## 📚 Documentation

| Documentation | Overview |
| --- | --- |
| 📚 **[Documentation index](docs/public/README.md)** | Browse all deployment documentation. |
| 📖 **[Policy and configuration descriptions](docs/public/policy-collections.md)** | Review the preserved descriptions of every workload collection. |
| 🐧 **[Linux requirements for Desktop and Servers](docs/public/linux-prerequisites.md)** | Device types and OS versions supported |
| 🚀 **[General prerequisites for Desktop og Server versions](docs/public/general-prerequisites.md)** | Review roles, licensing, prepare Intune and Defender. |
| 🧩 **[Dependencies prerequisites](docs/public/dependencies-and-errors.md)** | Review required configuration, assignments, and Linux Server DeviceOSVersion values. |
| 📖 **[Policy naming](docs/public/policy-naming.md)** | Understand licence tags and naming components. |
| 📂 **[File structure](docs/public/file-structure.md)** | Find the package and policy files. |
| 🛡️ **[Security information](SECURITY)** | Read the security and usage information. |
| 📜 **[License](LICENSE)** | Read the repository licence. |
