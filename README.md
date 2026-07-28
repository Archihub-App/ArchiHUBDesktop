# ArchiHUB Desktop

A desktop AI agent for organizing, cataloging, and processing local files. It combines a file explorer with a chat-driven agent that can read/summarize documents, transcribe audio, OCR PDFs, and push resources into an [ArchiHUB](https://archihub-app.github.io/archihub.github.io/) instance.

**This repository contains only packaged installers, published automatically as GitHub Releases.** No source code is published here — ArchiHUB Desktop's source is maintained in a private repository.

## Installation

Grab the installer for your platform from the [Releases page](https://github.com/Archihub-App/ArchiHUBDesktop/releases/latest).

### Windows

1. Download `ArchiHUB_<version>_x64-setup.exe` (or the `.msi`).
2. Run it. The installer isn't code-signed yet, so SmartScreen will likely show a "Windows protected your PC" warning — click **More info**, then **Run anyway** to continue.
3. Follow the installer prompts.

### macOS

1. Download `ArchiHUB_<version>_universal.dmg` (one file, works on both Intel and Apple Silicon).
2. Open the `.dmg` and drag the app into `/Applications`.
3. The app isn't notarized yet, so Gatekeeper blocks it on first launch ("can't be opened" / "unidentified developer"). Clear the quarantine flag and open it once from Terminal:
   ```bash
   xattr -cr /Applications/Acquiloom.app
   open /Applications/Acquiloom.app
   ```
4. After that first launch, it opens normally from Launchpad/Finder like any other app.

### Linux

- **Debian/Ubuntu** (`.deb`): `sudo dpkg -i ArchiHUB_<version>_amd64.deb`
- **Fedora/RHEL** (`.rpm`): `sudo rpm -i ArchiHUB-<version>-1.x86_64.rpm`
- **Portable** (`.AppImage`): `chmod +x ArchiHUB_<version>_amd64.AppImage && ./ArchiHUB_<version>_amd64.AppImage`

## First launch

On first launch you'll be asked to configure an AI provider (and, optionally, connection details for an ArchiHUB backend instance) — this is a one-time setup step.

## Issues

Found a bug or have a feature request? [Open an issue](https://github.com/Archihub-App/ArchiHUBDesktop/issues) on this repo.
