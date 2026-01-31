# TECHNICAL LEARNINGS

inherits: /CANONIC/OPERATIONS/LEARNINGS/

## Axiom

**Architecture patterns from MammoChat and HadleyLab implementations.**

---

## CHAT Architecture (MammoChatApp Pattern)

1. **RAG System** - Retrieval-Augmented Generation
   - crawlers/ → Medical literature API integrations
   - database/ → Supabase + pgvector
   - rag/ → Evidence-based responses with citations

2. **Stack**
   - Python 3.11+
   - Streamlit (rapid prototyping)
   - OpenAI API (LLM)
   - Supabase (PostgreSQL + pgvector)

3. **Pattern**
   ```
   User Query → RAG Retrieval → LLM + Citations → Response
   ```

---

## Mobile Architecture (beeware_chat Pattern)

1. **Cross-platform**
   - BeeWare/Toga framework
   - Briefcase for iOS/Android packaging
   - toga_dummy for headless testing

2. **Structure**
   - controllers/ → UI logic
   - services/ → Business logic (auth, chat, memory)
   - models/ → Data structures
   - utils/ → Config, async helpers

3. **Config**
   - .env for secrets (DEEPSEEK_API_KEY, HEYSOL_API_KEY)
   - app_config.json for settings
   - MAMMOCHAT_CONFIG_PATH for override

---

## API Client (heysol-api-client Pattern)

1. **Backend integration**
   - Async client for streaming responses
   - Memory/conversation persistence
   - Auth service integration

---

## Key Patterns

| Pattern | Implementation | Lesson |
|---------|---------------|--------|
| RAG | MammoChatApp | Citations = trust |
| Cross-platform | BeeWare/Toga | One codebase, all platforms |
| Config | JSON + .env | Secrets separate from settings |
| Streaming | heysol-api-client | Async for real-time |

---

## Extinct (Retired)

These implementations are now extinct. Patterns live on:
- MammoChatApp → MAMMOCHAT/ (hadleylab-dexter)
- MedChat → MEDCHAT/ (hadleylab-dexter)
- beeware_chat → Mobile pattern
- ucfwealth → SHOP pattern

---

*TECHNICAL | Architecture | LEARNINGS*
