# CompanionClaude

A Fallout 4 companion mod built with [Mutagen](https://github.com/Mutagen-Modding/Mutagen) 0.52.0.

## Project Status: Help Wanted

This project generates an ESP file programmatically for a custom companion NPC with full dialogue scenes. Currently experiencing persistent issues with:

- **Friendship greeting "bounces"** - Dialog closes immediately when clicked in Creation Kit
- **Scene Quest links** - Full 8-slot PlayerDialogue actions cause "parent quest 00000000" errors
- **Voice file mapping** - Some mappings work, others don't

## What Works

- NPC creation with proper factions
- Pickup/Dismiss scenes with voice
- Basic scene structure

## What Doesn't Work

- Friendship greeting (bounces in CK)
- Full 8-slot Admiration scene (Quest link corrupts)
- Various edge cases in dialogue flow

## Tech Stack

- .NET 10.0
- Mutagen.Bethesda.Fallout4 v0.52.0
- Fallout 4 Creation Kit

## Building

```bash
cd CompanionClaude_v13_GreetingFix
dotnet build
dotnet run
```

Outputs ESP to: `Fallout 4\Data\CompanionClaude.esp`

## Help Needed

If you have experience with:
- Mutagen scene/dialogue creation
- Fallout 4 companion quest structure
- Creation Kit dialogue debugging

Please open an issue or PR. The codebase includes extensive documentation in `/docs`.

## Reference

Based on reverse-engineering Piper's companion quest (COMPiper) from Fallout4.esm.
