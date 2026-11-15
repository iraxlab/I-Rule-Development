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

## Rules applied
Applied 15 Nov 2026 from [doc 32](32-rules-of-successful-games.md). None of these add a HUD, text or a score.

1. **Before each stage (PY-8).** The camera drifts for up to 3 seconds to the empty bar of the next Line in the sky. Cinder looks toward the goal. No card, no text.
2. **After each stage (PY-9, PY-10).** The Line lighting is the ceremony: slow light, a chord and the sky answering. It is the reward. No score screen.
3. **Easy way back in (PY-S3, PY-S4).** From the game icon to standing at the last anchor takes 30 seconds or less. No logo longer than 3 seconds. Autosave at every anchor, every landing and every stage start.
4. **Natural stops (PY-S6).** Each Line lit is a quiet moment where he can stop. Cinder settles and the world goes calm.
5. **Welcome back (PY-S7).** On return, Cinder greets him. The lit Lines in the sky show how far he came.
6. **First 10 minutes (PY-K1, FP-11).** A tour, not a lesson. The first reward comes within 60 seconds. The first stillness discovery comes in about 3 minutes. Log both.
7. **Light relief (PY-S10).** One calm pocket in about every 3 minutes of play.
8. **No game over (FP-12).** Every failure resets in under 5 seconds to the last anchor. No fail text.
9. **Loops of five sizes (FP-3).** A hold, a bridge, an island, a stage, the game.
10. **Quiet help (UN-9).** After 3 failures in a row at one spot, the world helps: the wind eases and Cinder points. Hold times never change.
11. **Damage (UN-4).** Show damage by suit seams flickering, a short edge flash and a sound. No health bar.
12. **Still Path record (GF-20).** Store time and clean builds for each stage. Show no numbers. How it shows is not decided yet.
