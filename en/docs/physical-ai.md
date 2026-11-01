# Physical AI and hardware

[中文](../../docs/physical-ai.md) | English

[Home](../index.md)

ESP32, robots, and other physical devices

### [esp32-iphone-agent](https://github.com/onehumanbeing/esp32-iphone-agent)

Use an ESP32 that costs about $7 to let AI operate a physical iPhone

![esp32-iphone-agent GitHub preview](https://opengraph.githubassets.com/1/onehumanbeing/esp32-iphone-agent)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | 4,120 | [Video 1](https://www.facebook.com/reel/2050168028979180) |

Use an ESP32 that costs about $7 to let AI operate a physical iPhone

### [Microduck: four small biped robots chatting (Grok dashboard)](https://github.com/pollen-robotics/microduck)

An open-source small biped robot. The dashboard in the video is post-production.

![Microduck: four small biped robots chatting (Grok dashboard) GitHub preview](https://opengraph.githubassets.com/1/pollen-robotics/microduck)

| Credibility | Stars | Source |
| --- | --- | --- |
| Post-production packaging | 13.2k | Screenshot (DeepRepo.ai) |

The robot is real: Pollen Robotics × Hugging Face's Microduck, 25 cm / 800 g, 15 motors. An RL policy trained with MuJoCo and PPO is exported to ONNX and run on the robot. Preorder $399. The software is Apache-2.0 (the 3D models in microduck_rl are CC BY-NC-SA 4.0). Official abilities are walking, rollers, picking things up, and getting up after a fall. The four voiceprints and the "Grok Robot Brain Engine" digital-twin dashboard have no source and look like post-production packaging. apirrone's Open Duck Mini (4,605 stars, Apache-2.0) looks similar. How the two relate is still unconfirmed.

### [Edge0: run a 35B MoE model on a phone or laptop (stream expert weights from SSD)](https://github.com/Edge0-AI/Edge0) ⚠️

Do not load the whole model into memory. Read an expert's weights from SSD only when they are used, so a 35B MoE model runs in about 3 GB of memory.

![Edge0-AI/Edge0 GitHub preview](https://opengraph.githubassets.com/1/Edge0-AI/Edge0)

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · medium-high credibility | 8.8k | [Video 38](https://www.facebook.com/share/r/1CcD2Vgk2Y/) ⚠️ |

A 38-second video uploaded by GitHunt: a scrolling README plus an AI voiceover, with no live demo. The end says "Comment EDGE and I'll send you the repo link", which is engagement bait. Mechanism: SSD expert offload (peak memory depends on the experts that are active, not the total parameter count). Prerouter (a trained prediction head guesses the next route so reads overlap compute; decode speed up to +59%). Recover-LoRA (an int4 base plus a distilled LoRA adapter that makes up quantization loss). Models: Edge0-35B-A3B-preview (based on Qwen3.6-35B-A3B) and Edge0-8B-A1B-preview. Platforms: Python / MLX, macOS, iOS, Android, Windows (Vulkan). There is an arXiv paper, 2609.18063. README benchmark: the 35B peak memory is about 2.9 GB, and about 15–18 tok/s on a Mac mini M4 Pro with 24 GB. Apache-2.0, created 2026-09-08. Credibility: medium-high. The repo, the paper, and the models are real. The copy says 2.5 GB, which does not match the README's 2.9 GB. Speed also depends on SSD read speed. The claim that a humanoid-robot company is using it has no evidence. Music: low-volume electronic / ambient synth. No GIF clip (it only scrolls the README). Interview takeaway: a memory bottleneck can be solved with streaming plus predictive prefetch. That is the systems-design idea of cache and prefetch applied to model inference.
