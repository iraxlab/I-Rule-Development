# Prompts

| File | What it is |
|---|---|
| [key-art-prompts.md](key-art-prompts.md) | The 25-page key-art prompt set (Page 24 is the redesigned Throne) |
| [elias-character-reference-prompts.md](elias-character-reference-prompts.md) | Five-view Elias turnaround prompts |
| [3D Reference Prompt Pack](../art-pipeline/3D_Reference_Prompt_Pack.pdf) | 76 assets, sheet and single-angle prompts |
| [cover-regeneration.md](cover-regeneration.md) | Cover prompt with equal-width bars (canon fix) |
| [Throne Wow Direction](../design/Throne_Wow_Direction.pdf) | Throne hero, scale, seat, turnaround, ignition prompts |

## Prompt rules that matter
- Self-contained: repeat the look in every prompt.
- Put the asset name as a short bold label that appears only once.
- Use explicit negatives (not modern, not glossy, no city, no glass).
- Avoid trigger words: hexagram, pyramid, ritual circle, slit, rope, swaying; and for the Throne: mirror, polished, floating, rods.

## Title rule
Every image carries `ID - NAME` as a visible title (for example `ENV-01 - STARTING SHELF ISLAND`), and single angles add the view (`... - FRONT`). See [asset library rules](../docs/15-asset-tracker.md).


## Per-asset prompt files

**Paste one prompt per message into Gemini, never a whole file.** Pasting everything at once runs the image tool out of turns.

- Core set per asset: 1 turnaround sheet, plus 4 detail close-ups where details exist (all 13 islands have them). That is 5 images per island.
- `prompts/assets/<ID>/sheet.txt`, `detail-1.txt` ... `detail-4.txt` and the single views (`front.txt`, `back.txt` ...): one file per prompt, one image per prompt.
- The same text is on the website (Art, Islands and All assets) with Copy and Download buttons. Source data: `data/prompts.json`.
