# Policy and configuration descriptions

[Public documentation](README.md)

This page summarizes the policy exports currently included in the repository. Use it to understand each policy's workload and configured settings before importing; the linked JSON is the authoritative export.

## Available policies

| Policy | Workload | Platform and scope | Tier and version |
| --- | --- | --- | --- |
| [Defender Antivirus - AV Configuration (Advanced)](<../../ALSO_LINUX_SERVER/SettingsCatalog/ALSO – HI – MDBS – Advanced – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json>) | Microsoft Defender Antivirus | Linux Server; device policy (`D`) | Advanced; v1.0 |
| [Defender Antivirus - AV Configuration (Basic)](<../../ALSO_LINUX_SERVER/SettingsCatalog/ALSO – MI – MDBS – Basic – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json>) | Microsoft Defender Antivirus | Linux Server; device policy (`D`) | Basic; v1.0 |
| [Endpoint Security - AV Configuration](<../../ALSO_LINUX_DESKTOP/SettingsCatalog/ALSO- HI- E5- Basic- v.1.0- Linux Desktop- Endpoint Security - AV- AV Configuration - D.json>) | Endpoint Security antivirus | Linux Desktop; device policy (`D`) | Basic; v1.0 |
| [Compliance - Device encryption](<../../ALSO_LINUX_DESKTOP/CompliancePoliciesV2/ALSO- HI- E5- HI- Basic- v.1.0- Linux Desktop- Compliance- Device encryption - U.json>) | Device compliance | Linux Desktop; user policy (`U`) | Basic; v1.0 |
| [Compliance - Password Encryption](<../../ALSO_LINUX_DESKTOP/CompliancePoliciesV2/ALSO- HI- E5- HI- Basic- v.1.0- Linux Desktop- Compliance- Password Encryption - U.json>) | Device compliance | Linux Desktop; user policy (`U`) | Basic; v1.0 |

The current collection contains five Intune policy exports across Linux Server and Linux Desktop. The filename tags identify impact and minimum-license categories; see [Policy naming](policy-naming.md) and verify licensing against your tenant's current Microsoft entitlements.

## Linux Server Defender Antivirus - AV Configuration

The Basic and Advanced policies configure antivirus, cloud protection, and network protection options for Linux servers managed through Microsoft Intune and Microsoft Defender for Endpoint. Review each export independently because its configured values may differ.

| Area | Configuration in the export |
| --- | --- |
| Cloud protection | Enabled; cloud block level set to **High** |
| Security intelligence | Automatic definition updates enabled |
| Antivirus engine | Enforcement level `0`; behavior monitoring enabled |
| Scanning | Archive scanning and scanning after a definition update enabled |
| File and memory analysis | File hash computation enabled; memory scanning enabled |
| Network protection | Enforcement level `2` |

The numeric enforcement-level values are reproduced from the export. Review their current meaning and impact in Intune and Microsoft Defender documentation before deployment; do not assume these values are equivalent to another platform's settings.

### Before deployment

- Confirm the [Linux and Defender prerequisites](general-prerequisites.md) and supported [Linux versions](linux-prerequisites.md).
- Check the [policy naming](policy-naming.md) guide and validate the required license for your tenant.
- Review the policy's settings and any assignments in the export. Import without assignments, then choose an appropriate device group in your tenant.
- Pilot the policy on representative devices, check reporting and Defender health, and evaluate performance or application impact before expanding deployment.

See [How to import](how-to-import.md) for the import workflow and [File structure](file-structure.md) for the package location.
