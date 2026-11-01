# Crystal Worlds im Google Play Store – Store-Eintrag

Erst nach Piplosion. Standardsprache **Englisch (USA) – en-US**, dazu die Übersetzung **Deutsch – de-DE**
(Store-Eintrag → „Übersetzungen verwalten“ → eigene Übersetzungen hinzufügen).

Hinweis: Google Play erlaubt keine Verweise auf andere App-Stores – Zapstore/itch/APK daher hier nicht erwähnen.
Welt 5 und die Überraschung für die volle Sammlung bleiben unerwähnt.

## Grafiken

| Feld | Datei | Vorgabe |
|---|---|---|
| App-Symbol | `assets/icon.png` | 512 × 512 PNG, max. 1 MB |
| Vorstellungsgrafik | `assets/play-feature.png` (erzeugt mit `crystal-worlds/tools/store-art.mjs`) | 1024 × 500, PNG ohne Transparenz oder JPEG |
| Smartphone-Screenshots | `assets/itch-screenshots/01 … 06` | 2–8 Stück, Seitenverhältnis max. 2:1 – die 1080 × 2160-Bilder passen genau, der Zapstore-Satz (2280 px) ist zu hoch |
| Tablet-Screenshots | optional, leer lassen | |

Hochgeladen wird das App Bundle `crystal-worlds-X.Y.Z.aab` (Artefakt des GitHub-Builds, signiert mit dem Upload-Schlüssel).

## en-US (Standard)

**App-Name** (max. 30): `Crystal Worlds`

**Kurzbeschreibung** (max. 80):

```
Lead your party, seal monsters and win back the crystals – a tactical 16-bit RPG.
```

**Vollständige Beschreibung** (max. 4000):

```
Crystal Worlds is a tactical RPG in 16-bit style – with monsters to collect.

A shadow has scattered the five crystals that keep the worlds in balance. Lead Lian and friends across grid battlefields, from green plains through dark woods and fiery mountains to icy peaks – and beyond.

TACTICS
• Turn-based battles on a grid: terrain gives cover, elements decide the upper hand, the fast strike twice
• Danger zone shows where enemies and monsters can reach next turn
• Dark caves where only lamps and torches light the way
• Every world ends in a castle guarded by a boss

MONSTERS
• Weaken wild monsters and seal them – 15 species to collect
• Each one evolves through three stages
• Companions give their hero bonus stats, fight on their own and unleash co-op attacks
• Complete the collection for a special surprise

MORE
• Weapons and armour from chests and loot
• Battles are saved after every action
• Chiptune music and sound effects on an emulated 16-bit sound chip
• English and German

No ads, no in-app purchases, no tracking. Plays completely offline – your progress stays on your device.
```

## de-DE

**App-Name:** `Crystal Worlds`

**Kurzbeschreibung:**

```
Führe deine Truppe, banne Monster, hol die Kristalle zurück – Taktik-RPG in 16 Bit.
```

**Vollständige Beschreibung:**

```
Crystal Worlds ist ein Taktik-Rollenspiel im Stil der 16-Bit-Ära – mit Monstern zum Sammeln.

Ein Schatten hat die fünf Kristalle zerstreut, die die Welten im Gleichgewicht halten. Führe Lian und seine Gefährten über rasterförmige Schlachtfelder – von grünen Ebenen über finstere Wälder und feurige Berge bis zu eisigen Gipfeln und noch weiter.

TAKTIK
• Rundenkämpfe auf dem Raster: Gelände gibt Schutz, Elemente entscheiden über Vorteile, wer schneller ist, schlägt doppelt zu
• Die Gefahrenzone zeigt, wohin Gegner und Monster im nächsten Zug reichen
• Dunkle Höhlen, in denen nur Lampen und Fackeln den Weg erhellen
• Am Ende jeder Welt wartet eine Burg mit einem Boss

MONSTER
• Schwäche wilde Monster und banne sie – 15 Arten zum Sammeln
• Jedes entwickelt sich in drei Stufen
• Begleiter geben ihrer Figur Bonuswerte, kämpfen allein und lösen Ko-Op-Angriffe aus
• Wer die Sammlung vervollständigt, erlebt eine besondere Überraschung

AUSSERDEM
• Waffen und Rüstungen aus Truhen und Beute
• Der Kampf wird nach jeder Aktion gesichert
• Chiptune-Musik und Soundeffekte auf einem emulierten 16-Bit-Soundchip
• Deutsch und Englisch

Keine Werbung, keine In-App-Käufe, kein Tracking. Läuft komplett offline – dein Spielstand bleibt auf deinem Gerät.
```

## Datensicherheit (App-Inhalte)

- **Werden Nutzerdaten erhoben oder geteilt?** Nein. Das Spiel speichert den Spielstand nur lokal auf dem Gerät
  und hat keine Server-Verbindung (die Berechtigung INTERNET bringt die Capacitor-Hülle mit; genutzt wird sie nur
  für die Links zu Impressum und Datenschutz, die im Browser öffnen).
- **Werbung:** Nein · **Zielgruppe (Vorschlag):** ab 13 (Kampfdarstellung im Comic-Stil, kein Blut)
- **Altersfreigabe (IARC-Fragebogen):** Gewalt – Fantasy-Gewalt gegen Fantasiefiguren, nicht realistisch

## Kontaktdaten (Store-Einstellungen)

- **E-Mail:** Pflicht, wird öffentlich angezeigt – am besten eine Projekt-/Support-Adresse
- **Website:** `https://crystalworlds.tvir.games`
- **Datenschutzerklärung:** `https://tvir.games/datenschutz.html`
