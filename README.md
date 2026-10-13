# Xieon's Gaming Corner — Nintendo Switch Program Bundle
[![Discord Widget](https://discord.com/api/guilds/829181609156411463/widget.png?style=banner2)](https://discord.gg/Xieon)


> **XGC Release Bundle**
>
> This repository bundles official releases of Atmosphère, sys-botbase, and TegraRcmGUI for convenience. Unless explicitly noted otherwise, bundled binaries are unchanged from their respective official upstream releases.

---

## Updated by XGC

This repository is based on the official [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere) project and includes an XGC-maintained program bundle for Nintendo Switch homebrew and custom firmware workflows.

### XGC Changes

- Added custom GitHub workflow files under [`.github/`](.github/).
- Bundled official upstream releases of Atmosphère, sys-botbase, and TegraRcmGUI for ease of use.
- Included `fusee.bin` for compatible RCM injection workflows.
- Included the Atmosphère SD-card package for extraction to the root of a compatible SD card.
- Included release notes and installation guidance for the bundled files.

> This repository is intended as a convenience bundle and mirror. XGC does not claim authorship of Atmosphère, sys-botbase, TegraRcmGUI, or their included binaries.

### Latest XGC Release

The latest release is available here:

[**XGC Nintendo Switch Program Bundle Releases**](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/releases)

The historical Atmosphère mirror release is available here:

[**Atmosphère 1.12.0 **](https://github.com/Xieons-Gaming-Corner/ATMOSPHERE_1.12.0/releases)

---

## XGC Nintendo Switch Program Bundle

This bundle combines releases from the following upstream projects:

| Project | Bundled version | Official source |
|---|---:|---|
| Atmosphère | 1.12.0 | [Atmosphère 1.12.0 release](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/1.12.0) |
| sys-botbase | 2.5 | [sys-botbase v2.5 release](https://github.com/olliz0r/sys-botbase/releases/tag/v2.5) |
| TegraRcmGUI | Latest bundled release | [TegraRcmGUI releases](https://github.com/eliboa/TegraRcmGUI/releases) |

## Included Files

### Atmosphère 1.12.0

Source: [Official Atmosphère 1.12.0 release](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/1.12.0)

| File | Purpose | Installation |
|---|---|---|
| `fusee.bin` | Atmosphère payload for compatible RCM injection workflows | Select this file in TegraRcmGUI before injecting |
| `atmosphere-1.12.0-master-28d6a2e11+hbl-2.4.5+hbmenu-3.6.1.zip` | Atmosphère SD-card package | Extract its contents to the root of the SD card |

### sys-botbase v2.5

Source: [Official sys-botbase v2.5 release](https://github.com/olliz0r/sys-botbase/releases/tag/v2.5)

| File | Purpose | Installation |
|---|---|---|
| `sys-botbase25.zip` | Recommended full sys-botbase SD-card package | Extract its contents to the root of the Switch SD card |
| `sys-botbase.nsp` | sys-botbase module binary | Rename and place it at `sd:/atmosphere/contents/430000000000000B/exefs.nsp` |

> **Recommended:** Extract `sys-botbase25.zip` to the root of the SD card rather than manually placing the `.nsp` file.

The included `sys-botbase.nsp` and `sys-botbase25.zip` are identical to the binaries published in the official sys-botbase release linked above.

### TegraRcmGUI

Source: [Official TegraRcmGUI releases](https://github.com/eliboa/TegraRcmGUI/releases)

| File type | Purpose |
|---|---|
| Portable ZIP release | Run TegraRcmGUI without a traditional installer |
| MSI installer | Install TegraRcmGUI on Windows |

The TegraRcmGUI files included in this bundle are identical to the binaries available from the official project releases.

- [Official TegraRcmGUI GitHub releases](https://github.com/eliboa/TegraRcmGUI/releases)
- [Official TegraRcmGUI website](https://tegrarcmgui.com/)

<img width="595" height="248" alt="TegraRcmGUI" src="https://github.com/user-attachments/assets/4dffdb67-e045-4af8-a7ea-ce33725698b5" />

---

## Installation Overview

1. Download the appropriate XGC release bundle.
2. Extract the Atmosphère package to the root of a compatible Switch SD card.
3. Extract `sys-botbase25.zip` to the root of the same SD card if sys-botbase is required.
4. Place the SD card in the console.
5. Use a compatible RCM injection workflow with `fusee.bin`, such as TegraRcmGUI.
6. Follow the documentation from the original projects for version compatibility, updates, and troubleshooting.

> **Important:** Confirm that your console firmware, Atmosphère version, payload, and installed modules are compatible before updating or booting.

---

## Bundled Binaries

The following projects are bundled strictly for convenience:

- [sys-botbase](https://github.com/olliz0r/sys-botbase/releases/tag/v2.5)
- [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/1.12.0)
- [TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI/releases/tag/2.6)
- [Official TegraRcmGUI website](https://tegrarcmgui.com/)

> The bundled releases are intended to remain identical to their official upstream binaries. The XGC bundle does not replace the official documentation, support channels, source repositories, or release notes.

---

## Release Notes

### What's Changed

- Added bundled release files by [@Xieon](https://github.com/Xieon) in [Xieons-Gaming-Corner/switch_program_bundle#1](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/pull/1).

### New Contributors

- [@Xieon](https://github.com/Xieon) made their first contribution in [Xieons-Gaming-Corner/switch_program_bundle#1](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/pull/1).

### Full Changelog

[View the full changelog for `v_10_13_2026`](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/commits/v_10_13_2026)

---

## Special Thanks

XGC thanks [@Manu098VM](https://github.com/Manu098vm) for assistance resolving an issue that prevented this version from working correctly.

<img width="616" height="168" alt="Special thanks acknowledgement" src="https://github.com/user-attachments/assets/502b8dd4-9db6-4a26-b550-a5799e1b8174" />

---


## Disclaimer

Nintendo Switch, Nintendo, and related names are trademarks of Nintendo. This repository is not affiliated with, endorsed by, or sponsored by Nintendo.

Use unofficial software only where lawful and at your own risk. Always preserve backups of important data and follow the official documentation for each upstream project.

## Licensing

Atmosphère is licensed under the terms of the GPLv2, subject to project-specific exemptions.

A copy of the license is available in the [LICENSE](https://github.com/Atmosphere-NX/Atmosphere/blob/master/LICENSE) file.
