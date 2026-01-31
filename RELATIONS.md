# CANONIC OPERATIONS — RELATIONS

inherits: canonic-operations/CANON.md
dimension: R (Relational)

---

## Axiom

**RELATIONS = Inheritance graph. The Relational dimension.**

---

## Inheritance Hierarchy

```
/CANONIC/ (root)
    │
    ├── FOUNDATION/ (parent)
    │   ├── LANGUAGE/
    │   ├── MACHINE/
    │   └── COMPLIANCE/
    │
    └── OPERATIONS/ (this)
        ├── ORGS/
        ├── DEALS/
        ├── DISCOVERY/
        │   └── IDFs/
        ├── LEARNINGS/
        ├── FINANCIALS/
        ├── FORECASTS/
        └── PROVISIONALS/
```

---

## Domain Relationships

| Child | Parent | Relationship |
|-------|--------|--------------|
| ORGS/ | OPERATIONS | Org-user coordination |
| DEALS/ | OPERATIONS | Commercial evidence |
| DISCOVERY/ | OPERATIONS | IDF generation |
| LEARNINGS/ | OPERATIONS | Strategic intel |
| FINANCIALS/ | OPERATIONS | Actuals evidence |
| FORECASTS/ | OPERATIONS | Projections evidence |
| PROVISIONALS/ | OPERATIONS | USPTO filing queue |

---

## IDF → PROVISIONALS Flow

```
CANONVERSE domains
        ↓
    DISCOVERY scan
        ↓
    IDF generation
        ↓
    PROVISIONALS bundle
        ↓
    USPTO filing
        ↓
    PRIORITY DATE
```

---

## External Dependencies

| Dependency | Type | Status |
|------------|------|--------|
| canonic-foundation | parent | REQUIRED |
| ~/.canonic | runtime | REQUIRED |
| USPTO | filing | PENDING |
| arXiv | publication | QUEUED |

---

## Cross-Domain References

| Domain | Relationship |
|--------|--------------|
| hadleylab-dexter.github.io | SHOP source |
| canonic-discovery | Discovery patterns |
| canonic-shop | Shop templates |

---

## Constraints

1. All children MUST inherit from OPERATIONS CANON.
2. IDFs MUST reference source domains.
3. PROVISIONALS MUST bundle IDFs before filing.
4. Circular dependencies PROHIBITED.

---

*OPERATIONS | R (Relational) | canonic-operations*
