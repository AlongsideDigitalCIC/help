---
title: Installing Presenter on Linux
description: How to install Presenter on Ubuntu, Debian, Fedora, and other Linux distributions using AppImage, .deb, or .rpm.
---

Presenter provides native Linux builds for **Ubuntu**, **Debian**, **Fedora**, and universal **AppImage** support across Linux distributions.

---

## 1. Choose Your Package

Visit **[alongsidedigital.co.uk/products/presenter/download](https://alongsidedigital.co.uk/products/presenter/download)** and choose the package for your distribution:

### Option A: AppImage (Universal — Works on Most Distros)
1. Click **Download AppImage**.
2. Make the file executable:
   ```bash
   chmod +x presenter_*_amd64.AppImage
   ```
3. Double-click the `.AppImage` file (or run `./presenter_*_amd64.AppImage` in your terminal).

### Option B: Ubuntu / Debian (`.deb`)
1. Click **Download `.deb` (Debian)**.
2. Install via your software centre or terminal:
   ```bash
   sudo apt install ./presenter_*_amd64.deb
   ```

### Option C: Fedora / RHEL (`.rpm`)
1. Click **Download `.rpm` (Fedora)**.
2. Install via your software centre or terminal:
   ```bash
   sudo dnf install ./presenter_*.x86_64.rpm
   ```

---

## Next Step

Once Presenter launches, follow **[Connecting Your Media Folder](/presenter/media-folder-setup)** to choose where your songs and media files are saved.
