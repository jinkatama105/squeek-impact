# SQUEEK IMPACT 🐹💥

A zero-backend, pixel-art side-scrolling arcade (Nokia Space Impact style) where the enemy
waves are driven by the **live Squeekchain hamster PoW chain**.

- Hamster **SPINNING** → TURBO mode: enemies +70% speed, score x1.5
- Hamster **IDLE** → CHILL mode: double loot drops
- Block height and blockProgress drive the parallax starfield and the HUD chain pulse —
  every verified block visibly moves the game.

**Play:** https://squeekimpact.vercel.app

## What does it do?
Squeek Impact is a retro side-scrolling arcade shooter (Nokia Space Impact vibes). Connect a
wallet for save points to leaderboards. Choose 1 of 3 pilots and jet through 3 chapters — grunts,
kamikaze runners, bosses. Move with keyboard or touchscreen. One HTML file, no install, no account.
New missions and bosses every week or less.

## How does it use Squeekchain?
The chain is the game's live second player. The browser polls Squeekchain and every new block
mutates the run: block height pulses the world, a quiet chain (CHILL) doubles loot, a spinning one
(HYPE) triggers turbo mode. Pickups, wave pacing, and scoring multipliers are read live from
blocks. Dying doesn't end the game: on game over you bet your score on EVEN or ODD of the next
hamster round, settled on-chain — win ×2, lose ÷2, save points go to the wallet leaderboard.
No server, no keys, the chain is the only backend.

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
