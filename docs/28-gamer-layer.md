# The gamer layer: filling the six-pillar gaps

> **What this is:** the fixes for every gap found in [the six pillars check](27-six-pillars-check.md). Each fix is written the way a gamer would want to play it.
>
> **Rules kept:** no HUD, no text, no score popups, no skill tree, no shop, no new props. Every reward is the world answering the player.
>
> **STATUS:** **APPROVED by the producer (15 Nov 2026):** the Chord, the bronze rail, the rusty beam, the Still Secrets, the Mastery layer, the Still Path, the choice on every stage, the mid-stage beats and the seven decisions in section 8. Other ways to build each part are in [the options page](29-gamer-layer-options.md). Developers may swap one only after a playtest.

## 1. What a gamer loves (the test)

1. "I did something clever and the game noticed."
2. "I found something nobody told me about."
3. "I got better and I can feel it."
4. "I want one more try."
5. "I want to show a friend."

Every fix below answers at least one of these.

---

## 2. Fun: the Chord (fills the first 22 minutes)

**The problem.** Stages 1 and 2 have no combat. The fun must come from moving and stopping.

**The fix: the Chord.** Every clean move adds one note to a soft chord. A mistake drops a note.

1. A clean move is: a smooth turn, a landing without a stumble, a dash that ends on a bronze line, a stop that holds.
2. Each clean move adds one note. The notes stack up to six, one for each line.
3. At three notes the suit seams glow warm. At six notes the Cinder opens wide and the camera widens a little (FOV 68 to 74, already in the canon).
4. A rushed or panicked move drops a note and adds a little dust.
5. There is no number, no bar, no popup. Only sound and light.
6. Six notes is the Beauty state. This is the best feeling in the game, and players chase it.

**The bronze line is a rail.** The thin bronze line on every island already guides the player.
1. Running along it with a steady rhythm gives a small smooth speed-up. It is the "alignment boost" from [doc 06](06-core-systems.md).
2. Leaving the line is fine. It just loses the boost.
3. This gives stages 1 and 2 a skill to enjoy without combat. Gamers call it "flow".

**Juice for every action** (the small things that make it feel good)
| Action | The feel |
|---|---|
| First stop on island 1 | The wind drops, the sound clears, the Cinder locks in place |
| Fire arrow hits an open frame | A 0.06 s freeze, a glass chime, shards fly |
| Perfect parry | A 0.15 s slow-down, a bell, the shield drops |
| Ignition | The column hums, the line in the sky lights bar by bar |
| Landing on a landing | A soft dust puff and a low stone note |

## 3. Game Loop: the first rush (fills "it only teaches if you rush")

**The problem.** A very careful player may never feel Entropy.

**The fix.** Island 1 has one place that punishes a sprint gently.
1. The rusty beam on island 1 (step 3 of the route) shakes if he sprints across it. Dust falls. The sound turns harsh.
2. If he slows down, it goes quiet and steady.
3. If he keeps sprinting, a plank gives way and the Cinder catches him (see the fall rule in section 8). No damage.
4. Every player feels the rule in the first 3 minutes, in their own way.

---

## 4. Curiosity: the Still Secrets (fills the biggest gap)

**The rule.** Each island hides one Still Secret. You find it only by standing still near it. There is no icon, no marker and no item.

**How it works**
1. Near a secret there is a faint tone. It is quiet. Only a still player hears it.
2. If he stands still for 3 seconds within 6 m, a seam in the rock glows and opens.
3. **The reward is the world:** one lantern on that island lights and stays lit. Then the Fire Eye turns toward him for 4 seconds.
4. The lantern he lit burns gold in the ending.

| Island | Where | What opens |
|---|---|---|
| ENV-01 Starting Shelf | A seam beside the bronze disc | A lantern on the cliff lights |
| ENV-02 Spire | A seam at the root of the dead tree | A lantern on the tree's branch lights |
| ENV-03 Rest | A seam under the rest stone | A lantern on the rim lights |
| ENV-04 Crater | A seam low in the crater wall | A lantern at the crater edge lights |
| ENV-05 Blade | A seam under the middle spire pair | A lantern at the middle of the blade lights |
| ENV-06 Arena | A seam in one dull vent, found after the fight | A lantern at the east gap lights |
| ENV-07 Summit | A seam at the foot of the Throne stair, found while still | The first brazier on the stair lights early |

ENV-08 has its Still Secret proposed in [doc 31](31-env08-blueprint.md), not decided yet. ENV-09 and ENV-10 get theirs when blueprinted.

**Why a gamer loves it**
1. It rewards the exact thing the game teaches.
2. It is private. Two players find different things.
3. A friend says "did you find the one under the tree?" That is word of mouth.

**The big payoff.** If he finds all seven:
1. In the ending, every lantern he lit burns gold.
2. The Fire Eye stays open to the last second instead of closing.
3. The Throne shows one extra thing: its six cracks glow gold, not amber.

**Steam achievements (names only, no text in the game)**
1. "Still Enough" (first secret)
2. "The Quiet Ones" (all seven)
3. "Six Notes" (hold the full Chord for one whole island)
4. "No Hurry" (finish stage 3 without a storm)

---

## 5. Skill: the Mastery layer (fills "nothing to master after stage 3")

**No skill tree.** Skill is shown by how calm and clean you are.

1. **Flawless wave.** Keep the Chord at four notes or more through a whole wave. The enemies go passive. The Dragon flies lower over the arena. Nothing is said.
2. **Resonance strike.** An open-frame hit followed by a parry within 4 seconds makes the Cinder flare. The next arrow is a one-shot (already in the combat table). Skilled players chain this on purpose.
3. **The Calm Score.** After the ending, the Fire Eye shows how calm the run was, as a glow, not a number. A private Steam stat records the average forcing value. There is no leaderboard and no rank (canon: no ranks or scores).
4. **The Still Path (the second run).** After the ending, the same world starts again with a stronger wind and a harsher storm. The 10 second hold now has a gust every 3 seconds. The Throne ending stays the same. This is the replay for skilled players.
5. The 10 second hold is never shortened.

---

## 6. Motivation: a real choice on every stage (fills "few choices")

Every stage gets one choice with a risk and a reward. All choices are about where and when to stop.

| Stage | The choice | Safe | Risky | What the risky one gives |
|---|---|---|---|---|
| 1 | Cross the beam slowly or fast | Slow: quiet and steady | Fast: dust, a shake | A faster path to the door |
| 2 | Which of three lanes | The stable lane | A narrow lane | A view of the Throne early |
| 3 | Where to hide in the arena | The monolith pocket (radius 4.5 m) | A rim gap | A shorter reset, but leeches reach him |
| 4 | Which way across the canyon | The near way: bridge 1, bridge 2 and the Spine | The long bridge, 72 m, 6 s to build | A calmer wind on the last bridge |
| 5 | Which heat lane | The centre lane | A side lane | The Still Secret is easier to hear |
| 6 | When to start the 10 seconds | After the wind eases | Right away | The Throne echo is stronger (see section 9) |

**A hook that pulls the player on.** The Throne is seen from island 1. On each stage the camera shows it a little closer and a little clearer. The player always sees how far there is to go.

---

## 7. Progression: a beat in the middle of long stages (fills "stages 3 and 5 are long")

| When | Beat | What the player sees |
|---|---|---|
| About 5:00 (stage 1) | The door opens | The first reward |
| 22:30 | Line 2 lights | A sky bar |
| **About 30:45 (middle of stage 3)** | **After the storm reset the Fire Eye turns a little toward Elias** | New |
| 39:00 | Line 3 lights | A sky bar |
| 46:00 | The second bridge forms | Stage 4 |
| **About 61:30 (middle of stage 5)** | **First clean heat current: the Dragon answers with a long low sound** | New |
| 70:00 | Line 5 lights | A sky bar |

Nothing new on screen. No bars, no numbers, no text.

---

## 8. The open questions, decided (approved)

| Question | Decision | Why |
|---|---|---|
| Fall rule for the arena | **Option A: the Cinder catch** | It helps, it teaches, no punishment ([doc 25](25-env06-blueprint.md)) |
| ENV-01 ledge fight | **A gentle bow lesson.** Combat stays off until he takes the bow. Then 2 weak enemies, one opening each, no splitting. Dash stays penalised. | Fixes the clash with "stage 1 combat off" |
| The Shadow fight on island 1 | **No.** Move the idea to the Summit as a faint echo during the 10 second hold. | There is no villain. The Summit is the right place |
| Leeches on ENV-05 | **No.** The long bridge walk is the calm breath before the arena. Wind and the spire pairs are the challenge. | Pacing: a quiet part makes the fight feel bigger |
| The 3 cracking slabs on ENV-06 | **Yes.** One second of red glow and rumble first. The Cinder catches him. | Fair and readable |
| 6 braziers on the Throne stair | **Yes.** 3 on each side, dark until the ending. | Fits the six lines |
| Dragon drop | **At the foot of the Throne stair.** He climbs it himself. | The climb is the last effort. Then the Throne |

## 9. The Summit echo (the Shadow idea, moved)

1. During the 10 second hold, a faint glass figure of Elias appears far off, in the wind.
2. It stands still. It does not attack.
3. If he stays still, it fades. If he moves, it flickers and the timer resets.
4. A gamer reads it as a mirror of himself. No fight and no villain.

---

## 10. What comes next

1. Update the stage docs to match this page.
2. Prepare the Gemini pictures for a secret seam.
3. Other options for every part: [the options page](29-gamer-layer-options.md).

Continue: [Six pillars check](27-six-pillars-check.md) · [Core systems](06-core-systems.md) · [Stages](stages/README.md)
