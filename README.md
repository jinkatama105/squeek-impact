# SQUEEK IMPACT 🐹💥

A zero-backend, pixel-art side-scrolling arcade (Nokia Space Impact style) where the enemy
waves are driven by the **live Squeekchain hamster PoW chain**.

- Hamster **SPINNING** → TURBO mode: enemies +70% speed, score x1.5
- Hamster **IDLE** → CHILL mode: double loot drops
- Block height and blockProgress drive the parallax starfield and the HUD chain pulse —
  every verified block visibly moves the game.

**Play:** https://squeekimpact.vercel.app

## Features
- 3 chapters (The Wheel / Squeektown / Deep Burrow) with distinct palettes and enemy mixes
- 3 selectable ships with real stat trade-offs (speed vs fire-rate vs lives), choice persisted
- Kamikaze runners, armored heavies, wheel + twin bosses, extra-life pickup
- Chain-status HUD polled from the public Squeekchain community API
- Local high-score board + one-tap score share
- Single HTML file. No server, no build step, no libraries. 60fps on a phone browser.

## Run
Just open `index.html`, or:
```
python3 -m http.server 8000
```

Built for the Squeekchain code lane — the chain isn't a leaderboard bolted onto a game,
it IS the game's difficulty engine.

squeekchain-project: 73c23635-c3e1-4025-9be0-ee4988a76195
