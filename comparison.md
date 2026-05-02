# AI Coding Assistant Pricing Comparison
## GitHub Copilot vs Claude Code (2026)

---

## Overview

| | GitHub Copilot | Claude Code |
|---|---|---|
| **Maker** | GitHub (Microsoft) | Anthropic |
| **How it works** | IDE plugin + chat (VS Code, JetBrains, etc.) | Terminal-first CLI + IDE integrations |
| **Billing model** | Changed from request-based to token-based on **June 1, 2026** | Subscription tiers (Pro / Max) or pay-per-token API |

---

## Part 1: GitHub Copilot

### BEFORE June 1, 2026 — Request-Based Billing

Each plan included a fixed number of **"premium requests"** per month.
Standard/included models (GPT-4o, GPT-4.1, GPT-5 mini) were free and did not count against premium requests. Advanced models consumed premium requests at a multiplier rate.

| Plan | Price | Code Completions | Premium Requests/Month |
|------|-------|-----------------|------------------------|
| **Free** | $0 | 2,000/month | 50/month |
| **Pro** | $10/month | Unlimited | 300/month |
| **Pro+** | $39/month | Unlimited | 1,500/month |
| **Business** | $19/user/month | Unlimited | 300/user/month |
| **Enterprise** | $39/user/month | Unlimited | 1,500/user/month |

#### What is a "Premium Request"?
A premium request is one interaction (e.g., one chat message, one agent task) with an advanced model. Each model had a **multiplier** — how many premium requests it costs per use.

| Model | Multiplier (before June 1) | Example cost on Pro (300 budget) |
|-------|---------------------------|----------------------------------|
| GPT-4o / GPT-4.1 / GPT-5 mini | **Included (0x)** | Unlimited — free |
| Claude 3.5 Sonnet | 1x | Uses 1 premium request per chat |
| GPT-4.5 / o1 | ~10x | Uses 10 premium requests per chat |
| Claude 3.7 Sonnet | ~1x | Uses 1 premium request per chat |

#### Example (Before June 1, Pro Plan — $10/month)
> You have **300 premium requests**. You chat 300 times with Claude 3.5 Sonnet = budget used up.
> But if you switch to GPT-4o for those same 300 chats = **no cost at all** (included model).

---

### AFTER June 1, 2026 — Usage-Based (AI Credits)

GitHub replaces premium requests with **GitHub AI Credits**.

> **1 AI Credit = $0.01 USD**

Each plan includes a monthly credit allowance matching the plan's dollar price.
Cost per interaction = **model used × tokens consumed**.

| Plan | Price | Included AI Credits/Month | Overage |
|------|-------|--------------------------|---------|
| **Free** | $0 | Limited free tier | Not available |
| **Pro** | $10/month | $10 worth (1,000 credits) | Pay-as-you-go at published rates |
| **Pro+** | $39/month | $39 worth (3,900 credits) | Pay-as-you-go at published rates |
| **Business** | $19/user/month | $19 worth per user (pooled) | Org-level budget controls |
| **Enterprise** | $39/user/month | $39 worth per user (pooled) | Org-level budget controls |

#### How Tokens Work
- Every word/code snippet sent to or received from AI = tokens
- ~750 words = ~1,000 tokens (rough estimate)
- You pay for **input tokens** (your prompt + code context) AND **output tokens** (AI response)

#### Model Credit Costs (approximate, after June 1)

| Model | Input Cost | Output Cost | Notes |
|-------|-----------|-------------|-------|
| GPT-5 mini | Low | Low | Included / cheapest |
| GPT-4.1 | Low | Low | Included |
| GPT-5.4 | Higher | Higher | ≤272K token context |
| Gemini 2.5 Pro | Medium | Medium | ≤200K token context |
| Gemini 3 Flash | Low | Low | No long-context surcharge |

#### Example (After June 1, Pro Plan — $10/month = 1,000 AI Credits)

**Scenario A: Light use with GPT-5 mini (included/cheap model)**
- 50 chat messages × ~2,000 tokens each = 100,000 tokens total
- Approximate cost: ~$0.50–$1.00
- Result: Credits barely touched, well within $10 budget

**Scenario B: Heavy use with GPT-5.4 (expensive model, long context)**
- 20 chat messages with large code files (~50,000 tokens each) = 1,000,000 tokens
- At higher token rates, this could exhaust or exceed the $10 credit budget
- Result: You either hit a wall or pay overage

**Key insight:** On the new model, **what model you choose and how much code context you send** directly determines your bill.

---

## Part 2: Claude Code

Claude Code is Anthropic's terminal-native AI coding assistant. It operates differently — you use it via CLI and it reads/edits your files directly.

### Subscription Plans (2026)

| Plan | Price | Usage Level | Best For |
|------|-------|-------------|----------|
| **Pro** | $20/month | Moderate — 5-hour rolling window | Individuals, occasional use |
| **Max 5x** | $100/month | 5x more than Pro | Daily power users |
| **Max 20x** | $200/month | 20x more than Pro | Intensive/professional use |
| **API (pay-as-you-go)** | No subscription | Unlimited, billed per token | Teams, automation, heavy usage |

> No free tier for Claude Code.

### How Usage Limits Work (Pro/Max Plans)

Claude Code uses a **5-hour rolling window**, not a simple monthly counter.

- Your token budget constantly refills over a rolling 5-hour period
- If you burn through your budget in a 2-hour burst of heavy coding, you may be paused for a few hours
- Pro plan: ~44,000 token rolling window per 5-hour period
- Max plans multiply this window (5x or 20x)

#### Example: Claude Code Pro — $20/month

**Scenario A: Focused 1-hour coding session**
- You ask Claude to refactor a 500-line file, write tests, and explain the changes
- Estimated token use: ~30,000–40,000 tokens
- Result: Likely within budget for that session, minimal throttling

**Scenario B: Intensive all-day coding sprint**
- You run Claude Code continuously for 6+ hours, large codebase
- You may hit the rolling window limit and get paused mid-session
- Fix: Wait ~1 hour for window to refill, or upgrade to Max

### API Pricing (For Teams/Automation)

If you use Claude via the Anthropic API directly (no subscription):

| Model | Input | Output |
|-------|-------|--------|
| Claude Sonnet 4.6 | $3 / 1M tokens | $15 / 1M tokens |
| Claude Opus 4.6 | Higher | Higher |

#### API Example
> You send a 10,000-token prompt (a large code file + instructions).
> Claude returns a 2,000-token response (rewritten code).
> Cost: (10,000 × $0.000003) + (2,000 × $0.000015) = **$0.03 + $0.03 = $0.06 per request**
> At 100 requests/day × 22 workdays = ~$132/month

---

## Part 3: Side-by-Side Comparison

| | GitHub Copilot Pro (after June 1) | Claude Code Pro |
|---|---|---|
| **Price** | $10/month | $20/month |
| **Billing unit** | AI Credits (token-based) | Rolling usage window |
| **Monthly budget** | $10 in credits | Fixed tier, not dollar-based |
| **IDE integration** | Native (VS Code, JetBrains, etc.) | Via plugin + terminal |
| **Code completions** | Yes, inline as you type | No inline completions |
| **Chat / Q&A** | Yes | Yes |
| **File editing** | Limited (Copilot Edits) | Full file system access |
| **Model choice** | Multiple (GPT, Gemini, Claude) | Claude models only |
| **Predictable bill?** | Less predictable (token usage varies) | More predictable (flat tier) |
| **Risk of surprise bill** | Yes, if you use expensive models heavily | No, capped at tier price |

---

## Part 4: Which Should You Choose?

### Choose GitHub Copilot if you...
- Want **inline code completions** as you type
- Work inside a **full IDE** (VS Code, JetBrains)
- Want access to **multiple AI models** (GPT, Gemini, Claude)
- Already have a GitHub subscription in your organization
- Do moderate chat usage (can stick to included models to stay in budget)

### Choose Claude Code if you...
- Prefer a **terminal-first workflow**
- Want Claude to **read and edit your files** autonomously
- Value a **flat, predictable monthly price**
- Do deep, multi-file refactoring or long agentic tasks
- Are okay paying $20–$100/month for serious use

---

## Summary: The Biggest Change for Copilot Users

| | Before June 1, 2026 | After June 1, 2026 |
|---|---|---|
| **What you pay for** | A fixed number of premium requests | Tokens consumed × model rate |
| **Predictability** | High — you know your request budget | Low — depends on how much context you send |
| **Cheap heavy use** | Possible (use included models) | Possible (use cheap models like GPT-5 mini) |
| **Expensive mistake** | Using high-multiplier models (o1, GPT-4.5) | Sending large code files to expensive models |
| **Power users** | Could hit 300 request limit quickly | Could exhaust $10 credit budget quickly |

> **Bottom line:** Copilot's new model rewards users who choose cheaper models and send focused, smaller prompts.
> Claude Code's flat-rate model rewards users who want unlimited depth within a session without tracking token costs.

---

*Sources verified as of May 2026. Prices subject to change.*
