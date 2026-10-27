# 📂 File structure

[Public documentation](README.md)

This repository contains Linux Server and Desktop policy exports. Policy files are grouped by device type and workload under the `ALSO_LINUX_SERVER` and `ALSO_LINUX_DESKTOP` package folders.

## 📦 Available packages

| Package | Workloads | Scope |
| --- | --- | --- |
| [`ALSO_LINUX_SERVER`](../../ALSO_LINUX_SERVER) | `SettingsCatalog` | Linux Server policies |
| [`ALSO_LINUX_DESKTOP`](../../ALSO_LINUX_DESKTOP) | `SettingsCatalog`, `CompliancePoliciesV2` | Linux Desktop policies |

The repository currently includes four policy exports: one Linux Server Settings Catalog policy, one Linux Desktop Settings Catalog policy, and two Linux Desktop compliance policies.

## 🗂️ Package contents

```text
ALSO_LINUX_SERVER/
└── SettingsCatalog/
    └── ALSO – HI – MDBS – Advanced – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json

ALSO_LINUX_DESKTOP/
├── CompliancePoliciesV2/
│   ├── ALSO- HI- E5- HI- Basic- v.1.0- Linux Desktop- Compliance- Device encryption - U.json
│   └── ALSO- HI- E5- HI- Basic- v.1.0- Linux Desktop- Compliance- Password Encryption - U.json
└── SettingsCatalog/
    └── ALSO- HI- E5- Basic- v.1.0- Linux Desktop- Endpoint Security - AV- AV Configuration - D.json
```

`SettingsCatalog` contains Intune Settings Catalog policy exports, while `CompliancePoliciesV2` contains Intune device compliance policy exports. The filenames identify license, baseline, version, platform, workload, configuration, and assignment scope. See [Policy naming](policy-naming.md) for the naming convention.

Each JSON file is a policy export to review and import; it is not a package manifest or overview document. Check [Policy and configuration descriptions](policy-collections.md), [prerequisites](general-prerequisites.md), and [How to import](how-to-import.md) before deployment. Assign reviewed policies to a pilot group and validate their impact before expanding deployment.
