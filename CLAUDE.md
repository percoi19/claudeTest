# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **marketing AI agent configuration repository** for **Koin App** — a Brazilian BNPL (Buy Now, Pay Later) mobile app by Grupo Prosus. The core product is **Pix Parcelado**: installment purchases via Pix, without a credit card, targeting underbanked consumers (classes C/D/E, ages 20–55).

There is no application code to build, test, or run. All work here involves reading, creating, and updating markdown-based context files and agent definitions.

## Architecture

### Knowledge Base (`.claude/`)

All agents read these shared files before responding. They are the single source of truth:

| File | Purpose |
|------|---------|
| `koin_app_context.md` | Product, audience, funnel, KPIs, acquisition channels, competitors — the foundational Koin context every agent reads |
| `marketing-ideas.md` | Library of 139 proven marketing ideas organized by category, stage, budget, and timeline |
| `content-strategy.md` | Content planning framework: pillars, topic clusters, buyer-stage mapping, searchable vs. shareable content |
| `social-content.md` | Platform-native social strategy: hook formulas, content calendars, engagement routines, repurposing systems |
| `customer-research.md` | Two research modes (analyze existing assets / find online), extraction frameworks, persona generation, synthesis templates |
| `marketing-psychology.md` | 50+ mental models: foundational thinking, buyer psychology, persuasion, pricing psychology, growth models |
| `paid_ads.md` | Paid ads playbook: platform selection, campaign structure, copy frameworks (PAS/BAB), targeting, optimization |
| `referral.md` | Referral and affiliate program design: the referral loop, incentive structures, launch checklist, metrics |
| `settings.json` | Claude Code project settings: permissions, model, env vars, hooks |

### Agent Team (`.claude/agents/`)

Four specialized sub-agents, each with a defined role and collaboration contract:

| Agent | Role | Primary Files Read |
|-------|------|-------------------|
| `strategy-master.md` | Marketing strategy, channel prioritization, go-to-market planning | `marketing-ideas.md`, `koin_app_context.md` |
| `content-strategist.md` | Content pillars, editorial calendar, social media content | `content-strategy.md`, `social-content.md`, `koin_app_context.md` |
| `ads-expert.md` | Paid campaigns across Meta/Google/LinkedIn/TikTok | `paid_ads.md`, `koin_app_context.md`, `customer-research.md` |
| `customer-expert.md` | Customer research, personas, psychology, referral programs | `customer-research.md`, `marketing-psychology.md`, `referral.md`, `koin_app_context.md` |

Agents are designed to collaborate: the Strategy Master commissions others; the Customer Expert validates strategy assumptions; the Ads Expert pulls from the Content Strategist's top-performing organic content.

## Working in This Repo

### Updating context
When Koin's product, audience, or competitive landscape changes, update `koin_app_context.md` first — all four agents depend on it.

### Adding new agent knowledge
Add new playbooks as `.md` files in `.claude/`, then update the relevant agent definition in `.claude/agents/` to reference them in the "Knowledge Base" section.

### Agent product-marketing context
A `product-marketing-context.md` file (at `.agents/product-marketing-context.md`) is the expected output of the `product-marketing-context` skill. Once it exists, all agents will auto-read it. Currently this file does not exist — running the `product-marketing-context` skill will create it from `koin_app_context.md`.

## Key Business Context

- **Activation event**: First purchase (not registration). A registered user without a purchase is not considered active.
- **Core funnel**: Install → Cadastro → Credit evaluation (~35% receive a limit) → First purchase (Activation) → Recurrence
- **Credit limits**: R$200–R$500 initial; grows with on-time payments
- **Top stores by volume**: Shopee, iFood, MercadoLibre, Amazon
- **Acquisition channels**: Marketplaces de crédito, Mídia (paid ads), Organic, B2B
- **User communication channels**: Email, Push notifications, WhatsApp
- **Primary KPIs**: Activation rate, GMV, CAC per channel, retention/recurrence
