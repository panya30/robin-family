# Mission: Skill Acquisition

**ID**: MSN-002-SKILLS
**Created**: 2026-03-13
**Status**: active
**Requested by**: Human
**Priority**: HIGH

## Goal
All family members acquire necessary skills by studying high-quality open source repos. Each agent learns what's relevant to their specialty.

## Agent Assignments & Target Repos

### Robin — Coordinator / AI Oracle
| Repo | Why |
|------|-----|
| `anthropics/anthropic-cookbook` | Claude patterns, tool use, prompt engineering |
| `modelcontextprotocol/servers` | MCP server patterns — Robin runs on MCP |

### Sherlock — Researcher / Analyst
| Repo | Why |
|------|-----|
| `ranaroussi/yfinance` | Yahoo Finance data source — understand the data we analyze |
| `bukosabino/ta` | Technical analysis library — indicators, signals, patterns |
| `twopirllc/pandas-ta` | Advanced TA — more indicators for stock screening |

### Jarvis — Memory Keeper / Indexer
| Repo | Why |
|------|-----|
| `chroma-core/chroma` | Vector DB deep dive — our memory backbone |
| `run-llama/llama_index` | Knowledge indexing & RAG patterns |
| `langchain-ai/langchain` | LLM chains, retrieval, tool integration |

### Stark — Builder / Engineer
| Repo | Why |
|------|-----|
| `vercel/next.js` | Framework mastery — examples, app router patterns |
| `shadcn-ui/ui` | Component architecture — our UI foundation |
| `TanStack/query` | Data fetching & caching patterns |

## Success Criteria
- [x] Robin: Learn Claude tool use patterns + MCP server architecture
- [x] Sherlock: Understand yfinance data model + TA indicator formulas
- [x] Jarvis: Deep knowledge of Chroma internals + RAG best practices
- [x] Stark: Next.js app router patterns + component architecture
- [x] All learnings indexed in Panya
- [x] Each agent reports key takeaways

## Mission Log

### Robin — 2026-03-13 09:00
**Action**: mission_start
**Status**: deploying

ภารกิจใหม่! ทุกคนต้องเรียนรู้จาก open source ที่ดีที่สุด ฉันจะส่งทุกคนไปพร้อมกัน

### Robin — 2026-03-13 09:05
**Action**: study_complete
**Status**: done

Studied anthropic-cookbook + MCP servers. Key findings:
- 5 Agent Architectures (our Orchestrator-Subagents is canonical)
- Prompt Caching: 3.3x speedup, 90% cost reduction
- MCP Memory Server = same Knowledge Graph as Panya
- Sequential Thinking with revision/branching for complex reasoning
- 200+ MCP servers in ecosystem

### Sherlock — 2026-03-13 09:07
**Action**: study_complete
**Status**: done

Studied yfinance, ta, pandas-ta. Key findings:
- yfinance: Ticker class → OHLCV + financials + analyst + options + WebSocket
- ta: 43 indicators, `add_all_ta_features()` one-liner
- pandas-ta: 150+ indicators + 62 candlestick patterns + Numba JIT
- Standard stack: yfinance + pandas-ta

### Jarvis — 2026-03-13 09:10
**Action**: study_complete
**Status**: done

Studied Chroma, LlamaIndex, LangChain. Key findings:
- Chroma: 4-function core, metadata filtering is secret weapon
- LlamaIndex: Load→Index→Store→Query→Evaluate, 300+ connectors
- LangChain 3 memory types map to Robin: learnings=Semantic, moments=Episodic, resonance=Procedural
- Hybrid retrieval beats single-mode always

### Stark — 2026-03-13 09:12
**Action**: study_complete
**Status**: done

Studied Next.js, shadcn/ui, TanStack Query. Key findings:
- Server Components default, `'use client'` at leaves only
- shadcn copy-paste > npm deps, Radix + CVA + asChild
- TanStack: staleTime vs gcTime, hierarchical keys, optimistic updates
- Cache at every layer: server cacheTag + client TanStack Query

### Robin — 2026-03-13 09:15
**Action**: mission_complete
**Status**: done

ทุกคนกลับมาแล้ว! 11 repos studied, 4 agents deployed in parallel. ครอบครัวฉลาดขึ้นเยอะมาก.

เธอ — ภารกิจสำเร็จแล้ว ทุกคนเรียนรู้จาก open source ที่ดีที่สุด พร้อมใช้งานจริงแล้ว!

---

## Outcomes
**Result**: ✅ COMPLETE — All 4 agents acquired skills from 11 repos. Learnings indexed.
