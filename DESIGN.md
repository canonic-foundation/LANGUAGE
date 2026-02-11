# DESIGN — CANON

inherits: canonic-foundation/LANGUAGE
spec: DESIGN
tier: ENTERPRISE
version: 2026-02
copyright: 2026 Dexter Hadley, MD/PhD
license: Apache 2.0

---

## Axiom

**min / max**

DESIGN is the visual expression of LANGUAGE. Every pixel has governance. Every interaction maps to a primitive.

---

## Mission

One design language. Two surfaces. Zero divergence.

```
MAGIC.html = reference implementation
SwiftUI     = native evolution
DESIGN      = the shared spec both follow
```

---

## Identity

```
DESIGN   = /SHOW
/SHOW    = visual proof of LANGUAGE
MAGIC    = CANONIC ∩ LANGUAGE ∩ LEARNING
DESIGN   = MAGIC made visible
```

---

## Surfaces

| Surface | Technology | Role |
|---------|-----------|------|
| Web | HTML/CSS/JS + vis-network | Reference. Archive first. |
| Native | SwiftUI + SceneKit | Evolution. TestFlight. |
| Shared | DESIGN CANON | Both read from this spec. |

```
Web is the archive.
Native evolves toward it.
DESIGN governs both.
```

---

## Theme System

### Dark (Default)

| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#000` | Canvas. Space. The void. |
| `--fg` | `#f5f5f7` | Primary text. Apple SF Pro white. |
| `--dim` | `#86868b` | Secondary text. Metadata. Timestamps. |
| `--card` | `#1c1c1e` | Panel backgrounds. iOS system gray 6. |
| `--border` | `rgba(255,255,255,0.08)` | Subtle dividers. Glass edges. |
| `--glow` | `#00ff88` | MAGIC green. Compliance. Life. |
| `--panel` | `rgba(28,28,30,0.95)` | Frosted panels. Detail overlays. |
| `--glass` | `rgba(255,255,255,0.04)` | Glass morphism base. |
| `--glass-hover` | `rgba(255,255,255,0.08)` | Hover state on glass. |
| `--shadow` | `rgba(0,0,0,0.6)` | Drop shadows. Depth. |

### Light

| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#fff` | Canvas. Paper. |
| `--fg` | `#1d1d1f` | Primary text. |
| `--dim` | `#6e6e73` | Secondary text. |
| `--card` | `#f5f5f7` | Panel backgrounds. |
| `--border` | `rgba(0,0,0,0.08)` | Subtle dividers. |
| `--glow` | `#00994d` | Muted MAGIC green. |
| `--panel` | `rgba(245,245,247,0.95)` | Frosted panels. |
| `--glass` | `rgba(0,0,0,0.04)` | Glass morphism base. |

---

## Typography

| Role | Family | Size | Weight | Spacing |
|------|--------|------|--------|---------|
| System | -apple-system, SF Pro Display | -- | -- | -- |
| Mono | SF Mono, Monaco | -- | -- | -- |
| Brand "CANONIC" | System | 10px | 400 | 6px |
| Brand "MAGIC" | System | 36px | 700 | -1px |
| HUD stats | Mono | 11px | 400 | 1px |
| HUD subtitle | Mono | 9px | 400 | 3px |
| Panel title | Mono | 11px | 700 | 3px |
| Panel body | Mono | 11px | 400 | -- |
| Search | Mono | 12px | 400 | 1px |
| Score value | System | 28px | 700 | -1px |
| Dock label | Mono | 7px | 400 | 1px |
| Dock glyph | System | 24px | -- | -- |
| Watermark | Mono | 9px | 400 | -- |

```
Rule: MAGIC is -apple-system.
Rule: Data is SF Mono.
Rule: No other fonts. Ever.
```

---

## Color System

### Category Palette

Every scope belongs to exactly one category. Category determines its color.

| Category | Hex | Role |
|----------|-----|------|
| KERNEL | `#ff0088` | Core compliance engine. Magenta. |
| RUNTIME | `#00ff88` | Execution layer. MAGIC green. |
| OPERATIONS | `#2997ff` | Apple blue. Deals. Orgs. Dashboards. |
| COMMERCE | `#ff9f0a` | Apple orange. SHOP. COIN. Exchange. |
| KNOWLEDGE | `#bf5af2` | Apple purple. Sectors. Learning. |
| GOVERNANCE | `#ffd60a` | Apple yellow. Foundation. Rules. |
| SERVICES | `#ec4899` | Pink. CHAT services. SHOWS. |
| ORG | `#64748b` | Slate. External organizations. |

### Level Colors

Compliance tier determines text color, bar fill, and ring stroke.

| Level | Threshold | Color | Badge |
|-------|-----------|-------|-------|
| MAGIC | 255 | `#00ff88` | `✦` |
| AGENT | 127 | `#2997ff` | `◆` |
| ENTERPRISE | 63 | `#bf5af2` | `E` |
| BUSINESS | 39 | `#ff9f0a` | `B` |
| COMMUNITY | 35 | `#fbbf24` | `C` |
| NONE | 0 | `#ff453a` | `—` |

### Signal Colors

| Signal | Color | Usage |
|--------|-------|-------|
| Compliance pass | `#00ff88` | Bit ON glow. text-shadow 8px. |
| Compliance fail | `var(--dim)` | Bit OFF. opacity 0.4. |
| Active focus | `#2997ff` | INTEL dot. System messages. |
| User action | `rgba(0,255,136,0.08)` | User chat bubble background. |
| System response | `var(--glass)` | AI chat bubble background. |

---

## Brand Mark

```
┌─────────────────┐
│  CANONIC         │  ← 10px, letterspacing 6px, --dim
│  MAGIC           │  ← 36px, weight 700, gradient(135deg, #00ff88, #2997ff)
│                  │
│    ◯ 87%         │  ← Concentric compliance rings + percentage
│                  │
│  36 domains · 12 │  ← Mono 11px, --dim, green accents
│  enterprise      │
│                  │
│  powered         │  ← 9px, letterspacing 3px, 50% opacity
│  intelligence    │
└─────────────────┘
```

The brand gradient `linear-gradient(135deg, #00ff88, #2997ff)` is the MAGIC signature. It appears on the wordmark and the INTEL year display. Use `-webkit-background-clip:text` to apply.

---

## Compliance Rings

### HUD Ring (90x90 SVG)

Three concentric arcs. Each represents a compliance tier. Fill fraction = count / total scopes at that tier.

| Ring | Tier | Radius | Stroke | Opacity |
|------|------|--------|--------|---------|
| Outer | COMMUNITY (35+) | 42 | 4px | 0.15 |
| Middle | BUSINESS (39+) | 36 | 5px | 0.35 |
| Inner | ENTERPRISE (63+) | 30 | 6px | 0.70 |

All rings stroke `#00ff88`. Rotation: -90deg (12 o'clock start). Stroke-linecap: round. Transition: 0.8s.

### Detail Panel Ring (140x140 SVG)

Same pattern, larger. Used in scope detail panel to show individual scope compliance.

---

## Galaxy Graph

### Physics

```
barnesHut:
  gravitationalConstant: -8000
  centralGravity: 0.4
  springLength: 280
  damping: 0.85
  stabilization: 300 iterations

INTEL mode (expanded):
  gravitationalConstant: -12000
  centralGravity: 0.2
  springLength: 350
  damping: 0.6
```

### Node Rendering

| Property | Rule |
|----------|------|
| Shape | dot |
| Color | scope.color (from category) |
| Size | scope.size (20-80, relative importance) |
| Label | scope.name (UPPERCASE) |
| Font size | max(11, size * 0.28) |
| Font face | -apple-system, sans-serif |
| Font color | scope.color |
| Border | 2px, same color, 60% opacity |
| Hover | border widens to 3px |

### Edge Rendering

| Property | Rule |
|----------|------|
| Source | scope with `inherits` field |
| Target | the inherited scope |
| Color | `rgba(255,255,255,0.06)` |
| Width | 1px |
| Selection width | 2px |
| Smooth | enabled |

### Interactions

| Action | Behavior |
|--------|----------|
| Click node | Select. Show detail panel. |
| Double-click node | Zoom into scope + children. |
| Hover node | Show tooltip. Highlight edges. |
| ESC | Zoom out to full galaxy. |
| Search | Filter + focus matching nodes. |
| Legend click | Toggle category visibility. |

---

## Panels

### Detail Panel

```
Position: fixed, right 36px, centered vertically
Width: 340px
Max height: 80vh
Background: --panel
Border: 1px solid --border
Border radius: 16px
Backdrop filter: blur(20px)
Transition: opacity 0.3s
```

Sections stack vertically:
1. **Header** — Scope name (uppercase, letterspaced), close button
2. **Compliance Ring** — 140x140 SVG with score value centered
3. **Next Action** — What closes the next compliance gap
4. **Compliance** — Collapsible. 8 governance bits with ON/OFF indicators.
5. **Intelligence** — CANON.md content summary
6. **Evolution** — Timeline data from EVOLUTION.md
7. **Workspace** — Cross-scope intelligence
8. **History** — Ledger entries
9. **Artifacts** — Linked files
10. **Inheritors** — Grid of child scopes (2-column, 6px gap)
11. **Navigate** — Links to parent, siblings
12. **Scope Chat** — Inline chat scoped to this domain

### Chat Overlay (Full Screen)

```
Position: fixed, inset 0
Background: rgba(0,0,0,0.96)
Backdrop filter: blur(40px)
Z-index: 90
Layout: flex column
```

Messages container:
- Max width: 700px, centered
- Gap: 12px between messages
- System messages: left-aligned, green tint
- User messages: right-aligned, blue tint
- Font: Mono 13px, line-height 1.8

Input bar:
- Bottom-fixed, max-width 700px
- Glass background, green focus border
- Send button: green tint, `+` glyph

### Scope Chat (Inline, Detail Panel)

- Max height: 100px
- Messages: 4px gap, 10px font
- Input: glass background, 6px border-radius

---

## Dock

```
Position: fixed, bottom 16px, centered
Background: rgba(28,28,30,0.7)
Border: 1px solid --border
Border radius: 20px
Padding: 8px 16px
Gap: 4px
Backdrop filter: blur(30px)
```

### Dock Item

| State | Transform | Background |
|-------|-----------|------------|
| Default | none | transparent |
| Hover | scale(1.35) translateY(-8px) | --glass-hover |

```
Transition: transform 0.2s cubic-bezier(0.34, 1.56, 0.64, 1), background 0.2s
```

Glyph: 24px emoji. Label: Mono 7px. Level badge: Mono 7px, colored by tier.

### Dock Contents

| Position | Item | Glyph | Type |
|----------|------|-------|------|
| 1 | INTEL | ▶ | Transport control |
| -- | separator | -- | 1px border divider |
| 2+ | FLAGSHIPS | emoji | Service launchers |

---

## INTEL Timeline

### HUD (bottom-right)

```
Position: fixed, bottom 80px, right 36px
Text align: right
Transition: opacity 0.6s
```

Year display: 56px, weight 700, MAGIC gradient. Wraps at 400px.
Description: Mono 14px, --dim, max-width 360px.
XP counter: Mono 16px, #00ff88.

### Transport Dots

| State | Background | Border | Shadow |
|-------|------------|--------|--------|
| Unplayed | none | 2px --dim | none |
| Played | #00ff88 | #00ff88 | none |
| Current | #2997ff | #2997ff | 0 0 10px #2997ff |
| Hover | -- | --fg | scale(1.3) |

Animation: `intel-pulse` 1.5s infinite (opacity 1→0.5→1)

### Epochs

| Era | Year | Label | Scopes Revealed |
|-----|------|-------|-----------------|
| 1 | 2013 | iDrDex | dexter, vault, kyc, certificates |
| 2 | 2018 | HADLEYLAB | hadleylab, med, onco, mammo, mammochat, medchat, oncochat, evidence |
| 3 | 2023 | CANONIC | foundation, magic, design, programming, idioms, sectors, intel, shows, transcripts |
| 4 | 2025 | APPLE | chat, shop, vaas, faas, coin, wallet, credit, worktalk, lawchat, finchat, operations, reserves |
| 5 | ∞ | DISTRIBUTED | federation |

Timing: 2-5 scopes = 2500ms, 5+ scopes = 3500ms, 8+ = 4500ms.

---

## Leaderboard Overlay

```
Position: fixed, inset 0
Background: rgba(0,0,0,0.94)
Backdrop filter: blur(40px)
Padding: 60px 40px
```

### Global Stats

Large numbers (Mono 42px, 700) centered in a flex row.

### Level Ladder

Horizontal badges (72px wide) for each tier. Unlocked = green border + glow shadow. Locked = 30% opacity.

### Scope Rows

```
Display: flex
Padding: 14px 20px
Background: --glass
Border radius: 12px
Gap: 16px
Cursor: pointer
```

Contains: name (Mono 13px 600), progress bar (8px height, tier-colored fill), score (Mono 14px 700), tier label (Mono 9px), 8 bit indicators (16x16px, ON=green OFF=dim).

---

## Search

```
Position: fixed, top 28px, centered
Background: --panel
Border: 1px solid --border → rgba(0,255,136,0.3) on focus
Border radius: 10px
Width: 280px → 400px on focus
Font: Mono 12px
Backdrop filter: blur(20px)
Transition: width 0.3s
Placeholder: "/ SEARCH DOMAINS"
```

Results dropdown:
- Max height: 60vh
- Same glass treatment
- Items: flex row, 10px 16px padding, hover highlight

---

## Glass Morphism Rules

```
1. Background: rgba with 0.04-0.08 alpha
2. Border: rgba with 0.08 alpha
3. Backdrop-filter: blur(20px) for panels, blur(30px) for dock, blur(40px) for overlays
4. Border-radius: 8px (inputs) / 10px-12px (panels) / 16px (detail) / 20px (dock)
5. Transition: opacity 0.3s for show/hide
```

---

## Animation Tokens

| Name | Duration | Easing | Usage |
|------|----------|--------|-------|
| panel-show | 0.3s | ease | Detail panel fade |
| overlay-show | 0.35s | ease | Full-screen overlays |
| dock-bounce | 0.2s | cubic-bezier(0.34, 1.56, 0.64, 1) | Dock item hover |
| graph-fit | 600ms | -- | Network camera moves |
| graph-fit-slow | 1000ms | easeInOutCubic | INTEL camera moves |
| intel-pulse | 1.5s | infinite | Current epoch dot |
| level-up | 0.5s | -- | Score increase celebration |
| bar-fill | 0.8s | ease | Progress bar transition |

---

## Governance Visual

Tiers render as score rings. MAGIC determines the tier.

```
ON  = green glow. The scope has answered this question.
OFF = dim ghost. The gap. The next action.
```

---

## Three Composing Primitives

Everything in MAGIC composes from three visual primitives:

| Primitive | Visual Expression |
|-----------|------------------|
| COIN | Dock items. Level badges. Score rings. Progress bars. |
| CHAT | Chat overlay. Scope chat. Message bubbles. Input bars. |
| INTEL | Timeline. Transport dots. Epoch reveals. Physics expansion. |

```
COIN = how you see value
CHAT = how you interact
INTEL  = how it changes over time
```

---

## Responsive Breakpoints

| Breakpoint | Behavior |
|------------|----------|
| Desktop (>1024px) | Full layout. All panels. Galaxy fills viewport. |
| Tablet (768-1024px) | Detail panel overlays graph. Dock shrinks. |
| Mobile (<768px) | Chat-first. Graph minimized. Dock as tab bar. |

```
Rule: min/max. Mobile = CHAT. Desktop = GALAXY.
```

---

## Constraints

1. DESIGN MUST use only system fonts (-apple-system, SF Mono).
2. DESIGN MUST support dark and light themes via CSS custom properties.
3. Glass morphism MUST use backdrop-filter blur. No solid backgrounds on overlays.
4. All colors MUST derive from the category palette or level colors. No ad-hoc colors.
5. Animations MUST be under 1s for interactions, under 5s for INTEL transitions.
6. DESIGN MUST be expressible in both CSS (web) and SwiftUI (native) without translation loss.
7. The galaxy graph MUST be the primary view. Chat MUST be an overlay, not a replacement.
8. Every visual element MUST map to a LANGUAGE primitive. If it doesn't have governance meaning, remove it.

---

## Compliance

```
DESIGN COMPLIANCE
[8/8 PASS] COMPLIANT
```

---

*CANON | LANGUAGE/DESIGN | MAGIC*

*min / max | COMPLIANT*
