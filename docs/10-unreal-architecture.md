# Unreal Engine architecture

**Engine:** Unreal Engine 5. **Platform:** PC (Steam) first; console is future scope.

| Area | Choice |
|---|---|
| Rendering | Lumen and Nanite where performance allows, scaled back for mid-range hardware |
| Camera | Camera / Spring Arm (smooth follow and aim, pitch clamp) |
| Input | Enhanced Input System (controller and KBM, rebind-ready) |
| Audio | MetaSounds (adaptive layered mix) |
| Language | C++ for core systems; Blueprints for content and orchestration |

## Core systems
| System | Responsibility |
|---|---|
| **CreativeEnergyController** | Invisible Actor Component tracking ForcingIndex and Entropy / Freshness / Beauty; drives all world responses without any UI |
| **SkyLadderController / HexagramController** | Six mesh line-bars with dormant and ignited materials; persistent across level loads; always framed in view; orchestrates unlocks |
| **CinderGuidance** | Vector-based logic replacing NavMesh for guidance; clean visual cues, no navigation clutter |
| **FireEyeController** | Progressive pupil activation, brightness curves and ray emission per line ignition |
| **AudioStateController** | Three-layer mix (wind, harmony, distortion) driven by the creative state |
| **StageDirector** | Stage timelines, beat events, stage-specific input locks |
| **IgnitionController** | Column holds, stillness requirement, line ignition event |
| **StormSystem** | Storm triggers, cover and calm-pocket resets |
| **BridgeBuilder (Stage 4)** | Builds bridge segments only while the player is still |
| **RingOfFire** | IgniteNode graph propagation for the ending |

## Data-driven design
The original spec was written in Unity terms. Translate to Unreal like this:

| Source term | Unreal equivalent |
|---|---|
| ScriptableObject (SO_GameConfig, SO_CreativeCycleWeights, SO_StageConfig, SO_EnemyConfig, SO_WorldFeedbackConfig, SO_TimelineBeatList) | `UDataAsset` / `UPrimaryDataAsset` |
| MonoBehaviour | `AActor` / `UActorComponent` |
| Prefab | Blueprint Actor |
| AnimationCurve | `UCurveFloat` |
| Trigger volume | `ATriggerVolume` / box component |

Source Y-up positions become Unreal Z-up (see [world design](03-world-and-level-design.md)).

## Asset strategy
- Modular **floating island kits** reused across all six stages.
- A reusable obsidian-and-bronze material library.
- Lighting quality over asset quantity.
- All world objects are reusable Blueprint actors orchestrated by the sky-ladder controller.
- No water systems, no vegetation shaders, no city assets.
- Every stage has an expected failure loop with a soft-reset anchor.

## Geometry kit (blockout names)
Ground plates (L 32x32, M 16x16, long 12x36), void-gap modules, monolith slabs (S/M/L), moving and pulse platforms, bronze spans, XL lantern anchors, ignition columns and stage gates, bridge builder segments (4 m / 8 m), heat-current volumes, throne zone.
