# CANONIC OPERATIONS — OPERATIONS

inherits: canonic-operations/CANON.md
dimension: O (Operational)

---

## Axiom

**OPERATIONS = MUST | MAY | SHOULD | SHALL. The Operational dimension.**

**This is where the messy implementation details live.**

---

## Constraint Levels

| Level | Meaning | Enforcement |
|-------|---------|-------------|
| MUST | Required | BLOCKED if violated |
| MUST NOT | Prohibited | BLOCKED if present |
| SHOULD | Recommended | FLAGGED if absent |
| SHOULD NOT | Discouraged | FLAGGED if present |
| MAY | Optional | No enforcement |
| SHALL | Future requirement | Tracked |

---

## DISCOVERY Constraints

| Component | Constraint | Level |
|-----------|------------|-------|
| IDF-*.md | MUST follow IDF template | MUST |
| Source Reference | MUST point to CANONVERSE | MUST |
| Inventor | MUST be Dexter Hadley, MD/PhD | MUST |
| Status | MUST be DRAFT until human review | MUST |
| Confidentiality | MUST be PRIVILEGED | MUST |

---

## PROVISIONALS Constraints

| Component | Constraint | Level |
|-----------|------------|-------|
| PROV-* | MUST bundle related IDFs | MUST |
| Filing | MUST precede EVOLUTION | MUST |
| Priority Date | MUST be established before arXiv | MUST |
| Gate | MUST NOT disclose before filing | MUST NOT |

---

## IDF Operations

| Operation | Input | Output | Constraint |
|-----------|-------|--------|------------|
| discover() | domain | IDF | MUST extract axioms |
| bundle() | IDFs | PROV | MUST group by version |
| file() | PROV | USPTO | MUST establish priority |
| publish() | PROV | arXiv | MUST follow priority |

---

## Messy Details

### DISCOVERY Workflow
```
1. Scan CANONVERSE domain
2. Extract CANON.md axioms
3. Generate IDF template
4. Hash content for integrity
5. Write to DISCOVERY/IDFs/
6. Log to LEDGER
```

### PROVISIONALS Workflow
```
1. Group IDFs by version
2. Bundle into PROV-*
3. Human review gate
4. Patent counsel review
5. File with USPTO
6. Record PRIORITY DATE
```

### Error Handling
```
Missing CANON.md in domain → SKIP (not CANONVERSE)
Missing axiom → FLAG for human review
Duplicate IDF → MERGE with existing
Filing rejected → RETRY with amendments
```

---

## IP Boundary

| Layer | Visibility | Protection |
|-------|------------|------------|
| IDFs | PRIVILEGED | Pre-filing confidential |
| PROVISIONALS | PRIVILEGED | Attorney-client |
| PRIORITY DATE | PUBLIC | USPTO record |
| arXiv paper | PUBLIC | Post-priority |

---

## Constraints

1. OPERATIONS MUST list all constraint levels.
2. IDFs MUST NOT be disclosed before PRIORITY DATE.
3. PROVISIONALS MUST bundle IDFs by version.
4. Filing MUST precede EVOLUTION.
5. Messy details MAY live here.

---

*OPERATIONS | O (Operational) | canonic-operations*
