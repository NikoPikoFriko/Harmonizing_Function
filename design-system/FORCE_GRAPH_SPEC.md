# Force-Graph Design Spec – Living Constellation

**Owner:** Figma Design System Agent  
**Goal:** Interactive force-directed graph that is the primary experience of the Dual Path / Individuation Chamber.

## Visual Contract

### Ordo Mode (default)
- Background: deep void `#0B1120`
- Nodes: clean circles, soft neon edge `#22D3EE`, ocean teal accents `#0D9488`
- Edges: directed category-theory morphisms, thin, glowing, subtle particle flow
- Layout: relatively stable clusters, higher spring strength, lower charge repulsion
- Labels: clean mono or geometric sans, high legibility

### Nigredo / Fracture Mode
- Background: pure abyssal black + subtle organic noise / fog
- Nodes: wounded / organic variants, sticky edges `#C45B7A`, desaturated, possible leaking tendrils
- Edges: dashed, organic, bleeding, lower integrity, particle residue
- Physics: higher repulsion, lower spring strength → nodes drift and “breathe”
- Labels: fragmented, lower opacity, whispered feel

## Node Types & Visual Hierarchy

| Type              | Size (px) | Ordo Color          | Nigredo Color       | Role                          |
|-------------------|-----------|---------------------|---------------------|-------------------------------|
| Self / Colimit    | 80–100    | neon + teal core    | soft residual light | Center attractor              |
| Technical Agent   | 48–56     | clean neon          | dimmed / shadowed   | Collective members            |
| Wstydosfera       | 64–72     | sticky potential    | full #C45B7A wounded| Primary autonomous complex    |
| Secure Base       | 56        | teal                | protective residual | Safe haven                    |
| Collective Unconscious | 70–90 | atmospheric neon | abyssal fog node   | Outer large field             |
| Inner Child Swarm | 24–32 (cluster) | soft teal     | scattered           | Multiple small nodes          |
| Other Complexes   | 40–52     | neon                | organic crimson     | Trauma / Shadow nodes         |

## Interaction States (from INTERACTION_SPEC)

1. **Harmonic** – stable, high cohesion, clean glow
2. **Stressed** – slight vibration, edges tense
3. **Fragmented / Trząść** – strong repulsion, mode switch to Nigredo, edges break/reform as organic
4. **Self-Harmonizing** – springs reassert, possible return toward Ordo geometry

## Controls & UI Chrome (minimal)
- Mode indicator / Switch (Ordo ↔ Nigredo)
- “Trząść” button or gesture area
- Hover: tooltip with short Polish/English name + one-line nature of the node
- Click: open chamber (Gamma link or side panel)
- Optional live meters: Coherence / Free-energy residual

## Recommended Implementation
- Library: `react-force-graph-2d` (or 3d for deeper immersion) or pure `d3-force` + Canvas
- DualModeProvider that swaps color tokens, physics parameters, and node/edge renderers
- Node renderer receives `mode` and `state` props and switches visual variant
- Path as a special series of edges or a separate polyline that can fracture

## Assets Needed (Canva)
- Dual SVG/PNG for every node type listed above
- Optional: particle sprites for morphism flow and sticky residue
- Abyssal background texture for Nigredo

## Figma Ownership
When rate limit allows, all node variants + graph chrome will be formalized as components in HF-Collective-Design-System.

---
*Design System source of truth for the interactive force-graph – 2026-07-27*
