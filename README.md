# 🛡️ ALSO Microsoft Security Linux Server and Desktop Policy Templates
> A collection of Microsoft Security Linux Server and Desktop policies to help organizations accelerate secure deployments to servers with Defender for Endpoint, Defender for Servers (Defender for Cloud), Defender Business for Servers and Endpoint for Servers with Intune. 

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

# Linux Server and Desktop licensing guide 

### Works with following licenses for Servers 

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Defender for Business for Servers -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3, F3 or Microsoft 365 E5 and E7 + Defender for Endpoint for Servers - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Any of those above + Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

### Works with following licenses for Desktops

| Tag | Minimum Required License |
|:---:|--------------------------|
| **E5** | Microsoft 365 Business Premium + Defender Suite
| **E5** | Microsoft 365 E5 
| **E5** | Microsoft 365 E7
| **E5** | Microsoft 365 F3/F1 + Defender Suite

| Resource | Description |
| --- | --- |
| 📚 **[Documentation index](docs/public/README.md)** | Browse all deployment documentation. |
| 📖 **[Policy and configuration descriptions](docs/public/policy-collections.md)** | Review the preserved descriptions of every workload collection. |
| 🐧 **[Linux requrements for Desktop and Servers](docs/public/linux-prerequisites.md)** | Device types and OS versions supported |
| 🚀 **[General prerequisites for Desktop og Server versions](docs/public/general-prerequisites.md)** | Review roles, licensing, prepare Intune and Defender. |
| 🧩 **[Dependencies prerequisites](docs/public/dependencies-and-errors.md)** | Review required configuration, assignments, and Linux Server DeviceOSVersion values. |
| 📖 **[Policy naming](docs/public/policy-naming.md)** | Understand licence tags and naming components. |
| 📂 **[File structure](docs/public/file-structure.md)** | Find the package and policy files. |
| 📥 **[How to import](docs/public/how-to-import.md)** | Follow the original illustrated import guidance. |
| 🐛 **[Reporting issues](docs/public/reporting-issues.md)** | Open an issue. |
| 🛡️ **[Security information](SECURITY)** | Read the security and usage information. |
| 📜 **[License](LICENSE)** | Read the repository licence. |

----
