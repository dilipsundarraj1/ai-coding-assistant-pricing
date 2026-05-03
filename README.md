<!-- TOC -->
* [AI Coding Assistant Pricing Comparison](#ai-coding-assistant-pricing-comparison)
  * [Why This Matters](#why-this-matters)
  * [Part 1: GitHub Copilot](#part-1-github-copilot)
    * [BEFORE June 1, 2026 — Request-Based Billing](#before-june-1-2026--request-based-billing)
      * [Model Multipliers (Before June 1)](#model-multipliers-before-june-1)
    * [AFTER June 1, 2026 — Usage-Based (AI Credits)](#after-june-1-2026--usage-based-ai-credits)
      * [Model Credit Costs (After June 1)](#model-credit-costs-after-june-1)
  * [Part 1b: Free Tier vs. Included vs. Premium — Before & After June 1](#part-1b-free-tier-vs-included-vs-premium--before--after-june-1)
    * [Billing Comparison Table](#billing-comparison-table)
    * [Included (Non-Premium) Models](#included-non-premium-models)
    * [Premium Models](#premium-models)
      * [OpenAI](#openai)
      * [Anthropic](#anthropic)
      * [Google](#google)
      * [Other](#other)
  * [Part 2: Claude Code](#part-2-claude-code)
    * [Subscription Plans (2026)](#subscription-plans-2026)
    * [How Usage Limits Work](#how-usage-limits-work)
    * [API Pricing](#api-pricing)
  * [Part 3: Side-by-Side Comparison](#part-3-side-by-side-comparison)
  * [Part 4: Direct Dollar Comparison — Real Developer Scenarios](#part-4-direct-dollar-comparison--real-developer-scenarios)
    * [Persona 1: The Student / Casual Learner](#persona-1-the-student--casual-learner)
    * [Persona 2: The Working Developer](#persona-2-the-working-developer)
    * [Persona 3: The Power User / Full-Time AI Developer](#persona-3-the-power-user--full-time-ai-developer)
    * [Dollar Summary Table](#dollar-summary-table)
  * [Part 5: Spending Controls](#part-5-spending-controls)
    * [GitHub Copilot — Spending Controls (After June 1, 2026)](#github-copilot--spending-controls-after-june-1-2026)
      * [For Individual Users (Pro / Pro+)](#for-individual-users-pro--pro)
      * [For Teams / Organizations (Business / Enterprise)](#for-teams--organizations-business--enterprise)
    * [Claude Code — Spending Controls](#claude-code--spending-controls)
      * [For Subscription Users (Pro / Max)](#for-subscription-users-pro--max)
      * [For API Users (Pay-as-you-go)](#for-api-users-pay-as-you-go)
    * [Spending Control Comparison](#spending-control-comparison)
  * [Part 6: Which Should You Choose?](#part-6-which-should-you-choose)
    * [GitHub Copilot is the better choice for most developers](#github-copilot-is-the-better-choice-for-most-developers)
    * [When Claude Code makes sense](#when-claude-code-makes-sense)
  * [Summary: The Biggest Change for Copilot Users](#summary-the-biggest-change-for-copilot-users)
<!-- TOC -->

# AI Coding Assistant Pricing Comparison

---

## Why This Matters

AI coding tools are now standard in developer workflows, but their pricing is getting more complex. Understanding costs helps you:

- **Use AI confidently** — without unconsciously avoiding features to stay under budget
- **Avoid bill shock** — especially with Copilot's shift to token-based billing on June 1, 2026
- **Save real money** — choosing the right model can save a team hundreds of dollars per month

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

#### Model Multipliers (Before June 1)

| Model | Provider | Multiplier | Notes |
|-------|----------|-----------|-------|
| GPT-4.1 | OpenAI | **Included (0×)** | Unlimited — free on all paid plans |
| GPT-5 mini | OpenAI | **Included (0×)** | Unlimited — free on all paid plans |
| GPT-4o | OpenAI | **Included (0×)** | Unlimited — free on all paid plans |
| GPT-5.2 / 5.2-Codex / 5.3-Codex | OpenAI | 1× | 1 request per chat |
| GPT-5.4 | OpenAI | 1× | 1 request per chat |
| GPT-5.4 mini | OpenAI | 0.33× | ~3 chats per premium request |
| GPT-5.4 nano | OpenAI | 0.25× | ~4 chats per premium request |
| GPT-5.5 | OpenAI | 7.5× | 7.5 requests per chat |
| Claude Haiku 4.5 | Anthropic | 0.33× | ~3 chats per premium request |
| Claude Sonnet 4 / 4.5 / 4.6 | Anthropic | 1× | 1 request per chat |
| Claude Opus 4.5 / 4.6 | Anthropic | 3× | 3 requests per chat |
| Claude Opus 4.6 (fast mode) | Anthropic | 30× | 30 requests per chat |
| Claude Opus 4.7 | Anthropic | 15× | 15 requests per chat |
| Gemini 2.5 Pro | Google | 1× | 1 request per chat |
| Gemini 3 Flash | Google | 0.33× | ~3 chats per premium request |
| Gemini 3.1 Pro | Google | 1× | 1 request per chat |
| Grok Code Fast 1 | xAI | 0.25× | ~4 chats per premium request |

> **Copilot Free:** every interaction with any premium model counts as 1 request against the 50/month limit, regardless of model.

---

### AFTER June 1, 2026 — Usage-Based (AI Credits)

GitHub replaces premium requests with **GitHub AI Credits**.

> **1 AI Credit = $0.01 USD**

| Plan | Price | Included AI Credits/Month | Overage |
|------|-------|--------------------------|---------|
| **Free** | $0 | Limited free tier | Not available |
| **Pro** | $10/month | $10 worth (1,000 credits) | Pay-as-you-go at published rates |
| **Pro+** | $39/month | $39 worth (3,900 credits) | Pay-as-you-go at published rates |
| **Business** | $19/user/month | $19 worth per user (pooled) | Org-level budget controls |
| **Enterprise** | $39/user/month | $39 worth per user (pooled) | Org-level budget controls |

#### Model Credit Costs (After June 1)

> Rates are per 1 million tokens (MTok). 1 AI Credit = $0.01. **Code completions and Next Edit Suggestions are not billed** — they remain unlimited for all paid plans.

| Model | Provider | Type | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Notes |
|-------|----------|------|---------------|----------------------|----------------|-------|
| GPT-5 mini | OpenAI | **Included** | $0.25 | $0.025 | $2.00 | Cheapest option |
| GPT-4.1 | OpenAI | **Included** | $2.00 | $0.50 | $8.00 | — |
| GPT-5.2 | OpenAI | Premium | $1.75 | $0.175 | $14.00 | — |
| GPT-5.2-Codex | OpenAI | Premium | $1.75 | $0.175 | $14.00 | — |
| GPT-5.3-Codex | OpenAI | Premium | $1.75 | $0.175 | $14.00 | — |
| GPT-5.4 | OpenAI | Premium | $2.50 | $0.25 | $15.00 | ≤272K token context |
| GPT-5.4 mini | OpenAI | Premium | $0.75 | $0.075 | $4.50 | — |
| GPT-5.4 nano | OpenAI | Premium | $0.20 | $0.02 | $1.25 | Chat/Edit only |
| GPT-5.5 | OpenAI | Premium | $5.00 | $0.50 | $30.00 | Most expensive OpenAI model |
| Claude Haiku 4.5 | Anthropic | Premium | $1.00 | $0.10 | $5.00 | — |
| Claude Sonnet 4 / 4.5 / 4.6 | Anthropic | Premium | $3.00 | $0.30 | $15.00 | — |
| Claude Opus 4.5 / 4.6 / 4.7 | Anthropic | Premium | $5.00 | $0.50 | $25.00 | — |
| Gemini 2.5 Pro | Google | Premium | $1.25 | $0.125 | $10.00 | ≤200K token context |
| Gemini 3 Flash | Google | Premium | $0.50 | $0.05 | $3.00 | No long-context surcharge |
| Gemini 3.1 Pro | Google | Premium | $2.00 | $0.20 | $12.00 | ≤200K token context |
| Grok Code Fast 1 | xAI | Premium | $0.20 | $0.02 | $1.50 | — |

> **Note for Anthropic models:** Cache write also incurs a cost — $1.25/MTok (Haiku), $3.75/MTok (Sonnet), $6.25/MTok (Opus).

---

## Part 1b: Free Tier vs. Included vs. Premium — Before & After June 1

### Billing Comparison Table

| | **Free Tier** | **Included Models** (Paid Plans) | **Premium Models** (Paid Plans) |
|---|---|---|---|
| **Models** | All models (limited quota) | GPT-4.1, GPT-5 mini, GPT-4o | All other models |
| **Before June 1 — unit** | Premium requests | Unlimited — no requests consumed | Premium requests |
| **Before June 1 — monthly budget** | 50 requests/month | Unlimited | 300/mo (Pro) · 1,500/mo (Pro+) |
| **Before June 1 — cost per chat** | 1 request per chat (any model) | $0 | 0.25×–30× requests per chat |
| **After June 1 — unit** | AI Credits (limited allowance) | AI Credits (token-based) | AI Credits (token-based) |
| **After June 1 — input cost range** | Same rates as premium models | $0.25–$2.00 / MTok | $0.20–$5.00 / MTok |
| **After June 1 — output cost range** | Same rates as premium models | $2.00–$8.00 / MTok | $1.25–$30.00 / MTok |
| **Inline completions** | 2,000/month (not token-billed) | Unlimited (not token-billed) | Unlimited (not token-billed) |

> **Key shift:** Before June 1, included models were truly unlimited and free. After June 1, every model costs credits based on tokens — but included models remain the cheapest options.

---

### Included (Non-Premium) Models

| Model | Provider | Before June 1 | After June 1 — Input / Output (per MTok) |
|-------|----------|--------------|------------------------------------------|
| **GPT-4.1** | OpenAI | Included — unlimited | $2.00 / $8.00 |
| **GPT-5 mini** | OpenAI | Included — unlimited | $0.25 / $2.00 |
| **GPT-4o** | OpenAI | Included — unlimited | Legacy (superseded by GPT-4.1) |

Sources: [Supported models](https://docs.github.com/en/copilot/reference/ai-models/supported-models) · [Models and pricing](https://docs.github.com/en/copilot/reference/copilot-billing/models-and-pricing) · [Copilot requests](https://docs.github.com/en/copilot/concepts/billing/copilot-requests)

---

### Premium Models

#### OpenAI

| Model | Multiplier (Before June 1) | Input / Output (After June 1, per MTok) |
|-------|---------------------------|------------------------------------------|
| GPT-5.2 | 1× | $1.75 / $14.00 |
| GPT-5.2-Codex | 1× | $1.75 / $14.00 |
| GPT-5.3-Codex | 1× | $1.75 / $14.00 |
| GPT-5.4 | 1× | $2.50 / $15.00 |
| GPT-5.4 mini | 0.33× | $0.75 / $4.50 |
| GPT-5.4 nano | 0.25× | $0.20 / $1.25 |
| GPT-5.5 | 7.5× | $5.00 / $30.00 |

#### Anthropic

| Model | Multiplier (Before June 1) | Input / Output (After June 1, per MTok) |
|-------|---------------------------|------------------------------------------|
| Claude Haiku 4.5 | 0.33× | $1.00 / $5.00 |
| Claude Sonnet 4 / 4.5 / 4.6 | 1× | $3.00 / $15.00 |
| Claude Opus 4.5 / 4.6 | 3× | $5.00 / $25.00 |
| Claude Opus 4.6 (fast mode) | 30× | $5.00 / $25.00 |
| Claude Opus 4.7 | 15× | $5.00 / $25.00 |

#### Google

| Model | Multiplier (Before June 1) | Input / Output (After June 1, per MTok) |
|-------|---------------------------|------------------------------------------|
| Gemini 2.5 Pro | 1× | $1.25 / $10.00 |
| Gemini 3 Flash | 0.33× | $0.50 / $3.00 |
| Gemini 3.1 Pro | 1× | $2.00 / $12.00 |

#### Other

| Model | Provider | Multiplier (Before June 1) | Input / Output (After June 1, per MTok) |
|-------|----------|---------------------------|------------------------------------------|
| Grok Code Fast 1 | xAI | 0.25× | $0.20 / $1.50 |
| Raptor mini | GitHub (fine-tuned) | — | Public preview |
| Goldeneye | GitHub (fine-tuned) | — | Public preview |

Sources: [Supported models](https://docs.github.com/en/copilot/reference/ai-models/supported-models) · [Models and pricing](https://docs.github.com/en/copilot/reference/copilot-billing/models-and-pricing) · [AI model comparison](https://docs.github.com/en/copilot/reference/ai-models/model-comparison) · [Copilot requests](https://docs.github.com/en/copilot/concepts/billing/copilot-requests)

---

## Part 2: Claude Code

Claude Code is Anthropic's terminal-native AI coding assistant. It reads and edits your files directly via CLI.

### Subscription Plans (2026)

| Plan | Price | Usage Level | Best For |
|------|-------|-------------|----------|
| **Pro** | $20/month | Moderate — 5-hour rolling window | Individuals, occasional use |
| **Max 5x** | $100/month | 5x more than Pro | Daily power users |
| **Max 20x** | $200/month | 20x more than Pro | Intensive/professional use |
| **API (pay-as-you-go)** | No subscription | Unlimited, billed per token | Teams, automation, heavy usage |

> No free tier for Claude Code.

### How Usage Limits Work

Claude Code uses a **5-hour rolling window**, not a monthly counter. If you burn through your budget in a short burst, you may be paused for a few hours while the window refills.

### API Pricing

| Model | Input | Output |
|-------|-------|--------|
| Claude Sonnet 4.6 | $3 / 1M tokens | $15 / 1M tokens |
| Claude Opus 4.6 | Higher | Higher |

---

## Part 3: Side-by-Side Comparison

| | GitHub Copilot Pro (after June 1) | Claude Code Pro |
|---|---|---|
| **Price** | **$10/month** | $20/month |
| **Free tier** | **Yes ($0/month)** | No |
| **Billing unit** | AI Credits (token-based) | Rolling usage window |
| **Minimum monthly cost** | **$0** | $20 |
| **IDE integration** | **Native (VS Code, JetBrains, etc.)** | Via plugin + terminal only |
| **Inline code completions** | **Yes — as you type** | No |
| **Chat / Q&A** | Yes | Yes |
| **Model choice** | **GPT, Gemini, Claude, and more** | Claude models only |
| **Included (free) models** | **Yes — GPT-4.1, GPT-5 mini at $0** | No — all usage counts against tier |
| **File editing** | Copilot Edits (improving rapidly) | Full file system access |
| **Spending controls** | **Granular — per user, team, enterprise** | Tier-based only |
| **Risk of surprise bill** | Low if overage is disabled (1 setting) | None — but throttled when limit hit |

> **Copilot wins on price, IDE integration, model variety, and spending flexibility.**
> Claude Code's advantage is deeper autonomous file editing for terminal-first workflows.

---

## Part 4: Direct Dollar Comparison — Real Developer Scenarios

### Persona 1: The Student / Casual Learner
**Usage:** ~30 min/day, asks questions, gets help with assignments, light code generation

| | GitHub Copilot (after June 1) | Claude Code |
|---|---|---|
| **Plan** | Pro — $10/month | Pro — $20/month |
| **Included credits** | $10 (1,000 AI credits) | Flat subscription |
| **Estimated token use** | ~100 chat messages × 2,000 tokens = 200K tokens | Same light usage |
| **Model used** | GPT-5 mini (included, near-zero cost) | Claude Sonnet 4.6 |
| **Estimated credit spend** | ~$0.50–$1.00 of the $10 budget | N/A — flat rate |
| **Monthly bill** | **$10** (plenty of headroom) | **$20** |
| **Verdict** | Copilot wins on price for light use | Overkill for casual use |

> **Dollar difference: Copilot saves you $10/month** for light, casual usage — as long as you stick to included models.

---

### Persona 2: The Working Developer
**Usage:** 4–6 hours/day coding, daily AI chat, code reviews, refactoring tasks, some agentic sessions

| | GitHub Copilot (after June 1) | Claude Code |
|---|---|---|
| **Plan** | Pro+ — $39/month | Pro — $20/month |
| **Included credits** | $39 (3,900 AI credits) | Flat subscription |
| **Estimated token use** | 300 chat messages, mix of models, some large file contexts | Heavy daily sessions |
| **Model used** | GPT-4.1 (included, free) for most tasks; GPT-5.4 only when needed | Claude Sonnet 4.6 |
| **Estimated credit spend** | ~$5–$15 if using included models smartly | N/A |
| **Monthly bill** | **$39** (well within credits with smart model choice) | **$20** (may hit rolling window limits and pause) |
| **Verdict** | Copilot wins: inline completions + IDE integration + multiple models, all within budget | Claude Code is cheaper but throttles during sprints and lacks inline completions |

---

### Persona 3: The Power User / Full-Time AI Developer
**Usage:** 8+ hours/day, autonomous agentic tasks, large codebases, multi-file rewrites, running multiple sessions

| | GitHub Copilot (after June 1) | Claude Code |
|---|---|---|
| **Plan** | Enterprise — $39/user/month | Max 5x — $100/month |
| **Included credits** | $39 worth per user (pooled in org) | Flat subscription, 5x usage headroom |
| **Estimated token use** | 500+ messages + large file contexts + agent runs | Continuous deep coding sessions |
| **Model used** | GPT-5.4 / Gemini 2.5 Pro (high-cost models) | Claude Opus 4.6 |
| **Estimated credit spend** | Likely exhausts $39 credits mid-month; overage could add $20–$60+ | N/A |
| **Monthly bill** | **$59–$100+** (base + overage, unpredictable) | **$100** (fixed, predictable) |
| **Verdict** | Copilot cost becomes unpredictable at this level | Claude Code is flat and reliable |

> **Dollar difference: roughly the same cost ($100), but Claude Code is predictable while Copilot can surprise you** with overages.

---

### Dollar Summary Table

| Developer Type | Copilot Monthly Bill | Claude Code Monthly Bill | Better Value |
|----------------|---------------------|--------------------------|--------------|
| Student / Casual | **$10** (or $0 on Free) | $20 | **Copilot** — half the price |
| Working Developer | **$39** (smart model use) | $20 + throttling risk | **Copilot** — more features for $19 more |
| Power User | **$39–$100** (org controls) | $100 (fixed) | **Copilot** — pooled credits, more flexibility |

---

## Part 5: Spending Controls

### GitHub Copilot — Spending Controls (After June 1, 2026)

#### For Individual Users (Pro / Pro+)
| Control | How It Works |
|---------|-------------|
| **Model selection** | Manually pick a cheaper model (e.g., GPT-5 mini instead of GPT-5.4) to reduce token cost |
| **Included models** | GPT-4.1 and GPT-5 mini are free — using them means zero credit spend |
| **Preview bill dashboard** | GitHub is launching a billing preview in May 2026 so you can see projected costs before June 1 |
| **Overage toggle** | You can choose to block additional usage once credits run out (hard cap at your plan price) |

#### For Teams / Organizations (Business / Enterprise)
| Control | Who Sets It | What It Does |
|---------|------------|--------------|
| **Enterprise-level budget** | Admin | Sets a monthly cap for the whole organization |
| **Cost center budgets** | Admin | Splits budget across teams or departments |
| **Per-user budgets** | Admin | Limits how much each individual can spend |
| **Pooled credits** | Automatic | Unused credits from one user can be used by others in the org |
| **Block overage** | Admin | Stops usage when the pool is empty instead of charging more |

---

### Claude Code — Spending Controls

#### For Subscription Users (Pro / Max)
| Control | How It Works |
|---------|-------------|
| **Tier selection** | You choose Pro ($20), Max 5x ($100), or Max 20x ($200) upfront |
| **No overage** | When your rolling window is exhausted, Claude Code pauses — it does NOT charge you more |
| **Hard ceiling = your plan price** | Impossible to spend more than your tier. Period. |
| **Upgrade on demand** | If you keep hitting limits, you upgrade to the next tier — a conscious, deliberate choice |

#### For API Users (Pay-as-you-go)
| Control | How It Works |
|---------|-------------|
| **Anthropic Console spending limits** | Set a hard monthly dollar cap in the API console |
| **Model selection** | Use Sonnet 4.6 ($3/MTok input) instead of Opus 4.6 (higher) for cheaper runs |
| **Prompt caching** | Cache repeated context (like large codebases) to reduce input token costs significantly |
| **Per-key limits** | Set spend limits on individual API keys for teams |

---

### Spending Control Comparison

| | GitHub Copilot (after June 1) | Claude Code Subscription | Claude Code API |
|---|---|---|---|
| **Can you set a hard spending cap?** | Yes (toggle overage off) | Built-in — no overage possible | Yes (console limit) |
| **Risk of surprise charges** | Low if you disable overage; higher if left on | None | None if cap is set |
| **Granularity of control** | Enterprise/team/user level budgets | Choose your tier | Per API key |
| **What happens when limit is hit** | Usage stops (if overage blocked) | Throttled for ~1 hour, then resumes | API calls rejected |
| **Cheapest possible bill** | $0 (Free plan) or $10 (Pro, use included models only) | $20 (Pro plan minimum) | Pay only what you use |
| **Most predictable bill** | Copilot with overage disabled | Any Claude Code tier | With a hard cap set |

---

## Part 6: Which Should You Choose?

### GitHub Copilot is the better choice for most developers

| Reason | Why It Matters |
|--------|---------------|
| **Free tier available** | You can start at $0 — Claude Code has no free option |
| **Inline code completions** | Suggestions appear as you type in your IDE — Claude Code has nothing like this |
| **Native IDE experience** | Works inside VS Code, JetBrains, Visual Studio — no terminal required |
| **Multiple AI models** | Access GPT, Gemini, and Claude models — not locked into one provider |
| **Included free models** | GPT-4.1 and GPT-5 mini cost $0 — use them all month within your plan |
| **Granular budget controls** | Set hard caps at user, team, or enterprise level |
| **Lower entry price** | $10/month vs $20/month minimum for Claude Code |
| **Already in your workflow** | Integrates with GitHub PRs, code review, and Actions |

### When Claude Code makes sense

Consider it **in addition to** Copilot only if:
- You frequently do large autonomous refactors across many files at once
- You prefer working primarily in the terminal
- You're on a team already paying for Claude API access

---

## Summary: The Biggest Change for Copilot Users

| | Before June 1, 2026 | After June 1, 2026 |
|---|---|---|
| **What you pay for** | A fixed number of premium requests | Tokens consumed × model rate |
| **Predictability** | High — you know your request budget | Low — depends on how much context you send |
| **Cheap heavy use** | Possible (use included models) | Possible (use cheap models like GPT-5 mini) |
| **Expensive mistake** | Using high-multiplier models (o1, GPT-4.5) | Sending large code files to expensive models |
| **Power users** | Could hit 300 request limit quickly | Could exhaust $10 credit budget quickly |

> **Bottom line:** GitHub Copilot is the smarter investment for most developers — lower price, more features, model flexibility, and a free tier. Use included models for everyday work and reserve premium models for hard problems.

---

*Sources verified as of May 2026. Prices subject to change.*
