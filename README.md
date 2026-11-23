# Revenue-Centric Design — an Agent Skill

![Agent Skill](https://img.shields.io/badge/Agent-Skill-5b4ee6)
![Principles](https://img.shields.io/badge/principles-158-2ea44f)
![Themes](https://img.shields.io/badge/themes-12-2ea44f)
![Updated](https://img.shields.io/badge/updated-2026--11--23-e67e22)

> A distilled, English-language playbook for designing SaaS & startup products that **convert, retain, and monetize** — packaged as an [Agent Skill](https://agentskills.io) for Claude Code, Cursor, Codex, Copilot, Gemini, and any [skills.sh](https://skills.sh)-compatible agent.

**158 principles** distilled from the X/Twitter writing of **Richard ([@richardrx](https://x.com/richardrx))** — a product designer specializing in conversion-rate optimization, churn reduction, and applied behavioral science (**ex-Volkswagen, ex-PayPal, ex-IBM**). The throughline is his coined philosophy, **Revenue-Centric Design (RCD)**: design should serve the user _and_ the business — value and revenue, not one or the other.

> **Last updated:** 23 November 2026
> **Coverage:** @richardrx's curated posts from **3 Nov 2025 → 20 Nov 2026** (166 posts). Anything posted after this date is not yet included — see [Updating](#updating).

## Install

```bash
npx skills add heliocosta-dev/revenue-centric-design
```

This pulls the skill into your agent's skills directory (`.claude/skills/`, `.agents/skills/`, …) and works with any Agent Skills–compatible agent.

**Already installed it?** Pull the latest version with `npx skills update revenue-centric-design` (or a bare `npx skills update` to refresh every installed skill). The command re-fetches from GitHub; your agent picks up the new content on its next session.

Or install it manually:

```bash
git clone https://github.com/heliocosta-dev/revenue-centric-design.git ~/.claude/skills/revenue-centric-design
```

## ⚠️ Usage boundary

> 🚫 **Not for betting, casino, or gambling products.** The author granted permission to reuse this material on the explicit condition that it is **never used for gambling/betting/casino work** (including loot-box / real-money-gaming mechanics). The skill instructs agents to decline such requests. See [LICENSE](LICENSE).

## What's inside

The skill loads only the theme relevant to your question (progressive disclosure). Each principle follows a fixed shape — **Principle → Apply when → The move → Evidence → Visual → Source** — so your agent gets the _named lever_ (decoy effect, Swiss Knife Index, GBB, Eugene Schwartz's awareness levels, loss aversion, peak-end rule…), the concrete action, and the proof.

| Theme                                                                      | Principles | Covers                                               |
| -------------------------------------------------------------------------- | ---------: | ---------------------------------------------------- |
| [Conversion & Landing Pages](references/conversion-and-landing-pages.md)   |         28 | hero/copy, CTAs, social proof, awareness levels, CRO |
| [Checkout & Forms](references/checkout-and-forms.md)                       |          9 | checkout, lead forms, cart abandon, field friction   |
| [Onboarding & Activation](references/onboarding-and-activation.md)         |         23 | empty states, aha moment, TTV, activation, trials    |
| [Revenue-Centric Design](references/revenue-centric-design.md)             |         13 | the RCD principles, design process & method          |
| [Pricing & Monetization](references/pricing-and-monetization.md)           |         19 | decoy/anchoring, GBB, trial-with-card, upgrades      |
| [Churn & Retention](references/churn-and-retention.md)                     |         14 | cancellation UX, expectation debt, NRR, JTBD         |
| [Dashboards & Data Visualization](references/dashboards-and-data-viz.md)   |          3 | KPIs, actionable panels, F-pattern, role context     |
| [Behavioral Science Toolkit](references/behavioral-science-toolkit.md)     |          7 | the cross-cutting biases & persuasion levers         |
| [Product Strategy & Features](references/product-strategy-and-features.md) |         13 | Swiss Knife Index, feature adoption, attention       |
| [Positioning, ICP & GTM](references/positioning-icp-and-gtm.md)            |          9 | ICP, niche, TAM/SAM/SOM, PLG, first customers        |
| [AI-Era Differentiation](references/ai-era-differentiation.md)             |          9 | moats, commoditization, vibe-coding pitfalls         |
| [Metrics & Experimentation](references/metrics-and-experimentation.md)     |         11 | A/B rigor, vanity metrics, churn→LTV math            |

The agent entry point is [`SKILL.md`](SKILL.md); informational diagrams referenced by the principles live in [`assets/`](assets/).

## The spine: RCD in 9 principles

1. **Neutrality is omission** — an interface that doesn't direct hurts conversion.
2. **Who talks to everyone convinces no one** — no ICP → generic value → worse retention.
3. **Value first, ask later** — proof must arrive before the user questions their choice.
4. **Your promise is the size of your proof** — the market believes what you demonstrate, not what you claim.
5. **Same competes on price, different on category** — no contrast, no margin.
6. **Default is the decision you made for the user** — the initial state defines mass behavior.
7. **Retention is built, not requested** — perceived loss retains more than promised benefit.
8. **Expansion is born of usage** — upgrade at the moment of the limit, never by interruption.
9. **Price is a filter** — pricing defines who enters, who stays, and who expands.

## Updating

This is a point-in-time snapshot. The **Coverage** date above marks the latest included post (**20 Nov 2026**); anything newer from [@richardrx](https://x.com/richardrx) isn't here yet. To extend it: gather the newer posts, distill each into the same principle shape, file it under the right `references/` theme, then bump the dates in this README and in [CHANGELOG.md](CHANGELOG.md).

## Provenance & attribution

All ideas, frameworks, examples, and the coined term _Revenue-Centric Design_ belong to **Richard ([@richardrx](https://x.com/richardrx))**. This repository is a curated, distilled, English-translated index of 166 of his public X posts, created **with his permission** for educational reference. Every principle links back to its original post, and it reproduces distilled principles rather than his full posts verbatim.

## License

Source-available under custom terms — **attribution required, no gambling/betting/casino use**. See [LICENSE](LICENSE). The underlying ideas remain the author's.
