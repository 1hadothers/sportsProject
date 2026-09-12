---
name: tennis-board-design
description: Visual design system for a tennis scoreboard UI. Use when styling or building the look of a tennis scorekeeper app.
---

## Purpose
Define the visual style for a tennis scoreboard: layout, colors, type, and motion.

## When to Use
When building or restyling the UI of a tennis scorekeeper app.

## Design Direction
- **Vibe**: Broadcast-style. Clean, bold, high-contrast, like a TV match scoreboard.
- **Layout**: Two horizontal player rows stacked vertically. Name on the left, score on the right. Sets and games columns in the middle. Server dot next to the serving player's name.
- **Colors**: Dark navy background `#0B1220`. White text. Player 1 accent `#00E0A4` (mint). Player 2 accent `#FF5C7A` (coral). Active server dot glows in the accent color.
- **Typography**: System font stack. Player names in bold uppercase, letter-spaced. Points in huge numerals (clamp 3rem–6rem). Sets/games in smaller muted gray.
- **Motion**: When a point is scored, the number pops (scale 1 → 1.15 → 1 over 200ms). No other animation. Keep it snappy.

## Concrete Step
Create `styles.css` that lays out the board as a full-viewport grid with two player rows, applies the color palette and typography above, and adds the point-pop animation. Wire it to the scoreboard's existing DOM.\