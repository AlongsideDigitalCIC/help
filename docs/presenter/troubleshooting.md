---
title: Sunday Morning Troubleshooter
description: Quick, 60-second fixes for common live presentation issues.
---

If you are setting up right before a service or event and something isn't working, follow these quick diagnostic steps.

---

## 1. Projector is Black or Showing Desktop Wallpaper

### The Problem
You click "Go Live" in Presenter, but the projector only shows your Windows/Mac wallpaper or remains black.

### The 60-Second Fix
1. Press `Windows Key + P` on your keyboard (or go to Mac **System Settings &rarr; Displays**).
2. Check that **Extend** is selected (not *Duplicate*).
3. In Presenter, click the **Settings (gear icon)** in the top-right corner and open **Display & Transitions**.
4. Under **Projector Monitor Output**, make sure your external screen is selected (or choose **Auto**), close Settings, and click **END LIVE** followed by **GO LIVE**.
5. Check whether the **Black Screen** button in the right-hand Live Controls panel shows **Black Screen Active**—if so, click it once to restore projection.

---

## 2. No Sound When Playing a Video

### The Problem
The video plays on screen, but no audio comes through the venue speakers or sound desk.

### The 60-Second Fix
1. Click the Windows or Mac speaker icon in your system tray and make sure the audio output is set to your HDMI connection or audio interface.
2. Check the volume slider inside Presenter's video player panel.
3. Verify that your external mixer or amplifier channel is unmuted and the fader is up.

---

## 3. Remote Control Won't Connect on Mobile Phone

### The Problem
Scanning the QR code produces a "Page Cannot Be Found" or loading spinner on your mobile browser.

### The 60-Second Fix
1. Confirm both your computer and phone are connected to the **exact same Wi-Fi network**.
   * *Note:* If your church has separate "Church-Guest" and "Church-Private" networks, both devices must be on the private network. Guest networks typically block devices from talking to each other (client isolation).
2. Check Windows Firewall: If prompted, allow Presenter through private networks.
3. Open **Settings (gear icon) &rarr; Network & Remotes**, copy the **Remote Control URL** (served on port `:5178`, e.g., `http://192.168.1.100:5178/?remoteControl=...`), and enter it directly in your phone's browser. If your hostname URL does not resolve on mobile, click **Use IP** under **Detected Network Addresses**.

---

## 4. Text or Lyrics Overflowing the Slide

### The Problem
The text is too large or feels crowded on the projector screen.

### The 60-Second Fix
1. In the centre preview toolbar, lower **Lines** (for songs/liturgy, e.g. from `4` down to `2`) or **Verses** (for Bible readings) so Presenter splits long stanzas across more slides automatically.
2. Hover over an individual slide tile and click **Quick Fix** (or click **Edit Song**) to add line breaks or blank lines between stanzas.
3. To adjust text sizing globally across every slide, open **Settings (gear icon) &rarr; Display & Transitions** and lower **Output Text Scale**.

---

## Need More Help?

If you are stuck and need urgent guidance, reach out to us at [help@alongsidedigital.co.uk](mailto:help@alongsidedigital.co.uk).
