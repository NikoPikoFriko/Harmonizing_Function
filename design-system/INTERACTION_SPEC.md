# Interaction Spec: Self-Balancing Compartmentalization

## Core Metaphor
Kompartmentalizacja (protective, executive-preserving structure) vs Fragmentacja (loss of control / executive function).

The visual system is a living force-directed graph of the psyche.

## States

### 1. Harmonic / Compartmentalized (Rest State)
- Nodes clustered into functional compartments: Executive Core, Emotional Regulation, Trauma Vault (contained), Creative Flux, Relational Interface.
- Strong attractive forces within compartments, moderate between.
- Edges (morphisms) smooth, high glow, stable thickness.
- Low noise, soft teal/neon harmony.
- Harmony Score high (0.8–1.0).

### 2. Stressed
- Increased mouse velocity or moderate clicking.
- Edges begin to tense/wave.
- Nodes vibrate slightly.
- Glow intensifies unevenly.

### 3. Fragmented Chaos (High Entropy)
- Rapid mouse shaking + high click rate injects entropy.
- Repulsive forces dominate.
- Edges break or become dashed/particle trails.
- Nodes scatter, lose cluster identity.
- Visual glitch, high frequency noise, desaturated or flickering neon.
- Harmony Score low (0–0.3).
- Executive function visually "lost" (core node dimmed or disconnected).

### 4. Self-Harmonizing Recovery
- When input entropy drops, restoring springs + damping activate.
- Nodes slowly re-cluster into original compartments.
- Broken edges reform with progressive glow.
- System always tends toward the harmonic attractor (self-balancing).

## Technical Requirements for Implementation
- Real-time physics (Verlet or Euler integration with springs, charge repulsion, damping).
- Mouse force field + click impulse as entropy source.
- Harmony index computed from average edge integrity + cluster cohesion.
- Visual parameters driven by harmony index (glow, stroke, particle density, noise amplitude).
- Responsive, 60fps target, WebGL or high-performance Canvas preferred.

## Design Tokens Reference
See /design-tokens/colors.json
Primary: deep-void #0B1120, ocean-teal #0D9488, graph-neon #22D3EE

## Figma Ownership
Prototypes of all 4 states + component variants will live in HF-Collective-Design-System as single source of visual truth.
