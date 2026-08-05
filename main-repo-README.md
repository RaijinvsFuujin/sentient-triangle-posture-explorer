# Sentient Triangle Toolkit

AI-behavior ideation tooling built on Josh Clark & Veronika Kindred's [*Sentient Design*](https://rosenfeldmedia.com/books/sentient-design/) framework (Rosenfeld Media) — a lens for pushing AI-mediated feature design past the chatbot default by mapping experiences across three attributes (**grounded**, **interoperable**, **radically adaptive**) into four archetypes and 18 named postures.

This repo packages that framework as working tooling across the AI coding/design tools our team actually has access to, so the same divergent-thinking process runs the same way regardless of which tool someone opens.

## What's here

| Folder | Tool | What it does |
|---|---|---|
| [`claude-skill/`](./claude-skill) | Claude (claude.ai, Claude Code, Claude Design) | Full skill — ideation *and* keeps prototype builds faithful to their assigned posture |
| [`cursor-rule/`](./cursor-rule) | Cursor | Repo rules — ideation prompt + build-fidelity checks, auto-load when relevant |
| [`copilot-prompts/`](./copilot-prompts) | Microsoft Copilot Chat | Copy-paste prompt for ideation (Copilot Chat has no repo access or persistent memory, so this one's manual) |

Each folder has its own README with setup/usage specifics.

## The core idea

Most AI feature scoping defaults to "make it a chatbot" without examining the alternatives. This toolkit forces a deliberate pass through genuinely different **postures** — Tools, Chat, Agents, Copilots, and the finer postures within each — before anyone commits to an interaction pattern. The output is a handful of divergent prototype briefs, each specifying who has initiative, what interface (if any) appears, and how failure is handled — differences a builder can actually implement differently, not just re-skin.

## Where the framework content lives

The full posture taxonomy and provocation questions are maintained once, in [`claude-skill/references/postures.md`](./claude-skill/references/postures.md), and referenced from there by the Cursor and Copilot implementations rather than duplicated. If you're updating the taxonomy, edit it there first.

## A note on how to use this

The postures and provocation questions are meant to be sparks for divergent thinking, not a checklist to complete. Pull what's relevant to the problem in front of you; don't feel obligated to work through every posture or every question every time.
