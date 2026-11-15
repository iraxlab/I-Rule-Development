# Alignment and win check

> **STATUS:** run on 15 November 2026, after ENV-08 was filed. Every check below was run against the files, not from memory.

## 1. What changed in this pass
1. **ENV-08 Canyon Cliffs is in.** 11 pictures are filed: a sheet, front, back, top, underside and details 1 to 5.
2. **The pictures show five rock masses, not four.** The doc, the three blueprint sheets, the prompts and the data now follow the pictures. The old four-cliff doc is in `docs/archive/31-env08-blueprint-4cliff-OLD.md`.
3. **The long bridge is decided.** The pictures drew it, and it gives Stage 4 a real choice (see section 2).
4. **The sheet is composed** from the four accepted views. The Gemini sheet showed only two cliffs per view and is in `_superseded`.
5. **One back picture was dropped.** It had a confused run of chains and is in `_superseded`.

## 2. ENV-08 as it now stands
| Part | What it is |
|---|---|
| West Cliff | Arrival. Three black needles. Calm pocket. |
| South shelf | After bridge 1 (20 m). Calm pocket. |
| Middle shelf | After bridge 2 (26 m, the Dragon holds it 5 s). Calm pocket. |
| North shelf | After the Spine (21 m, two Glass Shadows). Calm pocket. |
| East Cliff | After bridge 3 (20 m, leeches). Column, 3 s hold, launch lip. |
| Long bridge | West Cliff to North shelf, 72 m, 6 s to build, leeches below. Skips the Middle shelf and the Spine. |

**The choice:** the near way teaches and helps (bridge 1, the Dragon, the fight). The long bridge is for players who trust their stillness. Its reward is a calmer wind on bridge 3.

**Not drawn in the pictures:** bridge 1. Build it from Sheet A. Other small differences are in doc 31, section 11.

## 3. What was checked and what was fixed
| Check | Result | Fix |
|---|---|---|
| Every picture on disk has a prompt | Pass, 76 assets, no view without a prompt | none |
| Every asset ID used in docs exists | Pass | none |
| Hold times S1 2.5 s, S2 3 s, S3 4 s, S4 3 s, S5 5 s, S6 10 s | Same in all six stage pages | none |
| Stage times add up | **Failed.** Stage 6 beats ran 70:00 to 76:00 and the ending 76:00 to 85:00, but the targets say 9:00 and 6:00 | Stage 6 now runs 70:00 to 79:00 and the ending 79:00 to 85:00. The ending now follows the 360 s budget in doc 06. The 48 beat labels in the playthrough prompts were moved to match |
| Line 6 lights at 79:00 | **Failed.** Stage 6 says 77:00 | Doc 27 now says 77:00 |
| Stage 4 order | **Failed.** The Spine fight came before the Dragon bridge, but the layout puts the Spine after bridge 2 | Stage 4 beats, the playthrough and the blueprint now run bridge 1, bridge 2 (Dragon), the Spine, bridge 3 |
| Asset tracker lists every asset | **Failed.** 23 of 76 were missing (props, sky, effects) | All 76 are in the tracker. Effects have their own table |
| Tracker names match the data | One mismatch (SKY-03) | Fixed |
| Doc links | One broken link in the stages overview | Fixed |
| Props match the blueprints | **Failed.** STR-27 was 120 m with six glowing rungs. ENV-08 says 72 m and four glowing rungs | STR-27 and STR-08 now say four rungs. The bridge posts belong to STR-08. The stray anchor socket entry is gone from ENV-08 |
| No HUD, no minimap, no ranks or scores | **Failed** in two docs that said "leaderboard" | Docs 28 and 29 now say a private stat, no leaderboard |
| Elias is 21 | Pass | none |

## 4. What is still missing
| Group | Pictures | Next |
|---|---|---|
| ENV-01 to ENV-08 | Done | none |
| ENV-09 Drifting Fragment Cluster | [Doc 35](35-env09-blueprint.md) | Done, 11 pictures filed |
| ENV-10 Debris Rocks | [Doc 36](36-env10-blueprint.md) | Done |
| ENV-11 Moving Platform Slab | [Doc 37](37-env11-blueprint.md) | Done |
| ENV-12 Brittle Slab | [Doc 38](38-env12-blueprint.md) | Done |
| ENV-13 Windbreak Ridge | [Doc 39](39-env13-blueprint.md) | Done (role still proposed) |
| STR-01 to STR-35 (props) | None | Do the ones named in the ENV docs first: STR-08, STR-10, STR-27, STR-28 |
| THR-01 | [Doc 40](40-throne-blueprint.md) | Done (14 pictures) |
| THR-02, THR-03 | [Doc 40](40-throne-blueprint.md) | Blueprinted and aligned with ENV-07. Make the pictures |
| SKY, CRE, VFX | None in the asset library | The Dragon next |

All the prompts are ready for these.

## 5. Is it a winning game? The eight checks
The eight checks from [doc 32](32-rules-of-successful-games.md), section 11, against what is written now.

| # | Check | Now |
|---|---|---|
| 1 | Stillness is an input | Covered by the dead zone and the 0.20 s debounce in doc 06 |
| 2 | Answer stillness fast | 100 ms cue in doc 06 |
| 3 | Make failure worth watching | 3 or more variants of every fall and break in doc 06 |
| 4 | Show a Still Path record | Still open. A tint on the ember at stage end is proposed |
| 5 | Pre and post cards | Answered: the world frames each stage, the Line lighting is the ceremony |
| 6 | Test with strangers | In the production plan: 5 strangers per build |
| 7 | Keep it honest | Written in the production plan |
| 8 | Watch the first 10 minutes | Written in doc 09 |

**Straight verdict.** The design is consistent and every stage now has a clear lesson, a helper, a test and a choice. The risks are not in the documents. They are in three places only play can answer:
1. Does a 3 s stillness hold feel like power, or like waiting? Test it on grey boxes first.
2. Is the first 22 minutes fun before combat arrives?
3. Do players find the long bridge, and is it worth it?

## 6. Not decided yet
1. Steam achievements, the Still Path record and a Stillness Assist setting (doc 33).
2. The Still Secret on the North shelf (doc 31).
3. The world coordinates for Stage 4 (doc 31, section 11).
4. The ENV-04 rock gate, the ENV-07 Throne position and the Stage 6 echo details.
