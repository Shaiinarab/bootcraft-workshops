<div align="center">

# BOOTCRAFT
### Understand the Boot. Own the System.

**از فشردن Power تا کنترل کامل سیستم**

A student-led, hands-on workshop series for understanding firmware, disks, operating-system installation, bootloaders, and recovery.

[🌐 GitHub Pages website](https://shaiinarab.github.io/bootcraft-workshops/) · [Vercel preview](https://bootcraft-workshops.vercel.app/) · [🧭 Learning path](docs/PROGRAM.md) · [🛡️ Lab safety](docs/LAB-SAFETY.md) · [📚 References](docs/REFERENCES.md)

![GitHub Pages](https://img.shields.io/badge/site-GitHub%20Pages-c7f36b?labelColor=101820&style=flat-square)
![Status](https://img.shields.io/badge/status-foundation%20in%20progress-ff8059?labelColor=101820&style=flat-square)
![Languages](https://img.shields.io/badge/language-Persian%20%2B%20English-7b9cff?labelColor=101820&style=flat-square)

</div>

---

## The idea

Installing an operating system should not feel like following a mysterious recipe. BOOTCRAFT makes the hidden path visible: power-on, firmware, boot manager, kernel, and userspace. Participants learn how storage is laid out, how Windows and Linux start, how to install them safely, and how to reason about boot failures.

The format is intentionally modular:

| Session | Focus | Duration |
|---|---|---:|
| **01 — Under the System's Skin** | Firmware, UEFI/BIOS, GPT/MBR, partitions, filesystems, boot media | 3.5 h |
| **02 — Install, Boot, Choose** | Live media, Windows/Linux installation, boot managers, dual-boot concepts | 4 h |
| **03 — The Rescue Clinic** *(advanced)* | WinRE, GRUB recovery, diagnostics, backup and restore scenarios | 3 h |

The first two are the core pathway. The third is an optional advanced clinic, not a prerequisite for the main series.

## Learning outcomes

By the end of the core pathway, a participant should be able to:

- Explain the major stages between pressing the power button and reaching the desktop.
- Distinguish UEFI from legacy BIOS and GPT from MBR.
- Identify the role of an EFI System Partition and common Windows/Linux partitions.
- Explain the purpose of common filesystems such as NTFS, FAT32, and ext4.
- Create and verify bootable installation media from a trusted image.
- Navigate a Linux live environment and identify storage devices without modifying them.
- Describe the Windows Boot Manager and GRUB roles in a boot flow.
- Complete a supervised installation on a university-owned lab device or disposable virtual disk.
- Choose a sensible first diagnostic step when a machine does not boot.

## Safety is not optional

**No installation, formatting, partition deletion, firmware reset, or bootloader modification is performed on a participant's personal device.** Hands-on work uses university-owned machines, dedicated lab SSDs, or disposable virtual machines. Device ownership, backups, encryption recovery keys, target-disk identity, and a rollback plan must be confirmed before any write operation.

Read the [full lab safety policy](docs/LAB-SAFETY.md) before preparing a session.

## Repository map

```text
.
├── index.html
├── docs/
│   ├── PROGRAM.md
│   ├── LAB-SAFETY.md
│   ├── ORGANIZER-PROPOSAL.md
│   └── REFERENCES.md
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── workflows/
│       └── pages.yml
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
└── LICENSE
```

The website is a lightweight, dependency-free static page. The learning materials are maintained as Markdown so instructors can review, fork, translate, and print them easily.

## Run locally

No package manager or build step is required.

```bash
git clone https://github.com/Shaiinarab/bootcraft-workshops.git
cd bootcraft-workshops
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## GitHub Pages

The repository includes a GitHub Actions workflow at `.github/workflows/pages.yml`. In the repository's **Settings → Pages → Build and deployment**, select **GitHub Actions** as the source once. Every push to `main` then publishes the static site automatically.

GitHub Pages URL: https://shaiinarab.github.io/bootcraft-workshops/\n\nThe workflow uses `actions/configure-pages` with `enablement: true` and attempts to enable GitHub Pages automatically. If the first run cannot enable the site, open **Settings → Pages → Build and deployment → Source → GitHub Actions** once, then rerun the workflow. The Vercel preview remains available as a fallback while Pages is being configured.

## Project status

This repository is the independent home of BOOTCRAFT. It is not a continuation or dependency of `workshop-zero`. The current website and planning documents are a first public foundation, not a claim that a university event has been approved or scheduled.

Before announcing dates, organizers still need to confirm the host institution, room, lab devices, instructor team, supported OS images, and equipment recovery process.

## Contributing

Corrections to technical content, Persian editing, translated material, lab scenarios, accessibility improvements, and instructor notes are welcome. Start with [CONTRIBUTING.md](CONTRIBUTING.md) and cite authoritative sources for technical claims.

---

<div align="center">

**BOOTCRAFT / Learn the chain. Control the system.**

</div>
