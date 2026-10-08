# Card Game 2 — playtest builds

A roguelike deckbuilder with live head-to-head **Versus** matches. This repository only hosts **playtest builds**
(the game's source is private).

## Download
Get the latest Windows build from **[Releases](../../releases/latest)**: `CardGame2-<version>-windows.zip`.
Unzip it anywhere and run `CardGame2.exe`.

- Windows SmartScreen may say the publisher is unknown (the build isn't signed): click **More info** → **Run anyway**.
- Both players must use the **same version** (it's in the file name). Current: `2026-10-07-a670160`.

## Playing Versus with friends
No server to rent: one of you **hosts** (the match runs inside the host's game) and the other **joins**.

### One-time setup (both players)
1. Install the game (Windows: unzip the build and run `CardGame2.exe`).
2. Make sure you can reach each other. Easiest: **Tailscale** (free).
   - Each of you installs Tailscale (tailscale.com/download) and signs in.
   - The host invites the friend to their tailnet (or you both sign in with accounts on the same tailnet).
   - Tailscale gives every machine a `100.x.y.z` address; that's what the friend types in.
   - Alternatives: on the same Wi-Fi it just works (use the `192.168…`/`10…` address); or the host forwards TCP port
     **7777** on their router to their PC and shares their public IP (fiddly; doesn't work behind some ISPs).

### Each time you play
- **Host:** Main menu → **Versus** → enter your name → **Host Game**. The screen lists your addresses
  (the one marked *Tailscale* is the one to share over the internet). Windows may ask to allow the game through the
  firewall the first time: allow it (private networks is enough for Tailscale/LAN). Keep the game open.
- **Friend:** Main menu → **Versus** → enter your name, type the host's address in **Host / server address**
  (e.g. `100.101.102.103`) → **Find Match**.
- You're paired at once. Both shop at the same time, press Ready, battle each other, repeat until someone hits 0 HP.

### Good to know
- Both players need the **same version** of the game; a mismatch is refused with "please update the game".
- If the host quits or loses the connection, the match ends. If either player closes the game or presses Forfeit,
  the other wins.
- There are no timers yet: take your time, but don't walk away mid-match.

## Credits and licenses
Third-party assets, fonts and sounds are listed in [CREDITS.md](CREDITS.md); their licenses (and Godot Engine's) are in
[licenses/](licenses/). All rights to the game itself are reserved.
