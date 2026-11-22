# AMMORPG — GDD Decisions

## GDD-01: Core concept (APPROVED 2026-11-22)

- WORLD-001: C — Hybrid inspired by WoW and Lineage 2: colorful fantasy adventures, serious clan politics and conflict, original intellectual property.
- GAME-001: C — PvE + PvP hybrid: quests, exploration, dungeons, guilds, open-world conflicts and sieges.
- VIS-001: A — Stylized Fantasy 3D, Android-first performance.
- SCALE-001: C — Hybrid world: large open regions, transitions between continents, separate dungeon instances.

All four decisions are approved by the project owner. No third-party code or plugins may be integrated without separate approval.

## Approval workflow
1. Present GDD options and recommendation.
2. Obtain explicit owner approval.
3. Search GitHub deeply for relevant original projects and alternatives; assess licenses, maintenance, Godot compatibility, Android builds, performance and security.
4. Present specific proposals with integration/adaptation scope and risks.
5. Obtain separate approval before implementing third-party code.
6. Record decisions and update ROADMAP after each stage.

## GDD-01 GitHub candidates (OWNER DECISIONS 2026-11-22)
- GH-001 Terrain3D: TEST APPROVED ONLY in isolated prototype; validate Android GDExtension binaries, FPS and memory; no integration into main game authorized. https://github.com/TokisanGames/Terrain3D
- GH-002 Inventory System: LATER, defer to GDD-13. https://github.com/expressobits/inventory-system
- GH-003 Legends MMO: STUDY ONLY, architectural reference, no code integration. https://github.com/voullume/legends-mmo
No dependencies have been installed. GDD-02 design is pending owner approval.
