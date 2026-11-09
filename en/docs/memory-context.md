# Memory and context

[中文](../../docs/memory-context.md) | English

[Home](../index.md)

Knowledge graphs, code graphs, long-term memory, handoff across agents

### [Graphify](https://github.com/Graphify-Labs/graphify)

Turn code and documents into a knowledge graph you can query

![Graphify GitHub preview](https://opengraph.githubassets.com/1/Graphify-Labs/graphify)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 139,236 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Turns code, documents, and schemas into a knowledge graph you can query

### [ai-memory](https://github.com/akitaonrails/ai-memory)

Long-term memory for an agent CLI, so one agent can hand work to another

![ai-memory GitHub preview](https://opengraph.githubassets.com/1/akitaonrails/ai-memory)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 14,563 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Long-term memory for an agent CLI, so work can be handed across agents

### [Graphicle](https://github.com/Graphicle-AI/graphicle)

One Rust program that provides both a code graph and memory

![Graphicle GitHub preview](https://opengraph.githubassets.com/1/Graphicle-AI/graphicle)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 477 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

A single Rust program that provides both a code graph and memory

### [Hy-Memory](https://github.com/Tencent-Hunyuan/Hy-Memory)

Tencent Hunyuan's agent memory engine, shared across tools

![Hy-Memory GitHub preview](https://opengraph.githubassets.com/1/Tencent-Hunyuan/Hy-Memory)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 1,876 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Tencent Hunyuan's agent memory engine. Memory is shared across tools

### [CodeGraph](https://github.com/colbymchenry/codegraph)

Index the code into a knowledge graph ahead of time, and give the agent precise context through MCP

![CodeGraph GitHub preview](https://opengraph.githubassets.com/1/colbymchenry/codegraph)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 76.1k | Brian's recommendation list 2026-10-31 |

colbymchenry's local code knowledge graph (Rust core). It indexes functions, classes, call chains, and cross-file relations in advance, and updates when the code changes. An MCP server lets Claude Code, Cursor, Codex, Gemini, Copilot, Grok Build, and others query it directly instead of grepping the whole repo each time. It stays 100% local. Install with `curl -fsSL https://raw.githubusercontent.com/colbymchenry/codegraph/main/install.sh | sh` (or `npm i -g @colbymchenry/codegraph`), then `codegraph install` to attach an agent, and `codegraph init` in each project. MIT. There are many projects with the same name (CodeGraphContext has 4.4k stars, among others). This one has the highest star count. Interview takeaway: one way to do context engineering is to give the agent the right structure map first. That spends fewer tokens and changes the wrong place less often than letting it search at random.

### [RAG Design Patterns: a chart of 7 RAG architectures](https://www.facebook.com/reel/4570321283241437)

One picture of seven RAG architectures, from basic retrieval to multi-agent collaboration

| Credibility | Stars | Source |
| --- | --- | --- |
| — | — | [Video 21](https://www.facebook.com/reel/4570321283241437) |

A static chart, "RAG Design patterns (You must know in 2026)", made by @MindBoost-Tutorix (YouTube) / @MindBoostTutorix (X) and reshared by Ankur Mishra. (1) Naive RAG (the chart misspells it Native RAG): chunk documents, embed them, store them in a vector database, embed the query, fetch context, send it to the LLM. Fine for a start and for simple Q&A. (2) Retrieve-and-Rerank: after retrieval, a reranker reorders the hits. Use it when recall is enough but the top hits are wrong. (3) Multimodal RAG: chunk and embed images and video too, and hand them to a multimodal LLM. Use it when the data is not only text. (4) Graph RAG: extract entities, have an LLM build a graph, store it, and retrieve over the graph. Use it when the question needs relations across documents. (5) Hybrid RAG: merge vector, keyword, and graph retrieval into one context. Use it when proper nouns, codes, and other exact matches matter. (6) Agentic RAG (Router): an agent decides whether to search and where, and can query the vector store again. Use it when question types vary. (7) Multi-Agent RAG: a lead agent assigns sub-agents (code tools, web search, vector engines A/B, Slack/Gmail). Use it when the task crosses several sources and tools. Small problems in the chart: "Native" is a typo, Hybrid's keyword search is not connected to any index, and the Router cell does not draw data ingest. Drawn by hand, not AI-generated. Music: no narration; generic royalty-free upbeat synth-pop. Interview takeaway: pick RAG complexity from the need. Start with Naive. Add rerank or hybrid only after you measure that recall or precision is short. Agentic and multi-agent add latency and cost, and they need an evaluation to justify them.

### [ai-pdf-chatbot-langchain: a LangGraph PDF Q&A template](https://github.com/mayooear/ai-pdf-chatbot-langchain)

A full-stack PDF Q&A template with LangGraph and Next.js

![ai-pdf-chatbot-langchain: a LangGraph PDF Q&A template GitHub preview](https://opengraph.githubassets.com/1/mayooear/ai-pdf-chatbot-langchain)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 16.6k | [Video 27](https://www.facebook.com/reel/1687227069493469) |

mayooear's monorepo template, also the companion example for O'Reilly's Learning LangChain. A Next.js front end and a Node/TypeScript LangGraph agent. Graph nodes cover ingest, retrieval routing, and the reply. Supabase is the vector store, OpenAI is the LLM, tokens stream, each thread keeps its own history, and LangSmith traces the run. Compared with the RAG chart in Video 21, this is roughly Naive RAG plus a router that decides whether to retrieve. Maintenance: MIT. It is archived on GitHub. The last commit is 2026-03-28 (Taipei time). The README says it is no longer maintained and is only a reference. The video (AI Star Pick) is an architecture animation, not a screen recording. Music: no narration and no music, only UI sounds. Interview takeaway: the tradeoff between a graph agent (state, loops, routing) and a linear chain. Tracing such as LangSmith is a quality-control tool. Before you adopt open source, look at whether it is still maintained.

![Stack, Workflow, and Delivery light up in order, borders draw on, a node diagram connects step by step, and the bottom caption changes. Recreate it with SVG stroke drawing and staged reveal.](../../assets/gifs/v27-pdf-chatbot-motion-graphic.gif)

Stack, Workflow, and Delivery light up in order, borders draw on, a node diagram connects step by step, and the bottom caption changes. Recreate it with SVG stroke drawing and staged reveal.

### [gbrain: YC CEO Garry Tan's open-source agent second brain](https://github.com/garrytan/gbrain)

Garry Tan's opinionated OpenClaw/Hermes agent brain; every fact keeps its source

![GitHub preview for garrytan/gbrain](https://opengraph.githubassets.com/1/garrytan/gbrain)

| Credibility | Stars | Source |
| --- | --- | --- |
| concept animation · high credibility | 31.9k | [Video 46](https://x.com/imryven/status/2119433356584604119) |

A 27s X video by Ryven (@imryven): motion graphics with GBRAIN / GARRY TAN and a glowing node network (not a screen recording); no full URL on screen. Caption names gbrain (by garrytan). Verified: https://github.com/garrytan/gbrain exists, MIT, "Garry's Opinionated OpenClaw/Hermes Agent Brain", GitHub API 2026-11-09: 31.9k stars / 4.7k forks, not archived, last push 2026-11-09 (Asia/Taipei). SkillSpector scan pending. Interview takeaway: a second brain must keep provenance on every fact to stay auditable.

![gbrain network](../../assets/gifs/v46-gbrain-network.gif)

GIF: 0:00–0:02.5, gbrain network animation.

### ⚠️ [Altair AI: Claude + Obsidian Second Brain — 10-repo list](https://github.com/kepano/obsidian-skills) ⚠️

Motion graphics listing open-source repos for a Claude + Obsidian second brain; most on-screen text is unreadable, so only caption-named matches were verified

![GitHub preview for kepano/obsidian-skills](https://opengraph.githubassets.com/1/kepano/obsidian-skills)

![GitHub preview for AgriciDaniel/claude-obsidian](https://opengraph.githubassets.com/1/AgriciDaniel/claude-obsidian)

![GitHub preview for Astro-Han/karpathy-llm-wiki](https://opengraph.githubassets.com/1/Astro-Han/karpathy-llm-wiki)

![GitHub preview for undefined-ui/second-brain-os](https://opengraph.githubassets.com/1/undefined-ui/second-brain-os)

![GitHub preview for vouchdev/vouch](https://opengraph.githubassets.com/1/vouchdev/vouch)

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · concept animation · medium credibility | — | ⚠️ [Video 48](https://www.facebook.com/reel/1666945238466731) ⚠️ |

A 22s Facebook Reel by Altair AI. Confirmed from the caption: ⚠️ [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) ⚠️ (51.2k; same as Video 47); ⚠️ [AgriciDaniel/claude-obsidian](https://github.com/AgriciDaniel/claude-obsidian) ⚠️ (16.3k); ⚠️ [Astro-Han/karpathy-llm-wiki](https://github.com/Astro-Han/karpathy-llm-wiki) ⚠️ (2.7k); ⚠️ [undefined-ui/second-brain-os](https://github.com/undefined-ui/second-brain-os) ⚠️ (1.5k); ⚠️ [vouchdev/vouch](https://github.com/vouchdev/vouch) ⚠️ (66; matches "no source means error / you approve writes"). Other names left unverified. Comment-the-number CTA = engagement bait. SkillSpector scan pending. Interview takeaway: keep raw sources read-only, error when there is no source, require human approval for writes, and use progressive disclosure.

### [Lamis Mukta (Anthropic): agent memory from CLAUDE.md to Dreaming](https://x.com/David_eficaz/status/2118745007628726684)

An Anthropic engineer on agent memory: CLAUDE.md → tool memory → skills → a memory/ directory, then async Dreaming consolidation

| Credibility | Stars | Source |
| --- | --- | --- |
| high credibility · caption framing unverified | — | [Video 49](https://x.com/David_eficaz/status/2118745007628726684) |

~31-minute English conference talk by Lamis Mukta (Member of Technical Staff, Anthropic) at AI DevCon by Tessl, shared by David (@David_eficaz). Timecodes: memory evolution CLAUDE.md → tool memory → skills → agent-managed memory/ (03:16); progressive disclosure skills (05:30); concurrency via hashing the memory file before/after edits (10:05); memory permissioning — read-only org knowledge vs read/write scratchpad (11:45); limits of in-band memory updates (14:59); Dreaming — async out-of-band batch consolidation from transcripts (17:49); Dreaming architecture — orchestrator + subagents finding recurring errors (21:27). Quantitative claims (e.g. "97% fewer first pass errors") unverified. The X caption's "Opus 5.5" framing does not appear in the talk — mark caption framing unverified. Interview takeaway: split read-only org knowledge from a writable scratchpad, then consolidate with async Dreaming; hash-based concurrency is a practical detail.
