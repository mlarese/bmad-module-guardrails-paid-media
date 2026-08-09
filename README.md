# Guardrails Paid Media (`gpm`)

A focused BMad module for paid media, Google Ads, tracking, consent, social content, and creative production. It keeps campaigns and assets behind evidence, approval, and rollback gates.

This is a focused BMad module in the [Guardrails](https://github.com/mlarese/bmad-module-guardrails)
bundle. It keeps the same behavior and shared memory while installing only the figures and
workflows for the paid media area.

> **Generated.** This repository is produced by `tools/build_modules.py` in the
> [bmad-module-guardrails](https://github.com/mlarese/bmad-module-guardrails) repository.
> Make changes there and regenerate; local changes here will be overwritten.

## Agents

| Agent | Role | Skill | Focus |
| ----- | ---- | ----- | ----- |
| 🛡️ Vera | Data Protection Officer | `grl-agent-privacy` | Personal data, GDPR, DPIAs, retention, analytics, logs, and data in prompts. |
| ⚖️ Aldo | Tech Lawyer | `grl-agent-legal` | Licenses, contracts, DPAs, ownership, AI outputs, and AI Act obligations. |
| 👁️ Iris | Design Critic | `grl-agent-ui-critic` | UI, landing pages, markup, CSS, typography, palettes, density, and layout. |
| 🔎 Nora | SEO Strategist & Search Systems Auditor | `grl-agent-seo` | Search intent, crawling, indexing, content, structured data, and Search Console. |
| 📣 Dalia | Media Manager & Paid Advertising Strategist | `grl-agent-ads` | Google Ads, paid advertising, audiences, creative, tracking, consent, budgets, and policies. |
| 📱 Sofia | Social Media & Content Strategist | `grl-agent-social` | Organic strategy, content pillars, calendars, posts, captions, community, and metrics. |
| 🎬 Marco | Advertising Creative Director & Short-form Video Producer | `grl-agent-creative` | Advertising concepts, design, scripts, storyboards, shot lists, Reels, TikToks, and Shorts. |

## Skills and workflows

| Skill | Purpose |
| ----- | ------- |
| `gpm-profile` | Project profile | Collects the project context shared by every installed figure. |
| `gpm-board` | Multidisciplinary review | Convenes the relevant figures on one artifact and returns a review summary or release verdict. |
| `grl-ads` | Paid media operations | Audits, plans, tracks, optimizes, preflights, and applies paid-media change sets behind approval and rollback gates. |
| `grl-social` | Organic social strategy | Builds social strategies, calendars, content, audits, and measurement plans without scheduling or publishing. |
| `grl-social-creative` | Social creative production | Turns a brief into producible concepts, scripts, storyboards, shot lists, specifications, and channel variants. |
| `grl-automation` | Controlled automation | Routes work from read-only checks through dry-run to observable execution, with explicit approvals and rollback. |

## Installation

```
bmad install gpm
```

As a first step, run `gpm-profile`. It collects the project profile — sector, data,
market, stack, and criticality — so each figure can calibrate its review. Without a profile,
the default remains `normal` and the figures start without context.

## Shared memory

The profile lives in `{project-root}/_bmad/memory/grl-shared/project-profile.md`, together
with `decisions.md` and `accepted-risks.md`. All Guardrails modules use the same path, so two
installed modules still share one profile.

## Using it with the bundle

This module installs skills with **the same names** as the `grl` bundle — `grl-agent-privacy`
is identical in both. Do not install the full bundle and thematic modules in the same project:
choose the complete bundle, or only the thematic modules you need.

## License

MIT.
