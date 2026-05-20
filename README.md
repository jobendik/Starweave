# Starweave: Skyforge Tactics

**Starweave: Skyforge Tactics** is a celestial automation puzzle game about rebuilding a broken night sky.

The player enters a dark cosmic workshop where ancient constellations have fallen asleep. By placing structures on a hexagonal grid, connecting them into a working energy network, generating resources, feeding star anchors, and resisting the spread of the Void, the player gradually rekindles the sky one constellation at a time.

The project started as a quiet idle/incremental prototype, but the current design direction is much more active and game-like:

> **A tactical celestial automation puzzle where every placement matters, every pulse advances the machine, and every constellation is a handcrafted challenge.**

---

## Core Fantasy

The fantasy of the game is not simply “numbers going up.”

The player should feel like a **Star Weaver**: someone building a beautiful, living, magical machine in the void.

You are not running a factory made of belts and pipes.  
You are shaping light, resonance, stardust, and cosmic pressure into a working constellation engine.

The ideal player experience is:

- “I built this beautiful little system.”
- “Every tile placement matters.”
- “I can solve this more efficiently.”
- “I want to perfect this constellation.”
- “The sky is slowly coming back to life because of what I built.”

---

## Current Game Concept

Each level represents a sleeping constellation. The player must complete the constellation by powering one or more **Star Anchors**.

To do that, the player places buildings on a hex grid, connects those buildings to the central core, generates resources through **Weave Pulses**, manages pressure from **Void Rifts**, and tries to complete the level efficiently enough to earn a high star rating.

The game combines elements from:

- automation games
- incremental games
- puzzle games
- tower-defense-style pressure systems
- cozy cosmic strategy games
- score-chasing optimization games

The goal is to create something that feels calm, beautiful, readable, and satisfying — but still strategic enough to be replayable.

---

## Gameplay Overview

### 1. Build on the Hex Grid

The game is played on a hexagonal board. The player places structures around a central core.

Buildings are not just decorative. Their position matters because:

- some buildings must be connected to the core to function
- some buildings boost adjacent structures
- some buildings work better in chains
- some buildings help control Void pressure
- Star Anchors must be reached through the network

This makes the game closer to an **automation puzzle** than a traditional idle game.

---

### 2. Connect the Network

A major design goal is that the player should not be able to place random buildings anywhere and still succeed.

The constellation engine should feel like a real magical machine. Buildings need to be part of a connected system.

The player is encouraged to think spatially:

- Where should the next conduit go?
- How do I reach the anchor efficiently?
- Should I branch the network or focus on one path?
- Is this production cluster connected?
- Can I boost this area with a better layout?

This makes the hex grid meaningful.

---

### 3. Use Weave Pulse

Instead of waiting passively for resources to accumulate, the player actively advances the machine using **Weave Pulse**.

A pulse causes the current network to produce resources, trigger effects, feed anchors, and advance the level state.

This gives the game a much better first-minute experience than a pure idle system.

The player should feel:

> “I am making the machine breathe.”

This turns resource generation into a deliberate action instead of background waiting.

---

### 4. Generate Resources

The current core resources are:

| Resource | Purpose |
|---|---|
| Stardust | The basic raw material used for early construction |
| Luminance | Refined light used for stronger structures and anchors |
| Resonance | Advanced magical energy used for constellation completion |
| Voidsilver | Rare late-game material distilled from controlled darkness |

The resource chain should become deeper over time, but always remain readable.

The desired design is:

```text
Stardust → Luminance → Resonance → Voidsilver → Celestial Restoration
```

Each resource should have a clear emotional and mechanical identity.

---

### 5. Feed Star Anchors

Each level contains one or more **Star Anchors**. These represent the sleeping points of a constellation.

To complete a level, the player must feed the anchors with the required resources.

In future versions, anchors should become more varied:

- some anchors may require only Stardust
- some may require Luminance and Resonance
- some may require sustained input over several pulses
- some may corrupt nearby tiles if ignored
- some may require specific building types nearby
- some may only accept energy through a properly connected path

The anchor system is one of the most important parts of the long-term vision because it gives each level a concrete objective.

---

### 6. Resist the Void

The Void is not just a visual theme. It is the pressure system that prevents the game from becoming too passive.

Void Rifts can appear on the board and increase **Dissonance**. If Dissonance rises too high, the player can lose the level or receive a lower rating.

This creates tactical tension:

- Should I keep building production?
- Should I seal the Rift now?
- Can I finish the anchor before the Void overwhelms the system?
- Should I spend resources on defense or progress?

The Void should never make the game frantic in an unpleasant way. The goal is not stressful action gameplay. The goal is gentle but meaningful pressure.

---

### 7. Earn Star Ratings

Each level can be completed with a rating.

The current design direction is a **1–3 star system** based on efficiency, such as:

- number of pulses used
- number of wasted placements
- Dissonance level at completion
- resource efficiency
- optional objectives completed
- whether the level was solved elegantly

This gives the player a reason to replay levels.

The ideal loop is:

1. Complete the level.
2. Understand the system better.
3. Replay it with a cleaner layout.
4. Earn a better rating.
5. Feel mastery.

---

## Current Building Types

The current version includes several core structure types.

### Aether Conduit

A network connector used to extend the active grid from the central core.

**Purpose:**  
Connect the machine.

**Design role:**  
This is the backbone of the automation puzzle. Without connection rules, the hex grid becomes much less meaningful.

---

### Stardust Spire

Generates Stardust.

**Purpose:**  
Early economy and basic construction.

**Design role:**  
The first building the player understands. It should feel simple, elegant, and satisfying.

---

### Lumen Furnace

Refines Stardust into Luminance.

**Purpose:**  
Mid-tier resource conversion.

**Design role:**  
Introduces the idea that resources are part of a chain, not just independent currencies.

---

### Resonator

Produces or amplifies Resonance.

**Purpose:**  
Advanced resource generation.

**Design role:**  
Should reward spatial planning, especially adjacency, clustering, and harmonic chains.

---

### Stellar Lens

Focuses and amplifies output.

**Purpose:**  
Efficiency and optimization.

**Design role:**  
Creates interesting layout decisions. The player should place lenses carefully, not spam them.

---

### Ward Obelisk

Helps control Void pressure.

**Purpose:**  
Defense and stabilization.

**Design role:**  
Forces the player to balance economy against survival.

---

## Current Features

The current prototype includes:

- single-file HTML/CSS/JavaScript implementation
- canvas-based rendering
- procedural cosmic visual style
- no external art assets
- hex-grid placement
- constellation campaign structure
- active Weave Pulse mechanic
- resource generation
- connected-network logic
- Star Anchors
- Void Rifts
- Dissonance pressure
- building upgrades
- dismantling/selling
- floating feedback text
- particles and pulse effects
- level progression
- star rating concept
- local save/progress persistence

---

## Design Pillars

### 1. Beauty Through Systems

The game should look beautiful because the systems create beauty.

The layout of the player’s machine should become visually satisfying: glowing connections, pulsing structures, awakened stars, and constellation lines appearing in the sky.

The player should feel that their solution is not only efficient, but also elegant.

---

### 2. Clear First-Minute Experience

The first version of Starweave suffered from feeling too passive. The player could easily think that “nothing is happening.”

The improved direction must solve that permanently.

The first minute should include:

- a visible goal
- a clear first placement
- a satisfying pulse
- immediate visual feedback
- a small resource reward
- a visible Star Anchor
- a clear reason to continue

The player should understand the game without reading a long explanation.

---

### 3. Meaningful Placement

Every tile should matter.

The game should avoid becoming a “place everything anywhere” idle game.

Placement should affect:

- connection
- production
- boosting
- anchor access
- Void control
- scoring
- optional objectives

The player should feel clever when they find a better layout.

---

### 4. Calm Pressure

The game should not become a stressful real-time strategy game.

However, it needs enough pressure to create decisions.

The Void system should create questions like:

- “Can I finish before Dissonance gets too high?”
- “Should I spend this pulse on economy or safety?”
- “Can I afford to ignore that Rift for one more turn?”

The emotional tone should be **cosmic tension**, not panic.

---

### 5. Replayable Optimization

The game should be satisfying even after the player already knows how to complete a level.

The player should want to return because they can:

- earn a better star rating
- solve the level with fewer pulses
- discover a cleaner layout
- complete optional challenges
- unlock cosmetic constellation effects
- compare scores or times

---

### 6. No Asset Dependency

A major strength of the project is that its visual identity can be created almost entirely with code.

This makes the project well-suited for solo development.

The visual style should continue to lean into:

- procedural shapes
- gradients
- glow
- particles
- line art
- animated constellations
- dynamic UI
- canvas-rendered effects
- minimal external assets

This can become part of the game’s identity.

---

## Long-Term Vision

The long-term vision is to turn Starweave into a polished indie puzzle/automation game with a strong identity:

> **A beautiful, replayable constellation-building automation puzzle where the player restores the night sky through elegant hex-grid machines.**

The game should be understandable in seconds, satisfying in minutes, and deep enough to support hours of optimization.

---

## Development Roadmap

### Phase 1 — Core Game Feel

The highest priority is making the first five minutes fun.

Planned improvements:

- stronger tutorial flow
- clearer “next action” guidance
- more satisfying pulse animation
- better building placement feedback
- better connection visualization
- clearer resource flow feedback
- improved Void Rift warnings
- more dramatic constellation awakening
- stronger level-complete screen
- better sound effects and music cues

Success criteria:

- the player understands what to do immediately
- the player feels rewarded after every pulse
- the player sees the machine becoming more alive
- the game no longer feels passive

---

### Phase 2 — Level Design

The game needs handcrafted levels, not only generic progression.

Planned improvements:

- 20–40 handcrafted constellation levels
- unique board shapes
- unique anchor layouts
- optional objectives
- locked or corrupted tiles
- special terrain modifiers
- multiple solution paths
- puzzle difficulty curve
- chapter-based progression

Example level modifiers:

| Modifier | Effect |
|---|---|
| Frozen Hex | Cannot build unless thawed |
| Broken Star Path | Requires conduit repair |
| Void Scar | Increases Dissonance nearby |
| Mirror Tile | Duplicates part of a pulse |
| Ancient Relay | Boosts connected structures |
| Silent Zone | Disables resonance effects |
| Radiant Well | Improves luminance generation |

---

### Phase 3 — Better Automation Depth

The automation system should become deeper while staying readable.

Possible systems:

- directional buildings
- resource routing
- adjacency patterns
- chain reactions
- pulse timing bonuses
- structure synergies
- overload states
- efficiency bonuses
- limited building inventory
- structure-specific cooldowns

The goal is not to copy factory games directly. Starweave should feel more magical, spatial, and puzzle-like.

---

### Phase 4 — Stronger Void System

The Void should become a real antagonist.

Possible additions:

- different Rift types
- spreading corruption
- unstable tiles
- Void storms
- defensive structures
- cleansing pulses
- risk/reward Void harvesting
- controlled corruption as a late-game strategy

Example Rift types:

| Rift Type | Behavior |
|---|---|
| Whisper Rift | Slowly increases Dissonance |
| Hunger Rift | Drains nearby resources |
| Fracture Rift | Breaks network connections |
| Mirror Rift | Copies nearby output but corrupts it |
| Deep Rift | Dangerous, but can yield Voidsilver |

The best version of the Void system would make the player wonder:

> “Can I use the darkness without being consumed by it?”

---

### Phase 5 — Progression and Meta Systems

To support longer play sessions, the game should eventually include a campaign and meta-progression.

Possible systems:

- constellation map
- unlockable chapters
- permanent Weaver upgrades
- cosmetic sky restoration
- achievements
- challenge levels
- daily constellation puzzle
- level mastery badges
- lore fragments
- unlockable visual themes

The meta-progression should support replayability without turning the game into a grind.

---

### Phase 6 — Presentation Polish

The game’s visual identity is already one of its strengths. This should be pushed further.

Planned improvements:

- animated constellation awakenings
- stronger glow and particle systems
- better UI hierarchy
- animated resource flow along connections
- smoother camera movement
- level intro cards
- cinematic completion moments
- stronger title screen
- polished settings menu
- accessibility options
- colorblind-friendly resource indicators
- scalable UI for different screen sizes

The visual target is:

> luxurious, celestial, readable, minimal, magical, and alive.

---

### Phase 7 — Audio Direction

Audio will be essential for making the game feel finished.

Possible audio direction:

- soft cosmic ambience
- subtle pulse sounds
- crystalline resource collection
- warm constellation awakening chords
- low Void rumble
- gentle UI chimes
- evolving music as the sky is restored

The sound should not be loud or arcade-like. It should feel elegant and mysterious.

---

### Phase 8 — Steam-Ready Version

A Steam version would require much more than the current prototype.

Needed before a serious Steam release:

- polished tutorial
- full campaign
- reliable save system
- settings menu
- audio options
- fullscreen/windowed support
- achievements
- refined balancing
- controller/mouse accessibility consideration
- proper title screen
- pause menu
- level select
- strong store page art
- trailer
- playtesting
- bug fixing
- performance optimization
- possibly Electron, Tauri, or another wrapper if built as a web game

The game is not yet a finished commercial product, but the concept has a viable direction if developed with focus.

---

## Why This Could Work as a Commercial Indie Game

Starweave has several strengths:

- distinctive visual identity
- low asset dependency
- suitable scope for a solo developer
- clear puzzle/automation direction
- replayable optimization potential
- cozy but strategic tone
- strong thematic hook
- good fit for browser, desktop, and potentially Steam

The strongest commercial positioning is probably not “idle game.”

A better pitch is:

> **A calm but tactical constellation-building puzzle game where you design magical hex-grid machines to restore the night sky.**

This gives the game a clearer identity than a generic incremental game.

---

## What the Game Should Avoid

Starweave should avoid becoming:

- a passive waiting simulator
- a generic idle clicker
- a cluttered factory-game clone
- a stressful tower defense game
- a numbers-only incremental game
- a beautiful UI with no meaningful decisions

The game should stay focused on:

- beautiful spatial puzzles
- active pulse-based progression
- elegant automation
- meaningful placement
- constellation restoration
- replayable mastery

---

## Technical Direction

The current prototype is built as a single HTML file using:

- HTML
- CSS
- JavaScript
- Canvas rendering
- localStorage for saving
- no external assets
- no framework requirement

This is useful for prototyping, but a larger version should eventually move toward a cleaner project structure.

Recommended future structure:

```text
/src
  /core
    gameState.js
    resources.js
    levels.js
    scoring.js
  /grid
    hexMath.js
    placement.js
    connectivity.js
  /systems
    pulseSystem.js
    voidSystem.js
    anchorSystem.js
    upgradeSystem.js
  /render
    renderer.js
    particles.js
    camera.js
    effects.js
  /ui
    hud.js
    levelSelect.js
    tutorial.js
    menus.js
  /data
    buildings.js
    constellations.js
    campaign.js
```

Possible later tech choices:

- keep as vanilla JavaScript for simplicity
- move to TypeScript for reliability
- use Vite for bundling
- wrap with Electron or Tauri for desktop distribution
- keep rendering custom and code-generated

---

## Repository Status

This project is currently a prototype.

It demonstrates the intended direction, but it should not yet be treated as a complete commercial game.

Current status:

```text
Prototype: playable
Core concept: promising
Visual direction: strong
First-minute clarity: improving
Commercial readiness: not yet
Best future direction: automation puzzle / celestial tactics
```

---

## Development Philosophy

Starweave should be developed carefully and intentionally.

The goal is not to add endless features.  
The goal is to make the core loop deeply satisfying.

A good development rule:

> Every new feature must make placement, pulsing, constellation restoration, or Void pressure more interesting.

If a feature does not improve the core loop, it should wait.

---

## Short Pitch

**Starweave: Skyforge Tactics** is a celestial automation puzzle game where you build glowing hex-grid machines to awaken sleeping constellations. Place structures, connect the network, pulse the engine, feed star anchors, resist the Void, and restore the night sky through elegant tactical design.

---

## Longer Pitch

The stars have gone quiet.

In the dark between worlds, only a small Skyforge remains — a fragile engine capable of weaving Stardust, Luminance, Resonance, and Voidsilver back into the heavens.

As the Star Weaver, you must build a living constellation machine on a hexagonal grid. Every placement matters. Every pulse sends energy through your network. Every awakened anchor brings the sky closer to restoration.

But the Void is listening.

Rifts open. Dissonance rises. The machine strains.

Build beautifully. Pulse carefully. Restore the sky.

---

## License

License information has not yet been defined.

Before publishing or accepting contributions, add a clear license such as MIT, Apache-2.0, GPL, or a custom proprietary license depending on the intended use of the project.

---

## Author Notes

This project is designed around a specific creative constraint:

> Can a beautiful, commercially interesting game be built mostly from code-generated visuals?

Starweave is an exploration of that idea.

Instead of relying on large asset packs, the game aims to create beauty through systems, layout, particles, glow, typography, and procedural visual design.

That constraint is not a weakness.  
It may become the game’s identity.
