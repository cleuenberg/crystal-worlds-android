# Crystal Worlds for Android

Android releases of **[Crystal Worlds](https://crystalworlds.tvir.games)** – a tactical RPG in 16-bit style
with monsters to collect: lead your party across grid battlefields, seal wild monsters as companions
and win back the five crystals. Plays fully offline, no ads, no tracking.

**Download:** [Zapstore](https://zapstore.dev) · or the APK from the
[latest release](https://github.com/cleuenberg/crystal-worlds-android/releases/latest)

This repository only hosts signed release builds, the Zapstore listing (`zapstore.yaml`) and the store
material (`assets/`, `ITCH.md`, `PLAY.md`). Play in the browser: <https://crystalworlds.tvir.games>

---

## Publishing to Zapstore (maintainer)

1. Install `zsp`: <https://github.com/zapstore/zsp/releases>
2. **First time:** in a local clone of this repo run `zsp publish --wizard`.
   - It adds your `pubkey` to `zapstore.yaml` → commit and push it.
     Zapstore reads this file from this public repo to whitelist you.
   - It links the APK signing certificate to your Nostr identity once
     (needs `crystalworlds-release.jks`).
3. **Every new release** (after the `vX.Y.Z` release appears here):
   `zsp publish zapstore.yaml`

## Store material

Generated from the game (repo `crystal-worlds`, local server `python3 tools/serve.py` running):

| File | Tool |
|---|---|
| `assets/icon.png` (512 × 512) | `python3 tools/make-icons.py` |
| `assets/screenshots/` (1080 × 2280, Zapstore) | `node tools/store-screenshots.mjs ../crystal-worlds-android/assets/screenshots` |
| `assets/itch-screenshots/` (1080 × 2160, itch.io and Google Play) | `node tools/store-screenshots.mjs ../crystal-worlds-android/assets/itch-screenshots 720` |
| `assets/itch-cover.png` (630 × 500), `assets/play-feature.png` (1024 × 500) | `node tools/store-art.mjs ../crystal-worlds-android/assets` |

World 5 and the reward for a complete collection are deliberately not shown anywhere.
