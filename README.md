# FGH-FPS — Multiplayer FPS (A-Level Computer Science project)

A lightweight online multiplayer first-person shooter built in **Unity (C#)** with
**Photon PUN 2** for networking. I built it for my OCR A-Level Computer Science
coursework. The brief I set was a multiplayer game that could run within school
network restrictions and still be easy for several players to join.

**Status (23 Sep 2026): complete. Kept as a portfolio piece.** The project scored
**86% overall**. I learned Unity and C# independently to build it. It was made in
2022 and has not been changed since. In September 2026 the repo was cleaned up so it
holds only the project source (see below).

## What's in the game

- A main menu and lobby: create or join rooms (`Launcher`, `RoomButton`).
- Two playable maps, plus a movement-testing scene.
- First-person movement, shooting and weapon handling (`PlayerController`, `Gun`).
- Networked spawning and respawning (`SpawnManager`, `PlayerSpawner`).
- Match flow and a live leaderboard (`MatchManager`, `LeaderboardPlayer`, `UIController`).

## Structure

```
FGH-FPS/
├── Assets/
│   ├── Scripts/        # the game code (10 C# scripts)
│   ├── Scenes/         # Main Menu, Map 1, Map 2, Movement Testing
│   ├── Prefabs/, Materials/, Resources/
│   ├── Photon/         # Photon PUN 2 (third-party networking)
│   ├── TextMesh Pro/   # Unity text rendering (third-party)
│   └── …               # plus an imported third-party art/asset pack
├── Packages/           # Unity package manifest
└── ProjectSettings/    # Unity project settings (Unity 2020.3.36f1)
```

## Opening it

1. Install **Unity 2020.3.36f1** (LTS) with Unity Hub.
2. Open the folder as a project. Unity rebuilds `Library/` and the IDE project
   files on first open, which takes a few minutes.
3. Add your own Photon App ID under *Window → Photon Unity Networking → Highlight
   Server Settings*, then play from the **Main Menu** scene.

**Technologies:** Unity, C#, Photon PUN 2, object-oriented programming.
