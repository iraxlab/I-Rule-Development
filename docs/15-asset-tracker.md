# Asset library

Every asset the game needs, what to drop where, and what is still missing. **Drop each image into its folder with the exact file name below; the website tracker updates by itself.** No list to edit.

Live view with thumbnails and status: open the site and choose **Asset library**.

## How to name files
Inside `art/assets/<ASSET-ID>/` (for example `art/assets/ENV-01/`):

| File | What it is |
|---|---|
| `sheet.jpg` | The multi-angle turnaround sheet (first step: lock the design) |
| `front.jpg`, `back.jpg`, `left.jpg`, `right.jpg`, `top.jpg`, `under.jpg` | Single-angle renders |
| `tq_fl.jpg`, `tq_fr.jpg`, `tq_bl.jpg`, `tq_br.jpg` | Three-quarter views (front-left, front-right, back-left, back-right) |
| `low.jpg`, `high.jpg` | Low and high angle (Throne only) |
| `model.png` | Optional: screenshot of the finished 3D model |

Which views each asset needs is in the table. Prompts for every one are in the [3D Reference Prompt Pack](../art-pipeline/3D_Reference_Prompt_Pack.pdf) (page numbers below).

> The Status column in the tables below is a **snapshot from when the tracker was made**. The live status is on the website tracker, which checks which files exist.

## Title rule: every image names itself
Every generated image must show a large, readable title with the **asset ID and name**, so a developer can tell what it is at a glance:

| Image | Title text (exact format) |
|---|---|
| Turnaround sheet | `ENV-01 - STARTING SHELF ISLAND` banner at the top, size note beside it (for example `~40 m wide`), plus a small label under each view |
| Single angle | `ENV-01 - STARTING SHELF ISLAND - FRONT` at the bottom |
| Throne extras | `THR-01 - THE THRONE OF STILLNESS - DETAIL: SIX FISSURES` |

All prompts in the [3D Reference Prompt Pack](../art-pipeline/3D_Reference_Prompt_Pack.pdf) already carry this exact text. If the tool changes or invents a title, regenerate; do not file an image whose title does not match its ID.

## Status key
- **Missing**: no `sheet.jpg` yet.
- **Sheet only**: sheet locked, single views not done.
- **In progress**: some single views done.
- **Complete**: sheet and all views done.
- **Reference exists**: the key art already shows this object; use it as the look target, it does not replace the sheet.


## Islands

| ID | Asset | Size | Views needed | Pack page | Look reference | Status |
|---|---|---|---|---|---|---|
| ENV-01 | Starting Shelf Island | ~40 m wide | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 6 | [key art](../art/world/stage-1-lurking.jpg) | Sheet v2 + front, top, underside + 4 details filed |
| ENV-02 | Small Stepping Island | ~12 m wide | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 10 | none yet | Sheet v2 + front, back, top, underside + 4 details filed |
| ENV-03 | Medium Island with Windbreak | ~30 m wide | 10: sheet, front, back, top, under, detail-1 to detail-5 | 10 | none yet | Complete: sheet + front, back, top, underside + 5 details filed (rock massif, column, rest stone; no towers, no bell, no nest) |
| ENV-04 | Large Plateau Island | ~60 m wide | 10: sheet, front, back, top, under, detail-1 to detail-5 | 10 | [key art](../art/world/stage-2-emerging.jpg) | Complete: sheet + front, back, top, underside + 5 details filed. Known picture differences in docs/22 section 11 |
| ENV-05 | Long Causeway Island | ~80 m long, 10 m wide | 10: sheet, front, back, top, under, detail-1 to detail-5 | 10 | none yet | Complete. 10 images filed. Natural rock, leaning spire pairs, no props. Connection and leeches in docs/23 (Sheet C). ATTENTION: picture mistakes and fixes are in docs/23 section 12 |
| ENV-06 | Arena Island | ~64 m wide | 10: sheet, front, back, top, under, detail-1..detail-5 | 22 | [key art](../art/world/stage-3-the-toil.jpg), [doc 25](25-env06-blueprint.md) | Redesigned. Sheets A, B, C done. All 10 pictures filed. Read ATTENTION in doc 25 |
| ENV-07 | Summit Peak Island | ~150 m wide, 90 m tall | 10: sheet, front, back, top, under, detail-1..detail-5 | 25 | [key art](../art/world/stage-6-the-summit.jpg), [doc 26](26-env07-blueprint.md) | Redesigned HUGE (zigzag of rock steps, the Throne on top, no towers). Sheets A, B, C done. 10 pictures filed (see doc 26 section 12) |
| ENV-08 | Canyon Cliff Pair | two ~35 m islands | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 28 | [key art](../art/world/stage-4-the-leap.jpg) | Sheet v1 filed |
| ENV-09 | Drifting Fragment Cluster | cluster ~50 m | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 31 | [key art](../art/world/stage-5-flying.jpg) | Missing |
| ENV-10 | Debris Rocks Set | 1-4 m each | 8: front, left, top, tq_fl, detail-1, detail-2, detail-3, detail-4 | 34 | none yet | Sheet v1 filed |
| ENV-11 | Moving Platform Slab | ~8 m wide | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 37 | none yet | Missing |
| ENV-12 | Brittle Slab | ~6 m wide | 9: front, back, left, top, under, detail-1, detail-2, detail-3, detail-4 | 40 | none yet | Missing |
| ENV-13 | Windbreak Ridge | ~25 m long, 8 m tall | 8: front, left, top, tq_fl, detail-1, detail-2, detail-3, detail-4 | 43 | none yet | Missing |

## Structures

| ID | Asset | Size | Views needed | Pack page | Look reference | Status |
|---|---|---|---|---|---|---|
| STR-01 | Tower Ruin, Large | ~30 m tall | 5: front, back, left, top, under | 47 | none yet | Missing |
| STR-02 | Tower Ruin, Capped | ~22 m tall | 5: front, back, left, top, under | 49 | none yet | Missing |
| STR-03 | Rock Spire Cluster | ~25 m tall | 5: front, back, left, top, under | 51 | none yet | Missing |
| STR-04 | Monolith Slab | ~12 m tall | 5: front, back, left, top, under | 53 | none yet | Missing |
| STR-05 | Locked Bronze Gate | ~8 m tall | 5: front, back, left, top, under | 55 | none yet | Missing |
| STR-06 | Fixed Stone Bridge | ~20 m long | 5: front, back, left, top, under | 57 | none yet | Missing |
| STR-07 | Plank and Metal Causeway Segment | ~10 m long | 5: front, back, left, top, under | 58 | none yet | Missing |
| STR-08 | Light Bridge Segment | ~6 m long | 4: front, left, top, tq_fl | 60 | none yet | Missing |
| STR-09 | Anchor Socket | ~2 m wide | 5: front, back, left, top, under | 61 | none yet | Missing |
| STR-10 | Ignition Column, Dormant | ~6 m tall | 5: front, back, left, top, under | 63 | none yet | Missing |
| STR-11 | Ignition Column, Ignited | ~6 m tall | 5: front, back, left, top, under | 64 | none yet | Missing |
| STR-12 | Peak Column | ~10 m tall | 5: front, back, left, top, under | 66 | none yet | Missing |
| STR-13 | Lantern Anchor XL, Hanging | ~9 m tall | 5: front, back, left, top, under | 67 | none yet | Missing |
| STR-14 | Lantern Anchor XL, Tower-Mounted | ~12 m tall | 5: front, back, left, top, under | 68 | none yet | Missing |
| STR-15 | Lantern Anchor XL, Ground | ~8 m tall | 5: front, back, left, top, under | 69 | none yet | Missing |
| STR-16 | Lantern Anchor XL, Lit | ~9 m tall | 5: front, back, left, top, under | 70 | none yet | Missing |
| STR-17 | Heat Vent | ~3 m wide | 4: front, left, top, tq_fl | 71 | none yet | Missing |
| STR-18 | Energy Reservoir | ~10 m wide | 5: front, back, left, top, under | 72 | none yet | Missing |
| STR-19 | Fossil Tree | ~6 m tall | 5: front, back, left, top, under | 73 | none yet | Missing |
| STR-20 | Six-Line Pylon | ~6 m tall | 4: front, left, top, tq_fl | 74 | none yet | Missing |
| STR-21 | Small Lantern Post | ~1.2 m tall | 4: front, left, top, tq_fl | 75 | none yet | Missing |
| STR-22 | Summit Staircase | ~30 m long | 5: front, back, left, top, under | 76 | none yet | Missing |
| STR-23 | Leaning Broken Tower | ~28 m tall | 5: front, back, left, top, under | 77 | none yet | Missing |
| STR-24 | Needle Spire Tower | ~45 m tall | 5: front, back, left, top, under | 79 | none yet | Missing |
| STR-25 | Twin Towers with Broken Arch | ~26 m tall, 30 m wide | 5: front, back, left, top, under | 81 | none yet | Missing |
| STR-26 | Gatehouse Tower | ~24 m tall | 5: front, back, left, top, under | 83 | none yet | Missing |

## Sky

| ID | Asset | Size | Views needed | Pack page | Look reference | Status |
|---|---|---|---|---|---|---|
| SKY-01 | Six-Line Ladder, Dormant | ~120 m wide total | 5: front, back, left, top, under | 86 | [key art](../art/world/04-six-lines-the-sky-is-the-map.jpg) | Missing |
| SKY-02 | Six-Line Ladder, Progress States | ~120 m wide total | 4: front, left, top, tq_fl | 88 | [key art](../art/world/04-six-lines-the-sky-is-the-map.jpg) | Missing |
| SKY-03 | Fire Eye Structure | ~200 m wide | 5: front, back, left, top, under | 89 | [key art](../art/characters/companion-the-fire-eye.jpg) | Missing |
| SKY-04 | Ringed Planet | sky object | 4: front, left, top, tq_fl | 90 | none yet | Missing |
| SKY-05 | Plain Planet | sky object | 4: front, left, top, tq_fl | 91 | none yet | Missing |

## Throne

| ID | Asset | Size | Views needed | Pack page | Look reference | Status |
|---|---|---|---|---|---|---|
| THR-01 | The Throne of Stillness | ~40 m tall | 15: front, back, left, right, top, tq_fl, tq_fr, tq_bl, tq_br, low, high, detail-fissures, detail-ribs, detail-seat, ignited | 93 | Sheet v1 at `art/assets/THR-01/sheet.jpg` | Sheet only (revise: six fissures, two ribs) |
| THR-02 | The Throne Stairs and Platform | ~50 m long | 5: front, back, left, top, under | 97 | none yet | Missing |
| THR-03 | Throne on Summit | ~70 m overall | 15: front, back, left, right, top, tq_fl, tq_fr, tq_bl, tq_br, low, high, detail-fissures, detail-ribs, detail-seat, ignited | 99 | [key art](../art/world/stage-6-the-summit.jpg) | Missing |

## Creatures

| ID | Asset | Size | Views needed | Pack page | Look reference | Status |
|---|---|---|---|---|---|---|
| CRE-01 | The Cinder (guide) | ~30 cm | 5: front, back, left, top, under | 104 | [key art](../art/characters/companion-the-cinder.jpg) | Missing |
| CRE-02 | Fire Dragon | ~60 m long | 5: front, back, left, top, under | 106 | [key art](../art/characters/companion-the-fire-dragon.jpg) | Missing |
| CRE-03 | Glass Shadow | ~2 m tall | 5: front, back, left, top, under | 107 | [key art](../art/characters/enemy-glass-shadows.jpg) | Missing |
| CRE-04 | Burn Knight | ~3 m tall | 5: front, back, left, top, under | 108 | [key art](../art/characters/enemy-burn-knights.jpg) | Missing |
| CRE-05 | Ember Leech | ~40 cm | 4: front, left, top, tq_fl | 109 | [key art](../art/characters/enemy-ember-leeches.jpg) | Missing |
| CRE-06 | Storm Wraith (VFX reference) | ~5 m | 4: front, left, top, tq_fl | 110 | [key art](../art/characters/enemy-storm-wraiths.jpg) | Missing |

## Totals
- 76 assets: 13 islands, 35 structures, 10 sky, 3 throne, 6 creatures, 9 effects (new ones are not in the snapshot table above).
- Sheets needed: 53. Single views and detail close-ups (combined count): 394.
- Plus four Throne detail renders (six fissures, dragon ribs, seat and armrest, ignited state): `art/assets/THR-01/detail-fissures.jpg`, `detail-ribs.jpg`, `detail-seat.jpg`, `ignited.jpg`.


## Detail close-ups

**Per island: 1 five-angle sheet, then the single views (front, back, side, top, underside) and 4 detail close-ups, all shown openly on the site.** Each island has four detail close-ups, saved as `detail-1.jpg` to `detail-4.jpg` (labels and prompts are on the website and in the PDF).
