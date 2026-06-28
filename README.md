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

- **Create your hero** when you first open the game: pick **heroine or hero**, your
  **skin tone** (four options), **hair color** (six) and **hair style** (short, long, or
  bald), a **suit color**, a name, and an **origin** (the origin shapes your strengths
  for the whole run). A live preview updates as you choose. You can restyle your hero
  any time in **⚙️ Settings → Appearance**.
- **Tap the medallion** on the City screen to earn **Valor** — *or* flip on
  **🤖 Auto-Patrol** (right under the medallion) and the game taps for you, hands-free,
  while you watch. It's there from the very start, so you never have to grind taps.
  Upgrades in **Powers** make Auto-Patrol faster and hit harder.
- Spend Valor in **Team** to recruit allies who earn Valor automatically. Use the
  **Buy 1 / 10 / 100 / Max** toggle to buy in bulk.
- New tabs unlock as you earn: **Powers** (abilities + upgrades), **🌐 Network**
  (your living, self-running city), **Threats** (villains), and **Legacy** (prestige).
- **🌐 Network** is the payoff: every ally type you own becomes an animated **sector**
  that works on its own — icons moving, gauges sweeping, energy pulses streaming into a
  central core, and numbers ticking up everywhere. The more you unlock and automate, the
  busier and more alive it gets. Just sit and watch the machine run.
- **Powers** has active abilities on cooldowns — tap them for big bursts.
- **Threats** are supervillains with a health bar. Your team damages them automatically;
  tap **Strike** to hit harder. Beating a major villain grants a **permanent** production
  bonus.
- **Legacy** lets you **Retire** once you hit 1M Valor: you reset your run for **Legend**
  (permanent production) and unlock a **Mastery** tree — including **auto-recruit** and
  **auto-powers**, which run the game for you. Retiring is how you get strong.
- **Power Surges** ⚡ — glowing alerts drift across the screen now and then. Tap one to
  grab a random boon: **Frenzy** (×7 production), a **Tap Storm**, an instant **Valor
  Cache**, **Overdrive**, or a full ability **Recharge**. Want it hands-free? Turn on
  **⚙️ Settings → Auto-collect alerts** (or unlock the **Auto-Dispatch** Mastery node) and
  they collect themselves.
- **City Crises** 🚨 — every few minutes a situation pops up with a real choice: storm the
  bank heist for a huge payout but take a beating, or set a trap and play it safe; go
  public for a fame boost or stay in the shadows. Your call shapes the reward — and a
  couple of choices grant temporary buffs you'll see tick down up top.
- **Mystery Caches** 🎁 — rare loot crates drift by now and then (and often drop when you
  beat a villain). Tap to open one for a suspenseful reveal and a random reward: a Valor
  cache, a random buff, a full **Recharge**, **Legend Shards** (prestige currency without
  prestiging!), or a rare **Jackpot**. Auto-collect picks these up too.
- The city is **alive**: searchlights sweep the skyline, aircraft blink past, stars shoot
  overhead, windows flicker, and your hero breathes and blinks on the medallion. Hit a new
  **Rank** and you'll get a confetti celebration. (All of this respects **Reduce effects**
  and your device's reduced-motion setting.)
- **Contracts** 📋 (top-left button) — a rotating board of jobs like "foil 5 crimes,"
  "catch 3 Power Surges," or "earn X Valor." Each shows a live progress bar; finish one
  and **Claim** it for a reward (Valor, a buff, or even **Legend**), and a fresh contract
  takes its place. A red dot on the button means something's ready to claim.
- The 🏆 button tracks **achievements** — 57 of them across six categories (Combat,
  Wealth, Team, Villains, Events, Legacy), each shown with a **progress bar** toward the
  next tier so you always know what you're chasing. Every one grants **+1% production
  forever**, so completion is its own reward.

Have fun, and go become a legend. ✊
