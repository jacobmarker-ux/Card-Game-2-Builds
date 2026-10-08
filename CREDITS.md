# Credits

Card Game 2 uses the following third-party assets. Each pack's original license file is kept next to it as
`assets/third_party/<pack>/LICENSE.txt`. Packs are imported with `tools/import_assets.py` (see `docs/ASSETS.md`).

> **This repository is private, and must stay private as long as it contains non-CC0 packs.** Assets under the
> Quaternius Asset License (QAL), currently `quaternius_bestiary/`, must not be published as raw files. Before this repo
> ever goes public, remove `_incoming/` (it's git-ignored, but check) and every non-CC0 pack **from the entire git
> history** (e.g. with `git filter-repo --path assets/third_party/quaternius_bestiary --invert-paths`), not just from
> the latest commit. Shipping these assets inside a built game is allowed.

## 3D models

### KayKit — Kay Lousberg (www.kaylousberg.com) · CC0 1.0
- **Dungeon Pack 1.1** — `assets/third_party/kaykit_dungeon/`
- **Forest Nature Pack 1.0** — `assets/third_party/kaykit_forest_nature/`
- **Adventurers Character Pack 2.0** — `assets/third_party/kaykit_adventurers/`
- **Skeletons Character Pack 1.1** — `assets/third_party/kaykit_skeletons/`

### Quaternius (quaternius.com)
- **Medieval Village MegaKit (Standard)** — CC0 1.0 — `assets/third_party/quaternius_medieval_village/`
- **Fantasy Props MegaKit (Standard)** — CC0 1.0 — `assets/third_party/quaternius_fantasy_props/`
- **Stylized Nature MegaKit (Standard)** — CC0 1.0 — `assets/third_party/quaternius_stylized_nature/`
- **3D Card Kit – Fantasy (Standard)** — CC0 1.0 — `assets/third_party/quaternius_card_kit/`
- **Modular Character Outfits – Fantasy (Standard)** — CC0 1.0 — `assets/third_party/quaternius_outfits/` (textures downscaled to 1024²)
- **Universal Base Characters (Standard)** — CC0 1.0 — `assets/third_party/quaternius_base_characters/` (textures downscaled to 1024²)
- **Dinosaur Animated Pack** — CC0 1.0 — `assets/third_party/quaternius_dinosaurs/`
- **LowPoly Animated Monsters** — CC0 1.0 (as listed at https://quaternius.itch.io/lowpoly-animated-monsters; the
  download has no license file) — `assets/third_party/quaternius_monsters/`
- **LowPoly Animated Animals** — CC0 1.0 (as listed at https://quaternius.itch.io/lowpoly-animated-animals; the
  download has no license file) — `assets/third_party/quaternius_farm_animals/`
- **Bestiary – Dungeon Monsters Kit (Standard)** — Quaternius Asset License (QAL) v1.0 —
  `assets/third_party/quaternius_bestiary/`. Free for commercial use, no credit required. **Not CC0:** the
  raw assets may not be redistributed *as assets*. Shipping them inside the game is fine, but don't publish this
  folder (e.g. a public repo or an asset dump) without checking the license.

## Sound effects and particles

### Kenney (www.kenney.nl) · CC0 1.0
- **Casino Audio 1.1** — `assets/third_party/kenney_casino_audio/`
- **Impact Sounds 1.0** — `assets/third_party/kenney_impact_sounds/`
- **Interface Sounds 1.0** — `assets/third_party/kenney_interface_sounds/`
- **RPG Audio** — `assets/third_party/kenney_rpg_audio/`
- **Particle Pack** — `assets/third_party/kenney_particle_pack/` (transparent PNG sprites)
- **Nature Kit 2.1** — `assets/third_party/kenney_nature_kit/` (GLB models; battlegrounds, P3)
- **Castle Kit 2.0** — `assets/third_party/kenney_castle_kit/` (GLB models; battlegrounds, P3)

## Fonts

### Google Fonts · SIL Open Font License 1.1 (https://openfontlicense.org)
- **Cinzel** — The Cinzel Project Authors (https://github.com/NDISCOVER/Cinzel) — `assets/third_party/font_cinzel/` (titles, buttons, card names)
- **Alegreya Sans** — The Alegreya Sans Project Authors (Juan Pablo del Peral, Huerta Tipográfica) — `assets/third_party/font_alegreya_sans/` (body text)

## Icons

### game-icons.net · CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/)
`assets/third_party/game_icons/<author>/<icon>.svg` (white on transparent).
- Icons made by **Delapouite** (https://delapouite.com): anticlockwise-rotation, check-mark, exit-door, fast-forward-button, info, move, player-next, rolling-dices, shop, sound-on, stack, two-coins, upgrade
- Icons made by **Faithtoken** (http://fungustoken.deviantart.com): card-discard, card-draw
- Icons made by **Lorc** (http://lorcblog.blogspot.com): anvil-impact, aura, bleeding-wound, broken-shield, cog, crossed-swords, crown, crystal-ball, dead-wood, energise, fist, holy-symbol, hourglass, laurel-crown, magic-swirl, poker-hand, portal, power-lightning, rune-stone, scales, semi-closed-eye, skull-crack, snowflake-1, sprout
- Icons made by **Sbed** (http://opengameart.org/content/95-game-icons): cancel

This list must stay in sync with `ICONS` in `tools/import_assets.py`. The in-game credits screen (M7) should
show this file's icon section.
