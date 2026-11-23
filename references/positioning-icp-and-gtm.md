# Positioning, ICP & Go-to-Market

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Get into the AI answer: name your category, publish price and comparisons
**Principle.** Buyers now ask ChatGPT which tool to use, mostly with category questions that name no brand. To make the list that comes back, the model has to understand your category, who you serve and what you cost — and it takes that from your site and from what other sites say about you. Several of those signals are simple to influence.
**Apply when.** B2B buyers research vendors with AI assistants, and you don't appear when you ask your own category question.
**The move.**
- First fold of the home: the category as customers type it, who it's for, and the result — "the platform that transforms how you work" can't be matched to "best recurring-billing software for gyms."
- Public pricing in text: AIs can't cite a price they haven't read, and many prompts include a budget ("up to R$500/month").
- An "alternatives to [competitor]" and a "[you] vs [competitor]" page for each tool customers already use — otherwise the competitor's comparison is the one that gets cited.
- robots.txt: blocking "AI bots" wholesale also blocks OAI-SearchBot (ChatGPT search) and PerplexityBot; you can block GPTBot (training) and keep search crawlers.
- Page text present in HTML without JavaScript — AI crawlers generally don't run JS; `curl` the URL and look for your category phrase.
- Bing Webmaster Tools (ChatGPT search uses Bing as one source); SoftwareApplication schema with category and price, plus an FAQ of sales-call questions in customers' words.
- Off-site: complete G2/Capterra profiles with recent reviews, ask to be included in existing "best X for Y" articles, answer honestly in specialist forums.
- Measure monthly: run 10 category and alternative questions in ChatGPT, Perplexity and Gemini, note who appears and which sources are cited; filter analytics by `utm_source=chatgpt.com`.
**Evidence.** Wynter asked 200 B2B buyers (November 2026) for the first prompt they wrote the last time they researched a vendor with AI: 62% opened with a category question naming no vendor ("What are the best X for Y?"); another 17% asked for alternatives to, or tools like, a named vendor.
**Source.** [@richardrx · 2026-11-18](https://x.com/richardrx/status/2123036224810070357)

## Size the market with TAM → SAM → SOM (and know which one matters)
**Principle.** Your real market is far smaller than the population — TAM is a theoretical ceiling (Brazil's 213M becomes ~101M credit-card holders for a paid app). Investors often ignore a TAM under ~R$1B, but the number that matters is the **SOM** — what you can actually capture.
**Apply when.** Sizing a market, writing a deck, or judging whether a niche is big enough.
**The move.** TAM = total addressable ceiling; **SAM** = the realistic slice your model reaches (~40% in his example); **SOM** = the 1–5% you truly win in ~36 months — and SOM isn't a guessed %, it comes from real CAC, activation, support capacity and LTV. You can't change your TAM; you change how much of your SAM you convert and retain.
**Evidence.** RepareCar: ~76k mechanic shops (honest TAM) → SAM ~47k → ~3% ≈ 1,414 shops ≈ R$1.6M ARR; current pace (~10 shops/day) ≈ 7% of SAM in 12 months.
**Visual.** TAM/SAM/SOM concentric-circle diagram with definitions — `../assets/2070140923380420796__1.jpg`
**Source.** [@richardrx · 2026-06-25](https://x.com/richardrx/status/2070140923380420796)

## Frame the referral prize as a gift to the friend, not a commission to the referrer
**Principle.** Member-get-member (MGM) referral programs win on framing and timing, not just on a two-sided reward. Money makes the exchange feel transactional; an in-product benefit feels like a genuine gift.
**Apply when.** Designing or fixing a referral program and defaulting to "refer a friend, get $20."
**The move.** Apply the framing effect: surface the prize on the receiver's side ("João gave you 500MB"). Ask for the referral at the peak of value (right after a concrete win, or when the user hits a limit). Avoid cash; give a reward that deepens use of your own product. Embed it as continuous in-product operation, not a one-off campaign. Caveat: referral amplifies a product people already love; it can't fix one nobody recommends for free.
**Evidence.** Dropbox grew 3900% in 15 months (100k → 4M users), peaking near 3M invites in a single month; ~1/3 of users already arrived via word-of-mouth before the program.
**Voice.** "A referral amplifies a product people already love — it doesn't fix a product nobody recommends for free."
**Source.** [@richardrx · 2026-06-02](https://x.com/richardrx/status/2061766945582559509)

## Pick a deliberately under-served niche as your ICP
**Principle.** A clear ICP (ideal customer profile) is not "everyone who could use my product." It's a deliberately chosen, under-served niche — and a sharp niche beats no niche, because you can't out-fight the entrenched generalist giant.
**Apply when.** Early traction; tempted to "embrace the world" out of fear of a small TAM.
**The move.** Validate four ICP filters: (1) feels the pain with real weight — pain is proportional to what's lost when unsolved (a lost lead costs a face-aesthetics clinic R$3,000 vs. R$60 for a barber); (2) big enough TAM to sustain operations; (3) money to pay your required ticket so unit economics close; (4) founder-fit, giving native language, a fast validation network, and instinct that money can't buy. With a clear ICP, failure has a diagnosis ("I got the messaging wrong"); without one, you can't tell if product, copy, channel, price, or audience failed — and every test burns runway.
**Voice.** "A generalist ERP is hard to sell; an ERP for cabinetmaking is a different conversation."
**Source.** [@richardrx · 2026-05-19](https://x.com/richardrx/status/2056789797646029232)

## Don't claim PLG without the four structural conditions
**Principle.** Product-led growth (PLG) is a consequence of structural conditions, not a product decision you declare. Most B2B SaaS that pitches PLG is really sales-led wearing a PLG label.
**Apply when.** Writing a pitch deck or strategy and calling the motion "self-service" / PLG.
**The move.** Require all four conditions: (1) TTV < 10 minutes — if it needs a consultant demo, API support, or paid implementation, it's not PLG (tell: full trial, zero activation); (2) ticket below ~R$1,000 — higher means a buying committee; (3) native virality or collaboration (Notion, Figma, Slack pull users in; a CRM/AI tool needs SDRs, demos, follow-up); (4) a huge addressable market with a real bottom-up TAM. If you fail these, run sales-led honestly.
**Evidence.** Brazil has ~20,000 companies with 100+ employees, and only ~a dozen B2B SaaS where PLG makes real economic sense.
**Voice.** "Founders love PLG because it seems to delete the part they don't master — selling."
**Source.** [@richardrx · 2026-05-04](https://x.com/richardrx/status/2051262752547536941)

## Charge your first ten users from day one
**Principle.** The first ten users define the product's entire curve, and payment is the cheapest test of real pain — curiosity is free, an open wallet demands a concrete problem.
**Apply when.** Validating a new product and tempted to give early access away to "build a base."
**The move.** Source the first ten from closed communities, personal reach, or pure guerrilla. Charge even while in prototype. When someone says they can't pay, ask directly: "What does the system need to do for you to pay right now?" Treat the payment friction as part of the test. Collect dense feedback; only start visual design after ~20 paying users. For B2C apps the method shifts (e.g., pre-sale of a solution-in-progress) but the principle holds.
**Evidence.** RepareCar's first 25 auto shops tested the product in prototype; the team visited each and charged at the end, designing visuals only after 20 paying shops.
**Voice.** "Curiosity is free; an open wallet demands a concrete problem."
**Source.** [@richardrx · 2026-04-26](https://x.com/richardrx/status/2048359526487716333)

## Reverse-engineer the funnel math before celebrating an MRR target
**Principle.** Building the product is the easy part; distribution is the game. A revenue target is really a traffic-and-retention problem, and churn quietly resets the whole funnel every month.
**Apply when.** Someone asks "is it hard to hit X MRR?" or you're sizing acquisition for a target customer count.
**The move.** Work backwards: to net 2,500 customers at 5% LP conversion you need 50,000 visitors; from ads at 3% creative CTR, ~1.6M impressions (5% and 3% are top-decile — most land at 1–2% LP and under 1% CTR, so you test dozens). Then add the leaky bucket: at 20% monthly churn, average customer life is 5 months, so you replace 500 customers every month forever just to stand still (≈10,000 visitors / 333,000 impressions). The problem lives at the intersection of dev, design, and marketing — none alone owns it.
**Evidence.** 20% monthly churn → 5-month average lifetime; at low ticket many operate at 40–50% churn, so "the bucket never fills."
**Voice.** "Building the product is the easy part; distribution is the game."
**Source.** [@richardrx · 2026-04-20](https://x.com/richardrx/status/2046222319912132977)

## Concentrate channels with the Bullseye framework, not scattershot testing
**Principle.** Testing ten channels at once means you never know what drove results and you blame the channel when the business stalls. Distribution needs prioritized focus — and a perfect channel still fails if the receiving structure leaks.
**Apply when.** You're spreading content and traffic across many channels with no clear read on what works.
**The move.** Use the Bullseye framework (from the book *Traction*): three rings of priority. Inner ring = at most three highest-potential channels with total focus; middle ring = up to six channels you probe with small experiments; outer ring = everything plausible long-term, no active focus now. Choose between channels with an ICE Score (Impact, Confidence, Ease, each 0–10, divide by 3, prioritize). Crucial gap the book skips: scaling distribution onto a broken reception structure (LP, onboarding, first product steps) yields no growth — distribution and retention are simultaneous, not sequential.
**Visual.** Bullseye as nested circles — What's Possible → What's Probable → What's Working — beside a "Marketing Framework for Startups" triangle (Prioritization, Testing, Quick Iteration). — `../assets/2036035304868434115__1.jpg`
**Source.** [@richardrx · 2026-03-23](https://x.com/richardrx/status/2036035304868434115)

## Diagnose the bottleneck: no entries is distribution, leaving without paying is design
**Principle.** Design can't save a "ghost product." Design optimizes and raises the LTV of something that already has traffic; it can't manufacture demand.
**Apply when.** A builder ships an app, gets near-zero users, and hopes a redesign will rescue it.
**The move.** Split the diagnosis cleanly: if nobody enters your product, it's a distribution problem; if they enter, don't pay, and leave, it's design. Read *Traction* even if you can afford an agency or a marketing team — the lever isn't just cost-per-channel but each channel's awareness level, which drives different conversion and retention behavior depending on where and how the user arrived.
**Voice.** "If nobody enters your product, it's distribution. If they enter, don't pay, and leave, that's design."
**Source.** [@richardrx · 2026-02-28](https://x.com/richardrx/status/2027721170569564521)
