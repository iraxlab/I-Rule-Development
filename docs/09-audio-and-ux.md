# Audio and UX

## Audio is the primary teacher
No tutorial text. Sound tells the player whether they are right.

**Layers (three, adaptive):**
1. **Base wind**
2. **Low harmonic drone**
3. **High clarity tone**

**Rules**
| Moment | Audio behaviour |
|---|---|
| Alignment | Harmonic layers bloom |
| Entropy | Noise and distortion intrude |
| Ignition | Chord resolution |
| Final | Wind and near-silence. **No epic melody.** |

Driven by the CreativeEnergyController state via an audio state controller (MetaSounds, adaptive layered mix). Absence of sound is, narratively, the sound of getting it right. Create the audio response layer **early**, not last.

Per-stage audio beats are in each [stage document](stages/README.md).

## UX: what we do not have
- No minimap, no quest markers
- No ranks or scores
- No text tutorials, no button-prompt pop-ups
- No HUD clutter

## UX: what we do have
- Audio feedback
- World behaviour (platform stability, storm onset, lantern flicker)
- Suit seams and Cinder feedback
- Landmark navigation (Eye, six lines, lanterns, Throne silhouette)
- Soft resets (falling is correction, not punishment)
- Discovery

## Design philosophy
*"The world is the interface."* *"Sometimes the correct action is to do nothing."* Hidden systems fail if feedback is too subtle (the player will not learn) or too loud (it becomes a HUD). Tune between the two with playtests.
