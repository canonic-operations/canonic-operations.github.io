# CANONIC OPERATIONS — STRUCTURE

inherits: canonic-operations/CANON.md
dimension: S (Structural)

---

## Axiom

**STRUCTURE = Files and tiers. The Structural dimension.**

---

## Directory Structure

```
canonic-operations/
├── CANON.md           # D (Declarative)
├── VOCAB.md           # E (Evidential)
├── SPEC.md            # T (Temporal)
├── RELATIONS.md       # R (Relational)
├── OPERATIONS.md      # O (Operational)
├── STRUCTURE.md       # S (Structural) <- you are here
├── COVERAGE.md        # Timeline evidence
│
├── ORGS/              # Org-user coordination
│   └── {org}-{user}.md
│
├── DEALS/             # Commercial evidence
│
├── DISCOVERY/         # IDF artifacts
│   └── IDFs/
│       └── IDF-*.md
│
├── LEARNINGS/         # Strategic intel
│   ├── CANON.md
│   ├── VOCAB.md
│   ├── TECHNICAL.md
│   ├── STRATEGY.md
│   ├── SALES.md
│   └── MARKET.md
│
├── FINANCIALS/        # Actuals evidence
│   ├── CANON.md
│   └── VOCAB.md
│
├── FORECASTS/         # Projections evidence
│   ├── CANON.md
│   └── VOCAB.md
│
└── PROVISIONALS/      # USPTO filing queue
    ├── README.md
    ├── PROV-001/
    └── PROV-002/
```

---

## DETROS File Mapping

| Dimension | File | Bit | Required For |
|-----------|------|-----|--------------|
| D | CANON.md | 1 | All tiers |
| E | VOCAB.md | 2 | All tiers |
| T | SPEC.md | 4 | BUSINESS+ |
| R | RELATIONS.md | 8 | ENTERPRISE |
| O | OPERATIONS.md | 16 | ENTERPRISE |
| S | STRUCTURE.md | 32 | All tiers |

---

## Tier Closure

```
COMMUNITY  = D + E + S         = 35 (100011)
BUSINESS   = D + E + T + S     = 39 (100111)
ENTERPRISE = D + E + T + R + O + S = 63 (111111)
```

**canonic-operations: ENTERPRISE (63)**

---

## IDF Structure

| File | Purpose |
|------|---------|
| IDF-0001.md | ADVENTHEALTH enterprise deployment |
| IDF-0002.md | ... |
| IDF-0063.md | ... |

---

## PROVISIONALS Structure

| Directory | Purpose |
|-----------|---------|
| PROV-001/ | V0 MACHINE (Compiler Correspondence) |
| PROV-002/ | V0 MACHINE (Governance Axioms) |
| PROV-003/ | V1 FOUNDATION (queued) |

---

## Constraints

1. STRUCTURE MUST map all files to dimensions.
2. IDF files MUST follow IDF-NNNN.md pattern.
3. PROV directories MUST follow PROV-NNN/ pattern.
4. Tier requirements MUST be enforced by runtime.
5. All children MUST have CANON.md.

---

*OPERATIONS | S (Structural) | canonic-operations*
