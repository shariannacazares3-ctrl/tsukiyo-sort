# 月夜マート · Tsukiyo Mart: Midnight Restock

A cozy, juicy goods-sorting puzzle game set in a Japanese konbini at 2 a.m.
Rain on the window, a humming fluorescent glow, lofi city-pop, and a cat who visits every night. 🌙🍙

**Everything lives in one file: [`index.html`](index.html).** No build step, no dependencies, no external images or sounds.
All art is drawn with canvas code, and all audio is synthesized with the Web Audio API.

## How to play

- **Drag** a good to another slot, or **tap** a good and then **tap** a slot.
- Line up **3 identical goods** in one slot to pop them. ✨
- Dim goods wait **behind** the front row, and slide forward when a slot's front row empties.
- Clear every good to finish the shift.

### Special goods & obstacles (introduced gradually)
| | |
|---|---|
| 🐱 **Maneki-neko** (Lv 5) | Wildcard that matches anything. Paired with two goods, it beckons their third twin from anywhere on the shelves. |
| 🧊 **Iced goods** (Lv 8) | Can't move or match. Clear a triple in a neighboring slot to thaw them. |
| 📦 **Taped boxes** (Lv 13) | Block a slot. Each neighboring triple tears one strip of tape (the number shows hits left). |
| 🔒 **Locked shelves** (Lv 19) | Clear the good with a golden 🔑 tag, and the key flies over to unlock the shelf. |

### Boosters (bought with earned coins, never real money)
💡 Hint (15) · ↩️ Undo (20) · 🔀 Shuffle (40) · ⏳ +30s (30, Timed mode)

## Features

- 40 handcrafted levels in 4 chapters (Rainy Station Street → Summer Festival Lane → Autumn Moon Alley → Snowy Crossing), then an **Endless Night Shift**.
  A built-in solver verifies that every generated board can be cleared.
- 🌙 **Relaxed** mode (no timer, up to ★★) and ⏱ **Timed** mode (beat the clock for ★★★).
- A night-street level map with konbini storefronts and neon signs.
- Story scenes with the late-night regulars: Yuzu the sleepy student, Tanaka-san the salaryman, Mochi the cat, and the manager's sticky notes.
- Juice everywhere: squash & stretch, sparkle bursts, floating points, screen shake, combo callouts ("Nice!" → "Great!" → "SUGOI!!") with rising pop pitch, and phone vibration.
- Lofi city-pop loop (royal-road progression), soft rain ambience, and synthesized SFX. Each has its own on/off toggle and volume slider in Settings (and in the pause menu); rain starts quiet so the music leads.
- Cosmetics: shelf themes (Classic, Cozy Wood, Pastel Mint, Neon Night) and seasonal decor (Sakura, Summer Festival, Snowy Winter).
- Optional pixel-art mode for the goods.
- Progress saved in `localStorage`.

## Run it locally

Open `index.html` in any modern browser. That's it!
(Or serve the folder with any static server, e.g. `npx http-server .`)

## Play it online with GitHub Pages

1. On GitHub, open the repository → **Settings** → **Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Pick the branch `main` and the folder `/ (root)`, then click **Save**.
4. Wait a minute or two. Your game will be live at `https://<your-username>.github.io/tsukiyo-sort/`.
