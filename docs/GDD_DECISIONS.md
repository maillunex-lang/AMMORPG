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

## CHAR-RIG-001 (APPROVED 2026-11-22)
- Option B: All playable characters, NPCs, and ordinary enemies are humanoid and suitable for Meshy AI rigging; rare bosses may have non-humanoid anatomy.
- Production constraint: prefer two arms, two legs, head and torso; A-pose/T-pose; shared skeleton conventions where possible. Retargeting and Godot import must be tested, not assumed.
- Applies to GDD-02 races, GDD-06 animations, GDD-10 enemies/bosses, and Android performance planning.
- GDD-02 lore/races/factions/war decisions remain UNAPPROVED; no implementation authorized.

## GDD-02: World history, races, factions (APPROVED 2026-11-22)
- LORE-001 A: Shattered ancient empire; successor kingdoms contest its legacy. No additional canon about causes or geography is approved yet.
- RACE-001 C: Four classic humanoid races plus two original humanoid races. Exact names, looks, cultures, and stat bonuses pending separate design.
- FACTION-001 D: Three major powers plus independent cities and organizations. Names, memberships, capitals, and politics pending.
- WAR-001 C: Faction wars plus clan wars, including territory/castle conflict. Exact rules pending GDD-12.
- CHAR-RIG-001 B remains binding: playable races, NPCs and ordinary enemies are humanoid for Meshy AI rigging; rare bosses may differ.
- These are GDD approvals, not authorization to install third-party software.

## GDD-02 GitHub research candidates (PENDING SEPARATE OWNER APPROVAL)
- GH-004 nathanhoad/godot_dialogue_manager — branching dialogue editor/runtime; MIT; v4 for Godot 4.6+, v3 for older 4.x. Proposed editor-only dialogue content + client presentation, no authoritative state mutations.
- GH-005 shomykohai/quest-system — Godot 4.4+ modular quest definitions; MIT; proposed data/content authoring, with server-authoritative quest progress/rewards.
- GH-006 bitbrain/beehave — Godot 4 behavior trees, MIT; proposed NPC prototype and AI reference, production server behavior to be separately designed.
- GH-007 limbonaut/limboai — C++ behavior trees and state machines, MIT; candidate for comparative study only; Android/native binary and maintenance burden must be assessed.
- Faction reputation and diplomacy: custom authoritative server domain model proposed; no sufficiently validated plug-and-play MMORPG solution found.
- Older godot-addons/godot-quest-system targets Godot 3 and is rejected as a direct Godot 4 dependency.
No GH-004–GH-007 components installed.

## GDD-02 GitHub candidate decisions (APPROVED 2026-11-22)
- GH-004 Dialogue Manager: TEST. Isolated prototype permitted; no main-game integration.
- GH-005 QuestSystem: TEST. Isolated prototype permitted; no main-game integration.
- GH-006 Beehave: TEST. Isolated prototype permitted; no main-game integration.
- GH-007 LimboAI: REJECT. Do not install, prototype, or integrate.
- Prototype tests must verify actual Godot compatibility, basic function, and Android constraints before recommending production use. No server-authoritative quest, dialogue, or AI logic is delegated to clients.
