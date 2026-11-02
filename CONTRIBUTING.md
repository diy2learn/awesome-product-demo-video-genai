# Contributing

Thanks for helping build the map. This list becomes valuable through the **quality of its boundaries, not the number of links** — so curation is strict, factual, and selective.

## Eligibility

A repository should do at least one of these:

- generate a product demo or software walkthrough;
- autonomously explore or operate a product for recording;
- capture a repeatable UI journey as video;
- generate narration, editing, or visual effects specifically useful for product demos;
- provide an open-source building block demonstrably used by a relevant end-to-end workflow.

The deciding question:

> **Does this repository materially reduce the work or expertise required to create a product demo video?**

### Out of scope by default

- generic text-to-image tools;
- generic chatbots;
- broad LLM or agent frameworks without a demo-production example;
- unrelated text-to-video projects;
- conventional screen recorders without automation or AI relevance;
- video players;
- generic editing libraries with no clear role in a demo pipeline;
- closed SaaS products without a relevant open-source repository.

Broad foundations (for example a browser-agent framework) can be listed, but their description must state the boundary explicitly ("an upstream interaction layer, not a demo generator").

## Entry format

Use a short bullet entry, in the most relevant section:

```markdown
- [**Project Name**](https://github.com/owner/repository) — One factual sentence
  explaining why it matters for product demo generation.  
  `Tag` `Tag` `License`
```

### Description style

Good:

> Records repeatable browser walkthroughs as MP4 and emits structured interaction metadata.

Avoid:

> The revolutionary next-generation platform that transforms content creation forever.

Describe what the project **does**, in your own words. Do not copy marketing copy.

### Tags

Use only tags that help a reader decide. Preferred vocabulary:

`End-to-end` `Agentic` `Real product` `Screenshots` `Scripted` `Playwright` `MCP` `Agent skill` `TTS` `Subtitles` `Video as code` `Post-production` `Self-hosted` `Foundation` `Early`

Always end with the license, as reported by the repository's license file (e.g. `MIT`, `Apache-2.0`). For non-OSI licenses use `Source-available` with a short note. If there is no license file, omit the tag.

Use `Early` for projects with little adoption or no release yet, so readers calibrate expectations.

## Required information in your PR

```text
Name:
URL:
Section:
License (from the license file):
Self-hostable: Yes / No
Demo-specific: Yes / No
Commercial affiliation with the project: Yes / No
Why it belongs here:
```

## Quality checklist

Before submitting, check that:

- [ ] the repository is public and not archived;
- [ ] its connection to product-demo generation is direct and explainable;
- [ ] there is a working README, example, or documented workflow;
- [ ] the description is factual and concise;
- [ ] the project is not already listed;
- [ ] the link points to the original repository (not a mirror or fork, unless the fork adds the relevant capability);
- [ ] the license is visible and accurately described;
- [ ] any commercial relationship is disclosed.

## Duplicates, forks, and stale projects

- **Duplicates:** if two projects do the same thing, keep the more mature or better-documented one, or merge both into one bullet when they are clearly related.
- **Forks:** list a fork only when it adds the demo-relevant capability (say so in the description).
- **Stale projects:** a repository with no activity for over 12 months may be marked `Stale` or moved to a removal PR. Archived repositories are removed.

## New categories

A new section is created only once there are **at least three strong entries** for it. Until then, candidates are tracked in the README's *Wanted* section.

## Corrections

Spotted a wrong license, a dead link, or an overstated capability? Open a [correction issue](.github/ISSUE_TEMPLATE/correction.yml) or send a PR directly.
