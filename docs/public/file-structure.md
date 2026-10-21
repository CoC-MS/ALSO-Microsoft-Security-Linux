# 📂 File structure

[Public documentation](README.md)

This repository contains Linux Server and Desktop policy exports. Policy files are grouped by workload under the `ALSO_LINUX_SERVER` package folder.

## 📦 Available package

| Package | Workloads | Scope |
| --- | --- | --- |
| [`ALSO_LINUX_SERVER`](../../ALSO_LINUX_SERVER) | `SettingsCatalog` | Linux Server and Desktop policies |

The repository currently includes one Settings Catalog policy export:

[`ALSO – MI – MDBS – Basic – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json`](<../../ALSO_LINUX_SERVER/SettingsCatalog/ALSO – MI – MDBS – Basic – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json>)

## 🗂️ Package contents

```text
ALSO_LINUX_SERVER/
└── SettingsCatalog/
    └── ALSO – MI – MDBS – Basic – v1.0 - Linux Server - Defender Antivirus - AV Configuration - D.json
```

`SettingsCatalog` contains the Intune Settings Catalog policy export. The filename identifies its license tag (`MDBS`), baseline tier (`Basic`), version (`v1.0`), platform (`Linux Server`), workload (`Defender Antivirus`), configuration (`AV Configuration`), and assignment scope (`D`, device). See [Policy naming](policy-naming.md) for the naming convention.

The JSON file is the policy export to review and import; it is not a package manifest or overview document. Check [Policy and configuration descriptions](policy-collections.md), [prerequisites](general-prerequisites.md), and [How to import](how-to-import.md) before deployment. Assign reviewed policies to a pilot group and validate their impact before expanding deployment.
