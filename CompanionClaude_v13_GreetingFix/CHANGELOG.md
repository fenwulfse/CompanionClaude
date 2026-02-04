# CompanionClaude v14 - Reverted to AlmostBack + Voice Mappings

**Date:** 2026-02-04
**Based on:** AlmostBack/Program (3).cs + Friendship/Admiration voice mappings

## Changes in v14
- **Reverted to Working Code:** Full 8-slot Admiration scene broke CK with "parent quest 00000000" error
- **Kept Simple Admiration Scene:** 6-phase, 3 exchanges (2-slot pattern)
- **Added Friendship Voice Coverage:** 21 NPC + 16 Player mappings
- **Added Admiration Voice Coverage:** 2 NPC + 3 Player mappings (simplified pattern)

## Voice Coverage
- Pickup Scene: 8 NPC + 4 Player
- Dismiss Scene: 7 NPC + 4 Player
- Friendship Scene: 19 NPC (2 missing) + 16 Player
- Admiration Scene: 2 NPC + 3 Player (simplified 2-slot)

**Total: 87 voice files**

## Known Issues
- Friendship greeting "bounces" in CK (to be troubleshot later)
- 2 silent NPC slots in Friendship (165940, 1658F9)
- 1 missing player pickup neutral (212B77)
- Admiration uses simplified 2-slot pattern (not full 8-slot)

## Scenes Included
- Pickup (voiced)
- Dismiss (voiced)
- Friendship (voiced) - greeting bounces, scene works
- Admiration (partial voice - simplified pattern)
- Confidant (scene only)
- Infatuation (scene only)
- Disdain (scene only)
- Hatred (scene only)
- Recovery (scene only)
- Murder (scene only)

## Test in CK
1. Load CompanionClaude.esp
2. Find COMClaude quest
3. Verify Admiration scene loads without errors
4. Check Friendship/Admiration scene actions for voice
