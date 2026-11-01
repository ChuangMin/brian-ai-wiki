# Skills / MCP / tools

[中文](../../docs/skills-mcp-tools.md) | English

[Home](../index.md)

Shared agent building blocks: MCP, skills, methodology skills, speech, and extraction models

### [earshot](https://github.com/Leonxlnx/earshot)

A tool that lets an agent handle speech locally

![earshot GitHub preview](https://opengraph.githubassets.com/1/Leonxlnx/earshot)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 3,290 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Lets an agent process speech on the local machine

### [axuse](https://github.com/ctoldigital/axuse)

An MCP tool that drives the browser through the accessibility tree

![axuse GitHub preview](https://opengraph.githubassets.com/1/ctoldigital/axuse)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 648 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Operates the browser through the accessibility tree, over MCP

### [imozuru](https://github.com/MaryCache/imozuru)

A Claude Code skill that follows citations back to the original paper

![imozuru GitHub preview](https://opengraph.githubassets.com/1/MaryCache/imozuru)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 1,385 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

A Claude Code skill that traces citations back to the original literature

### [audio-studio-mcp](https://github.com/kanaworksai-hue/audio-studio-mcp)

An MCP tool that generates music and sound effects locally

![audio-studio-mcp GitHub preview](https://opengraph.githubassets.com/1/kanaworksai-hue/audio-studio-mcp)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 541 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Generates music and sound effects locally

### [Cloudflare Clairic extraction model](https://blog.cloudflare.com/clairic-extraction-model/)

A Cloudflare model that extracts typed fields in one forward pass

| Credibility | Stars | Source |
| --- | --- | --- |
| — | — | Screenshot (Marc.AI) |

Workers AI preview model @cf/cloudflare/clairic, 2026-10-19. Give it text (up to 4 images) and a field schema, and one forward pass returns typed values. It does not generate tokens. It also returns a confidence score, a null probability, and character positions. $0.10 per million input tokens. Output is not charged. Open weights were previewed. Multi-step math and prediction are still weak.

### [Superpowers](https://github.com/obra/superpowers)

A skill methodology that makes a coding agent clarify the need, write a plan, and use TDD before it edits

![Superpowers GitHub preview](https://opengraph.githubassets.com/1/obra/superpowers)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 309.7k | Brian's recommendation list 2026-10-31 |

Jesse Vincent's (obra) agentic skills framework. When an agent starts, it brainstorms and asks until the need is clear, confirms the design in pieces, then writes an implementation plan a newcomer could follow. It stresses red-green TDD, YAGNI, and DRY, and finishes with subagent-driven-development that assigns work item by item and reviews the result. Skills trigger on their own. It supports Claude Code, Codex, Cursor, Gemini CLI, Copilot CLI, Grok Build, and others. Install on Claude Code with `/plugin install superpowers@claude-plugins-official`, and on Cursor with `/add-plugin superpowers`. MIT. By default it loads the site logo to count versions. Turn that off with `SUPERPOWERS_DISABLE_TELEMETRY`. Interview takeaway: making "clarify the need → confirm the design → plan → TDD → sub-agent implementation and review" a team process is the skeleton of an AI team methodology.

### [Matt Pocock Skills (Skills For Real Engineers)](https://github.com/mattpocock/skills)

Small engineering skills Matt Pocock uses every day. Align first, then write code.

![Matt Pocock Skills (Skills For Real Engineers) GitHub preview](https://opengraph.githubassets.com/1/mattpocock/skills)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 307.9k | Brian's recommendation list 2026-10-31 |

TypeScript teacher Matt Pocock published the skills from his own .agents directory. They are deliberately small, composable, and not a locked process (unlike GSD, BMAD, and Spec-Kit, which take over the whole flow). The signature commands are /grill-me and /grill-with-docs: before work starts, the agent interrogates your requirements, builds a shared project vocabulary (ubiquitous language), and writes hard-to-explain decisions as ADRs, so the agent stays concise and names things consistently. Install on Claude Code with `claude plugin install mattpocock-skills@claude-plugins-official`. Other agents use `npx skills@latest add mattpocock/skills`. MIT. Interview takeaway: the most common failure of AI code is a requirement that was never aligned. Grilling, a shared vocabulary, and ADRs cut rework at the source.

### [Ponytail](https://github.com/DietrichGebert/ponytail)

A skill that makes an agent write less code, like a senior engineer, and reuse what already exists

![Ponytail GitHub preview](https://opengraph.githubassets.com/1/DietrichGebert/ponytail)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 181.2k | Brian's recommendation list 2026-10-31 |

DietrichGebert's "lazy senior engineer" skill. Write only the code the task needs. Prefer components that already exist in the repo. Do not cut validation, error handling, security, or accessibility. It includes /ponytail-review (it also reviews files affected outside the diff) and /ponytail-audit. The README's own test of Ponytail 5 on 39 Claude Code tasks: code −53%, time −41%, cost −26%, tokens −45%, and 98% of high-risk logic has tests (68% with no skill). Those numbers are the author's own test. Install on Claude Code with `/plugin marketplace add DietrichGebert/ponytail` and then `/plugin install ponytail@ponytail`. Other agents can drop it into AGENTS.md. MIT. The author says to install only from this repo or npm `@dietrichgebert/ponytail`. Builds that ship .exe or .dll files are fakes. Interview takeaway: AI code quality is not only whether it is correct. It is also whether it wrote too much. Make "the least code that is still enough, without skipping tests and security" a review standard.

### [CLI-Anything: give every piece of software a command line](https://github.com/HKUDS/CLI-Anything)

Automatically generate a command line for professional software, so an AI agent can operate it without clicking the screen

![CLI-Anything: give every piece of software a command line GitHub preview](https://opengraph.githubassets.com/1/HKUDS/CLI-Anything)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 57.9k | [Video 26](https://www.facebook.com/reel/1857279712725267) |

An open-source project from HKUDS at the University of Hong Kong (repo blurb: Making ALL Software Agent-Native). It generates a CLI for professional software so an agent uses commands instead of screenshots and clicks. In Claude Code, `/cli-anything <software path or GitHub URL>` runs seven stages: analyze the code, design the CLI, implement it, plan tests, write tests, write test docs, and publish to PyPI. It calls the real software (LibreOffice to PDF, Blender to render) and emits structured JSON. The copy claims 2,000+ tests. CLI-Hub (https://clianything.cc/ ) lets an agent search and install community CLIs (SKILL.md). The video shows a FreeCAD Curiosity-style rover, a Blender orbital relay drone, and a Slay the Spire 2 CLI. The Slay the Spire on screen looks like the first game, not the second, and the demo frames are the polished shots from the README. It is the same direction as this wiki's blender-skills and Spider Walker: give the agent a testable interface to 3D software. Python, Apache-2.0, created 2026-03-08, 5.2k forks. The video is a Traditional Chinese AI voiceover by 小礦工挖挖礦. Music: none. Interview takeaway: for an agent that is reliable and testable, prefer a deterministic structured interface (CLI plus JSON) over GUI automation.

### [archify: turn an idea or code into an interactive architecture diagram](https://github.com/tt-a1i/archify)

Let an AI agent turn an idea, a plan, or code into an interactive diagram

![archify: turn an idea or code into an interactive architecture diagram GitHub preview](https://opengraph.githubassets.com/1/tt-a1i/archify)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 92.0k | Brian's recommendation list 2026-10-31 |

A skill for Claude Code, Codex, and similar agents. It turns an idea, a plan, or a whole codebase into an interactive diagram. Apache-2.0, created 2026-04-15. Site: https://archify.si . From a written recommendation by Brian. No video. Music: not applicable (no video). Interview takeaway: let an agent generate an architecture diagram from the codebase, and use review to check that the docs and the code still match.

### [diagram-design: an editorial-quality diagram skill](https://github.com/cathrynlavery/diagram-design)

Let an AI agent draw magazine-grade HTML and SVG diagrams

![diagram-design: an editorial-quality diagram skill GitHub preview](https://opengraph.githubassets.com/1/cathrynlavery/diagram-design)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 63.4k | Brian's recommendation list 2026-10-31 |

A diagram skill for Claude Code, Codex, Copilot, Cursor, and similar agents. It produces a standalone HTML file with embedded SVG at editorial quality. MIT. Site: https://diagramdesign.dev . The Chinese fork patrick-xin/diagram-design-zh (https://github.com/patrick-xin/diagram-design-zh , 48 stars) includes CJK typesetting. From a written recommendation by Brian. No video. Music: not applicable (no video). Interview takeaway: same as archify. Let an agent produce an architecture diagram from the codebase, and keep the docs and the code in sync during review.

### [PPT Master: a document or a topic becomes an editable native PPTX (an AI skill pack)](https://github.com/hugohe3/ppt-master)

Give it a PDF, Word, text, or only a topic. The AI makes a real PowerPoint whose text boxes, shapes, and charts can still be edited. It is not a picture.

![hugohe3/ppt-master GitHub preview](https://opengraph.githubassets.com/1/hugohe3/ppt-master)

![hugohe3/ppt-master-examples GitHub preview](https://opengraph.githubassets.com/1/hugohe3/ppt-master-examples)

| Credibility | Stars | Source |
| --- | --- | --- |
| High credibility | 71.6k | [Video 39](https://www.facebook.com/reel/1051071164608370) |

A 1:28 video uploaded by 小礦工挖挖礦. The picture is a recording of the official example site, not a live generation. A skill pack for Claude Code, Cursor, and Codex CLI. Before it generates, it confirms template, aspect ratio, page count, and other specs (only a fast mode skips that). Charts are editable shapes by default. A parameter can switch them to native charts. It adds transitions and animation, and writes the speaker script into the notes. Images come from AI generation or open libraries, and the slide marks the source. It can also apply a company template and keep the original design. The official example site has 72 decks and 1,012 pages, in Chinese, Japanese, Korean, and German. Example repo: https://github.com/hugohe3/ppt-master-examples (22 stars). Requirements: Python 3.10–3.14 and one AI coding assistant. The author says not to expect the first pass to be perfect. You still edit it. Forks worth a look: academic-ppt-master (paper to PPTX) and ppt-master-plus. MIT, created 2025-12-10, last push 2026-10-30. Credibility: high. The star count matches the GitHub API. The end of the video only asks which deck you want to make first. That is a light prompt to comment, not engagement bait. Music: light, playful electronic music (casual-game style). No GIF clip. Interview takeaway: AI output should still be editable, not a one-shot final. Human-in-the-loop design is the same idea as controlling the quality of AI code.

### [VibeVoice: Microsoft's open-source speech AI (long-audio ASR, speaker diarization, and realtime TTS)](https://github.com/microsoft/VibeVoice)

Take a recording up to about an hour and emit a transcript of who spoke, at what time, and what they said. It also has realtime speech synthesis that can run in Colab.

![microsoft/VibeVoice GitHub preview](https://opengraph.githubassets.com/1/microsoft/VibeVoice)

| Credibility | Stars | Source |
| --- | --- | --- |
| High credibility | 55.1k | [Video 40](https://www.facebook.com/watch/?v=2181912112534967) |

A 59-second video uploaded by AI懶人報, with an AI Mandarin voiceover. VibeVoice-ASR does not need the long recording cut up first. One pass handles up to about an hour, and it does speaker diarization and timestamps together (who spoke, from which second to which second, and what they said). It supports 50+ languages and hotwords to improve proper nouns (the voiceover says WhyVoice; the correct name is VibeVoice). There is also realtime TTS, with a Colab T4 quickstart notebook. The demo clip is the official demo of Jimmy Fallon interviewing Lady Gaga, with subtitles marking speaker 0 and speaker 1. What used to be ASR plus a separate diarization tool is now one model. MIT, created 2025-08-25, last push 2026-10-08. The video shows 54.9k stars. Credibility: high. It is Microsoft's official repo, and the video matches the README. The end only asks you to follow. There is no funnel. Music: ukulele plus light percussion. Interview takeaway: for meeting notes or call-center recordings, first ask whether you need speakers separated and whether you need timestamps. One end-to-end model avoids the alignment and the stacked errors of chaining tools, but before production you still sample your own recordings and measure accuracy.

![VibeVoice official demo: a Jimmy Fallon interview clip, with each line labeled speaker 1 or speaker 0 and subtitled](../../assets/gifs/v40-vibevoice-diarization.gif)

GIF: 0:22.5–0:26 of the video, a speaker-diarization demo.

### ⚠️ [Android phone AI agent (wireless ADB debugging plus Claude Code MCP) | the preview is the alternative mobile-mcp, not the video's repo](https://www.facebook.com/reel/1628595922149351)

It claims "some GitHub repo plus Opus 5.5" can turn any Android phone into a hands-free agent, but the account in the video does not exist. Underneath it is only wireless ADB plus screenshot, tap, and type.

Alternative preview (not the repo in the video): ⚠️ [mobile-next/mobile-mcp](https://github.com/mobile-next/mobile-mcp)

![Alternative mobile-next/mobile-mcp GitHub preview (not the video's repo)](https://opengraph.githubassets.com/1/mobile-next/mobile-mcp)

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · claim unverified · low credibility | — (alternative mobile-mcp: 10.2k) | ⚠️ [Video 43](https://www.facebook.com/reel/1628595922149351) |

A 17-second video uploaded by Tauhid IQ, with no narration. The top half is a GitHub page titled "dkrv-dev / Reverse Engineer Phone" (the page shows 17k stars and 2.1k forks). About says "Turn any Android phone into an agent that uses its own apps over Wi-Fi. Say one sentence. Claude taps the rest." The README lists tools/phone.py --probe, tools/agent.sh, and claude mcp add phone tools/venv/bin/python tools/mcp.py. The bottom half is a Windows cmd.exe log, plus a real phone on a desk playing fast, opening Telegram and then the ChatGPT page on the Play Store. The English steps: phone and laptop on the same Wi-Fi, turn on wireless debugging in developer options, paste the repo and a screenshot of About phone plus a prompt into Claude Code, Opus "finds a vulnerability" (it is really ADB over the network), probe model, version, and installed apps and save a restore point, write an agent with only 3 tools (see the screen, tap, type), add it to Claude Code as MCP, press Allow once, and say "open Telegram and install ChatGPT". It also claims 40 brands, 300+ models, and no root. The ending says "Find GitHub repo + full prompt below" and does not give a repo. Check: ⚠️ https://github.com/dkrv-dev returns 404 (the account does not exist), and a GitHub API search does not find this repo. A GitHub repo name also cannot contain a space, so the page is likely a fake screen or has been deleted. Opus 5.5 is only the model named in the copy. This entry does not judge that. Credibility: low. The repo cannot be found, the numbers cannot be checked, and the "repo and full prompt below" line plus the exaggerated tone is engagement bait. The technique itself is real and ordinary: adb connect over Wi-Fi, then screenshot, tap, and type. That is the standard way to operate a phone. A usable alternative (not the repo in the video): mobile-next/mobile-mcp (⚠️ https://github.com/mobile-next/mobile-mcp), 10,198 stars, Apache-2.0, an MCP server for emulators and real devices, and it can attach to Claude Code, Codex, and Cursor. Music: phonk / electronic. Interview takeaway: giving an agent full control of a device through ADB is a very large permission surface. You need an allowlist of commands and apps, a person must confirm installs and payments, and the network should be limited (wireless debugging only on an isolated segment, and turn it off when finished). Also, before you adopt a viral repo, confirm that it exists and who maintains it.

![The bottom half of the video: a cmd.exe log plus a phone on the desk opening Telegram and the Play Store by itself](../../assets/gifs/v43-android-adb-agent.gif)

GIF: 0:02–0:06 of the video, the terminal log and the phone operating itself (sped up).
