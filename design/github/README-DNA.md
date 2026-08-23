# X1 GitHub Visual DNA v2

## Authority

This document is the visual authority for X1 GitHub profile and repository README presentation.

The goal is not to make every repository identical. The goal is to make every X1 repository immediately recognizable as part of one engineering ecosystem.

## Core principle

**ONE X1 IDENTITY. DIFFERENT PRODUCTS.**

Every repository keeps its own product name, capability story and operational diagrams, while sharing the same X1 visual shell.

## Mandatory README hierarchy

1. X1 hero
2. product/status strip
3. one-sentence positioning statement
4. product visual, screenshot or system diagram
5. core capabilities
6. architecture / operational flow
7. quick start or usage
8. security / responsibility boundary
9. related X1 systems
10. community / support
11. X1 footer

Sections may be omitted when genuinely irrelevant, but the visual hierarchy must remain consistent.

## Visual language

- dark enterprise background
- restrained cyan as the primary X1 signal
- electric blue as secondary signal
- violet reserved for private/internal engineering accents
- glass-like dark cards with thin luminous borders
- minimal glow; never arcade/neon overload
- strong uppercase micro-labels
- concise large headlines
- diagrams built from the same shapes, spacing and line weights
- no random gradients, badge palettes or unrelated icon styles

## Public / commercial / internal distinction

### Public / Community

Use cyan-dominant accents.

Labels:

- `PUBLIC / FREE`
- `COMMUNITY`
- `SELF-HOSTED`
- `BUILT TO BE USED`

### Commercial / Private

Use cyan + electric blue.

Labels:

- `COMMERCIAL / PRIVATE`
- `PROTECTED ENGINEERING`
- `BUILT TO OPERATE`

### Internal Engineering

Use cyan + restrained violet.

Labels:

- `PRIVATE ENGINEERING`
- `CONTROLLED ACCESS`
- `INTERNAL SYSTEM`

## Product individuality

A repository may have its own secondary symbol, diagram and product-specific phrase.

Examples:

- TiviMate: device pairing / state verification
- XCIPTV: application control / configuration
- Smarters: runtime delivery / validation
- WAVEO: state / acknowledgement / verification
- EPG: ingest / validate / preserve / publish
- Picons: identity / artwork / provenance
- Stream Manager: configure / authorize / deliver / monitor

The product-specific visual must live inside the X1 shell, not replace it.

## X1 signature language

Preferred system phrases:

- `SOFTWARE · SYSTEMS · OPERATIONS`
- `PUBLIC SOFTWARE. PRIVATE ENGINEERING. ONE X1 IDENTITY.`
- `EVIDENCE > ASSUMPTION`
- `CONTROL → OBSERVE → VERIFY`

Do not force all phrases into every repository. Use only what is relevant.

## README density

A README must scan well before it reads well.

Rules:

- keep the first screen visually decisive
- avoid large walls of text directly below the hero
- use one visual every 2–4 major sections when useful
- use tables only when comparison benefits from them
- prefer short capability blocks over long marketing prose
- avoid repeating the same claim in multiple sections

## Screenshots

Repositories with a real UI should show a current product screenshot near the top.

Preferred order:

`HERO → POSITION → PRODUCT SCREENSHOT → CAPABILITIES`

Data/tooling repositories may use architecture or data-flow diagrams instead.

## SVG rules

- preferred canvas: 1600 × 420–520 for hero art
- corner radius: 24–32 px
- 1–2 px structural strokes
- 2–4 px active signal strokes
- avoid text below 13 px on 1600 px canvas
- no external fonts required
- use system-safe font stacks
- every SVG must include a useful `aria-label`

## Footer authority

Canonical footer:

**X1 // SOFTWARE · SYSTEMS · OPERATIONS**

`PUBLIC SOFTWARE. PRIVATE ENGINEERING. ONE X1 IDENTITY.`

Website · Forum · Store · Discord · Telegram

**© X1Tech Solutions SA · All Rights Reserved**

Do not hard-code the year in new GitHub README footers.

## Change control

Before a major visual redesign is propagated across repositories:

1. implement it first in `x1-dotcom/x1-dotcom`;
2. review it as the reference implementation;
3. only then propagate the approved pattern;
4. preserve product-specific content and runtime truth;
5. do not rewrite technical claims merely to make visual copy more uniform.
