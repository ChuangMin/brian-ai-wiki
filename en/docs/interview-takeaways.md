# Interview takeaways

[中文](../../docs/interview-takeaways.md) | English

[Home](../index.md)

Points from the collected videos that are worth using in an interview.

## AI team methodology

[Orca](https://github.com/stablyai/orca) and [Reason Network](https://github.com/reason-machines/reason-network): a person assigns work, tracks status, and decides the handoff points. Agents have an explicit channel between them.

## AI code quality control

[agentplay](https://github.com/Entelligence-AI/agentplay): review is not only the diff; it is also the agent's process. [git-ai](https://github.com/feder-cr/git-ai): small batches of commits, with CI and tests as the gate.

## Context engineering

[Graphify](https://github.com/Graphify-Labs/graphify) and [ai-memory](https://github.com/akitaonrails/ai-memory): give the agent the right code structure and rules (such as AGENTS.md) so it writes fewer mistakes from the start.

## A RAG path: let evaluation decide what to add

[Video 21](https://www.facebook.com/reel/4570321283241437): start with Naive RAG and a real evaluation set. Add rerank, hybrid, or graph only after recall or precision is shown to be short. Agentic and multi-agent are the last resort. Every extra layer has to say what quality it buys and what latency and cost it spends.

## Agent self-check

[video-to-game](https://github.com/lovisdotio/video-to-game): after the agent writes the game it plays it, records video, and compares frames with the source video. "Run it and look" is part of the process, not only reading the code.

## Rules first, AI second

[n8n ticket flow](https://www.facebook.com/reel/3209079722631476): if a clear rule can decide it, do not hand it to AI. The result is predictable and testable. Writes use idempotent retries (ON CONFLICT). That is also the basic discipline for governing AI output.

## An agent is a distributed system too

[Video 22](https://www.facebook.com/reel/3285768298275601): if a tool call will be retried, it has to be idempotent. Put a circuit breaker and a rate limit around the LLM API. Long agent jobs go on a queue. Every agent run keeps traces. Ordinary systems-design practice is what makes an agent platform reliable.

## Cost governance

[TokenEconomizer](https://github.com/microsoft/TokenEconomizer), [RTK](https://github.com/rtk-ai/rtk), and the [Claude Code vs Blender gag](https://www.facebook.com/reel/1867596277567322): an agent is not a universal answer. Measure cost against results. Filter noisy context before you talk about switching models.

## Align first, then write code

[Superpowers](https://github.com/obra/superpowers) and [Matt Pocock Skills](https://github.com/mattpocock/skills): before work starts, let the agent grill the requirements, confirm the design and the plan, and build a shared vocabulary. Then use TDD and sub-agent review. Turn the methodology into a skill the team shares. [GitHub Spec Kit](https://github.com/github/spec-kit) makes spec → plan → tasks → implementation a fixed flow.

## The least code that is still enough

[Ponytail](https://github.com/DietrichGebert/ponytail): review asks not only whether it is correct, but whether it wrote more than it needed. Reuse what is already there, and do not skip tests, checks, or security.

## A valid credential is not the same as a correct intent

[Video 16](https://www.facebook.com/reel/1863665758475395): the password, the device, and the approver can all be right, and the decision-maker can still be fooled by an AI voice clone or a fake message. High-risk actions in an agent flow need an intent check and an out-of-band approval, not only an identity check.
