# Card Game 2 — playtest builds

A roguelike deckbuilder with live head-to-head **Versus** matches. This repository only hosts **playtest builds**
(the game's source is private).

## Download
Get the latest build from **[Releases](../../releases/latest)**:
- **Windows:** `CardGame2-<version>-windows.zip`. Unzip it anywhere and run `CardGame2.exe`. SmartScreen may say the
  publisher is unknown (the build isn't signed): click **More info** → **Run anyway**.
- **Linux:** `CardGame2-<version>-linux.tar.gz`. Extract it and run `CardGame2.x86_64`.

Both players must use the **same version** (it's in the file name). Current: `2026-10-08-2b39635`.

## Playing Versus with friends
No server to rent: one of you **hosts** (the match runs inside the host's game) and the other **joins**.

### One-time setup
1. Both players: install the game (Windows: unzip the build and run `CardGame2.exe`; Linux: extract it and run
   `CardGame2.x86_64`).
2. The **host** forwards **TCP port 7777** on their router to their PC (look for "port forwarding" in the router's
   settings; give the PC a fixed local address so the rule keeps working). Then they look up their **public IP**
   (search "what is my IP"). That's the address the friend types in.
   - On the same Wi-Fi / network you don't need any of this: use the host's local address (`192.168…` or `10…`),
     which the Host screen shows.
   - Some ISPs put customers behind shared addresses (CGNAT), where port forwarding can't work. If friends can't
     connect even with the rule in place, ask the ISP for a public IP, or let the other player host.

### Each time you play
- **Host:** Main menu → **Versus** → enter your name → **Host Game**. The screen shows your local addresses and the
  port. Windows may ask to allow the game through the firewall the first time: allow it (tick both private and
  public networks, or the connection from outside is blocked). Keep the game open.
- **Friend:** Main menu → **Versus** → enter your name, type the host's public IP in **Host / server address**
  (e.g. `203.0.113.25`; add `:port` only if the host changed it from 7777) → **Find Match**.
- You're paired at once. Both shop at the same time, press Ready, battle each other, repeat until someone hits 0 HP.

### Good to know
- Both players need the **same version** of the game; a mismatch is refused with "please update the game".
- **Timers:** 90 seconds to shop and 60 seconds to plan each battle turn (a little extra after each battle's
  animations). The clock at the top shows what's left. When the shop timer runs out you go to battle with what you
  have. When the turn timer runs out, the cards you've already placed are played.
- **Lost connection (the joining player):** the game reconnects by itself. If your game crashed or you closed it,
  start it again, go to **Versus** and press **Rejoin your match**. You have **60 seconds**. Meanwhile your turns pass
  empty and your shop is skipped, and after that you forfeit. Your friend sees a countdown.
- If the **host** quits or loses the connection, the match ends (the match runs inside the host's game).
- **Forfeit** (press it twice) gives the match to the other player.

## Credits and licenses
Third-party assets, fonts and sounds are listed in [CREDITS.md](CREDITS.md); their licenses (and Godot Engine's) are in
[licenses/](licenses/). All rights to the game itself are reserved.
