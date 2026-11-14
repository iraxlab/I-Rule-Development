# Canon and open decisions

The single page that says what is **locked**, what the source documents **disagreed about** and how this repo resolved it, and what is still **open**.

## Locked canon (do not change without owner approval)
| # | Canon |
|---|---|
| 1 | **Elias is 21.** No decades-of-betrayal backstory. Chosen for capacity to align, not suffering. |
| 2 | **Enemies are symbolic forces**: Glass Shadows, Storm Wraiths, Burn Knights, Ember Leeches. Never specific people. |
| 3 | **No religious framing.** Companions are named by function. |
| 4 | **Engine: Unreal Engine 5.** Never Unity. |
| 5 | Companions: **Cinder** (guidance), **Fire Dragon** (guardian / trial), **Fire Eye** (world-level system), **Sacred Arc** (fire-arrow system). |
| 6 | World: **broken floating islands joined by fixed bridges.** Ruins, not a city. No skyscrapers, no glass. |
| 7 | Six-line sky ladder: **straight horizontal bars**, evenly spaced, ignite bottom to top. Never star, circle or pyramid. |
| 8 | Palette: warm gold-amber, bronze, obsidian. |
| 9 | **Stillness hold times:** S1 2.5 s, S2 3 s, S3 4 s, S4 3 s, S5 5 s, S6 **10 s**. |
| 10 | Closing stats: **75-95 minutes / 6 lines / 1 journey.** |
| 11 | No HUD, no minimap, no quest markers, no text tutorials. |
| 12 | The ending has **no boss and no explosion.** |
| 13 | The Throne: dark volcanic stone and bronze, about 40 m, six horizontal fissures, dragon ribs, staircase with braziers. See [The Throne](08-the-throne.md). |
| 14 | Tone: mythic but restrained. Confident, not mystical-overwrought. |
| 15 | Funding ask: $25,000-$50,000 (concept to first playable). |

## Conflicts found and how this repo resolved them

| Topic | Sources disagreed | Resolution here |
|---|---|---|
| **Sacred Arc** | The GDD and key art use "The Sacred Arc"; the pitch brief says no Sacred Arc, describe the fire system functionally | Kept as the **name** of the fire-arrow system (it is in the approved key art). "Sacred" carries no religious meaning. |
| **Stage names** | GDD / key art: Lurking, Emerging, The Toil, The Leap, Flying, The Peak. Brief / spec: Entering the Dark, Finding Direction, The Trial of Force, Shared Fire, Flight, The Still Peak | Use the **key-art names** as primary; the longer names are subtitles. |
| **Demo length and scope** | GDD: 15-20 min. Brief: Stages 1-3, 30-40 min. Spec: 20-22 min (Core Proof B) or 25-30 min (Compressed Six) | **Open.** All options listed in the [production plan](11-production-plan.md). |
| **Game length** | GDD stage sums vs timeline | Use **85:00** first-time golden path (75-95 min range). |
| **World wording** | Older docs say "floating obsidian islands", spec says "single sky-desert biome" | Use "broken floating islands joined by bridges". Obsidian is a **material**, not the whole look (sandstone-tan and charcoal-brown rock dominate the key art). |
| **Dragon appearance** | Present from Stage 3 (GDD / spec); "after Stage 3" (spec profile) | First glimpsed overhead at the end of Stage 3; interacts from Stage 4 only when aligned. |
| **Stage 4 name and mechanic** | "Shared Fire" (coordination) vs "The Leap" (bridges form under calm movement) | Same stage. Mechanic: bridges form only while still. |
| **Budget** | Slice $150-300k, full $400-800k vs grant ask $25-50k | Not a conflict: the grant covers concept to first playable Stage 1 only. |
| **Engine in spec** | The long spec was written Unity-style (ScriptableObjects, C#) | Translated to Unreal in [architecture](10-unreal-architecture.md). |

### Technical spec variants
The spec contains two threshold models for the Creative Energy Cycle:
1. **ForcingIndex model** (single meter, thresholds 0.62 / 0.28, 0.75 s hold). **Used as the baseline** in [core systems](06-core-systems.md).
2. **forcingScore / alignmentScore model** with hysteresis: enter Entropy at forcingScore >= 0.65 for 1.2 s, exit at <= 0.52 for 1.5 s with stillness >= 0.6 s; enter Freshness at alignmentScore >= 0.45 for 1.5 s, exit at <= 0.32 for 1.2 s; enter Beauty at alignmentScore >= 0.70 for 2.0 s and forcingScore <= 0.25, exit at forcingScore >= 0.35 or alignmentScore <= 0.55. `alignmentScore = wS * stillnessNormalized + wP * perfectActionScore - 0.35 * forcingScore`. Keep as the alternative if the single-meter model proves too twitchy in playtests.

## Open decisions (need an owner)
| # | Decision | Needed for | Options |
|---|---|---|---|
| 1 | **Demo scope** | Steam demo plan | See [production plan](11-production-plan.md) |
| 2 | **Fire Eye redesign ("Iris of Plates")** | Art | Keep approved render, or adopt the redesign |
| 3 | **Fire Dragon redesign ("River of Fire")** | Art | Keep approved render, or adopt the redesign |
| 4 | **Community benefit answer** for MegaGrants | Application | Open source part / share learnings / release a tool or plugin / combination |
| 5 | **Verticality** | Level design | Adopt the "whole game is a climb" recommendation in [world design](03-world-and-level-design.md) |
| 6 | **New Throne renders** | Art, deck | Generate with the prompts in [Throne Wow Direction](../design/Throne_Wow_Direction.pdf) |
| 7 | **Page 23 moderation** | Art | Capture the exact Freepik rejection message if it recurs |
| 8 | **Media link / trailer** | Application | Assemble the pitch deck or cut a short animatic |
| 9 | **License** | Repository | Choose before opening the repo publicly |
| 11 | **Stage 1 encounter and Stillness Duel** | Gameplay, level design | Approve the proposed Arms, Still Ring and mind-vision duel in [Playthrough](17-playthrough-start-to-throne.md#11-decisions-needed-from-the-project-owner) |
| 10 | **Cover art regeneration** | Art, deck | The current cover shows six bars of increasing width (a pyramid shape). Regenerate with equal-width bars using [cover-regeneration prompt](../prompts/cover-regeneration.md) |

## Known issues in the assembled pitch deck (audit, not yet fixed)
- Stage 6 hold shown as 6 s; canon is **10 s** (6 s is demo-only).
- World Structure text conflicts with the broken-islands canon.
- A box labelled "FIRE EYE" on page 3 is mislabeled.
- Demo length is stated inconsistently.
- Several layout and readability problems.

## Superseded files (do not use)
| File | Replaced by |
|---|---|
| Master GDD (earlier) | [GDD](../design/GDD_Legend_and_Game_Design.pdf) |
| Art Prompt Library (14 prompts) | [Key art prompts](../prompts/key-art-prompts.md) |
| Full Scope page prompts (21, pre-fix) | [Key art prompts](../prompts/key-art-prompts.md) |
| Presentation script (25 slides) | [Pitch deck brief](../design/Pitch_Deck_Master_Brief.pdf) |
| "Throne of Fire" and "Throne of Stillness" (mirror / rods) designs | [The Throne](08-the-throne.md) |
