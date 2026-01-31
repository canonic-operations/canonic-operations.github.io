# TECHNICAL — CANON

inherits: /CANONIC/OPERATIONS/LEARNINGS/

---

## Axiom

**DETROS CLOSURE for architecture. Patterns that guarantee compliance.**

---

## DETROS Closure

| Dimension | Technical Requirement |
|-----------|----------------------|
| **D** | CANON.md in every directory |
| **E** | Git history = LEDGER = evidence |
| **T** | Tiered validation (GENESIS → CLOSURE) |
| **R** | inherits: chain to parent |
| **O** | Hooks enforce at commit |
| **S** | TRIAD structure complete |

---

## CHAT Pattern

```
CANON.md (D)
    ↓
User Query (E: session logged)
    ↓
RAG Retrieval (R: citations)
    ↓
LLM Response (O: action)
    ↓
TRANSCRIPTS (S: archived)
```

**Closure:** Every response has evidence. Every session logged.

---

## EVO Pattern

```
LEDGER (git history)
    ↓ learn()
SPEC (CLOSURE + ROADMAP)
    ↓ comply()
PASS/FAIL
    ↓ output()
DISCOVERY/IDFs/
```

**Closure:** What you claim is what you have.

---

## SHOP Pattern

```
COIN (value) + WALLET (account) + VAULT (storage)
    ↓
Transaction (E: logged)
    ↓
Validation (O: VaaS)
    ↓
Settlement (S: immutable)
```

**Closure:** Every transaction evidenced.

---

## Architecture Principles

1. **Separation** - Secrets in CREDENTIALS/, config in CONFIG/
2. **Hooks** - pre-commit (VaaS gate), post-commit (EVO + SYNC)
3. **Streaming** - Async for real-time, persist to TRANSCRIPTS
4. **Cross-platform** - One doctrine, multiple implementations

---

## Stack (Current)

| Layer | Technology |
|-------|------------|
| LLM | Claude API (primary), DeepSeek (fallback) |
| DB | Supabase (PostgreSQL + pgvector) |
| Hosting | GitHub Pages (frontend), Cloudflare Workers (VaaS) |
| Runtime | ~/.canonic (AGENT) |

---

*TECHNICAL | DETROS CLOSURE | LEARNINGS*
