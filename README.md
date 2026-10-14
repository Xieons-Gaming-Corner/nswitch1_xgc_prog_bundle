# Xieon's Gaming Corner — Nintendo Switch Program Bundle

[![Discord Widget](https://discord.com/api/guilds/829181609156411463/widget.png?style=banner2)](https://discord.gg/Xieon)

> **XGC Release Bundle**
>
> This repository bundles official releases of Atmosphère, sys-botbase, and TegraRcmGUI for convenience, alongside source code associated with the XGC-maintained Tera Finder mirror release.
>
> Unless explicitly noted otherwise, bundled upstream binaries are unchanged from their respective official releases.

---

## Updated by XGC

This repository is based on the official [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere) project and includes an XGC-maintained program bundle for Nintendo Switch homebrew, custom firmware workflows, and related desktop tools.

### XGC Changes

- Added custom GitHub workflow files under [`.github/`](.github/).
- Bundled official upstream releases of Atmosphère, sys-botbase, and TegraRcmGUI for ease of use.
- Included `fusee.bin` for compatible RCM injection workflows.
- Included the Atmosphère SD-card package for extraction to the root of a compatible SD card.
- Added Tera Finder source code corresponding to the release referenced below, following successful GitHub Actions builds on the XGC mirror fork.
- Included release notes and installation guidance for the bundled files.

> This repository is intended as a convenience bundle and mirror. XGC does not claim original authorship of Atmosphère, sys-botbase, TegraRcmGUI, or Tera Finder. XGC-maintained workflows and other repository changes are identified separately.

### Latest XGC Release

[**XGC Nintendo Switch Program Bundle Releases**](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/releases)

### Related XGC Releases

- [Atmosphère 1.12.0 historical mirror](https://github.com/Xieons-Gaming-Corner/ATMOSPHERE_1.12.0/releases)
- [Tera Finder — `10_14_2026_mirror`](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror)

---

## XGC Nintendo Switch Program Bundle

This bundle brings together Switch-side software, desktop utilities, and release-associated source code.

| Project | Bundled version / reference | Role | Source |
|---|---|---|---|
| Atmosphère | 1.12.0 | Nintendo Switch custom firmware | [Official release](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/1.12.0) |
| sys-botbase | 2.5 | Switch-side communication module | [Official release](https://github.com/olliz0r/sys-botbase/releases/tag/v2.5) |
| TegraRcmGUI | Latest bundled release | Windows RCM payload injection utility | [Official releases](https://github.com/eliboa/TegraRcmGUI/releases) |
| Tera Finder | `10_14_2026_mirror` | Desktop application; release-associated source code included | [XGC mirror release](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror) |

> **Switch software and desktop tools are different.**
>
> Atmosphère and sys-botbase include files intended for the Switch SD card. TegraRcmGUI runs on Windows. Tera Finder runs on your computer and communicates wirelessly with your Switch—it is not a program installed or launched on the Switch itself.

---

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
- [TegraRcmGUI website](https://tegrarcmgui.com/)

<img width="595" height="248" alt="TegraRcmGUI" src="https://github.com/user-attachments/assets/4dffdb67-e045-4af8-a7ea-ce33725698b5" />

### Tera Finder — XGC Mirror

Release reference: [Tera Finder — `10_14_2026_mirror`](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror)

GitHub Actions builds are now working on XGC’s Tera Finder mirror fork. We have therefore incorporated Tera Finder into the Nintendo Switch Program Bundle.

> **Tera Finder is a desktop application—not Switch-side software.**
>
> It is intended to run on your computer and communicate wirelessly with your Nintendo Switch. Do not treat its files as an SD-card installation package.

The Tera Finder files included in this bundle are the source code corresponding to the build on which the linked release is based.

| Included content | Purpose |
|---|---|
| Release-associated Tera Finder source code | Provides the source corresponding to the referenced XGC mirror build |
| XGC mirror release link | Identifies the release associated with the bundled source |

For release details and available downloads, visit the [XGC Tera Finder mirror release](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror).

---

## Installation Overview

### Switch-Side Files

1. Download the appropriate XGC release bundle.
2. Extract the Atmosphère package to the root of a compatible Switch SD card.
3. Extract `sys-botbase25.zip` to the root of the same SD card if sys-botbase is required.
4. Place the SD card in the console.
5. Use a compatible RCM injection workflow with `fusee.bin`, such as TegraRcmGUI.
6. Follow the documentation from the original projects for version compatibility, updates, and troubleshooting.

> **Important:** Confirm that your console firmware, Atmosphère version, payload, and installed modules are compatible before updating or booting.

### Desktop Tools

- **TegraRcmGUI:** Use the portable package or Windows installer on your computer for compatible RCM payload injection workflows.
- **Tera Finder:** Runs on your computer and communicates wirelessly with your Switch. Refer to the linked XGC mirror release and project documentation for build, setup, and connection instructions.

> The bundled Tera Finder source code is separate from the Switch SD-card packages. Source code is not a ready-to-run application.

---

## Upstream Binaries & Mirror Source

The following upstream projects are bundled for convenience:

- [Atmosphère 1.12.0](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/1.12.0)
- [sys-botbase v2.5](https://github.com/olliz0r/sys-botbase/releases/tag/v2.5)
- [TegraRcmGUI releases](https://github.com/eliboa/TegraRcmGUI/releases)

The bundle also includes release-associated source code from:

- [Tera Finder — XGC mirror release `10_14_2026_mirror`](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror)

> Bundled official binaries are intended to remain identical to their upstream releases. Tera Finder is identified separately as source code associated with an XGC mirror release.
>
> This bundle does not replace the projects’ documentation, support channels, source repositories, or release notes.

---

## Release Notes

### What's Changed

- Added bundled release files by [@Xieon](https://github.com/Xieon) in [Xieons-Gaming-Corner/switch_program_bundle#1](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/pull/1).
- Incorporated Tera Finder following successful GitHub Actions builds on the XGC mirror fork.
- Included Tera Finder source code associated with [`10_14_2026_mirror`](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror).
- Clarified the distinction between Switch-side packages, desktop tools, and source code.

### New Contributors

- [@Xieon](https://github.com/Xieon) made their first contribution in [Xieons-Gaming-Corner/switch_program_bundle#1](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/pull/1).

### Changelog & Release References

- [Bundle changelog for `v_10_13_2026`](https://github.com/Xieons-Gaming-Corner/switch_program_bundle/commits/v_10_13_2026)
- [Tera Finder mirror release `10_14_2026_mirror`](https://github.com/Xieons-Gaming-Corner/Tera-Finder/releases/tag/10_14_2026_mirror)

---

## Special Thanks

XGC thanks [@Manu098VM](https://github.com/Manu098vm) for assistance resolving an issue that prevented this version from working correctly.

<img width="616" height="168" alt="Special thanks acknowledgement" src="https://github.com/user-attachments/assets/502b8dd4-9db6-4a26-b550-a5799e1b8174" />

---

## Disclaimer

Nintendo Switch, Nintendo, and related names are trademarks of Nintendo. This repository is not affiliated with, endorsed by, or sponsored by Nintendo.

Use unofficial software only where lawful and at your own risk. Always preserve backups of important data and follow the documentation for each project.

---

## Licensing

Each bundled project remains subject to its own license and any applicable redistribution requirements. Refer to the license files and notices accompanying each project.

Atmosphère is licensed under the terms of the GPLv2, subject to project-specific exemptions.

A copy of its license is available in the [Atmosphère LICENSE](https://github.com/Atmosphere-NX/Atmosphere/blob/master/LICENSE) file.

For Tera Finder, consult the license and notices included with the source code associated with the referenced XGC mirror release.
