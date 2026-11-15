# Production plan

## Build order (locked)
Movement first. If movement or stillness does not feel right, **stop and fix it before proceeding.**

1. Movement feel (camera, inertia, responsiveness): **gate 1**
2. Alignment and stillness mechanic
3. Cinder behaviour (drift, brightness, meditation lock)
4. Hexagram line ladder system (six bars, toggle ignitions)
5. Stage 1 (dark ignition)
6. Stage 2 (timing and direction gating)
7. Glass Shadow enemy
8. Entropy storm feedback and Storm Wraith system
9. Stage 3 arena (anti-spam combat loop)
10. Bridge build system (Stage 4)
11. Heat currents and Dragon traversal (Stage 5)
12. Stage 6 stillness peak
13. Throne and Ring of Fire world ignition sequence
14. Audio layering pass (must start early, not last)

## Vertical slice sprint plan (8 weeks, 4 phases)
| Phase | Weeks | Title | Deliverables |
|---|---|---|---|
| 1 | 1-2 | Foundation | Player controller, alignment detection, stillness timer, camera rig |
| 2 | 3-4 | Core loop | Stage 1 environment, Cinder behaviour, Line 1 VFX, audio pass |
| 3 | 5-6 | Conflict | Glass Shadow AI, Entropy storm mechanics, combat tuning, fire arrows |
| 4 | 7-8 | Polish | Audio layering, Dragon presence, optimisation, Steam demo build |

**Milestone:** a playable, shippable Steam demo by week 8.

## Demo scope: options (decision open)
| Option | Scope | Length | Source |
|---|---|---|---|
| **Core Proof** (GDD) | Stage 1 complete, compressed Stage 3 combat trial, Line 1 and 2 ignition, Glass Shadow, Entropy storm and calm reset, Cinder, Fire Eye presence, fire arrows. Dragon teased, Throne silhouette only. | 15-20 min | GDD |
| **Core Proof B** | Stages 1-3, Dragon flyover, Throne silhouette reveal and end card (S1 7:00, S2 6:00, S3 7:00, tease 2:00) | 22 min | Spec |
| **Compressed Six** | All six stages shortened to 3-5 min each; Stage 6 hold reduced to 6 s (demo only); end shows Ring of Fire start then title | 25-30 min | Spec |
| **Vertical slice (brief)** | Stages 1-3 | 30-40 min | Pitch brief |

**Demo success metric:** a new player, with no tutorial, discovers through play that rushing fails and stillness wins. If they need to be told, the demo has failed. See [open decisions](13-canon-and-open-decisions.md).

## Team (5-7 core)
| Role | Responsibilities |
|---|---|
| Creative Director | Vision, mechanics, narrative systems, art direction |
| Lead Gameplay Programmer | Player controller, CreativeEnergyController, state machine, combat |
| Technical Artist | VFX, fire shaders, line effects, Fire Eye, Dragon visuals |
| Environment Artist | Modular island kits, obsidian / bronze materials, lighting |
| Sound Designer | Adaptive audio, ignition chords, storm / calm responses |
| Animator (optional) | Elias movement blend tree, Dragon flight cycles |
| QA / Playtester | Vertical slice acceptance, Steam demo QA |

## Budget estimates (indie-realistic)
| Milestone | Scope | Estimate |
|---|---|---|
| Vertical slice / Steam demo | 8 weeks, 5-person core | $150,000 - $300,000 |
| Full game (6 stages) | 6-8 months, lean burn | $400,000 - $800,000 |

The same world kit scales all stages. Grant funding of $25,000-$50,000 covers concept to first playable Stage 1 slice only (see [funding](14-funding-and-submission.md)).

## Scope risks and guards
- **"By-seconds for the whole game"** can become rigid. Allow loops and failure correction (every stage has one).
- **Hidden-state feedback** fails if too subtle or too loud. Use the three feedback layers on every mechanic.
- **Lighting quality over asset quantity.** One biome, modular kits.
- Console is future scope.

## Definition of done for the first playable (Stage 1)
- Movement feel signed off by the playtest question.
- Player can discover, with no text, that standing still reveals the ignition.
- Rushing for about 30 s produces entropy; stopping 2 s restores calm.
- Line 1 ignites bottom bar; lantern anchor flickers alive; exit opens.
- Debug HUD available (dev-only).

## Rules applied
Applied 15 Nov 2026 from [doc 32](32-rules-of-successful-games.md).

1. **The first playable is the Minimum Awesome Product (PY-D3, PY-D4).** The smallest thing that makes a stranger say "awesome" and want more. Cut anything that does not serve it.
2. **Grey-box first, one mechanic at a time (UN-2, UN-3).** Test each before the next, in the locked build order.
3. **Watch strangers (PY-D2).** Test with 5 new players for each build. Watch. Do not explain. People do not say what they think.
4. **Test two things apart (PY-D6).** The feel of the control, and the feeling of progress.
5. **Six numbers only (PY-K6).** Time to first stillness realisation, time to first Line, stage completion, rewinds per bridge, where players quit, and return rate on the demo.
6. **Guess first (PY-K8).** Before each feature, each person writes which numbers will move and by how much. Compare after.
7. **Pivot meetings (PY-D7 to PY-D9).** Fix a date at the end of each sprint phase. Name what we will test and what result decides.
8. **NOW and LATER (PY-D11).** A feature is NOW or LATER, never IN or OUT.
9. **Data beats rank (PY-D12).** Any team member can challenge a feature with playtest data.
10. **Small tests with a goal (FP-14, FP-X1).** Name the number before the test. Try to prove our own idea wrong.
11. **Streamable moments (PY-K5).** Build moments that look great in a clip: a bridge forming, the Dragon's wind, a Line lighting.
12. **Honest store page (PY-K4).** Show the real game. Ask happy players for a review through the store.
13. **Ethics (PY-E1 to PY-E3, PY-E6).** No tricks, no random paid items, no manipulation. The game is premium.
