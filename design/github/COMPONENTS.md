# X1 GitHub Visual Components

## Component families

The README visual system is built from reusable component families. Individual repositories may vary the content but not the underlying geometry.

## 1. Hero

Purpose: brand, product identification and product classification.

Mandatory on primary repositories.

## 2. Status strip

A compact line immediately under the hero.

Recommended fields:

`PUBLIC / PRIVATE` · `RELEASE STATE` · `SELF-HOSTED / MANAGED` · `PRIMARY STACK`

Keep this factual. Do not use status labels that imply runtime verification without evidence.

## 3. Capability cards

Recommended layout: 2 × 2.

Each card contains:

- short uppercase micro-label
- capability title
- one sentence
- optional simple signal glyph

Use cards to explain the product quickly, not to list every feature.

### Card typography / overflow guard

For README command or capability decks using four cards around 330–340 px wide, use this GitHub-safe baseline:

- micro-label: **10.5 px**, letter-spacing no more than **1.5 px**;
- capability title: **17 px**; use **16 px** for unusually long titles;
- supporting copy: **12.5 px**;
- horizontal process strap: **10.5 px**, letter-spacing no more than **2 px**;
- inner horizontal text margin: at least **22–26 px**.

**GitHub rendering rule:** set `font-size` and `letter-spacing` directly on every SVG `<text>` element that participates in a card. Do not rely on embedded `<style>` selectors to resize README SVG text. GitHub image rendering/sanitization and browser font substitution can make CSS-based typography behave differently from the source preview.

No text may cross a card boundary or visually collide with the next card. If copy does not fit inside the safe card width, shorten it, reduce a long title to the 16 px exception, or deliberately split it into controlled lines. Never rely on clipping and never allow text to overflow into an adjacent card.

Check the rendered SVG at GitHub README display width, not only at the native 1600 px canvas size. The source must remain safe even when the preferred font is substituted.

## 4. Operational flow

A horizontal or vertical process diagram.

Examples:

`PAIR → DELIVER → ACK → OBSERVE → VERIFY`

`INGEST → VALIDATE → NORMALIZE → PRESERVE → PUBLISH`

`CONFIGURE → AUTHORIZE → DELIVER → MONITOR`

Rules:

- same line weight throughout
- one active signal color
- no ornamental arrows without meaning
- every step should be an actual system state or action

## 5. Authority / boundary card

Used for security, responsibility or trust boundaries.

Typical format:

- left: what X1 controls
- right: what remains external/operator-owned
- central dividing signal line

Use this instead of long disclaimer walls where possible.

## 6. Screenshot frame

For UI products.

Presentation rules:

- current real product screenshot
- crop tightly around the application
- no desktop/browser clutter unless relevant
- optional dark X1 frame
- concise caption below
- do not use fake data that could be mistaken for production evidence

## 7. Repository relation card

Use near the bottom to show related X1 systems.

Maximum 3–5 links. Avoid reproducing the entire ecosystem in every repository.

## 8. Community CTA

Canonical destinations:

- Website — `https://x1panel.space`
- Forum — `https://forum.x1panel.space`
- Store — `https://store.x1panel.space`
- Discord — `https://discord.gg/vSSw6jHmw`
- Telegram — `https://t.me/+XkuQS_QuD6g4Nzc0`

For public repositories, Forum / Discord / Telegram should normally be visible.

For private repositories, only include community links where they serve the product.

## 9. Footer

Canonical footer block:

`X1 // SOFTWARE · SYSTEMS · OPERATIONS`

`PUBLIC SOFTWARE. PRIVATE ENGINEERING. ONE X1 IDENTITY.`

`© X1Tech Solutions SA · All Rights Reserved`

No hard-coded year.

## Badge policy

External shields may still be used for factual technical metadata such as build status, release, language or license.

Do not use shields.io as the primary navigation or brand system.

Brand/navigation CTAs should be plain linked text or X1-owned visual assets.

## Diagram evidence policy

A diagram may explain intended architecture, but must not falsely imply runtime proof.

Use words carefully:

- `DESIGNED` for architecture intent
- `IMPLEMENTED` for source present
- `TESTED` for reproducible test evidence
- `RUNTIME VERIFIED` only when observed in a real runtime
- `PRODUCTION VERIFIED` only with genuine production evidence
