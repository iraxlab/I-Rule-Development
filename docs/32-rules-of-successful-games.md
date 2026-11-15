# 32 Rules of successful games

| Code | Book | Best for |
|---|---|---|
| GF | Game Feel, Steve Swink | How controls and feedback feel |
| PY | The Pyramid of Game Design, Nicholas Lovell | Loops, sessions, retention, making and launching |
| FP | Design Rules for Free-to-Play Games, Lovell and Fahey | First minutes, fairness, generosity, learning from players |
| UN | Unity All-In-One, Patrick Felicia | Building order, AI, feedback, difficulty |

**I-RULE01 column:** Fits = already in the game. Check = look at it. Not for us = true for free games, not for a premium Steam game. The engine is Unreal, so UN gives the idea and not the code.

## 1. The 12 master rules
| # | Master rule | From | I-RULE01 |
|---|---|---|---|
| M1 | Make the control feel good first. Nothing else saves a bad feel. | GF, PY | Check: stillness is the control (section 11) |
| M2 | Answer every input within 100 ms. | GF | Check |
| M3 | The first 10 minutes must be fun, not a lesson. | FP, PY | Fits: the bow lesson on ENV-01 |
| M4 | Never tell the player "you are not good enough". | FP | Fits: Cinder catch |
| M5 | Easy to start, deep to master. | GF, FP | Fits: chord, Still Path |
| M6 | Reward every good move with sound, light and motion. | FP, GF, PY | Fits: chord notes |
| M7 | Build short loops inside long loops. | FP, PY | Fits: bridge, island, stage |
| M8 | Let the player stop and let them come back. | PY | Check: save points |
| M9 | Look, sound, motion and rules must say the same thing. | GF | Fits: the look bible |
| M10 | Show the player what is new, why it matters and what it gives. | PY | Check |
| M11 | Put a small real version in front of players early. Learn. | PY, FP | Check |
| M12 | Never trick the player. Be open about what they buy and get. | PY, FP | Fits |

## 2. Game Feel rules (GF)
The book calls game feel three things together: real-time control, a simulated space, and polish that stresses each touch.

| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| GF-1 | Predictable results | The same input gives the result the player expects. | Check |
| GF-2 | Kill control ambiguity | Two buttons pressed together must never give a random result. | Check: stick drift vs stillness |
| GF-3 | Avoid state overload | Too many states on one button feels random. Make each state change easy to see. | Fits: few verbs |
| GF-4 | Stage the result | Make each input result clear. One idea at a time. Exaggerate with particles. | Fits |
| GF-5 | Hook in two minutes | Feel is the first loop the player meets. If it feels bad, they leave. | Check |
| GF-6 | Teach by inference | One hole that kills teaches "holes kill". Predictable means the player can guess what they have not tried. | Fits |
| GF-7 | Respond fast | A result by 70 to 100 ms feels instant. Over 100 ms feels laggy. | Check |
| GF-8 | Know the human clock | Seeing takes about 100 ms, thinking 70, moving 70. Past 240 ms the sense of control breaks. | Check |
| GF-9 | Hold the frame rate | 10 fps is the least for motion. 20 is better. 30 is smooth. | Fits: PC target |
| GF-10 | Easy but deep | Low skill floor, high skill ceiling. | Fits |
| GF-11 | Use natural mappings | Stick direction = move direction. Use the standard keys. | Fits |
| GF-12 | Add depth with a record | Showing the time of an action makes players want to beat it. Leaderboards make the ceiling endless. | Check |
| GF-13 | Keep it fresh | The same canned animation 10,000 times gets dull. Vary it. Add new mechanics as the game goes. | Fits: new rules per stage |
| GF-14 | Make the response lovely alone | Control should be a joy to play with in an empty room. | Check |
| GF-15 | Spend time on failure | Make crashes and falls varied and fun to watch. Players spend much time there. | Check: bridge breaks |
| GF-16 | Move in arcs | Curved motion looks alive. Move with forces, not by setting a position each frame. | Check |
| GF-17 | Keep harmony | Look, sound, motion, physics and rules must tell one story. Keep one level of detail across them. | Fits |
| GF-18 | Prefer iconic over photo-real | A cartoon or iconic world is easier to make feel right than a real one. | Fits: mythic look |
| GF-19 | Small slips add up | Clipping through walls, loose planks flying away: each one breaks the world a little. | Check |
| GF-20 | Aim for ownership | Mastery lets players improvise and express themselves. That is what makes them replay and tell friends. | Fits: Still Path |
| GF-21 | Polish sells the touch | Sound, dust, shake and weight cues tell the player how heavy or light a thing is. Match them to the animation. | Fits |
| GF-22 | Metaphor sets expectations | What a thing looks like tells the player how it should move. | Fits |
| GF-23 | Rules change the feel | A reward for coins changes how steering feels. Test rules with the control. | Check |
| GF-24 | Space gives control meaning | Level layout and collision decide how good a move feels. Space things so players can chain moves. | Fits: islands |
| GF-25 | Measure the feel | Judge input, response, context, polish, metaphor and rules. Then "floaty" and "tight" mean something. | Check |

## 3. The Pyramid rules (PY): shape of the game
| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| PY-1 | Layers, not separate games | Base layer (moment to moment), retention layer (progress), superfan layer (hobby). It is one game. | Fits |
| PY-2 | A good base layer is fun, replayable, connected and unpredictable | It must link to the retention layer so progress is felt. | Check |
| PY-3 | Unpredictability has three sources | Random chance, other players, and emergent systems. Too much random makes actions feel pointless. | Check |
| PY-4 | Fun is needed but not enough | Do not rely on "be really fun" alone for a long life. | Fits: progress layer |
| PY-5 | Give progress a face | Players need to see they moved forward. | Fits: six lines of fire |
| PY-6 | Do not assume skill is wanted | Many successful service games downplay skill. Know your audience. | Fits: our skill is calm |
| PY-7 | Connect base and retention in a "gearbox" | Fun in the moment must feed the long goal. | Fits |
| PY-8 | Use a pre-event screen | Before the action: show goals, progress and choices. | Check: stage cards |
| PY-9 | Use a post-event screen | After the action: celebrate, show reward, offer the next step. Make failure feel like progress. | Check |
| PY-10 | Use ceremony | Celebrate wins with animation, art and sound (Bejeweled, Peggle). | Fits: Line lights |
| PY-11 | Use the three razors | Before building a feature ask: will the player see it, understand it, and value it? | Check |
| PY-12 | Give the player a special world | Pre and post screens can follow the hero's journey. | Fits |
| PY-13 | Have an end only if the game suits it | Free games work best endless. Narrative games hit a wall there. | Fits: we end at the Throne |
| PY-14 | Narrative keeps players | "What happens next?" is the oldest trick. Leave something hanging. | Fits |
| PY-15 | Humans finish what they start | Loops, open quests and collections use this. Use with care. | Fits |

## 4. The Pyramid rules (PY): retention menu
The book lists 18 ways to keep players. Pick a few. Do not use all.

| Code | Technique | One line | I-RULE01 |
|---|---|---|---|
| PY-R1 | Be really fun | The base. Risky alone. | Fits |
| PY-R2 | High score | Beat your last best. | Check |
| PY-R3 | Persistent high score | Always show the best. | Check |
| PY-R4 | Leaderboards | Beat others. Suits achievers and competitors. | Check |
| PY-R5 | Seasons | Reset boards so players return. | Not for us |
| PY-R6 | Levels | Clear chunks. | Fits: 6 stages |
| PY-R7 | Getting to the end | Finish the game. | Fits |
| PY-R8 | Levelling up | A number that rises feels like progress. | Fits: chord |
| PY-R9 | Progress across a map | Seeing yourself move on a map. | Fits: islands |
| PY-R10 | Loops | Humans like to finish. | Fits |
| PY-R11 | Real time | Time passing inside the game. | Not for us |
| PY-R12 | Appointment mechanics | Timers that call players back. | Not for us |
| PY-R13 | Narrative | A cliffhanger pulls players back. | Fits |
| PY-R14 | Stars | 1 to 3 stars show how well you did. | Check: Still Path |
| PY-R15 | Stars as currency | Stars unlock more. | Check |
| PY-R16 | Challenges | Short temporary tasks. | Check |
| PY-R17 | Achievements | Permanent, once only. | Check |
| PY-R18 | Social | Friends, rivals, sharing. | Check |

## 5. The Pyramid rules (PY): the session
| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| PY-S1 | The session is the unit | The player chooses to come back now. That choice is the real battle. | Check |
| PY-S2 | Attention is scarce | The big challenge is getting players to want to play at all. | Fits |
| PY-S3 | Onboarding is not the on-ramp | Onboarding teaches once. The on-ramp makes it easy to start every time. | Check |
| PY-S4 | Pass the Starbucks test | Something meaningful inside the time a coffee takes. | Check: fast resume |
| PY-S5 | The session-length paradox | Promise a short session and the real session gets longer. | Check |
| PY-S6 | Design the off-ramp | Signal that the main tasks are done. Let people stay. Plant a hook to return. | Check: save points |
| PY-S7 | Give a welcome back | Make coming back feel good. | Check |
| PY-S8 | Build hooks into the core | Players should return because they want to, not because they were bribed. | Fits |
| PY-S9 | Test hooks after soft launch | Add bribes only after you know the game keeps people without them. | Not for us |
| PY-S10 | Add light relief | Pleasant, low-pressure tinkering gives ups and downs. Narrative games need less of it. | Check: calm pockets |

## 6. The Pyramid rules (PY): money and superfans
For a premium game, only a few apply.

| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| PY-M1 | Free beats cheap | Competing with free is the real rival. | Not for us |
| PY-M2 | Variable pricing | Players who love the game can spend more. | Not for us |
| PY-M3 | Averages mislead | A few big spenders warp the average. Look at groups. | Not for us |
| PY-M4 | Superfans are a hobby | They play your game more than any other. Serve them. | Check: Still Path |
| PY-M5 | Sell display, agency and permanence | Goods work when others can see them, they do something, and they last. | Not for us |
| PY-M6 | Do not call players whales | The word dehumanises them. Call them superfans, and make things people love. | Fits |
| PY-M7 | Do not call cosmetics vanity | The book prefers "self-expression items". Do not belittle players. | Not for us |
| PY-M8 | Freeloaders are valuable | They spread the word and fill the world. | Not for us |
| PY-M9 | Compete, do not sue | Respond to free copies with a better game. | Fits |
| PY-M10 | Ads are an option when people will not pay | Know the backlash risk. | Not for us |

## 7. The Pyramid rules (PY): making and launching
| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| PY-D1 | Nobody knows anything | Learn fast whether it is fun. Do not guess. | Fits |
| PY-D2 | Get it into real players' hands | People do not say what they think or do what they say. Watch them. | Check |
| PY-D3 | Four minimums | Feasible: can we make it. Viable: will people pay. Desirable: will they want it. Awesome: smallest thing that delivers the vision and makes players say "awesome". | Check |
| PY-D4 | Aim for the Minimum Awesome Product | Cut scope until only the awesome part is left. | Check |
| PY-D5 | Prototype to learn | A prototype is not the base of the product. Hack it. Do not future-proof. | Fits |
| PY-D6 | Prototype each layer | Test the base layer and the retention layer separately. | Check |
| PY-D7 | Pivot only with a reason | If you did not set out to learn it, it is a mistake, not a pivot. | Fits |
| PY-D8 | Use the scientific method | Guess, test, record, change. | Check |
| PY-D9 | Hold a pivot meeting | Fix a date to decide. | Check |
| PY-D10 | Five phases | Concept, production, launch (soft launch first), live, sunset. | Check |
| PY-D11 | NOW and LATER, not IN and OUT | Ideas not needed now go to LATER. Nobody has to defend them to death. | Fits |
| PY-D12 | Beware the loudest boss | A high-status leader raises both the risk and the hit chance. Let the team challenge. | Check |
| PY-D13 | Ban alpha and beta | Say what you mean. Name the test and the audience. | Fits |
| PY-D14 | Seasonal events come last | Do them only when the game already works. | Not for us |
| PY-D15 | Plus it | Build on an idea. Do not kill it. | Fits |
| PY-D16 | Write first, edit later | Make freely. Cut hard afterwards. | Fits |
| PY-D17 | Do not kill ideas early with analysis | Most ideas wither alone. | Fits |
| PY-D18 | Find local maxima | Squeezing metrics can trap you on a small hill. Sometimes make a big change. | Check |

## 8. The Pyramid rules (PY): marketing, metrics, ethics
| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| PY-K1 | Ban the word "tutorial" | The first experience shows the fun and earns the next 30 seconds. Learning is part of fun. | Fits |
| PY-K2 | Win high-quality players | Players who like the game matter more than many who do not. | Check |
| PY-K3 | Value must beat cost | Lifetime value must be more than cost to get the player. | Not for us |
| PY-K4 | Reviews matter | A middling store score cuts downloads. Ask happy players to review. | Check: Steam |
| PY-K5 | Reach influencers | Videos and streams have a huge passive audience. | Check |
| PY-K6 | Watch six or seven numbers | Too many metrics hide the signal. | Check |
| PY-K7 | Track retention by cohort | Look at groups of players by start day. Day 1, 7 and 30. | Check |
| PY-K8 | Play the guessing game | Before a feature, each person guesses which numbers will move. Compare. | Check |
| PY-K9 | Remember the compound metric | One number made of many parts can hide what drives it. | Check |
| PY-E1 | Ethics: intent, method, outcome | Is the goal fair, the method honest, the result harmless? | Fits |
| PY-E2 | Never deceive | Tricking players into buying is always wrong. | Fits |
| PY-E3 | Be open about hooks | Rewards that train behaviour are fair only if overt and harmless. | Fits |
| PY-E4 | Show how much was spent | Spending totals help players stay aware. | Not for us |
| PY-E5 | Publish drop rates | Laws are heading that way. | Not for us |
| PY-E6 | Protect the vulnerable | Children and people who cannot pay need care. | Fits |
| PY-E7 | Respect the player's time | Give clear off-ramps. | Check |
| PY-E8 | No right answer, only trade-offs | Choose the trade-offs that suit your game. | Fits |

## 9. Free-to-play rules (FP)
The 15 rules of the book. The ones about money do not apply to a premium game. The ones about fun, fairness and learning apply to all.

| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| FP-1 | Make it fun | Worry about fun before anything else. Fun is in the thumbs of the player. If they enjoy it, it is fun. | Fits |
| FP-2 | The Starbucks test | Something fulfilling in a few minutes. Short loops draw people back. | Check |
| FP-3 | Come for a minute, stay for an hour | A tight loop at the heart, then loops that last 30 minutes, three days, three weeks. | Fits |
| FP-4 | Complexity in layers | Casual players win by turning up. Dedicated players find depth. No wrong way to play. | Fits |
| FP-5 | Never end | Evergreen games last. Narrative games find this hard. | Not for us |
| FP-6 | Be generous | Generous players tell friends. A paywall makes them leave. | Fits: Cinder, calm pockets |
| FP-7 | Be free forever | Let players enjoy it all without paying. | Not for us |
| FP-8 | The no-brainer first dollar | One cheap purchase that is clearly good value. | Not for us |
| FP-9 | Make it possible to spend $100 | Do not cap what fans can spend. | Not for us |
| FP-10 | Pizzazz, not polish | Spend effort on feedback that rewards the action. Leave a week at the end for it. | Fits |
| FP-11 | Kill the tutorial | Give a tour, not a lecture. Hint at depth. | Fits |
| FP-12 | I must not fail | Everyone makes progress. No game over screen. Players always see room to improve. | Fits |
| FP-13 | Sell emotion, not content | Give the content away. Sell self-expression, progress, power, status, relationships. | Not for us |
| FP-14 | Experiment and learn | Many small survivable tests, not one huge bet. Write down what you test. Try to disprove your pet idea. | Check |
| FP-15 | Development never ends | You run a service. Keep learning from players. | Not for us |

**Extra rules from the book's second part:**

| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| FP-X1 | A/B test with a goal | Decide the number before the test. Beware confirmation bias. | Check |
| FP-X2 | Players cost money | Lifetime value must beat cost per player. | Not for us |
| FP-X3 | Let players choose their own appointment times | Offer short and long timers. Never punish a trip away. | Not for us |
| FP-X4 | Serve all four player types | Achievers, explorers, socialisers, killers. | Check |
| FP-X5 | Think in a funnel | Acquire, retain, monetise. You lose people at each step. | Check |
| FP-X6 | Ship a minimum viable version | Make the cheapest test of "people will want this". | Check |
| FP-X7 | Follow the power law | A few spend a lot. Do not cut off either end. | Not for us |
| FP-X8 | Want true fans, not whales | A true fan feels proud of what they spent. A whale feels regret. | Fits |

## 10. Unity rules (UN): building the game
Unity is a different engine from Unreal. The ideas carry over. The code does not.

| Code | Rule | What it means | I-RULE01 |
|---|---|---|---|
| UN-1 | Use an engine's built-in tools | Common mechanics, preview scenes, easy export save time. | Fits: Unreal |
| UN-2 | Greybox the world with boxes first | Test movement and layout before art. | Check |
| UN-3 | Build one mechanic at a time | Movement, collect, score, scenes, then weapons, then AI. Test each. | Check |
| UN-4 | Give feedback for damage | A screen flash and a health bar for the player and the enemies. | Check |
| UN-5 | Use a state machine for behaviour | Patrol, chase, attack. Switch by distance or event. | Check: Glass Shadows |
| UN-6 | Give paths a cost | Make AI prefer or avoid areas, like swamp or danger. | Check |
| UN-7 | Use random waypoints | Variety makes movement less predictable. | Check |
| UN-8 | Spawn pressure over time | Adding enemies at steady intervals pushes the player to act. | Check |
| UN-9 | Help the player when they need it | When health packs run out, spawn one. | Fits: calm pockets |
| UN-10 | Vary the start | A random start position keeps replays fresh. | Check |
| UN-11 | Let players pick difficulty | Easy, medium, hard change NPC speed, spawn rate and damage. Save the choice. | Check |
| UN-12 | Add helpers | Allies that follow, attack or withdraw on command add a layer. | Fits: Cinder |
| UN-13 | Animate with blends | Blend trees make motion smooth between states. | Check |
| UN-14 | Smooth the camera | A smooth follow camera and effects add feel. | Check |
| UN-15 | Add abilities to widen play | Crouch, sprint and interact add variety. | Check |
| UN-16 | Learn by building | Do the exercises. Explain the work to others. Learn in chunks. Do not fear mistakes. | Fits |

## 11. What these rules say about I-RULE01
These are checks, not decisions. Each is **not decided yet**.

1. **Stillness is an input.** Stick drift must not break a bridge (GF-2). Give a small dead zone and say clearly what counts as still.
2. **Answer stillness fast.** The first rung should light within 100 ms of him stopping (GF-7). A 3 s hold needs a response that shows the count is running.
3. **Make failure worth watching.** Bridge breaks and falls should vary in look and sound (GF-15).
4. **Show a Still Path record.** Record the time or the number of clean builds per stage (GF-12), tied to the approved Still Path.
5. **Pre and post cards.** A short card before each stage and a ceremony when each Line lights (PY-8, PY-9, PY-10). The Line lighting already is the ceremony.
6. **Test with strangers early.** Put a small slice of Stage 1 and 2 in front of real players and watch (PY-D2, PY-D3).
7. **Keep it honest.** No tricks, no hidden costs (PY-E2).
8. **Watch the first 10 minutes.** The bow lesson and the first stillness bridge must be fun without a long lesson (FP-11, PY-K1).
