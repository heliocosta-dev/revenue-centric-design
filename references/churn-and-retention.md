# Churn & Retention

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Don't cut the price on "too expensive" until you cross it with usage
**Principle.** "Too expensive" is rarely the real reason for cancelling: the customer already saw the price and bought, so something else changed. The reason chart can also be a default effect — Stripe's customer portal offers a list of reasons with "It's too expensive" first, ahead of "I need more features" and "I found an alternative", and someone rushing to finish cancelling clicks the first plausible option.
**Apply when.** The top cancellation reason in Stripe is price and someone proposes lowering it for everyone.
**The move.** Run the math first: 300 customers at R$500, 20 cancel citing price; dropping to R$400 saves R$8,000 MRR if all 20 stay, but the other 280 now pay R$100 less — R$28,000/month — so the discount must keep at least 70 would-be cancellers to break even. Then: (1) export 90 days of "too expensive" cancellations (Stripe Sigma or the canceled-subscriptions list); (2) cross them with usage in the 30 days before cancelling — logins and the product's core event — separating weekly users from those who barely came in; (3) send each a plain-text email from your own address with one question: "What made you cancel?"; (4) consider price only if most of the "expensive" group used the product heavily and their answers mention budget or a cheaper alternative — if they barely used it, it's ICP, onboarding, or activation. (5) Your base stalls at new customers per month ÷ monthly churn (30 new at 4% → 750); a discount only moves that if churn falls. "Expensive" tends to be true after a price increase at renewal or when the customer shrank and cut tools — both concentrate among renewals in the last 60 days. Pairs with "Design the cancel screen" (2026-05-13), which also prefers an open question to a dropdown.
**Voice.** "It becomes the default effect, often not the real cause."
**Source.** [@richardrx · 2026-11-19](https://x.com/richardrx/status/2123382731044221079)

## The funnel leaks at three points — diagnose which before fixing
**Principle.** The three most common SaaS funnel holes for Brazilian founders: (1) cancel in month 1–2 → onboarding missing or LP promised the wrong thing (brought off-ICP users); the first is a product problem (shorten path to value), the second marketing (tighten the promise). (2) Many trials, few paid → paywall at the wrong moment or a broken value ladder. (3) Many visits, few signups → confused ICP and/or generic value proposition — but check the acquisition source first; wrong traffic can't be saved by copy.
**Apply when.** Triage where the funnel is leaking.
**The move.** Match symptom to owner: month-1 churn → activation/expectation; trial-no-convert → paywall timing/value ladder; visit-no-signup → ICP/positioning/traffic source. These mix — a clear ICP + good offer first, then an experience aligned to the promise.
**Evidence.** Kyle Poyar/ChartMogul+ProductLed (Jan): median free-to-paid 8%; trial-without-card good 4–6%, great 10–15%; trial-with-card good 25–35% (US).
**Source.** [@richardrx · 2026-08-05](https://x.com/richardrx/status/2085056354360729949)

## Churn and payback are one problem, measured in two places
**Principle.** Churn and payback look like two problems (often with different owners) but are the same one — both decided in the user's first session, in the gap between entering and feeling the product works.
**Apply when.** You're fixing churn at the cancel screen and chasing cheaper CAC in the ad manager at the same time.
**The move.** Both are the wrong place — the decision was made earlier. Activation fixes both: shrink TTV and you retain more AND get each customer across the payback line before they vanish. A customer who dies in month 2 with a 4-month payback never closes the account. Caveat: not all churn is activation (price, a bad channel exist) — but before chasing cheaper CAC, count how many customers die before repaying what they cost.
**Voice.** "A customer who dies before repaying his CAC is a bill you paid and never collected."
**Source.** [@richardrx · 2026-06-30](https://x.com/richardrx/status/2071931705573748896)

## Switching cost is what turns months of LTV into years
**Principle.** The same product, designed differently, yields months vs. years of LTV. Switching cost = the effort a user *perceives* in leaving; low switching cost means thin history and an easy exit.
**Apply when.** Designing for retention/lock-in, or explaining why a useful product still churns.
**The move.** Engineer switching cost deliberately — a "compound interest" that grows the product's value over time. Five levers: **muscle memory** (Superhuman/Photoshop shortcuts), **mental model** (Mac↔Windows, Gmail labels), **accumulated personalization** (Spotify playlists, home-screen layout), the **vault effect** (iCloud/Drive/years of WhatsApp), and **autopilot/habit** (variable-reward Skinner-box loops). Sunk cost holds them the way it holds an investor in a falling stock; habit can take months to install but is the difference between LTV of months and years.
**Source.** [@richardrx · 2026-06-23](https://x.com/richardrx/status/2069382946214080985)

## Tell the existing base about upgrades before they want to leave
**Principle.** Reactive improvement communication is a sneaky churn vector: if you only market new versions to cold traffic to avoid cannibalizing the old product, your base assumes the old version is the ceiling and leaves when a competitor looks better.
**Apply when.** You shipped a better version/feature but only announced it externally; support pitches the migration only at the cancel moment.
**The move.** Proactively offer upgrades and migrations to active users — not release emails nobody reads or an Instagram post. Ask: "When we shipped the last relevant feature or version, how many active customers were told?" Offering migration at cancellation converts a clean expansion into emergency retention. Track Net Revenue Retention (NRR); in B2B SaaS, NRR above 110% separates sustainable growth from a leaky funnel.
**Voice.** "The migration only showed up as a reaction to my complaint, after I started making noise."
**Source.** [@richardrx · 2026-05-19](https://x.com/richardrx/status/2056715097796411514)

## Design the cancel screen — it's your last conversation, not a form
**Principle.** The cancellation screen is the most ignored yet one of the most important pages in the product; treating it as a bureaucratic form wastes your final chance to retain.
**Apply when.** Cancel flow is just "Are you sure?" with two buttons, or Stripe's default template, while signup was crafted with care.
**The move.** Three plays: (1) Show concrete loss — "You'll lose access to relationship data on your 476 configured clients and 8 months of history"; concrete loss outweighs abstract benefit (loss aversion). (2) Offer an alternative before goodbye — "Pause 30 days instead?" or one more free month (ChatGPT nails this). (3) Collect the reason usefully via an open question — "What was missing for you to stay?" — not a dropdown that rarely lists the real reason.
**Voice.** "If you invested to bring your user here, invest the last 30 seconds trying to keep them."
**Source.** [@richardrx · 2026-05-13](https://x.com/richardrx/status/2054562119962501186)

## Churn starts on the landing page, not at cancel
**Principle.** If the LP promises one thing and the product delivers another, you create an expectation debt that charges interest every day the user thinks "this isn't what I expected" — and the disappointment is pre-programmed even if the product is excellent.
**Apply when.** 30-day churn is high but NPS is fine — the problem is likely what you promised before they entered, not the product.
**The move.** Audit three common mismatches: (1) result promise vs. tool delivery ("Increase sales 30%" → a metrics dashboard); (2) simplicity promise vs. complex product ("Set up in 5 minutes" → 47 fields, 3 integrations, 20-min tutorial); (3) promise aimed at the wrong ICP (LP speaks to a 2-person startup; product was built for a 15-person team at scale). Recalibrate the promise to match real delivery and ICP.
**Voice.** "The user bought a result and got a colorful spreadsheet."
**Source.** [@richardrx · 2026-04-29](https://x.com/richardrx/status/2049568514311172355)

## Anchor one-time-job products to a recurring life event
**Principle.** A product hired to solve a one-off problem generates structural churn: a user who loves it and still cancels isn't unhappy — they finished the job they came to do, and there was no continuous value to bring them back.
**Apply when.** You have 4.2 stars and positive NPS yet rising churn; the product solves a point problem (resume builder, contract/legal-doc generator, data migration tool, pitch-deck builder, due-diligence platform).
**The move.** Use jobs-to-be-done thinking. Instead of faking engagement, anchor the product to an event that already recurs in the user's life and returns yearly without a push. Ask: "If the job my product does is finished, what life event justifies the user coming back?" If there's no answer, it's a business-model problem, not a product problem.
**Evidence.** TurboTax (US income-tax software) tied itself to tax season, turning the product into a ritual because the event makes the use inevitable.
**Source.** [@richardrx · 2026-04-24](https://x.com/richardrx/status/2047620778338795918)

## Treat support volume as a design problem, not a staffing one
**Principle.** What looks like a support problem is usually a design problem — you cut ticket volume during onboarding itself, with an interface that answers questions before they're asked. Low-ticket digital products generate up to 3x more support than conventional tickets.
**Apply when.** Support is your biggest bottleneck, especially with low-ticket/impulse-buy products; you're tempted to just automate tickets.
**The move.** Three drivers of low-ticket support load: different buyer profile (less patience, less digital familiarity, more expectation of human help); impulse purchase (low friction → buys without understanding → seeks support); inverted opportunity cost (asking is easier than searching). For SaaS, redesign the journey: contextual in-product FAQ, self-answering UI. Automating support treats the symptom; redesigning the journey fixes the cause and can cut churn too.
**Evidence.** An old McAfee case cut support volume by 90% by implementing an FAQ — plain text, no chatbot.
**Source.** [@richardrx · 2026-04-23](https://x.com/richardrx/status/2047289409238712726)

## Strip the jargon before you blame onboarding
**Principle.** Churn that looks like a product problem is often a language problem: a technical founder writes product and sales copy in jargon, the ICP buys on a leap of faith, never perceives value, accumulates small disappointments, and cancels — looking like a missing feature on the dashboard.
**Apply when.** Churn is high and you've already revised onboarding and product — revise language and structure next.
**The move.** Watch two biases: the curse of knowledge (you know too much and forget the other person doesn't) and the easy-speech bias (simple language reads as more trustworthy and raises awareness). Rewrite dense, jargon-heavy copy into plain language even for complex topics.
**Visual.** Side-by-side: a dense, legalese contract clause (red X) vs. a plain-language rewrite "In this contract you authorize the bank…" (green check), with an "Easy-speech bias" callout. — `../assets/2041829519611371727__1.jpg`
**Voice.** "On the dashboard it looks like a missing feature; it was a mismatch between your discourse and their understanding."
**Source.** [@richardrx · 2026-04-08](https://x.com/richardrx/status/2041829519611371727)

## Retention is raising the cost of leaving day after day — iFood's behavioral lock-in
**Principle.** iFood isn't just a business model — it's Brazil's most sophisticated behavioral lock-in. Each layer (delivery, data, credit, card) raises the psychological and operational cost of leaving: sunk-cost effect plus ecosystem dependency. The restaurant doesn't stay because iFood is good; it stays because leaving got too expensive. Retention isn't a feature — it's the accumulated cost of exit.
**Apply when.** Designing long-term retention/lock-in at any scale.
**The move.** Learn from the mechanism, ethically: every layer of value (data history, integrations, financial products, workflow embedding) makes leaving more expensive. The design goal isn't just "satisfy" — it's to increase the cost of leaving over time.
**Source.** [@richardrx · 2026-03-27](https://x.com/richardrx/status/2037543117612630126)

## Churn math: restructured onboarding can preserve R$4.8k MRR from an existing base
**Principle.** 6% churn on 900 users at R$300 ARPU is 54 cancellations, or R$16.2k MRR, leaving each month. Restructured onboarding (contextual welcome + empty state + activation checklist) cut cancellations by ~30%: about 16 accounts retained, preserving R$4.8k MRR — a R$57.6k ARR run-rate or R$52.8k over the post's stated 11-month average lifetime. No new traffic, no new feature.
**Apply when.** Justifying onboarding investment to a numbers-driven founder.
**The move.** Keep the units explicit: monthly cancellations = base × monthly churn; prevented cancellations = cancellations × relative reduction; recovered MRR = prevented cancellations × ARPU; ARR run-rate = recovered MRR × 12. For cohort value instead, multiply recovered MRR by the stated average lifetime in months. Lower churn also raises valuation because every growth action operates with more margin.
**Source.** [@richardrx · 2026-03-19](https://x.com/richardrx/status/2034571753263939621)

## Engineer addiction like a game so CS isn't a churn tax
**Principle.** Customer Success is the tax you pay for a non-addictive product — if you need an army of CSMs to stop cancellations, the product failed. Your real competitor isn't another startup; it's boredom, and boredom has infinite CAC. The CNPJ buying your SaaS is the same brain that plays Candy Crush; reward neuroscience is identical. Win retention across three game-design phases.
**Apply when.** Diagnose by behavior: dropout at minutes 2–8 of onboarding = Phase 1; ~1.3 logins/week when it should be 4x = Phase 2; one departing employee kills the whole account = Phase 3. LTV:CAC below 3:1 means you're funding a product that can't stand organically.
**The move.** **Phase 1 — Time-to-value vs. cognitive load:** ditch the setup wizard (asking work before delivering value reads as hostile territory in 10 seconds); use progressive disclosure, let users create and see results before asking for email/card. Mechanism: Zeigarnik effect (incomplete-loop tension) + endowment effect (people value 3x more what they helped build). Empty states must sell the dream — never show "0 data" or blank templates; populate a demo simulating day-30 usage. **Phase 2 — Habit loop / retention as biology:** passive software that only reacts is a failure to build dependency; ship proactive variable rewards. The mesolimbic reward system releases dopamine on anticipation, not the reward itself; predictable rewards (monthly report) build tolerance, variable ones ("we detected a positive anomaly yesterday") keep the loop alive. Convert vanity metrics into loss-aversion triggers: "Your team broke a record and you haven't seen it" + temporal data scarcity ("sync in 24h or lose the weekly benchmark"). **Phase 3 — Defensive moat:** single-player products die when the champion leaves — you built dependence on a person, not the org. Build multiplayer mode + data debt via social switching cost + network effects. Make User A's work block/depend on User B; reports needing multi-stakeholder approval; dashboards aggregating 3 departments. When quitting requires an alignment meeting across Sales, Ops and Finance, you reach negative churn by bureaucratic inertia; accumulated datasets add organizational endowment effect.
**Voice.** "Stop blaming the customer. Your product is boring. And in the attention game, boring is bankruptcy."
**Source.** [@richardrx · 2026-01-30](https://x.com/richardrx/status/2017274698699067466)

## The 3 biggest churn reasons — and the fix for each
**Principle.** Most churn traces to three causes, each with a distinct fix. (1) Bad onboarding → gradual guided immersion to what users value most, a Zeigarnik progress bar (incompleteness nags), and targeted tooltips on unexplored features. (2) Missing perceived value → show user ROI in a simple dashboard (Grammarly shows words helped), promote feature discovery continuously, build community. (3) Hard/confusing interface → fix via a proper product design project.
**Apply when.** Churn is high and you don't know which of the three it is.
**The move.** Diagnose first: users who never reach value (activation) vs users who reached it and still left (perceived value) vs users who struggled (interface). Each has a different owner and a different fix — don't treat all churn as one problem.
**Source.** [@richardrx · 2025-12-17](https://x.com/richardrx/status/2001408166404530231)
