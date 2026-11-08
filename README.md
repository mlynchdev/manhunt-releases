# Manhunt

A team-based 3D multiplayer chase-and-tag game: Hunters vs Runners, two teams of 3–4.
This repository only hosts the game's downloads; there is no source code here.

**[Download the latest release](https://github.com/mlynchdev/manhunt-releases/releases/latest)**

| Platform | File | Notes |
|---|---|---|
| macOS 11+ (Apple silicon and Intel) | `Manhunt-<version>-macos.zip` | signed and notarized by Apple: unzip, move to Applications, open |
| Windows 10/11 (64-bit) | `Manhunt-<version>-windows-x86_64.zip` | unzip and run `Manhunt.exe`. Not code-signed yet: SmartScreen asks first, choose *More info → Run anyway* |
| Linux (x86-64, with Vulkan drivers) | `Manhunt-<version>-linux-x86_64.tar.gz` | `tar -xzf` it, then `./Manhunt.x86_64` |

Keep everything in the unpacked folder together. `PLAYING.txt` inside explains joining and the controls.

## Playing

The main menu fills in the public server's address (45.63.94.202, port 2456): type your name and press
**Join**. **Public 1v1 server**, **Public 2v2 server** and **Public 3v3 server** join the one-on-one, two-a-side and three-a-side servers on the same address (ports 2457, 2458 and 2459). To play on someone else's server, type the address and port they gave you instead. Everyone
must use a release that speaks the same network protocol as the server.

Each match is best of three rounds. One team hunts while the other runs, then they swap; at 1–1 a coin toss
picks the Hunters for the deciding round. Hunters tag Runners (E or left click; the crosshair turns green when a
tag will land) and walk them to jail, where a free teammate can tag them out. Hunters win a round by catching
every Runner, Runners by keeping anyone free until time runs out. Every round starts with both teams at the base,
and the Runners get a 15-second head start at four times their speed while the Hunters wait.

## Checking a download

Each release lists SHA-256 checksums in `SHA256SUMS`. On macOS or Linux: `shasum -a 256 -c SHA256SUMS`.

## Status

Early alpha for playtesting with friends. No accounts, no data collected: the game talks to the server you join
and, from 0.11.0, asks GitHub once at startup whether a newer release is out (it sends only the game's version;
turn it off under Options → *Check for updates*). When one is, the main menu shows a button that opens its download page.
