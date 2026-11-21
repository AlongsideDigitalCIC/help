---
title: Installing Presenter on Linux
description: Download and install Presenter on Ubuntu, Debian, Fedora, and other Linux distributions using AppImage, .deb, or .rpm.
---

Presenter provides native Linux builds for **Ubuntu**, **Debian**, **Fedora**, and universal **AppImage** support across Linux distributions.

---

## 1. Download Your Linux Package

Choose the package for your Linux distribution below:

<div class="ad-card ad-download-card ad-platform-download">
  <div class="ad-card-header">
    <h3>Linux (64-bit)</h3>
  </div>
  <p class="ad-card-desc">Ubuntu, Debian, Fedora &amp; Universal AppImage</p>
  <div class="ad-download-actions">
    <a href="https://github.com/AlongsideDigitalCIC/presenter/releases/download/presenter-v1.0.6/presenter_1.0.6_amd64.AppImage" data-ext=".AppImage" data-arch="x64" class="ad-btn ad-btn-primary ad-btn-sm">Download AppImage (Universal)</a>
    <a href="https://github.com/AlongsideDigitalCIC/presenter/releases/download/presenter-v1.0.6/presenter_1.0.6_amd64.deb" data-ext=".deb" data-arch="x64" class="ad-btn ad-btn-secondary ad-btn-sm">Download .deb (Debian / Ubuntu)</a>
    <a href="https://github.com/AlongsideDigitalCIC/presenter/releases/download/presenter-v1.0.6/presenter-1.0.6-1.x86_64.rpm" data-ext=".rpm" data-arch="x64" class="ad-btn ad-btn-secondary ad-btn-sm">Download .rpm (Fedora / RHEL)</a>
  </div>
</div>

---

## 2. Install or Run Your Package

### Option A: AppImage (Universal — Works on Most Distros)
1. Make the downloaded `.AppImage` file executable:
   ```bash
   chmod +x presenter_*_amd64.AppImage
   ```
2. Double-click the `.AppImage` file (or run `./presenter_*_amd64.AppImage` in your terminal).

### Option B: Ubuntu / Debian (`.deb`)
Install via your software centre or terminal:
```bash
sudo apt install ./presenter_*_amd64.deb
```

### Option C: Fedora / RHEL (`.rpm`)
Install via your software centre or terminal:
```bash
sudo dnf install ./presenter-*.x86_64.rpm
```
