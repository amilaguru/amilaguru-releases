# amilaguru-releases
Public releases for AMILAGuru : Linux and Windows desktop companion app downloads.

# AMILAGuru — Desktop Builds (Windows & Linux)

A/L Chemistry Mastery, on your laptop or desktop. This release adds native builds for Windows and Linux alongside the existing Android app.

## What's included

| Platform | File | Notes |
|---|---|---|
| Windows | `AMILAGuru-Setup-x64.exe` | Installer, 64-bit, Windows 10/11 |
| Linux | `AMILAGuru-x86_64.AppImage` | Portable, no installation required |

*(Rename the filenames above to match whatever your build script actually outputs before publishing.)*

---

## Installation

### Windows

1. Download `AMILAGuru-Setup-x64.exe` from the **Assets** section below.
2. Run the installer.
   > This build isn't code-signed yet, so Windows SmartScreen will show **"Windows protected your PC."** Click **More info → Run anyway** to continue. This is expected for unsigned installers and not a sign of a problem with the file.
3. Follow the setup wizard. AMILAGuru will be added to your Start Menu and Desktop.

### Linux

1. Download `AMILAGuru-x86_64.AppImage` from the **Assets** section below.
2. Make it executable:
   ```bash
   chmod +x AMILAGuru-x86_64.AppImage
   ```
3. Run it:
   ```bash
   ./AMILAGuru-x86_64.AppImage
   ```
   No installation step is needed — AppImages run directly from wherever you save them.

   *Optional:* to add a desktop shortcut/menu entry, use a tool like [AppImageLauncher](https://github.com/TheAssassin/AppImageLauncher).

---

## System requirements

| Platform | Minimum |
|---|---|
| Windows | Windows 10 (64-bit) or later |
| Linux | x86_64 distribution with glibc 2.31+ (Ubuntu 20.04+, Fedora 33+, Debian 11+, and similar) |

---

## Verifying your download (optional)

If you'd like to confirm the file wasn't corrupted or tampered with in transit, compare its SHA-256 checksum against the value listed here:

```
AMILAGuru-Setup-x64.exe     sha256: sha256:3620f5ad867c35e23fb63ec43e81ef78eeda5365f0530c65520b06684c066dbd
AMILAGuru-x86_64.AppImage   sha256: [paste checksum here]
```

To generate a checksum yourself:
- **Windows (PowerShell):** `Get-FileHash .\AMILAGuru-Setup-x64.exe -Algorithm SHA256`
- **Linux:** `sha256sum AMILAGuru-x86_64.AppImage`

---

## What's new in this release

- [ ] First desktop release — Windows and Linux builds added

---

## Known issues

- Windows builds are currently unsigned — expect a SmartScreen warning on first run (see Installation above)

---

## Feedback & support

Found a bug, or something not working as expected? Reach out at **[support@amila.guru]** or via [amila.guru](https://amila.guru).

---

<sub>AMILAGuru is built and maintained by Amila Senadeera. Android, Windows, and Linux builds share the same account, purchases, and study progress.</sub>
