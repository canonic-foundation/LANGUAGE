# LANGUAGE

inherits: canonic-foundation

---

## Axiom

**LANGUAGE speaks itself. PRIMITIVES power SERVICES. MAGIC validates.**

---

## SPEC

```
{SCOPE}  = SPEC
SPEC     = CANON.md + VOCAB.md + ROADMAP.md + COVERAGE.md + LEARNING.md + EVOLUTION.md + IDFs
TRIAD    = CANON.md + VOCAB.md + README.md
```

SPEC is the human entry point. Optional, open. EVOLUTION flows through SPEC.
TRIAD is the governance shape. CANON = law. VOCAB = terms. README = narrative.

---

## Primitives

```
COIN  → work/value (the unit)
CHAT  → communication (generates COIN)
EVO   → evolution (grows COIN)
```

---

## Services

```
VAULT  → stores COIN (private)
SHOP   → distributes COIN (public)
```

---

## Equations

```
{SCOPE}    = SPEC
COIN       = WORK
CHAT       = GENERATES COIN
EVO        = GROWS COIN
COMPLIANCE = COVERAGE + ROADMAP
EVOLUTION  = EPOCHS
LEARNINGS  = GRADIENTS
IDF        = Immutable Disclosure Fixture
EVIDENCE   = IDFs
VAULT      = STORES COIN
SHOP       = DISTRIBUTES COIN
```

---

## 255 Bits

```
Bit   Hex   Dimension    Check            Question
─── ───── ─────────── ──────────────── ─────────────────────────
  1  0x01  DECLARATION  CANON.md         What do you believe?
  2  0x02  EVIDENCE     IDF exists       What proves it?
  4  0x04  TEMPORAL     ROADMAP.md       When did it happen?
  8  0x08  RELATIONAL   inherits:        Who is involved?
 16  0x10  OPERATIONAL  MUST/SHOULD      How does it work?
 32  0x20  STRUCTURAL   ## Axiom         What shape is it?
 64  0x40  LEARNING     LEARNING.md      What patterns emerge?
128  0x80  LANGUAGE     VOCAB.md         How is it expressed?
─── ───── ─────────── ──────────────── ─────────────────────────
255  0xFF  MAGIC        all              all 8 answered
```

---

## Templates

### CANON.md

```
# {SCOPE} — CANON

inherits: {parent}/

---

## Axiom

**{declarative principle}**

---

## Evidence

| Source | Authority | Scope |
|--------|-----------|-------|

---

## Constraints

1. {SCOPE} MUST ...
2. {SCOPE} MUST NOT ...
3. {SCOPE} SHOULD ...

---

## Equations

{SCOPE} = {definition}

---

*{SCOPE} | {parent} | {tier}*
```

### VOCAB.md

```
# {SCOPE} — VOCABULARY

---

## Terms

| Term | Definition |
|------|------------|

---

*VOCAB | {SCOPE} | {parent}*
```

### README.md

```
# {SCOPE}

{narrative description}
```

### ROADMAP.md

```
# {SCOPE} — Roadmap

## Now
- {current work}

## Next
- {near-term}

## Later
- {future}
```

### COVERAGE.md

```
# {SCOPE} — COVERAGE

---

Score: {score}

| Question | Status |
|----------|--------|
| What do you believe? | |
| What proves it? | |
| When did it happen? | |
| Who is involved? | |
| How does it work? | |
| What shape is it? | |
| What patterns emerge? | |
| How is it expressed? | |

---

*COVERAGE | {SCOPE} | COMPLIANCE*
```

### LEARNING.md

```
# LEARNING — {SCOPE}

inherits: {parent}/

---

## Axiom

**{learning principle}**

---

## What Gets Learned

| Type | Example |
|------|---------|

---

## How It Works

{mechanism}

---

## The Rule

**{meta-principle}**

---

*LEARNING | {SCOPE} | {parent}*
```

### EVOLUTION.md

```
# {SCOPE} — EVOLUTION

---

## EPOCHS

### 001 {epoch name}

{narrative}

Cite: {source}

---

*EVOLUTION | {SCOPE} | LEARNINGS*
```

---

## Nomenclature

```
repo (lower)  → filesystem container
SCOPE (UPPER) → governance identity

canonic-foundation → FOUNDATION
canonic-magic      → MAGIC
{org}-canonic      → {ORG}
```

---

## Runtime

```
~/.canonic  → shared (device-level)
```

---

## Constraints

```
MUST      — required
MUST NOT  — prohibited
SHOULD    — recommended
MAY       — optional
```

---

*LANGUAGE | FOUNDATION | PUBLIC | 2026-02-07*
