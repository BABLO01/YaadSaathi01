# Yaad Saathi — یاد ساتھی

A flat, dependency-free Progressive Web App designed specifically for GitHub Pages.

## GitHub Pages

Upload **all files in this folder directly to the repository root**. Do not put them inside another folder.

```text
index.html
styles.css
app.js
manifest.webmanifest
sw.js
icon.svg
icon-192.png
icon-512.png
.nojekyll
README.md
LICENSE
```

No Node.js, npm, Vite, React, Tailwind, build command, or package installation is required.

Then enable:

**GitHub → Settings → Pages → Deploy from a branch → main → /(root)**

## Included

- Premium soft-glass Yaad Saathi UI
- One-time-per-session splash screen
- Fixed/sticky header and fixed bottom navigation
- Clear active state for Home / Search / Reminders / Settings
- My Things
- Buy Again
- Memory Notes
- My Notebook
- Documents
- Warranty & Bills
- Gifts & Wishlist
- Future Me
- Up to two user-created Custom Categories
- Secure Vault for private account/login details using Web Crypto AES-GCM
- Global search and category filters
- Complete category history with edit/delete
- Camera + gallery photo selection
- Smart Capture
- Voice Capture saved inside Memory Notes (there is no separate Voice Notes category)
- Reminder start/end date and time
- Browser notification support where the browser allows it
- Future Me notification support where supported
- Profile photo and display name
- Soft Light / Clear Light / Dark themes
- English / اردو
- JSON backup and restore
- Share app link / copy app link
- PWA install support and install banner
- Offline-first local storage using IndexedDB with localStorage fallback

## Notification note

Web notifications depend on browser permission and platform background rules. A static GitHub Pages PWA cannot guarantee OS-level alarms after the browser has been completely terminated. When the page/PWA is active, scheduled timers and notifications are supported.

## Secure Vault note

Vault data is encrypted locally with AES-GCM using a passphrase-derived key. The app does not store the vault passphrase. If the passphrase is forgotten, the vault cannot be recovered by this app.

## Developer

Developer by Muhammad Usman Channa

## License

MIT

## Visual themes
Yaad Saathi now includes three intentionally different themes:
- **Botanical Glass** — the approved mint/teal glass style.
- **Pearl Aurora** — a brighter editorial lavender/pearl style.
- **Midnight Garden** — a deep premium night style.

The bottom navigation is fixed close to the device bottom edge with safe-area support. The header transitions into a soft glass bar while scrolling. Smart Capture uses photo/gallery/quick-note only; the old voice-capture mode has been removed from the UI and code path.
