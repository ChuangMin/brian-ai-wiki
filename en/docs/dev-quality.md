# Software development and quality

[中文](../../docs/dev-quality.md) | English

[Home](../index.md)

Version control, process replay, browser self-check, verify-then-gate

### [git-ai](https://github.com/feder-cr/git-ai)

Version control for many agents committing small batches at once

![git-ai GitHub preview](https://opengraph.githubassets.com/1/feder-cr/git-ai)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 1,028 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Version control for a lot of agents making small commits at the same time. Implemented from an Anthropic article. Unofficial.

### [agentplay](https://github.com/Entelligence-AI/agentplay)

Replay an agent's work as a map and a timeline

![agentplay GitHub preview](https://opengraph.githubassets.com/1/Entelligence-AI/agentplay)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 337 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Replay an agent's work as a map and a timeline

### [Playwright MCP](https://github.com/microsoft/playwright-mcp)

Let the AI open a real browser, test the page, and fix layout bugs itself

![Playwright MCP GitHub preview](https://opengraph.githubassets.com/1/microsoft/playwright-mcp)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 38.9k | [Video 9](https://www.facebook.com/reel/1780228483203385) |

From Microsoft. Claude opens a real browser, clicks through the page it built, takes screenshots, finds layout bugs, and fixes them. Apache-2.0.

### [OPUS 5.5 → REVERSE ENGINEER six-agent board](https://github.com/morluto/rea)

A six-agent reverse-engineering board. The tool behind it is REA.

![OPUS 5.5 → REVERSE ENGINEER six-agent board GitHub preview](https://opengraph.githubassets.com/1/morluto/rea)

| Credibility | Stars | Source |
| --- | --- | --- |
| Concept animation | 412.7k (REA) | Screenshot (DeepRepo.ai) |

A visualization of @skunzu's long post "Turn Opus 5.5 into a reverse engineer in one night: REA, clean-room, and a prompt pack" (@Klonzu forwarded a discussion; the board author is guessed to be him). Six agents, OWL, MEDUSA, CLAUDE, P&L, GUARD, and SHIP, follow ingest → plan → execute → verify → gate → commit. The board is a concept animation. The real tool behind it is MIT-licensed REA (an MCP server / CLI wired to Hopper, Ghidra, and IDA). The method is to write a spec that only describes behavior, then rewrite it in a clean context and test for consistency. Only for software you have the right to analyze. Interview takeaway: before commit there are always two gates, verify and gate, and every claim is marked observation, inference, or unknown, with evidence.

### [GitHub Spec Kit: spec-driven development](https://github.com/github/spec-kit)

GitHub's official tool: write the spec, the plan, and the tasks, then let AI implement them

![GitHub Spec Kit: spec-driven development GitHub preview](https://opengraph.githubassets.com/1/github/spec-kit)

| Credibility | Stars | Source |
| --- | --- | --- |
| High repo credibility · low-effort video | 144.2k | [Video 34](https://www.facebook.com/reel/1430221521958832) |

GitHub's official spec-driven development toolkit (MIT, docs at https://github.github.com/spec-kit/ ). The README's usage: install with `uv tool install specify-cli`, then `specify init my-project --integration ...` to create a project. `specify` also searches extensions, presets, workflows, and bundles. Flows include Spec-Driven Development, bug fixing, and idea assessment. The video (Dann Paker - LeadGen & AI) is only an AI voice reading the README over a scrolling screen, with no live demo. The repo's credibility is high. The video itself is simple. Music: none. Interview takeaway: spec-driven development is a way to control the quality of AI code. Write spec → plan → tasks, then implement, so review has something to check against. This matches the interview note "align first, then write code".
