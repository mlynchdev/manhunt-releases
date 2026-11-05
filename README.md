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

The game is played on a server run by whoever invited you; ask them for its address. In the game,
enter that address, the port (2456 unless told otherwise) and your name, then **Join**. Everyone must
use the same release as the server.

Each match is two rounds. One team hunts while the other runs, then they swap. Hunters tag Runners
(E or left click; the crosshair turns green when a tag will land); tagged Runners are frozen. Hunters win
a round by catching every Runner, Runners by keeping anyone free until time runs out.

## Checking a download

Each release lists SHA-256 checksums in `SHA256SUMS`. On macOS or Linux: `shasum -a 256 -c SHA256SUMS`.

## Status

Early alpha for playtesting with friends. No accounts, no data collected: the game only talks to the
server you join.
