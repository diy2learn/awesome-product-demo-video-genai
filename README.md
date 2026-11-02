# 🎬 Awesome Product Demo Video GenAI

> **From product to demo video, powered by GenAI.**

A curated collection of open-source projects for creating product demo videos with **GenAI, browser agents, automated recording, narration, and video-as-code**.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![License: CC0](https://img.shields.io/badge/license-CC0-blue.svg)](LICENSE)

```text
Product understanding → Demo planning → UI automation
→ Recording → Narration → Editing → Rendering
```

## Contents

- [End-to-End Demo Generators](#-end-to-end-demo-generators)
- [Agentic Recording & Product Capture](#-agentic-recording--product-capture)
- [Video Composition & Post-production](#-video-composition--post-production)
- [Wanted](#-wanted)
- [Vision](#-vision)
- [What Belongs Here?](#-what-belongs-here)
- [Contributing](#-contributing)
- [License](#license)

## 🏆 End-to-End Demo Generators

Projects that generate, or aim to generate, a product demo from a live app, URL, storyboard, script, or screenshots.

- [**supercut**](https://github.com/Co-Messi/supercut) — Films a live web app from its URL: an AI director analyses the app, writes a filming recipe, drives the real UI with Playwright, and renders a launch video with camera moves and music. Can also run from a coding agent, with the agent acting as director.  
  `Real product` `Agentic` `Playwright` `Agent skill` `MIT`

- [**ecommerce-video-skills**](https://github.com/iart-ai/ecommerce-video-skills) — Agent skills that turn product or app screenshots into animated demos with device framing, synthetic cursor and clicks, zoom-to-region, and feature captions.  
  `Screenshots` `Agent skill` `Motion graphics` `MIT`

- [**demo-video-generator**](https://github.com/JamesWuHK/demo-video-generator) — Generates narrated walkthroughs from YAML or JSON storyboards: Playwright recording, text-to-speech, timestamp-based sync, and subtitles.  
  `Scripted` `Playwright` `TTS` `Subtitles` `Early` `MIT`

## 🎥 Agentic Recording & Product Capture

Projects that explore, operate, or record real products and repeatable UI journeys.

- [**clickcast**](https://github.com/AlexKay28/clickcast) — Records deterministic browser walkthroughs as GIF, MP4, or WebP, with a machine-readable JSON sidecar (selectors, timing, console errors, page state) and an MCP server for live step-by-step control.  
  `Playwright` `MCP` `Recording` `Structured metadata` `Apache-2.0`

- [**playwright-recording skill**](https://github.com/JuanMarchetto/agent-skills/tree/main/skills/playwright-recording) — Agent skill with Playwright patterns for recording app walkthroughs: navigation and login flows, cursor highlighting, click ripples, viewport scaling, and Remotion output.  
  `Agent skill` `Playwright` `Cursor effects` `Remotion` `MIT`

- [**playwright-record-mcp**](https://github.com/korwabs/playwright-record-mcp) — Variant of Playwright MCP that adds video recording of LLM-driven browser sessions.  
  `MCP` `Playwright` `Recording` `Apache-2.0`

- [**Playwright MCP**](https://github.com/microsoft/playwright-mcp) — MCP server that lets LLMs operate web apps through Playwright and structured accessibility snapshots. A foundation for reproducible, AI-operated product journeys, not a recorder by itself.  
  `MCP` `Playwright` `Foundation` `Apache-2.0`

- [**browser-use**](https://github.com/browser-use/browser-use) — Python browser-agent library that can discover and execute the product journey to be captured. An upstream interaction layer, not a demo generator.  
  `Browser agent` `Product exploration` `Foundation` `Python` `MIT`

## ✨ Video Composition & Post-production

Projects for turning captured material into polished, reusable, programmatically rendered video.

- [**Remotion**](https://github.com/remotion-dev/remotion) — Create, parameterize, and render videos programmatically with React; a common target for composing recorded footage, titles, captions, audio, and branding.  
  `Video as code` `React` `Templates` `Source-available` (free for individuals and small companies; company license above that)

- [**Remotion Prompt-to-Video Template**](https://github.com/remotion-dev/template-prompt-to-video) — Reference template that generates a script, images, voice-over, and timeline from a prompt. Not demo-specific; useful as a reference for wiring generated media into a render.  
  `Reference implementation` `Voice-over` `Remotion`

- [**Auto-Editor**](https://github.com/WyattBlue/auto-editor) — CLI that automatically cuts video using loudness and motion signals; a quick first editing pass on raw demo recordings.  
  `Post-production` `CLI` `Silence removal` `Unlicense`

## 🙋 Wanted

Gaps we would like to fill. If you know a project that **demonstrates** one of these, please [open a PR](CONTRIBUTING.md):

- **Voice, captions & localization** — narration, subtitles, or translated voice applied to a product demo (not a generic speech model).
- **Script + UI actions + synchronized narration** in one pipeline.
- **Docs or repository → demo script and recording plan.**
- **Pull request or release → regenerated demo** (only affected scenes re-recorded).
- **Browser-agent session → Remotion timeline.**
- **Raw screen recording → automatically polished demo** (zooms, cursor, pacing).

A new category is created once it has at least three strong entries.

## 🌟 Vision

Today, a polished product demo still needs product knowledge, storytelling, screen-recording and editing skills, and time.

This list tracks the open-source projects changing that.

> **Give AI a product, an audience, and an objective. Get back a compelling, reproducible demo video.**

Longer notes live in [`docs/`](docs):

- [Vision](docs/VISION.md) — why demos are hard, automation levels, where this is heading.
- [Landscape](docs/LANDSCAPE.md) — the full pipeline, capability map, and idea backlog.
- [Evaluation](docs/EVALUATION.md) — how to assess a demo generator.
- [Reference Architecture](docs/REFERENCE-ARCHITECTURE.md) — one possible agentic pipeline.

## 🔍 What Belongs Here?

A repository should do at least one of these:

- generate a product demo or software walkthrough;
- autonomously explore or operate a product for recording;
- capture a repeatable UI journey as video;
- generate narration, editing, or visual effects specifically useful for product demos;
- provide an open-source building block demonstrably used by a relevant end-to-end workflow.

Generic text-to-video models, conventional screen recorders, broad agent frameworks, generic editing libraries, and closed SaaS without a relevant open-source repository are excluded unless they show a direct product-demo workflow.

> **Does this repository materially reduce the work or expertise required to create a product demo video?**

## 🤝 Contributing

Contributions are welcome. Use this format:

```markdown
- [**Project Name**](https://github.com/owner/repository) — One factual sentence
  explaining why it matters for product demo generation.  
  `Relevant tag` `Relevant tag` `License`
```

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the full curation policy.

## License

This list is released under [CC0 1.0 Universal](LICENSE).

Project names, trademarks, licenses, and linked content belong to their respective owners.
