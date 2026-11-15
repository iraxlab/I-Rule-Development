# The Throne

> The Throne is not a prize. It is a recognition. When Elias sits, he is not defeating anyone: he is completing himself.

## Status
**Final numbers: [doc 40](40-throne-blueprint.md).** The approved look is the new `art/assets/THR-01/sheet.jpg`.

**Redesigned. New renders pending.** The legacy key art ([art/throne](../art/throne/throne-final-activation-legacy.jpg)) shows an earlier, simpler throne and is superseded by the design below. Drop approved new renders into [`art/throne/`](../art/throne/README.md).

## Design brief (locked)
The Throne must look **hard, dark, fiery, mysterious and very tall**, matching the approved key art: black volcanic stone, aged bronze, molten-amber cracks, heavy ancient surfaces. It must be unmistakably a throne at first glance, and it must feel outstanding and never seen before.

| Element | Specification |
|---|---|
| **Height** | About **40 m**. A tiny figure at its base must make the player feel small. |
| **Seat** | Deep, massive block of black volcanic stone with two thick armrests |
| **Backrest** | A very tall, narrow **monolith** with straight parallel sides and a flat notched top |
| **Six fissures** | **Exactly six** equally spaced short **horizontal glowing amber bars** across the backrest like a ladder of fire: the six lines |
| **Dragon ribs** | **Three** colossal curved bronze ribs on each side (six in all), tapering like tusks, rising beside the seat and arching inward without touching, fire glowing between them: ties the Throne to the Fire Dragon. (Changed from two to match the approved sheet.) |
| **Approach** | A long, steep staircase of broken black stone with bronze braziers burning on both sides: the climb is the build-up |
| **Surface** | Rough, weathered; molten-amber cracks veining through dark stone like lava under a crust |
| **Never** | Modern, glossy, chrome, mirror-polished, minimal, floating on rods; no skulls, no wings, no readable text |

> **Lesson learned:** an earlier "mirror-black, polished, frozen wave, floating, rods" description rendered as a sleek modern chair. Lead with *ancient, hewn, volcanic, molten cracks, staircase, scale*.

## Why it feels outstanding: the world answers the player
The Throne is a **progress bar the size of a tower.** It is visible from the first island with six faint lines barely glowing.

| Beat | What the player sees |
|---|---|
| **First sight** | A dark monolith on the far summit; six faint fissures. A promise. |
| **Ignition ladder** | Each time a line is completed, one fissure ignites. Seen from every island. |
| **Midpoint** | Four fissures lit: the silhouette now burns like a ladder in the sky. |
| **The climb** | The summit staircase: braziers light as the player passes each one; the backrest rises out of frame. |
| **The turn** | When the sixth fissure ignites, lanterns, bridges and islands turn their light toward the Throne. The Dragon lowers its head. The Eye closes. |
| **The seat** | Sitting is the payoff. The camera pulls far back and up until the figure is a speck against a 40 m monolith in full blaze, then the world goes still. |

This is the "ego payoff": the whole world is built to face the player at the end. See [ending sequence](stages/the-throne-ending.md).

## Placement and interaction
- Source layout: seat at (0, 80, 350), yaw 180 degrees (faces back across the world). Sit trigger radius 2.0 m.
- The Throne **does nothing until the player stops.** Pressing to sit is the only moment of pure choice at the end.
- Ring of Fire root node: `IgniteNode_ThroneRoot` at the seat.
- End camera markers: wide world (0, 120, 310) looking at (0, 0, 0); lines and Eye (0, 180, 320) looking at (0, 320, 0).

## States (for VFX / materials)
1. **Dormant:** all fissures dark; cracks faintly warm.
2. **Progress:** 1-5 fissures lit according to lines ignited.
3. **Ignited:** all six blazing, dragon ribs glowing, every brazier lit, embers streaming upward: calm, stable, overwhelming.

## References and prompts
- [Throne Wow Direction PDF](../design/Throne_Wow_Direction.pdf): design intent, wow moments and Gemini prompts (hero low angle, scale shot, the seat, turnaround, ignition states).
- [3D Reference Prompt Pack](../art-pipeline/3D_Reference_Prompt_Pack.pdf): THR-01 (11 views), THR-02 stairs and platform, THR-03 throne on summit, plus detail prompts (six fissures, dragon ribs, seat and armrest, ignited state). Throne reference sheets use a **mid-gray backdrop with amber rim light** so dark edges and glowing cracks are both visible.
