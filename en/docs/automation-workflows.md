# Automation workflows

[中文](../../docs/automation-workflows.md) | English

[Home](../index.md)

n8n and similar automation: rules first, and a human approval gate

### [n8n customer-support ticket automation](https://www.facebook.com/reel/3209079722631476)

A rules-based support flow from a form to a SQL ticket

| Credibility | Stars | Source |
| --- | --- | --- |
| Concept animation | — | [Video 7](https://www.facebook.com/reel/3209079722631476) |

Form submit → webhook → validate the data → use rules (not AI) to treat urgent / payment failed as high priority → write a SQL ticket (INSERT … ON CONFLICT so a retry is not a duplicate) → send a notification email → return HTTP 200. The video is an After Effects-style simulated animation, not a real n8n screen (CODER.X).

![A neon-green terminal-style workflow UI: nodes light up and check off in order, a side panel shows JSON, and a log appears line by line. Recreate it with CSS keyframes and setTimeout flipping an active class.](../../assets/gifs/v07-n8n-workflow-ui-motion.gif)

A neon-green terminal-style workflow UI: nodes light up and check off in order, a side panel shows JSON, and a log appears line by line. Recreate it with CSS keyframes and setTimeout flipping an active class.

### [n8n Email Agent: Gmail → AI Agent → HubSpot / Docs / Sheets](https://n8n.io/workflows/7680-automate-gmail-lead-follow-up-with-openai-gpt-4o-hubspot-slack-and-google-sheets/) ⚠️

An n8n template: Gmail triggers, the AI looks up the CRM, then drafts a reply

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait | — | Screenshot (Maruf AI Automation Expert) |

A "comment Email Agent and get the template" funnel video by MD Abdullah Al Maruf, a Bangladesh n8n / Make freelancer. Gmail triggers → an AI agent checks HubSpot, Google Docs, and Sheets → send or save a draft. n8n's free official templates already include the same pattern (this link is #7680). #8967 drafts a reply from HubSpot data, then waits for a person to approve it in Slack before sending. Interview takeaway: the AI only drafts. A person approves before anything is sent. That is the quality gate on an outward action.

### [A photo and video auto-sort page made with Claude (a single HTML file)](https://www.instagram.com/reel/DfKEVgNSL3l/) ⚠️

Claude generates one HTML file. In Chrome you pick a folder, hand it to Claude to classify, then press Start and the thumbnails fly into categories.

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · medium credibility | — | [Video 41](https://www.instagram.com/reel/DfKEVgNSL3l/) ⚠️ |

A 19-second Instagram Reel by 亨利溫 Henry Wen, a phone filming a laptop screen. Flow: open the single HTML file Claude made in Chrome → pick a folder → paste the data to Claude for classification → download the result → press Start. Thumbnails fly from a pile in the middle into categories such as webpage screenshots, travel and sights, daily life, work, memes, and plain text. Photos and videos are in two areas. The caption says reply to any comment and the instruction pack will be sent in a private message. That is comment-driven engagement bait. Credibility: medium. You only get the instructions by commenting, and the video never shows whether the classification is right. It only shows the animation. Music: lofi. The voiceover sounds synthetic. Interview takeaway: split "AI judgment" from "local execution". The AI only produces the classification list. A deterministic program moves the files. Preview the result before applying it, so a mistake is easy to undo.

![After Start, thumbnails fly from a circular pile into category boxes](../../assets/gifs/v41-photo-sort-fly.gif)

GIF: 0:10.5–0:14 of the video, thumbnails flying into categories (a phone filming a screen).

▶ Interactive demo: [Open](../../demos/photo-sort-fly/) ⚠️（https://wiki.singularityengine.dev/demos/photo-sort-fly/ ⚠️）
