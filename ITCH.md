# Crystal Worlds auf itch.io – Seite einrichten

Alles, was beim Anlegen der Projektseite auf itch.io einzutragen ist (wie bei Piplosion).
Erst als **Draft** speichern, Vorschau testen, dann auf **Public** stellen.

## Dateien

| Was | Datei |
|---|---|
| Web-Version (im Browser spielbar) | `crystal-worlds-web-X.Y.Z.zip` – Artefakt des GitHub-Builds (Workflow „Android app“ im Repo `crystal-worlds`) |
| Android-APK | aus dem [neuesten Release](https://github.com/cleuenberg/crystal-worlds-android/releases/latest) |
| Titelbild (Cover, 630 × 500) | `assets/itch-cover.png` |
| Screenshots | `assets/itch-screenshots/01-battle.png` … `06-title.png` (1080 × 2160 – itch.io erlaubt max. 2160 px Höhe; `assets/screenshots/` ist der Zapstore-Satz mit 2280 px) |

## Grundeinstellungen („Create new project“)

- **Title:** Crystal Worlds
- **Project URL:** `…itch.io/crystal-worlds`
- **Short description or tagline:**
  `Lead your party, seal monsters and win back the crystals – a tactical 16-bit RPG.`
- **Classification:** Games
- **Kind of project:** HTML
- **Release status:** Released
- **Pricing:** **„$0 or donate“** (wie Piplosion)

## Uploads

1. **Web-ZIP** hochladen → Häkchen **„This file will be played in the browser“**.
2. **APK** hochladen → Plattform **Android** anhaken.

## Embed options (Web-Version)

- **Viewport dimensions:** `450` × `800`
- **Frame options:**
  - ✅ **Mobile friendly** → Orientation: **Portrait**
  - ✅ **Fullscreen button**
  - ☐ Automatically start on page load (aus lassen – der Klick auf „Run game“ erlaubt dem Browser auch den Ton)
  - ☐ SharedArrayBuffer support (nicht nötig)

## Details

**Description** (in den Editor einfügen):

> **Crystal Worlds** is a tactical RPG in 16-bit style – with monsters to collect.
>
> A shadow has scattered the five crystals that keep the worlds in balance. Lead Lian and friends across grid battlefields, from green plains through dark woods and fiery mountains to icy peaks – and beyond.
>
> **Tactics**
> - Turn-based battles on a grid: terrain gives cover, elements decide the upper hand, the fast strike twice
> - Danger zone shows where enemies and monsters can reach next turn
> - Dark caves where only lamps and torches light the way
> - Every world ends in a castle guarded by a boss
>
> **Monsters**
> - Weaken wild monsters and seal them – 15 species to collect
> - Each one evolves through three stages
> - Companions give their hero bonus stats, fight on their own and unleash co-op attacks
> - Complete the collection for a special surprise
>
> **More**
> - Weapons and armour from chests and loot
> - Battles are saved after every action
> - Chiptune music and sound effects on an emulated 16-bit sound chip
> - English and German
>
> **Play** right here in the browser, or install the Android app (APK below, also on [Zapstore](https://zapstore.dev)).
> Also playable at [crystalworlds.tvir.games](https://crystalworlds.tvir.games) – installable and offline-capable.
>
> *Privacy: the game stores your progress only on your device and sends no data anywhere.*

- **Genre:** Strategy (alternativ Role Playing)
- **Tags** (max. 10): `tactical-rpg`, `turn-based-strategy`, `monster-taming`, `pixel-art`, `retro`, `16-bit`, `chiptune`, `singleplayer`, `offline`, `fantasy`
- **AI generation disclosure:** itch.io fragt, ob das Projekt KI-erzeugte Inhalte enthält.
  Code, Texte, Musik und Soundeffekte sind mit KI-Unterstützung (Claude) entstanden, die Detailfiguren und
  Monsterbilder mit SpriteCook (KI-Bildgenerator) – hier also ehrlich **„Yes“** angeben und die betroffenen Bereiche anhaken.
- **Custom noun:** leer lassen
- **Community:** Comments (empfohlen)
- **Visibility:** erst *Draft*, nach dem Test *Public*

## Aussehen der Seite („Edit theme“, passend zum Spiel)

- Background: `#0c0a1a` · Inner background: `#14123a`
- Text: `#f0f4ff` · Link / Button: `#ffe08a`
- Cover: `assets/itch-cover.png`, Screenshots aus `assets/itch-screenshots/` in der Reihenfolge 01 … 06

## Automatische Updates (butler)

Sobald die Seite existiert, lädt GitHub Actions jedes neue Release automatisch hoch
(Web-Version in den Kanal `html5`, APK in den Kanal `android`). Einmalig einrichten:

1. itch.io → **Settings → API keys → Generate new API key** (oder den Schlüssel von Piplosion weiterverwenden)
2. Im Terminal (Schlüssel einfügen, wenn danach gefragt wird):
   ```bash
   gh secret set BUTLER_API_KEY -R cleuenberg/crystal-worlds
   gh variable set ITCH_GAME -R cleuenberg/crystal-worlds --body "IHR-ITCH-NAME/crystal-worlds"
   ```
3. Nach dem ersten automatischen Upload in den Uploads einmal prüfen, dass die Web-Datei
   als „played in the browser“ markiert ist.
