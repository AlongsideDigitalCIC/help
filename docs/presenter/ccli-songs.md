---
title: Song Library & CCLI SongSelect
description: Manage your worship repertoire, import CCLI SongSelect lyrics, display copyright attributions, and export CCLI reports.
---

Presenter allows you to manage a fast, searchable local database of worship songs, hymns, and contemporary anthems â€” complete with full-text lyric search, section arrangements, on-screen CCLI attribution, and automated CCLI reporting.

:::tip[Moving from ProPresenter, FreeShow, OpenLP, Quelea, or WorshipTools?]
You can bring your entire existing song database into Presenter in minutes using the **Universal Song Library Importer**. See **[Importing Your Song Library](/presenter/importing-songs)** for supported software and step-by-step instructions.
:::

---

## 1. Importing Songs from CCLI SongSelect

If your church holds a CCLI SongSelect subscription, Presenter supports two fast ways to bring official lyrics and metadata into your library:

### Option A: Bulk Import `.usr` or `.txt` Files
1. Download your song lyrics from CCLI SongSelect as **USR (`.usr`)** or **Lyrics (`.txt`)** files.
2. In Presenter, open the **Songs** tab and click **Import** (or simply drag and drop the downloaded files anywhere onto the Presenter window).
3. Presenter automatically extracts the song title, authors/writers, copyright notice, CCLI song number, and `[Verse]` / `[Chorus]` sections.
4. Click **Import Songs** to save them directly to your library.

### Option B: Quick Clipboard Paste (Single Song)
1. Copy the lyrics text from a CCLI SongSelect song page.
2. In Presenter, open the **Songs** tab and click **+ New**.
3. Click **Import Song Select** in the Song Editor toolbar â€” Presenter parses the pasted lyrics, author, copyright line, and CCLI number automatically.

---

## 2. Creating, Editing & Arranging Songs

Songs in Presenter are stored as clean, future-proof Markdown files inside your Media Library's `Songs/` folder and split into clear sections:
* `[Verse 1]`, `[Verse 2]`, `[Pre-Chorus]`, `[Chorus]`, `[Bridge]`, `[Tag]`, `[Outro]`

* **Quick Slash Shortcuts:** While typing in the Song Editor, type `/v1`, `/v2`, `/c`, `/pc`, `/b`, or `/o` on a new line to insert formatted section headers instantly.
* **Lines Per Slide:** Switch dynamically between **1, 2, 3, or 4 lines per slide** at the top of any song without rewriting your lyrics.
* **Flow Arrangement:** Click **Flow Arrangement** to build custom verse/chorus orders (for example `Verse 1 â†’ Chorus â†’ Verse 2 â†’ Chorus â†’ Bridge â†’ Chorus`) without duplicating lyric text.

---

## 3. CCLI Copyright Display & Annual Reporting

### On-Screen CCLI Attribution
1. Open **Settings** (gear icon) &rarr; **CCLI & Licensing**.
2. Enter your church's **CCLI Licence Number**.
3. Choose where your legal attribution line should appear: **First Slide Only**, **Last Slide Only**, **First & Last Slides**, or **All Slides**, along with **Bottom Left**, **Bottom Centre**, or **Bottom Right** alignment.

### Automated Song History & CSV Export
Presenter automatically logs songs projected live during your services. When it is time to submit your CCLI report:
1. Open **Settings** &rarr; **CCLI & Licensing**.
2. Under **Song History & Annual CCLI Reporting**, select your reporting date range.
3. Click **Export Song History to CSV** to download a ready-to-reference log containing Date Played, Song Title, Artist, CCLI Song Number, and Copyright details.
