# 🧱 Reference Architecture

Non-prescriptive sketches of how an agentic demo-generation pipeline can be assembled.

## 🤖 The Agentic Demo Pipeline

A particularly interesting direction is treating demo production as an **agentic workflow** rather than a video-editing problem.

Imagine giving an agent:

```text
Product:
https://my-product.example

Objective:
Show how a new user can create their first AI agent.

Audience:
Developers and solution architects.

Duration:
90 seconds.

Style:
Concise, technical, polished.
```

The system could then:

```text
1. Understand the product
       ↓
2. Explore the UI
       ↓
3. Identify the important user journey
       ↓
4. Generate the storyline
       ↓
5. Plan the interactions
       ↓
6. Operate the application
       ↓
7. Capture the screen
       ↓
8. Generate narration
       ↓
9. Synchronize voice + actions
       ↓
10. Edit the recording
       ↓
11. Add zooms / cursor effects / captions
       ↓
12. Apply branding
       ↓
13. Render
       ↓
🎬 Product Demo
```

This is where **LLMs + multimodal models + browser agents + programmatic video generation** start to converge.

## 🧱 Platform sketch

A possible architecture for an AI-native demo generation platform:

```text
                    ┌─────────────────────┐
                    │    Demo Request     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Demo Orchestrator │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             ▼                 ▼                 ▼
      Product Agent       Story Agent       Brand Context
             │                 │                 │
             ▼                 ▼                 │
       UI Understanding    Storyboard            │
             │                 │                 │
             └─────────┬───────┘                 │
                       ▼                         │
                Browser Agent                    │
                       │                         │
                 ┌─────┴─────┐                   │
                 ▼           ▼                   │
              Actions      Capture                │
                 │           │                   │
                 └─────┬─────┘                   │
                       ▼                         │
                Media Pipeline ◄─────────────────┘
                       │
             ┌─────────┼──────────┐
             ▼         ▼          ▼
           Voice     Editing    Captions
             │         │          │
             └─────────┼──────────┘
                       ▼
                    Renderer
                       │
                       ▼
                  🎬 DEMO VIDEO
```

This is only one possible architecture rather than a prescribed implementation.

## 🧪 Experiments & Proofs of Concept

Not everything needs to be production-ready.

Interesting experiments can reveal where product demo generation is heading.

### Product → Script

```text
README / Documentation
        ↓
       LLM
        ↓
 Demo storyline
        ↓
   Voice-over script
```

### Product → Browser Agent → Recording

```text
Demo objective
      ↓
  AI Agent
      ↓
Browser automation
      ↓
Screen capture
      ↓
Raw demo
```

### Fully Agentic Demo Generation

```text
                 Product
                    │
                    ▼
            Product Understanding
                    │
                    ▼
              Story Planner
                    │
            ┌───────┴───────┐
            ▼               ▼
      Browser Agent     Voice Agent
            │               │
            ▼               ▼
       UI Actions        Narration
            │               │
            └───────┬───────┘
                    ▼
              Video Editor
                    │
                    ▼
             Visual Polish
                    │
                    ▼
               🎬 DEMO
```

If you've built an experiment in this space, **we'd love to see it**.

---

[← Back to the list](../README.md)
