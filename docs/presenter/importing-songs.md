---
title: Importing Your Song Library
description: Migrate your existing worship song database from ProPresenter, FreeShow, OpenLP, Quelea, WorshipTools, EasyWorship, OpenSong, CCLI SongSelect, and more.
---

Moving to Presenter does not mean starting your worship repertoire from scratch. The **Universal Song Library Importer** converts existing song libraries, databases, and lyric archives into Presenter's clean Markdown song format â€” preserving titles, authors, copyright lines, CCLI song numbers, verse/chorus sections, and slide flow arrangements.

---

## 1. Opening the Universal Song Library Importer

Make sure you have connected a local **Media Library** folder in Presenter first (so Presenter knows where to save your converted `Songs/` files). You can then launch the importer in any of four ways:

1. **Songs Tab:** Click **Songs** in the top navigation bar, then click the **Import** button next to **+ New**.
2. **Drag & Drop Anywhere:** Drag song files, database files, `.zip` / `.qsp` packs, or an entire song folder directly onto the Presenter window.
3. **Settings:** Open **Settings** (gear icon) &rarr; **Storage** &rarr; **Import Song Library**.
4. **Single Song Editor:** When creating or editing a single song (**+ New** or **Edit Song**), click **Import File** to load a single file, or **Import Song Select** to paste copied CCLI SongSelect text straight from your clipboard.

:::tip[1-Click Migration on Desktop]
If you run the **Presenter Desktop App** on the same computer where **ProPresenter**, **FreeShow**, **OpenLP**, **OpenSong**, **VideoPsalm**, or **SongBeamer** is already installed, Presenter automatically detects those song folders and displays them under **Detected on This Computer**. Simply click **Scan** to load your entire library in one click.
:::

---

## 2. Supported Software & File Formats

Presenter supports **15+ church presentation formats**, databases, and archive types out of the box:

| Software / Source | Supported Files & Databases | Preserved Details |
| :--- | :--- | :--- |
| **ProPresenter 7+** | `.pro`, `.proBundle`, `.zip` | Lyrics, section labels (`Verse`, `Chorus`, `Bridge`), slide arrangements, author, copyright & CCLI # |
| **ProPresenter 4, 5 & 6** | `.pro6`, `.pro6x`, `.pro5`, `.pro4` | Lyrics (decoded from RTF), section groups, arrangement cues, author, copyright & CCLI # |
| **FreeShow** | `.show`, `.project`, JSON backups | Lyrics, group labels, active layout slide flow, author, copyright & CCLI # |
| **OpenLP** | `songs.sqlite`, OpenLyrics `.xml` | Full song database or exported XML, verse order (`v1 c1 v2`), authors, copyright & CCLI # |
| **Quelea** | `.qsp` (Song Pack), `.xml` | Entire zipped `.qsp` song packs or individual XML exports, sections, author & CCLI # |
| **WorshipTools** *(Presenter / Planning)* | ChordPro (`.cho`, `.chordpro`, `.txt`), SongSelect `.usr`/`.txt`, `.csv` | Lyrics (with automatic chord stripping), section headers, author, copyright & CCLI # |
| **EasyWorship 6 & 7** | `Songs.db` + `SongWords.db` *(selected together)* | Full database titles, authors, copyright, CCLI #, and RTF slide words |
| **OpenSong** | Extensionless XML files *(via folder import)* | Lyrics, `[V1]`/`[C]` tags, presentation order, chord-line filtering, author, copyright & CCLI # |
| **CCLI SongSelect** | `.usr`, `.txt`, or clipboard paste | Official lyrics, verse/chorus markers, writers, copyright notice & CCLI song number |
| **VideoPsalm** | `.vpc` SongBook files | Complete JSON/VPC songbooks, verses, composer/author, copyright & CCLI # |
| **SongBeamer** | `.sng` | Multi-slide lyrics (`---` separators), `#Title` / `#Author` / `#CCLI` headers & section tags |
| **EasySlides / EasiSlides** | `.xml` | Batch XML song exports, numbered regions/sections, writer, copyright & licence number |
| **MediaShout** | `.xml` | Exported XML song decks, stanza labels, author, copyright & CCLI # |
| **SoftProjector** | `.spb` (SQLite SongBook) | Full `.spb` database tables, verse markers & song metadata |
| **Generic Files & Archives** | `.csv`, `.tsv`, `.rtf`, `.txt`, `.md`, `.zip` | Multi-column spreadsheets with lyrics, plain text songs, ChordPro sheets & nested `.zip` archives |

---

## 3. Step-by-Step Instructions by Platform

Find your previous presentation software below to see where its songs are stored and what to select in Presenter.

### ProPresenter 7 (and newer)
* **No export needed** if migrating on the same computer â€” open the importer and click **Scan** next to ProPresenter, or click **Select Entire Folder** and choose:
  * **Windows:** `Documents\ProPresenter\Libraries`
  * **macOS:** `Documents/ProPresenter/Libraries`
* **Moving from another computer:** In ProPresenter, right-click your song library in the left sidebar and choose **Export** (as `.pro` files or a `.proBundle`), copy the files via USB or cloud drive, and drop them into Presenter.

### ProPresenter 4, 5 & 6
* Select your `.pro6`, `.pro6x`, `.pro5`, or `.pro4` files (or select your old ProPresenter library folder). Presenter automatically decodes embedded RTF slide text and converts slide group labels into sections.

### FreeShow
* **Direct folder import:** Click **Select Entire Folder** and select `Documents/FreeShow/Shows` (where FreeShow stores `.show` files).
* **Backup / Project import:** You can also drop individual `.show` files, `.project` files, or a full FreeShow JSON backup file directly into the importer.

### OpenLP
* **Fastest method (Full Database):** Import your `songs.sqlite` database file directly to bring every song across at once:
  * **Windows:** `C:\Users\<YourName>\AppData\Roaming\openlp\data\songs\songs.sqlite` *(Tip: paste `%APPDATA%\openlp\data\songs` into the file picker address bar)*
  * **macOS:** `~/Library/Application Support/openlp/Data/songs/songs.sqlite`
* **Alternative method (XML Export):** In OpenLP, go to **File &rarr; Export &rarr; Song**, export as **OpenLyrics XML**, and drop the exported folder or `.zip` into Presenter.

### Quelea
* In Quelea, go to **Database &rarr; Export &rarr; Quelea Song Pack (`.qsp`)** to save your entire repertoire into a single file.
* Drag that `.qsp` file straight into Presenter's importer (individual Quelea/OpenLyrics `.xml` exports are also supported).

### WorshipTools (Worship Extreme / Presenter & Planning)
* In WorshipTools, open your **Songs** list and export your songs as **ChordPro** (`.cho` / `.txt`), **CCLI SongSelect** (`.txt` / `.usr`), or a **CSV spreadsheet that includes lyrics**.
* Drop the exported files (or `.zip` archive) into Presenter. Keep **Strip Musical Chords** ticked so inline chords like `[G]` and `[D/F#]` are removed cleanly for projection.

:::note[CSV Exports Without Lyrics]
Some planning exports only export a summary table (Title, Author, CCLI #) without the song lyrics column. Make sure your export includes the **lyrics** or use ChordPro / SongSelect `.txt` exports so Presenter can build your slides.
:::

### EasyWorship 6 & 7
EasyWorship splits song metadata and slide text across two database files (`Songs.db` and `SongWords.db`).
1. In Presenter's importer, click **Select Files / Databases / ZIP** (or **Select Entire Folder**).
2. Navigate to your EasyWorship profile data folder:
   `C:\Users\Public\Documents\Softouch\Easyworship\Default\v6.1\Databases\Data\` *(folder version may vary slightly)*.
3. Select **both `Songs.db` and `SongWords.db` at the same time** (hold `Ctrl` while clicking both files, or select the entire `Data` folder) so Presenter can pair every song title and CCLI number with its lyrics.

### OpenSong
OpenSong saves each song as an XML file **without a file extension** (for example `Amazing Grace` rather than `Amazing Grace.xml`).
* Click **Select Entire Folder** in Presenter's importer and choose your `Documents/OpenSong/Songs` folder (or zip the folder first and drop the `.zip`).
* Presenter automatically inspects extensionless OpenSong files, strips `.`-prefixed chord lines when **Strip Musical Chords** is enabled, and preserves your `[V1]`, `[C]`, and `<presentation>` flow order.

### CCLI SongSelect
* Download **Lyrics (`.txt`)** or **USR (`.usr`)** files from SongSelect and drop as many as you like into the Universal Song Library Importer at once.
* For a quick single song on a Sunday morning, copy the lyrics page on SongSelect, open **Songs &rarr; + New** in Presenter, and click **Import Song Select**.

### VideoPsalm & SongBeamer
* **VideoPsalm:** Click **Select Files** and choose your `.vpc` SongBook file from `C:\Users\Public\Documents\VideoPsalm\SongBooks\`.
* **SongBeamer:** Click **Select Entire Folder** and choose `Documents\SongBeamer\Songs` (containing your `.sng` files).

### Spreadsheets (`.csv` / `.tsv`) & Plain Text (`.txt` / `.rtf`)
* **CSV / TSV:** Include a header row with columns such as `Title`, `Lyrics` (required), and optional `Artist` / `Author`, `CCLI`, and `Copyright`. Blank lines inside the `Lyrics` cell separate slides/sections.
* **Plain Text / RTF / ChordPro:** The first line (or `{title: ...}` directive) is used as the song title, and `[Verse 1]`, `[Chorus]`, or blank-line stanzas are converted into clean sections automatically.

---

## 4. Reviewing, Cleaning & Handling Duplicates

Once Presenter finishes scanning your files, you will see a live preview before anything is written to your library:

* **Search & Selective Import:** Filter parsed songs by title, artist, or source format, and tick or untick individual songs.
* **Live Section & Flow Preview:** Click any song on the left to inspect its converted `[Verse]`, `[Chorus]`, and `[Bridge]` sections and slide `Flow` badges on the right.
* **Strip Musical Chords:** Enabled by default. Toggle this off if your worship band prefers keeping inline chords inside the lyrics.
* **Duplicates Control:** Any song whose title already exists in your library is badged with **Exists**. Choose how Presenter should handle matches:
  * **Skip** *(Recommended)* â€” Keeps your existing Presenter song untouched and only imports brand-new songs.
  * **Overwrite** â€” Replaces existing songs with the newly imported version.
  * **Keep Both** â€” Saves the imported song alongside the original with a numbered suffix (e.g. `Amazing Grace (2)`).

---

## Related Guides

* [Song Library & CCLI SongSelect](/presenter/ccli-songs)
* [Presenter Quick Start Guide](/presenter/quick-start)
* [Sunday Morning Troubleshooter](/presenter/troubleshooting)
