# AMMORPG — ROADMAP

## Status
- GDD-01 Core concept: APPROVED; GH-001 Terrain3D isolated Android test AUTHORIZED (not yet executed); GH-002 deferred to GDD-13; GH-003 read-only study AUTHORIZED.
- GDD-02: DESIGN IN PROGRESS, not approved. CHAR-RIG-001 B approved as cross-stage Meshy AI production constraint. GDD-03 through GDD-20: NOT STARTED.
- Gameplay code: NOT STARTED.

## GDD stages
1. [x] Concept, world, visual style, scale (GDD-01)
2. [ ] World history, races, factions
3. [ ] Classes and character creation
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

## Cross-stage constraints
- [x] CHAR-RIG-001 B: humanoid playable characters, NPCs and ordinary enemies; rare bosses may differ. Meshy AI rigging workflow; validate skeleton compatibility and animation retargeting in Godot.
- [ ] Apply to GDD-02, GDD-06 and GDD-10.

## Next actions
- Execute GH-001 isolated Android compatibility/FPS/memory test when a runnable Godot Android environment is available; do not merge into main game without new approval.
- Perform GH-003 architecture review; no code integration.
- Present GDD-02 choices (world history, races, factions); do not implement dependencies before approval.
