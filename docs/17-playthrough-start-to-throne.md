# Playthrough: from the first frame to the Throne

**Read this to know exactly what happens, in order.** It follows Elias from the first second on island 1 to the moment the ring of fire spreads from the Throne. Every beat says what the player does, what the game does back, what the camera and sound do, and what to build.

## Status and what changes
This section combines the locked canon (stage docs, core systems, Throne) with a **new design direction from the project owner**: the *Stillness Duel*. Items marked **PROPOSED** are new and need owner approval. Everything else comes from existing canon.

| # | Change from current canon | Why |
|---|---|---|
| 1 | Stage 1 gets **one scripted enemy encounter** (before: "no enemies, combat disabled") | The game's rule is learned by *failing at force first*, then winning by stillness |
| 2 | Elias carries floating **Arms** (a diegetic ring of weapons) and a last tool, the **Still Ring** | The player tries weapons, they all fail, the last tool works |
| 3 | Entering stillness now has a **Meditation float**, then a **mind-vision duel** | The "wow" payoff of stillness; uses the meditation animation that already exists |
| 4 | The Stage 1 timeline grows by about 4.5 minutes | The encounter and the arms pickup; retime the later stages (total stays within 75-95 min) |

Still true: no health bar, no HUD, no inventory screen, no text. Enemies are **symbolic**, never people. No jump in Stage 1.

---

## 1. The one-sentence game
*Rushing and fighting make the world worse. Stopping makes it better. The first island teaches this by letting you fight, fail, stop, and win.*

## 2. What the player can do (Stage 1 control set)
| Action | Keyboard / mouse | Controller | Available in Stage 1? |
|---|---|---|---|
| Move / look | WASD / mouse | Left / right stick | Yes |
| Walk / run | Hold Shift to walk slowly | Light stick tilt | Yes |
| Dash | Space tap | A / Cross | Yes, but each dash adds +0.08 forcing (it makes the world noisier) |
| **Jump** | | | **No.** Not in Stage 1 (unlocks in Stage 2 with the moving platforms) |
| Interact | E | X / Square | Yes (bind Arms, ignition columns) |
| Strike | Left mouse | RT | **Only inside the encounter** |
| Heavy strike | Hold left mouse | Hold RT | Only inside the encounter |
| Guard / parry | Right mouse | LT | Only inside the encounter |
| **Cycle Arms** | Q / E or mouse wheel | LB / RB | Only inside the encounter |
| **Meditate (hold)** | Hold F | Hold Y / Triangle | Yes. Works anywhere, and is the key of the whole game |

### How vertical movement works on island 1
| Question | Answer |
|---|---|
| Do you jump up? | No. Height is gained by **stairs, ramps and broken slabs** that are walkable. Step-up is automatic for edges up to 0.5 m. |
| Do you jump down? | No jump needed. Walk off a **marked ledge** of up to 1.2 m and Elias drops with a short landing animation. |
| What if you fall off the island? | Every island rim has a **danger-edge volume**. Crossing it fades to cloud and returns Elias to the last safe ground. It is a correction, never a death. |
| Are there steps? | Yes. The Arrival Disc has three shallow steps; the Gateway has a wide cracked stair. |

---

## 3. Island 1: the Starting Shelf (ENV-01)
~40 m wide. Visible from the first frame: a dark shelf, a deep **ravine**, one colossal **fallen bronze beam** crossing it, a **broken gateway** at the far end holding a **still beam of light**, a shallow bronze **arrival disc**, huge cracked paving slabs, chains hanging into the void, one bare fossil tree. Above everything: the six unlit lines and, far away, the **Throne silhouette** (see [Throne](08-the-throne.md)).

### Route map
```
                          [ SIX LINES, UNLIT ]   Throne silhouette (far)
                                  |
   +----------------------------- N ------------------------------+
   |                                                              |
   |   [GATEWAY]  <- broken arch, still beam inside (locked)      |
   |      |   antechamber: Arms float here (E1)                   |
   |      |   ENCOUNTER ARENA (circle, 14 m) (E2)                 |
   |      |                                                       |
   |  ====[ FALLEN BRONZE BEAM over the RAVINE ]====  (walk only) |
   |      |                                                       |
   |   paving field, fossil tree, hanging chains (calm)           |
   |      |                                                       |
   |   [ARRIVAL DISC]  <- Elias begins here (S)                   |
   |                                                              |
   +--------------------------------------------------------------+
                  exit: bridge from the gateway side
                  to ENV-02 (Stepping Island)
```
| Waypoint | Purpose | Approx. position (source coords; set in level) |
|---|---|---|
| S: Arrival Disc | Spawn, first frame | (-290, 0, -290) |
| P: Paving field | Calm walk, first look at the sky | (-282, 0, -282) |
| B: Ravine crossing | Walk the beam, 3 m wide, no sway | (-274, 0, -274) |
| E1: Antechamber | Arms pickup | (-266, 0, -266) |
| E2: Encounter arena | The Duel | (-262, 0, -262) |
| G: Gateway | Beam unlocks, exit bridge appears | (-258, 0, -258) |

### Beat plan: island 1, minute by minute (golden path)
| Time | What Elias does | What the world does | Camera | Sound |
|---|---|---|---|---|
| 00:00-00:25 | Nothing yet | Black. Wind. Fade in on Elias on the Arrival Disc, standing, eyes open. Six lines visible but dark. | Fixed wide, slow push | Wind only (`AUDIO_S1_WindOnly_In`) |
| 00:25-01:30 | **First control.** Walks off the disc across the paving field | No UI. The Cinder is barely visible beside him. Suit seams dark. | Close, grounded third person | Low drone fades in (`AUDIO_S1_LowDrone_FadeIn`) |
| 01:30-02:30 | Explores the rim, the fossil tree, the chains | Looking up reveals the lines and the Throne silhouette. Edge = soft-reset volume. | Slight upward tilt hint when he looks up | Wind rises at the rim |
| 02:30-03:30 | **Crosses the fallen bronze beam** (walk, no jump) | Dust from the bronze. If he dashes: noise creeps in, dust lifts (first taste of Entropy). | Pull out to show depth under him | Metal resonance under footsteps |
| 03:30-04:15 | Enters the antechamber. **Three Arms float in the air.** Walks into each and presses Interact; each lights and begins to orbit him | The still beam in the gateway pulses once, as if it noticed | Orbit shot of the Arms binding | Three rising bronze notes, one per Arm |
| 04:15-04:45 | The beam casts **Elias's own shadow** across the floor. The shadow **stands up**: the **Unbroken Shadow** | It steps out, a dark amber-glass copy of Elias. The gateway beam dims. | Slow push to the Shadow | Drone drops; a single held low tone |
| 04:45-07:30 | **Fights it** with the Arms (Section 4, phases A-B) | The Shadow **copies every weapon** Elias uses and every strike. Spam makes it split. Entropy rises: wind, dust, noise. | Combat camera, FOV 68 | Noise bed rises (`AUDIO_S3_TensionBed` style) |
| 07:30-08:00 | Has tried all Arms. Nothing works. | The **Still Ring** drops from the gateway beam, floats above Elias, and stays | Gentle tilt up to the Ring | Wind falls away; a clear high tone |
| 08:00-08:30 | **Selects the Still Ring and holds Meditate** | Elias rises off the ground into the meditation float (existing animation). The Shadow freezes and mirrors his pose badly. | Wide, low, slow arc around him | Everything strips to wind and a soft harmonic |
| 08:30-09:10 | Holds still while the **mind-vision plays** | Full takeover (Section 5). The Shadow dissolves. | Vision camera | Vision score |
| 09:10-09:40 | Opens his eyes, lowers to the ground | The Shadow is gone. Amber dust drifts upward. The beam **relights** and the exit opens. The Cinder brightens. | Eye-level, then wide | Chord resolution, then calm |
| 09:40-10:30 | Walks through the gateway, over the bridge to island 2 | A far lantern anchor flickers alive | Follow | Drone and clarity tone |

**Where does the action actually start?** Control starts at 00:25. The first threat arrives at 04:15. The first fight is at 04:45. The first stillness is at 08:00.

### After the encounter: the rest of Stage 1 (unchanged canon)
Island 2 (ENV-02 Stepping Island), then island 3 (ENV-03 with ENV-13 windbreak ridge), as in [Stage 1](stages/stage-1-lurking.md): first calm pocket (stand 2 s to clear the sound), approach the ignition column, hold **2.5 s** facing it, the column ignites, **Line 1** (bottom bar) lights. The player now *already knows* what stopping does, so the column reads as a quieter, shorter version of the same act.

---

## 4. The Stillness Duel: the encounter, exactly
### 4.1 The enemy: the Unbroken Shadow (PROPOSED)
A symbolic copy of Elias made of dark amber glass, about 1.8 m. It represents **the self that insists on fighting**. It is a "Glass Shadow" archetype ([enemies](05-enemies.md)) with one added rule.

| Rule | Behaviour |
|---|---|
| **Mirror** | It uses the same weapon type Elias just used, one beat later |
| **Split** | If Elias attacks more than 1.4 times per second it splits into two weaker copies (canon anti-spam). More copies = more entropy. |
| **Cannot be killed by force** | Hits crack it but it re-forms within 2.5 s. No health bar. |
| **Cannot mirror stillness** | When Elias holds Meditate, it freezes, tries to copy his pose, and flickers |
| **Hits on Elias** | Stagger (0.4 s) and +0.12 ForcingIndex. No death, no health. |

### 4.2 The Arms: a diegetic weapon ring (PROPOSED, names are placeholders)
Three weapons float in a loose ring around Elias. **There is no HUD or wheel.** The one in use drifts to his hand; the others hover. They are real objects in the world.

| Arm | Reads as | Behaviour | Why it fails here |
|---|---|---|---|
| **Sacred Arc** (canon) | Fire-arrow bow | Light and charged arrows | The Shadow mirrors the arrow |
| **Ember Blade** | Short bronze blade with a hot edge | Fast close strikes | The Shadow blocks with a mirrored blade |
| **Bronze Lance** | Long reach, heavy | Slow thrust | The Shadow mirrors the lance and trades blows |

The Arms stay bound to Elias for the rest of the game and are used in the full combat stages (Stage 3 onward).

### 4.3 The Still Ring (PROPOSED, name is a placeholder)
A thin bronze ring that **floats above Elias's head and never rotates** while the Arms orbit. It is the last tool. It is the first fragment of the gateway's locked beam; at the Throne the beam finishes entering him ([ending](stages/the-throne-ending.md)).

| Question | Answer |
|---|---|
| When does it appear? | When Elias has used **each Arm at least once**, or **45 s** have passed in the fight, or ForcingIndex has stayed at **0.62 or higher** for 5 s (whichever comes first). It drops from the gateway beam. |
| Can the player find it earlier? | No. It is not selectable until it appears. It is dim and still before that. |
| How is it used? | Cycle to it like an Arm, then **hold Meditate** |
| Does it show text or a prompt? | No. A soft rising tone and the Ring's glow are the only prompt |

### 4.4 State machine
| State | Entry | What happens | Exit |
|---|---|---|---|
| **E0 Dormant** | Level load | Gateway beam locked, Arms hover as props | Player binds all three Arms |
| **E1 Armed** | Third Arm bound | Beam pulses. 8 s of silence. | Auto, after 8 s |
| **E2 Awakening** | Timer | Shadow forms from Elias's shadow, 30 s scripted entrance | Shadow ready |
| **E3 Fight** | Shadow ready | Mirror and split rules active. Entropy rises with forcing. | Still Ring appears |
| **E4 Ring offered** | Conditions in 4.3 | Ring descends. Fight continues at reduced intensity | Player selects the Ring and holds Meditate |
| **E5 Gathering** | Meditate held | Shadow freezes. Elias settles. ForcingIndex drops at -0.28/s (stillness) plus -0.22/s (meditation) once under 0.35. | ForcingIndex <= 0.35 and hold >= 1.5 s (max wait 4 s) |
| **E6 Float** | Gathering done | Elias lifts about 0.8 m, meditation animation plays (1.5 s rise) | Lift complete |
| **E7 Vision** | Float complete | Mind-vision plays (Section 5), 35 s while the hold continues | Vision complete |
| **E8 Dissolve and wake** | Vision complete | Shadow disperses, Elias opens his eyes and lowers (1.2 s) | Control returned |
| **E9 Cleared** | Wake done | Gateway relit. Exit bridge enabled. Encounter will not respawn. | |

**Release rule:** if the player releases Meditate or moves during E5-E7, the vision fades out over 0.6 s, Elias drops to the ground, and the Shadow resumes. The next attempt starts the vision from the beginning after a 3 s grace. Tune the look and velocity tolerance as in [core systems](06-core-systems.md) (mouse 0.35, velocity 0.06).

**Checkpoint:** at the start of E2 (Shadow forms). If the player quits and returns, they resume there.

### 4.5 ForcingIndex hooks
- Combat in E3 uses the standard ForcingIndex rules (move, turn, spam, dash).
- Being hit: +0.12. Whiffed heavy: +0.05 (canon).
- The Shadow's split count scales with forcing: 1 copy below 0.4, 2 above 0.5, 3 above 0.62 (cap 3).
- Meditation only counts as the -0.22/s reduction while ForcingIndex is below 0.35 (canon), so the player must first calm down, as in E5.

---

## 5. The mind-vision (the cinematic core)
The vision **overtakes the whole screen** like a film. The player does nothing but **keep holding Meditate** (holding is the only input; it can also be toggled on in Accessibility). Total target: **35 s**. All times are starter values.

| Movement | Time | What we see | Camera | Sound |
|---|---|---|---|---|
| **1. The Mirror Plain** | 0-8 s | The world falls away. A black plain. The six lines glow faintly on the horizon like a sunrise, evenly spaced. Elias stands facing the Shadow, 10 m apart. Both hold their weapons. | Slow push from a wide shot. Letterbox bars slide in. | Wind falls to a soft drone and a heartbeat at 60 bpm |
| **2. The Clash** | 8-20 s | They fight with *everything Elias tried*: arrows of fire, the ember blade, the bronze lance, fast and huge, with shockwaves and amber sparks. Each strike is mirrored. Every hit makes the plain more cluttered and noisier. | Fast cuts, speed lines, FOV up to 80. Camera shake up to 0.12. | Percussion builds, bronze impacts, noise bed rises |
| **3. The Stop** | 20-28 s | Elias **lowers his weapons**, opens his hands, and stops. Time slows to 10%. The Shadow keeps attacking and cannot stop: it strikes at its own reflection and cracks. The bottom line of the six lines flares. | Lock off. Slow, locked frame at eye level. FOV 60. | Everything cuts out except one clear tone and the heartbeat |
| **4. The Dissolve** | 28-35 s | The Shadow shatters into amber glass dust that drifts upward into the six lines. The vision whites to gold. | Pull up and back, following the dust | Chord resolution (4 s) as the light floods in |

### What to build for the vision
| Element | Notes |
|---|---|
| **Sequencer** | One Level Sequence with the camera work. Player input suppressed except the hold. |
| **Post process** | Letterbox, slight chromatic aberration in Clash, desaturation to gold in Dissolve |
| **Niagara** | Fire arrows, spark bursts, glass dust, six-line glow |
| **Time dilation** | Global time dilation 0.1 in The Stop only |
| **Rumble (controller)** | Ramps up through The Clash, cuts to zero at The Stop |
| **Duration safety** | If the player holds beyond the end, nothing else happens (no extra reward) |
| **Skip** | Not available on the first viewing. Available on replays. |

### Return to the world (E8)
1. Gold fades to the world. Elias, still floating, opens his eyes (blink animation, 0.4 s).
2. He lowers to the ground over 1.2 s. Dust motes drift up from where the Shadow stood.
3. The gateway beam **relights**, steady and calm. The Still Ring dims, then settles above him.
4. The Cinder brightens. A far lantern anchor flickers on.
5. Control returns. No text, no reward screen.

---

## 6. Stage by stage: how Elias gets to the Throne
**Tags:** *CANON* = already in stage docs. *PROPOSED* = new in this document.

| # | Stage and place | What the player does | New verb / tool | Enemy or trial | Stillness hold | Result |
|---|---|---|---|---|---|---|
| 1 | **Lurking.** Islands ENV-01 to ENV-03, southwest | Walks, crosses the beam, binds the Arms, meets the Shadow, learns stillness by the Duel, then calm-pockets and ignites the first column | Arms, Still Ring, Meditate float (*PROPOSED*); alignment, calm pockets (*CANON*) | Unbroken Shadow (*PROPOSED*) | 2.5 s at the column | **Line 1** |
| 2 | **Emerging.** ENV-11 platforms, ENV-04 plateau, south-central | Moving platforms, the three-path direction gate, the energy reservoir | **Jump** unlocks (*CANON*) | None. Timing is the trial. | 3 s | **Line 2** |
| 3 | **The Toil.** ENV-06 arena, southeast | First real combat with all Arms. Anti-spam lesson. Storm and calm pocket. Burn Knight. Dragon glimpsed. | Full combat kit, parry (*CANON*); each Arm has a job (*PROPOSED*) | Glass Shadows, Leeches, Burn Knight, Storm Wraith | 4 s | **Line 3** |
| 4 | **The Leap.** ENV-08 canyon, central-east | Bridges that form only while still, combat on narrow spans, Dragon assist when aligned | Meditate-style hold builds bridges (*CANON*) | Two Glass Shadows | 3 s | **Line 4** |
| 5 | **Flying.** ENV-09 and ENV-10, north-central | Heat currents, Dragon flight, commit without hesitation | Heat-current glide (*CANON*) | Optional enemies, bypassable | 5 s | **Line 5** |
| 6 | **The Peak.** ENV-07, far north | Climb the long staircase, stop under wind | None. Combat and dash off. | None | **10 s** (demo build 6 s) | **Line 6**, all six lit |
| End | **The Throne.** THR-01 to THR-03 | Dragon carries Elias to the foot of the stairs. He climbs on foot to the seat. He sits. | Sit (the only pure choice) | None | None | **Ring of Fire** |

**Where the Duel returns (PROPOSED, owner to decide):**
| Stage | Use |
|---|---|
| 3 | The Burn Knight's shield may be dropped by a short Meditate-hold *Duel-lite* (10 s) as an alternative to the parry. Optional. |
| 6 | The 10 s hold shows a faint echo of the vision (the six lines and the plain) at the edges of the screen. No enemy. |
Everywhere else, stillness stays as in canon (hold at the column, calm pocket, bridge building).

---

## 7. The route to the Throne
### 7.1 Stage 6 finale (CANON)
| Time | What happens |
|---|---|
| 70:00-71:20 | Arrive at the summit platform (0, 80, 340). Extreme wind. Narrow safe zones. |
| 71:20-72:30 | Instinct is to move; micro-slips punish it. |
| 72:30-74:30 | Hold still **10 s** at the ignition column (0, 80, 360). Any movement resets. Audio strips to wind and a distant harmonic. |
| 74:30-75:00 | **Line 6** ignites. All six lines burn. The Fire Eye is fully open. |

### 7.2 Dragon to the Throne (CANON, one clarification PROPOSED)
1. 75:00: The Fire Dragon lands at (-8, 80, 332).
2. Elias steps onto it. The Dragon lifts. A single wide flight over the whole world: lanterns, structures, planets, the Eye.
3. The Dragon lowers its head at the **foot of the Throne stairs** (THR-02). *PROPOSED clarification: the Dragon drops him at the foot, and Elias climbs the stairs on foot (the existing Throne doc calls the climb "the build-up").*
4. The Dragon withdraws and stays near, lowered, watching.

### 7.3 The climb (about 90 s)
| What happens | Detail |
|---|---|
| Elias walks up the long staircase of broken black stone | Walk only; no dash |
| **Braziers on both sides ignite as he passes** | Each brazier lights when Elias is within 2 m. They stay lit. |
| The backrest rises out of frame | Camera stays behind him and tilts up as the Throne grows |
| Wind drops steadily | The sound strips to a single drone and footsteps on stone |
| At the top | Elias stands before the seat. The Throne does **nothing** until he stops. |

---

## 8. The Throne sequence, exactly (about 6 minutes)
Seat at (0, 80, 350), yaw 180 degrees (faces back across the world). Sit trigger radius 2.0 m.

| Time | What the player does | What the world does | Camera | Sound |
|---|---|---|---|---|
| 77:20-78:10 | Stands before the Throne. May walk around. | Throne dormant: six fissures dark, cracks faintly warm. **It reacts to nothing.** When Elias stops for 2 s, the Cinder drifts toward the seat. | Low, behind Elias, tilting up the 40 m monolith | Wind, drone, footsteps |
| 78:10 | **Presses Interact to sit** (the only moment of pure choice) | Elias turns, lowers into the deep seat, hands on the armrests | Close, over the shoulder | Wind drops to near nothing |
| 78:10-78:40 | Nothing. He is still. | The **Cinder dissolves into his suit**: seams light for the first time. The still beam from Stage 1 completes its transfer into him. | Close on his chest, then slow pull back | A single clear tone |
| 78:40-79:10 | | **The six fissures ignite bottom to top**, one every 5 s. Each makes one rising bronze note (a six-note ladder). The two dragon ribs begin to glow between them. | Camera rises with each fissure | Six rising bronze notes over deep sub-bass |
| 79:00-79:30 | | **Braziers on the whole staircase flare**. Embers stream upward. The Fire Eye **opens fully**. The six sky lines **cascade-replay** bottom to top as the Throne's fissures finish | Pull back and up until Elias is a speck | Eye-open chord rises over 4-6 s (`AUDIO_END_EyeOpenChord`) |
| 79:10-81:30 | | **The Ring of Fire** begins at the seat (`IgniteNode_ThroneRoot`) and spreads outward along structures, bridges, platforms and lantern anchors by earliest arrival time. It reads as **activation**, not destruction: internal circuitry waking up, no explosions, no debris. | Wide world shot (0, 120, 310) | Rolling harmonic, spatialised along the spread |
| 81:30-83:30 | | **Lanterns ignite in sequence**, then **all together** at stable maximum. Architecture glows with fire veins. Planets reflect firelight. The Dragon lowers its head. | Lines and Eye shot (0, 180, 320) | Lantern chimes by distance, then one unison chord (`AUDIO_END_HarmonyMax`: harmony 0.65, drone 0.35, wind 0.55) |
| 83:30-84:30 | | The Fire Eye **slowly closes**. Glow settles to a steady warmth. | Slow pull away | Harmony decays to 0 over 40-60 s (`AUDIO_END_HarmonyDecay_ToWind`), then wind only |
| 84:30-85:00 | | Fade out | Hold on the wide shot | Wind only |
| 85:00 | | **I-RULE01 COMPLETE.** No speech, no lore dump. | Black | Near silence |

### Ending timeline in seconds from the sit (the 360 s budget)
| Seconds | Event |
|---|---|
| 0-60 | Sit, Cinder dissolves, six fissures ignite, Eye opens, first spread begins (seconds counted from the sit at 78:10) |
| 60-170 | Propagation and the lantern sequence |
| 170-210 | Harmony peak, all lanterns together |
| 210-270 | Propagation completes |
| 270-330 | Eye closes, harmony decays |
| 330-360 | Fade out |

### Throne states for VFX
1. **Dormant:** fissures dark, cracks faintly warm.
2. **Progress:** 1-5 fissures lit (follows the lines).
3. **Ignited:** all six blazing, dragon ribs glowing, braziers lit, embers streaming up.

### Note on the six lines
Line 6 ignites at the end of Stage 6, so the six sky lines are *already lit* when Elias sits. At the sit the lines **replay a full bottom-to-top cascade** in sync with the fissures. This is the reconciliation between the Stage 6 doc and the ending doc.

---

## 9. Sound map across the journey
| Moment | Wind | Drone | Harmony | Noise | Pulse | Notes |
|---|---|---|---|---|---|---|
| Island 1 open | 0.75 | 0 | 0 | 0 | 0 | Wind only |
| Walking, calm | 0.75 | to 0.25 | 0.15 when aligned | max 0.12 | 0 | Clarity tone |
| Rushing | falls | | | up | | Entropy: dust and noise creep in |
| Shadow forms | 0.5 | one held low tone | 0 | 0 | 0 | Single low tone |
| Fight | 0.6 | 0.35 | 0 | rising to 0.4 | 0 | Tension bed |
| Meditate hold | 0.3 | 0.2 | soft | 0 | heartbeat | Everything strips |
| Vision: Clash | | | | rising | rising | Percussion and bronze impact |
| Vision: Stop | | | | 0 | heartbeat only | One clear tone |
| Vision: Dissolve | | | rising | 0 | | Chord resolution over 4 s |
| Stage 6 hold | 0.70 | 0.10 | 0.10 | 0 | 0 | Silence bias |
| Throne sit | near 0 | | | 0 | | Six rising bronze notes |
| Ring of Fire | 0.55 | 0.35 | up to 0.65 | 0 | | Spatialised spread |

---

## 10. What the developer builds (by system)
| System | Needed for | Notes |
|---|---|---|
| **ForcingIndex and Creative Energy Cycle** | Everything | See [core systems](06-core-systems.md). Build first. |
| **Stillness detection and MeditateHold** | Island 1, every column, Stage 6 | Debounce 0.20 s; calm pockets 0.12 s |
| **ArmsRing component** | Stages 1 and 3-5 | Three orbiting weapons, a selected one in hand, diegetic, no HUD |
| **Still Ring item** | Island 1 | Floats, selectable only when conditions in 4.3 are met |
| **Encounter director (state machine E0-E9)** | Island 1 | One per encounter; checkpoint at E2 |
| **Unbroken Shadow AI** | Island 1 | Mirror, split, re-form, freeze under Meditate |
| **Meditation float and vision Sequencer** | Island 1 and any later Duel | Uses the existing meditation animation |
| **Danger-edge volumes and soft reset** | Every island | Cloud fade, return to last safe ground |
| **Staircase and brazier triggers** | Throne | 2 m trigger per brazier |
| **IgniteNode graph and Ring of Fire** | Ending | Throne root, earliest arrival, All Together event |
| **Debug HUD** | Tuning | F1-F4 as in core systems |

### Playtest questions to log
- Time from the Shadow forming to first stillness attempt.
- How many Arms the player tries before the Ring appears.
- How often the hold is broken during the vision.
- Whether players understood "stop" without text.

---

## 11. Decisions needed from the project owner
| # | Decision | Default used here |
|---|---|---|
| 1 | Approve the Stage 1 encounter (changes "no enemies in Stage 1") | Approved in this draft |
| 2 | Arms: names and count | Sacred Arc, Ember Blade, Bronze Lance (placeholders) |
| 3 | The last tool's name and look | Still Ring: floating bronze ring |
| 4 | Is the vision **interactive** or **cinematic** | Cinematic with a required hold |
| 5 | Vision length | 35 s |
| 6 | Does the Duel return later | Optional Duel-lite in Stage 3, echo in Stage 6 |
| 7 | Does the Dragon drop Elias at the stairs or at the seat | At the foot of the stairs; Elias climbs on foot |
| 8 | Camera in the vision | Third person, cinematic cuts |

Related: [Stage 1](stages/stage-1-lurking.md) · [Core systems](06-core-systems.md) · [Enemies](05-enemies.md) · [The Throne](08-the-throne.md) · [Ending](stages/the-throne-ending.md) · [Canon and open decisions](13-canon-and-open-decisions.md)
