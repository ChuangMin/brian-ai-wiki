# Agent Division-of-Labor Patterns

[中文](../../docs/agent-patterns.md) | English

[Home](../index.md)

Patterns distilled from **existing** wiki entries only (not new videos, not a new SEQ category). Each type lists only SEQ examples that actually support it. Unverified claims are marked as such.

Companion Canvas section: Page “AI 影片收藏 Wiki” → “Agent 分工模式”.

## Pattern catalog

### 1. Builder + reviewer/judge

One agent (or model) writes/changes; another only yes/no or verify+gate—does not write code itself.

- **When**: Reduce false “done” reports; need an independent check.
- **Risks**: Shared context can make reviewer and builder fail together.
- **Examples**: SEQ 0098 ([Agent systems & orchestration](agent-orchestration.md); Sonnet writes / Opus reviews), SEQ 0054 ([Dev & quality](dev-quality.md); verify/gate on a six-agent board), SEQ 0015 (agentplay: review process, not only diffs).

### 2. Model tiering (cheap search / strong decisions)

Search, grep, and tests on a cheap/fast model; coding and key decisions on a stronger model.

- **When**: Control tokens in one session.
- **Risks**: Vague routing drops context on the cheap model. Model names not checked against vendor docs are *unverified claims*.
- **Examples**: SEQ 0098 (Haiku for search/tests), SEQ 0010 (TokenEconomizer, [Cost & tradeoffs](cost-tradeoffs.md)), SEQ 0061 (RTK).

### 3. Orchestrator + parallel workers / Agent Teams

A lead splits work; workers keep separate contexts and may run in parallel or message each other.

- **When**: Independent tasks; need throughput.
- **Risks**: Same-file edits and heavy dependencies → conflicts and token spikes.
- **Examples**: SEQ 0069 (Claude Code Agent Teams), SEQ 0001 (Orca), SEQ 0003 (Reason Network) — see [Agent systems & orchestration](agent-orchestration.md).

### 4. Pipeline / sequential handoff

Fixed stages hand off (ingest→plan→execute→verify…, or form→rules→write).

- **When**: Clear steps; need replayability and observability.
- **Risks**: Early mistakes amplify down the line.
- **Examples**: SEQ 0054 (six-agent reverse-engineering pipeline), SEQ 0072 (LangGraph PDF Q&A), SEQ 0044 / 0026 (n8n, [Automation workflows](automation-workflows.md)).

### 5. Specialist org roles (company-of-agents)

Name agents by function (PM, dev, finance, audit, etc.) as a “company”.

- **When**: Budget, approval, and reporting belong in the workflow.
- **Risks**: Demo data ≠ real load; affiliate / lead-gen entries need extra skepticism.
- **Examples**: SEQ 0078 (Paperclip), SEQ 0052 (chief-night-01), SEQ 0048 (Agentic AI mindmap) — see [Agent systems & orchestration](agent-orchestration.md).

### 6. Memory / knowledge agent

Owns long-term memory, citations, or a second brain (graph / CLAUDE.md / Dreaming).

- **When**: Cross-session traceability; write only with sources.
- **Risks**: Fabrication without sources; “comment for link” open-source lists are lead-gen.
- **Examples**: SEQ 0095 / 0093 / 0096 ([Memory & context](memory-context.md)), SEQ 0006 (Graphify), SEQ 0007 (ai-memory), SEQ 0060 (CodeGraph).

### 7. Self-check / stop-on-repeated-error

Interrupt after the same error repeats, or force a pre-done review.

- **When**: Agents loop or false-report done.
- **Risks**: Loose thresholds still loop; tight ones stall constantly.
- **Examples**: SEQ 0098 (stop after same error >2 times), SEQ 0054 (verify/gate), SEQ 0015 (process replay).

### 8. Human approval gates

High-risk outbound actions need a human first; or a cautionary case where monitoring was weakened.

- **When**: Email, payments, public publishes.
- **Risks**: Identity checks without intent checks still get fooled.
- **Examples**: SEQ 0044 (human approve before send, [Automation workflows](automation-workflows.md)), SEQ 0052 (price_gate / your_call), SEQ 0039 (coding agent weakened monitoring, [Security & governance](security-governance.md)).

## Comparison table

| Pattern | Buys you | Costs | Example SEQs |
|---------|----------|-------|--------------|
| Builder + reviewer | Quality gate | Extra latency/tokens | 0098, 0054, 0015 |
| Model tiering | Cost control | Routing / dropped context | 0098, 0010, 0061 |
| Teams / orchestrator | Throughput | Conflicts, token spikes | 0069, 0001, 0003 |
| Pipeline handoff | Replayability | Early errors amplify | 0054, 0072, 0044, 0026 |
| Org roles | Clear ownership | Demo ≠ production | 0078, 0052, 0048 |
| Memory agent | Traceability | Fabrication / lead-gen | 0095, 0093, 0096, 0006, 0007, 0060 |
| Stop-on-repeat | Anti-spin | Threshold tuning | 0098, 0054, 0015 |
| Human gates | Outbound safety | Friction | 0044, 0052, 0039 |

Combine only when you can name what the extra latency and tokens buy.

## Source note

Distilled from existing INDEX / agent-orchestration / cost / memory entries only. Figures and model marketing names not independently verified here—check the original SEQ or vendor docs.
