# Days — Day Counter App

A simple, offline-first PWA to count days since or until any event.
No backend, no account, no cost.

---

## How to deploy on GitHub Pages (free hosting)

### Step 1 — Create a GitHub repository

1. Go to https://github.com and log in
2. Click the **+** button (top right) → **New repository**
3. Name it: `day-counter` (or anything you like)
4. Make sure it is set to **Public**
5. Leave everything else as default
6. Click **Create repository**

---

### Step 2 — Upload your files

You will see a page that says "Quick setup". Do this:

1. Click **"uploading an existing file"** link
2. Drag and drop these 3 files onto the page:
   - `index.html`
   - `manifest.json`
   - `sw.js`
3. Scroll down and click **Commit changes**

---

### Step 3 — Turn on GitHub Pages

1. In your repository, click **Settings** (top tab)
2. In the left sidebar, click **Pages**
3. Under "Branch", select **main** from the dropdown
4. Leave the folder as **/ (root)**
5. Click **Save**

GitHub will show you a message like:
> "Your site is live at https://YOUR-USERNAME.github.io/day-counter/"

It may take 1-2 minutes to go live.

---

### Step 4 — Open it on your phone

1. Copy your URL (e.g. `https://YOUR-USERNAME.github.io/day-counter/`)
2. Open it in your phone browser
3. **Android (Chrome):** tap the 3-dot menu → "Add to home screen"
4. **iPhone (Safari):** tap the Share button (box with arrow) → "Add to Home Screen"

It will appear as an app icon and open fullscreen — just like a native app.

---

## Icons (optional but recommended)

The app references `icon-192.png` and `icon-512.png` for the home screen icon.
To add your own icon:
- Create a square image (any image editor works, even paint.net or Canva)
- Export it as PNG in two sizes: 192×192 and 512×512
- Name them `icon-192.png` and `icon-512.png`
- Upload them to your GitHub repository the same way you uploaded the other files

If you skip this, the app still works — it just won't have a custom icon.

---

## How it works (quick summary)

| Part | What it does |
|---|---|
| `index.html` | The whole app — HTML, CSS, and JavaScript in one file |
| `manifest.json` | Tells the browser this is an installable app (name, icon, colors) |
| `sw.js` | Service Worker — caches the app so it works offline after first load |
| `localStorage` | Where your counters are saved — lives on your device, survives shutdown |

---

## Will I lose my data?

No. `localStorage` saves to your hard drive, not RAM.
Data survives: shutdowns, restarts, browser closes.
Data is lost only if you clear your browser cache, or use a different browser/device.
