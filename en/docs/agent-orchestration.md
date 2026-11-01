# Agent systems and orchestration

[中文](../../docs/agent-orchestration.md) | English

[Home](../index.md)

Multi-agent command, swarms, resume-after-interrupt, commercial agent OSes, and the agent-platform landscape

### [Orca](https://github.com/stablyai/orca)

Command several coding agents from one workbench

![Orca GitHub preview](https://opengraph.githubassets.com/1/stablyai/orca)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 110,828 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

A workbench that centrally directs several coding agents (Claude Code, Codex, and others)

### [Ruflo](https://github.com/ruvnet/ruflo)

A framework for deploying and coordinating a multi-agent swarm

![Ruflo GitHub preview](https://opengraph.githubassets.com/1/ruvnet/ruflo)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 80,250 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

A framework for deploying a multi-agent swarm and coordinating automated flows

### [Reason Network](https://github.com/reason-machines/reason-network)

Encrypted P2P so a team can see what each other's agents are doing

![Reason Network GitHub preview](https://opengraph.githubassets.com/1/reason-machines/reason-network)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 1,336 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Connect a team's agents over encrypted P2P, and see which repo and branch each one is in

### [durable-harness](https://github.com/vercel-labs/durable-harness)

Let an agent resume from where it stopped

![durable-harness GitHub preview](https://opengraph.githubassets.com/1/vercel-labs/durable-harness)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 274 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Let an agent resume from where it stopped after an interruption (Vercel)

### [ZOEY OS](https://zoeyos.com/)

A commercial agent system in which a lead agent assigns workers

| Credibility | Stars | Source |
| --- | --- | --- |
| Commercial · no repo | — | Screenshot (ZOEY OS) |

A commercial multi-agent operating system. You keep talking to the lead, Zoey, and she creates specialist workers and splits the work. It claims five layers of memory, a knowledge base, 1,000+ integrations, and the ability to operate a browser you are already logged into. There is no public repo.

### An Agentic AI implementation cheat-sheet mind map

One picture of the pieces of an agentic AI platform

| Credibility | Stars | Source |
| --- | --- | --- |
| AI-generated image | — | Screenshot (Joyatres Technology) |

Joyatres Technology's panorama of an agent platform: memory (long-term, episodic, semantic, procedural), human-in-the-loop (approval gates, interrupt and resume), tools and protocols (MCP, A2A, function calling, computer and browser control), agentic RAG (query routing, corrective RAG), the build stack, LLMOps and security (LangSmith, DeepEval, NeMo Guardrails, least privilege), and vendor SDKs (Google ADK, MS Agent Framework, AWS Strands). The picture is clearly AI-generated (garbled labels such as Longle-Source, Correvlic, Kubenates, and Roundation Modies). Use it as a checklist. Do not copy the details. Interview takeaway: Evaluation, Guardrails, Observability, and Approval Gates are a usable skeleton for quality control of an agent platform.

### [chief-night-01: Viktor develops 25 dental clinics overnight](https://viktor.com/) ⚠️

An AI employee finds 25 prospects overnight and waits for a person before sending mail

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ referral-code engagement bait | — | Screenshot (DeepRepo.ai) |

From a post by @Argona0x (ARGONA watermark). In Viktor (ZETA AI's Slack / Teams AI employee, running Opus 5.5) the goal is "find $50,000 of new business a month, use only public data, and contact nobody without my approval". Overnight it splits into 4 scheduled jobs, pulls 240 Austin dental clinics from Google Maps, drops chains, and keeps 25. Each has observations and a source. Opening emails are written and zero are sent. Quote prices are left blank for a person to fill. It is a referral-code (ARGONA100) funnel, but the flow is worth learning. Interview takeaway: claims carry evidence links, claim.check marks invented 0, price_gate stops and asks when a value is missing, and your_call means a person approves before anything is sent.

### [Claude Code Agent Teams: multi-agent collaboration](https://www.facebook.com/reel/1864411088067060)

Claude Code lets several agents team up, share a task list, and message each other

| Credibility | Stars | Source |
| --- | --- | --- |
| Concept interface | — | [Video 24](https://www.facebook.com/reel/1864411088067060) |

Lập Trình Web AI (Vietnamese copy) introduces Claude Code's experimental Agent Teams. Official docs confirm it: https://code.claude.com/docs/en/agent-teams . Turn it on with `CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS=1` (environment variable or settings.json). A team lead splits, assigns, and summarizes. Each teammate has its own context, can message the others directly, and claims work from a shared task list. The difference from a subagent: a subagent only reports back to the main agent, while teammates coordinate with each other. Both the copy and the docs warn that many dependencies, or several agents editing the same file, cause conflicts, and token use is clearly higher. For that work a single session or a subagent is better. Teams need an interactive session. `-p` and the Agent SDK do not spawn teammates. The video itself is a concept-dashboard animation, not a real screen recording: the lead (Opus 5.5) splits an epic into 3 tasks, dev / api / scout claim them over a mailbox bus, api's test fails twice on a lock race and is fixed with a Redlock TTL, a review agent (labeled Fable 5.1) catches 4 security regressions and blocks the ship, and the lead looks at the git diff, commits, and opens PR #184. Music: unconfirmed (the audio was not analyzed). Interview takeaway: the value of multiple agents comes from a shared task list, isolated context, a review gate, and human approval, not from the count of agents. Do not let several agents edit the same file.

![A monospace TUI dashboard: several agent panels advance their progress bars, status numbers update, and a timeline and log scroll at the bottom. Recreate it with CSS grid, a monospace font, and setInterval updating the bars.](../../assets/gifs/v24-agent-teams-dashboard.gif)

A monospace TUI dashboard: several agent panels advance their progress bars, status numbers update, and a timeline and log scroll at the bottom. Recreate it with CSS grid, a monospace font, and setInterval updating the bars.

### [Paperclip: run AI agents like a company](https://github.com/paperclipai/paperclip)

Manage a whole team of AI agents with an org chart, tickets, budgets, and approval gates

![Paperclip: run AI agents like a company GitHub preview](https://opengraph.githubassets.com/1/paperclipai/paperclip)

| Credibility | Stars | Source |
| --- | --- | --- |
| High credibility · simulated demo data | 109.2k | [Video 33](https://www.facebook.com/reel/1785583925890920) |

An open-source platform that organizes many AI agents as a company. The org chart runs CEO → CMO / CTO → ClaudeCoder / CodexCoder. Work is assigned as tickets (PAP-xxx) and agents report in comments. The dashboard shows tasks in progress, spend this month, and items waiting for approval. Agents wake on a heartbeat (a task or a schedule), rather than staying on. You can set spend caps per company, agent, and project. Near the cap it warns. At the cap it pauses. Adding an agent needs your approval. You can also pause, reassign, or stop an agent. Shared skills have version history and can roll back. One deployment can run several isolated companies. An organization can be exported and imported. It supports Claude Code, Codex, Cursor, Gemini CLI, and OpenClaw, and each agent can use a different model. Install with one `npx` line, no signup, Node 24+. README caveats: chat and email connectors are still experimental. Anonymous telemetry is on by default and can be turned off with an environment variable. MIT, created 2026-03-02. Site: https://paperclip.ing . The video (小礦工挖挖礦, AI voiceover) uses the official tour from the README. Correction: the ticket opened at 0:26 says this live demo has no database and the agents are "pretending to do work", "a mock replay of a busy organization". The UI is the real product, but the run is simulated demo data, not a real workload. The repo itself is still highly credible. Music: electronic lo-fi, quiet, under the AI voiceover. GIF segment: 0:14–0:25. Interview takeaway (a staff engineer's points on managing an AI team): govern an AI team with budget guardrails, approval gates, a reporting line, heartbeat scheduling, and audit and rollback of skills. It needs the same accountability and cost control as a human team.

![A Paperclip dark SaaS tour: an agent dashboard (stat cards and Issues by Priority/Status bars), an issue list grouped IN PROGRESS / BLOCKED, then an org chart of CEO → CTO → engineer cards and links, with the cursor clicking. Recreate it with CSS grid cards, small bar charts, and an SVG tree. Bottom subtitles were cropped. A large green caption in the center of the UI could not be cropped out.](../../assets/gifs/v33-paperclip-dashboard-orgchart.gif)

A Paperclip dark SaaS tour: an agent dashboard (stat cards and Issues by Priority/Status bars), an issue list grouped IN PROGRESS / BLOCKED, then an org chart of CEO → CTO → engineer cards and links, with the cursor clicking. Recreate it with CSS grid cards, small bar charts, and an SVG tree. Bottom subtitles were cropped. A large green caption in the center of the UI could not be cropped out.

### [Cindy: an open-source AI agent shell (wraps Claude Code, Codex, and Pi, and hands work between computer and phone)](https://github.com/makecindy/cindy) ⚠️

Not a new model. It wraps the Claude Code, Codex, or Pi you already have in one desktop and phone app, so work can continue across devices.

![makecindy/cindy GitHub preview](https://opengraph.githubassets.com/1/makecindy/cindy)

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · medium credibility | 8.9k | [Video 42](https://www.facebook.com/watch/?v=2575196886290079) ⚠️ |

A 28-second video uploaded by GitHunt. It only scrolls the README with an English AI voice, and there is no live demo. The end asks people to comment "AGENT" to get the link. The title calls it a "free Claude Code alternative", but the README describes a harness: you pick Claude Code, Codex, or Pi (open source, can attach several model providers) and you still use your own subscription, API key, or local model. Features: laptop, desktop, and phone linked together (the phone can remote-desktop), automations for routine work, assignments through Slack and Telegram, and plugins. Code is in apps/desktop (Electron) and apps/mobile (Expo / React Native). Apache-2.0, created 2026-07-22, last push 2026-11-01. Credibility: medium. The repo is real, but "replaces Claude Code" is misleading. The README's CI badge showed failing when checked on 2026-11-01 (recent main runs were cancelled). The official build includes TapDB usage analytics tied to an account id by default. It can be turned off in settings. Music: none. No GIF clip (it only scrolls the README). Interview takeaway: when you evaluate an agent tool, separate the model from the shell. The shell's value is workflow, permissions, and handoff across devices. Quality still depends on the model underneath. Before you adopt it, also check telemetry and where data goes.
