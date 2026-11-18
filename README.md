# Alongside Digital Help Centre

Customer help portal and user guides for **Presenter** and **Admin Centre**, built with **[Docsify](https://docsify.js.org/)** and managed via **[Pages CMS](https://app.pagescms.org/)**.

* **GitHub Repository:** [AlongsideDigitalCIC/help](https://github.com/AlongsideDigitalCIC/help)
* **Live Domain:** [help.alongsidedigital.co.uk](https://help.alongsidedigital.co.uk)
* **CMS Editor:** [app.pagescms.org](https://app.pagescms.org/)

---

## 📁 Repository Structure

```text
Documentation/
├── index.html                    # Docsify portal, Alongside Digital brand theme & instant search
├── .pages.yml                    # Pages CMS configuration (collections, sidebar & media)
├── .nojekyll                     # Ensures GitHub Pages serves _sidebar.md
├── netlify.toml                  # Static hosting configuration for Netlify
├── public/                       # Brand logos & favicons
│   ├── favicon.png
│   ├── logo.webp
│   └── logo.png
└── docs/                         # All Markdown documentation served by Docsify
    ├── README.md                 # Help Centre Homepage
    ├── _sidebar.md               # Sidebar Navigation menu
    ├── support.md                # Contact & Support page
    ├── media/                    # Screenshots & media uploaded via Pages CMS
    ├── presenter/                # Presenter App Guides
    │   ├── quick-start.md
    │   ├── importing-songs.md
    │   ├── presentation-mode.md
    │   ├── ccli-songs.md
    │   ├── scripture-bibles.md
    │   ├── liturgy.md
    │   ├── media.md
    │   ├── remote-control.md
    │   └── troubleshooting.md
    └── admin-centre/             # Admin Centre Guides
        ├── overview.md
        ├── organisation-setup.md
        ├── members-directory.md
        ├── volunteer-rotas.md
        ├── safeguarding-dbs.md
        ├── events-planning.md
        └── notifications.md
```

---

## ✏️ Editing Guides in Pages CMS

1. Open **[https://app.pagescms.org/](https://app.pagescms.org/)** and select **`AlongsideDigitalCIC/help`**.
2. In the left menu of Pages CMS, you will find:
   * **Presenter Guides** (`docs/presenter/*.md`)
   * **Admin Centre Guides** (`docs/admin-centre/*.md`)
   * **Help Centre Homepage** (`docs/README.md`)
   * **Contact & Support Page** (`docs/support.md`)
   * **Sidebar Navigation** (`docs/_sidebar.md`)
   * **Media** (`docs/media/`) for uploading screenshots and images.
3. Because Docsify renders Markdown on the fly, any change saved in Pages CMS goes live immediately with no build step required.

---

## 🚀 Previewing Locally

To run the Docsify portal locally on your computer:

```powershell
cd "C:\Users\jonat\OneDrive\Documents\Alongside Digital\Applications\Documentation"
npm.cmd run dev
```

Or using Python's built-in web server:

```powershell
cd "C:\Users\jonat\OneDrive\Documents\Alongside Digital\Applications\Documentation"
python -m http.server 4321
```

Then open **`http://localhost:4321`** in your browser.
