# AMMORPG — ROADMAP

## Status
- GDD-01 Core concept: APPROVED; GH-001 Terrain3D isolated Android test AUTHORIZED (not yet executed); GH-002 deferred to GDD-13; GH-003 read-only study AUTHORIZED.
- GDD-02: DESIGN IN PROGRESS, not approved. CHAR-RIG-001 B approved as cross-stage Meshy AI production constraint. GDD-03 APPROVED; GDD-04 through GDD-20 NOT STARTED.
- Gameplay code: NOT STARTED.

## GDD stages
1. [x] Concept, world, visual style, scale (GDD-01)
2. [x] World history, races, factions
3. [x] Classes and character creation
4. [ ] Stats, levels, talents
5. [ ] Combat and controls
6. [ ] Abilities, VFX, animations
7. [ ] Geography, regions, open world
8. [ ] Cities, settlements, NPCs
9. [ ] Quests, story, dialogue
10. [ ] Monsters, AI, world bosses
11. [ ] Dungeons, raids, parties
12. [ ] PvP, arenas, sieges
13. [ ] Items, equipment, loot
14. [ ] Economy, professions, trade
15. [ ] Guilds and social systems
16. [ ] Mounts, pets, transport
17. [ ] Server, networking, database
18. [ ] Android UI, graphics, optimization
19. [ ] Monetization, anti-cheat, admin
20. [ ] MVP, QA, RuStore release

## Editor-first requirements
- [x] EDITOR-001: desktop Godot visual UI editing, one .tscn per screen, reusable themes, responsive layout and offline preview.
- [x] EDITOR-002: desktop Godot visual region editing with modular scenes, reusable props and spawn/interaction markers.
- [ ] Design and validate scene-to-server content export/versioning and authoritative world-state boundaries.
- [ ] Evaluate editor tooling/plugins separately; no third-party integration without approval.

## Cross-stage constraints
- [x] CHAR-RIG-001 B: humanoid playable characters, NPCs and ordinary enemies; rare bosses may differ. Meshy AI rigging workflow; validate skeleton compatibility and animation retargeting in Godot.
- [ ] Apply to GDD-02, GDD-06 and GDD-10.

## GDD-02 GitHub research
- [x] GH-004 Dialogue Manager: isolated test approved; execution pending.
- [x] GH-005 QuestSystem: isolated test approved; execution pending.
- [x] GH-006 Beehave: isolated test approved; execution pending.
- [x] GH-007 LimboAI: rejected; do not use.
- [ ] Design faction reputation/diplomacy as custom authoritative server subsystem.
- [ ] Execute three isolated tests and document evidence/results; do not integrate into main game.
- [x] Owner decisions recorded for GH-004–GH-007.

## Next actions
- Execute GH-001 isolated Android compatibility/FPS/memory test when a runnable Godot Android environment is available; do not merge into main game without new approval.
- Perform GH-003 architecture review; no code integration.
- Begin GDD-03 classes and character creation design; do not implement dependencies before approval.

## GDD-03 approvals and research
- [x] CLASS-001 C: 8 classes; SPEC-001 C: 3 specializations/class; COMBAT-ROLE-001 B: tank/healer/damage/support; CHAR-CREATE-001 D: preset looks/cosmetics.
- [x] GitHub research completed; candidates GH-008–GH-012 documented in GDD_DECISIONS.md.
- [ ] GH-008 ability system isolated test, subject to separate approval.
- [ ] GH-009 Meshy animation library retargeting isolated test, subject to separate approval and licensing review.
- [ ] GH-010 native Godot SkeletonProfileHumanoid/BoneMap isolated test, subject to separate approval.
- [ ] GH-011 gameplay systems architecture review, subject to separate approval.
- [ ] GH-012 character customizer: no code reuse due to all-rights-reserved license and mismatch with preset looks.
- [ ] Complete previously approved isolated GH-004/005/006 tests and record evidence.
- [ ] GDD-04 stats, levels and talents design.
