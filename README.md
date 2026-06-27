# Cape City — Idle Hero

A single-page idle/incremental superhero game. Tap to fight crime, recruit a team
that earns for you automatically, unlock powers and villains as you grow, then retire
for permanent **Legend** bonuses. Runs entirely in the browser — no server, no
accounts, no tracking — and installs to your phone like a real app.

---

## Put it on GitHub and open it as an app

1. **Make a new repo** (e.g. `cape-city`) and upload the **contents of this folder**
   so that `index.html` sits at the repo root, with `icons/`, `preview/`, and
   `manifest.webmanifest` next to it:

   ```
   cape-city/
   ├── index.html              ← the game (this is the page GitHub serves)
   ├── manifest.webmanifest    ← install config
   ├── icons/                  ← home-screen app icons (incl. Android maskable + iOS)
   └── preview/                ← link-preview image + install screenshots
   ```

2. **Turn on Pages:** repo **Settings → Pages → Build and deployment →
   Source: Deploy from a branch → `main` / `/ (root)` → Save.**
   After ~1 minute your link is `https://<your-username>.github.io/cape-city/`.

3. **Install on your phone:**
   - **Android (Chrome):** open the link → **⋮ menu → Add to Home screen** (or tap the
     "Install" prompt). It launches fullscreen with the shield icon.
   - **iPhone (Safari):** open the link → **Share → Add to Home Screen.**

> Keep the folder together. `index.html` loads the icons and manifest by relative
> path, so upload all of it. (The game still *plays* if you upload only `index.html`,
> but the custom icon and install screenshots won't show.)

**Even faster, no GitHub:** rename nothing, go to **app.netlify.com/drop**, and drag
this whole folder onto the page — you get a live HTTPS link instantly.

---

## Your progress is saved — and survives closing the app

This was built to be safe to close at any time:

- The game **auto-saves every 8 seconds**, after **every purchase**, and **the moment
  you leave or background the app** (it listens for tab-hide, app-freeze, blur, and
  page-unload — the events Android/iOS actually fire before killing a backgrounded app).
- When you **reopen it**, it loads your save *and* pays out **offline earnings** for the
  time you were away (up to 4 hours by default — extendable with the Cosmic origin and
  Mastery upgrades). You'll see a "While you were away" summary.
- Saves live in your browser's local storage **for this site**. That means:
  - Same phone + same browser → your hero is always there.
  - **Clearing browser data / site data, or opening it in a different browser, starts
    fresh.** To move between devices, use **⚙️ Settings → Copy save**, then paste the
    code into **Settings → Load from box** on the other device.

---

## How to play (the short version)

- **Tap the medallion** on the City screen to earn **Valor**.
- Spend Valor in **Team** to recruit allies who earn Valor automatically. Use the
  **Buy 1 / 10 / 100 / Max** toggle to buy in bulk.
- New tabs unlock as you earn: **Powers** (abilities + upgrades), **Threats**
  (villains), and **Legacy** (prestige).
- **Powers** has active abilities on cooldowns — tap them for big bursts.
- **Threats** are supervillains with a health bar. Your team damages them automatically;
  tap **Strike** to hit harder. Beating a major villain grants a **permanent** production
  bonus.
- **Legacy** lets you **Retire** once you hit 1M Valor: you reset your run for **Legend**
  (permanent production) and unlock a **Mastery** tree — including **auto-recruit** and
  **auto-powers**, which run the game for you. Retiring is how you get strong.
- The 🏆 button tracks **achievements** (each adds +1% production forever).

Have fun, and go become a legend. ✊
