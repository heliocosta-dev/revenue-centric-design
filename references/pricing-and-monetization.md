# Pricing & Monetization Psychology

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Price the first purchase below the buyer's no-approval limit
**Principle.** Many B2B checkouts stall on authority, not value: above the amount a person can put on a card without asking anyone, a buyer who has already decided leaves the checkout tab open for days waiting for a boss's reply. Richard borrows ProfitWell's "Amex effect" (Patrick Campbell's name for the price a buyer pays on a card without deliberating): for consumer and user-led B2B, don't charge above that point on the first purchase — once you're in, expanding is easy.
**Apply when.** Card-based B2B checkout where the person who finds the tool isn't the one who owns the card, or checkout sessions expire and get paid days later.
**The move.** The limit tracks income in B2C and job role in B2B: the same R$549 is an impulse buy for the founder who holds the card and an approval request for the analyst who found you (at an automaker, Richard could buy tools up to US$99/month if compliance had pre-approved them). (1) In Stripe, count expired vs completed Checkout sessions over 90 days and flag expired ones later paid by the same account — sessions expire within 24 hours and fire `checkout.session.expired`, so a buyer who waited three days returns to an error page. (2) Turn on Checkout recovery (off by default): a link valid for 30 days that reopens the same purchase. (3) Ask in onboarding whether they needed approval, their role, and how much they can approve alone. (4) Test an entry plan below that limit, with expansion coming from usage. (5) Track expiry rate and time from first session to payment for 6–8 weeks; if both fall without average revenue per account collapsing, it worked. In demo/PO/legal sales, measure time stuck in the CRM's approval stage instead.
**Voice.** "You may be selling to the right person in the wrong role."
**Source.** [@richardrx · 2026-11-20](https://x.com/richardrx/status/2123760621233537146)

## Price the annual discount from your churn — and don't read annual as retention
**Principle.** An annual plan is a cash and churn-math lever, not proof that the product retains. "Two months free" only looks like lost money if you assume a monthly customer pays all 12 months; above a modest monthly churn, the discounted annual already earns more in year one. But annual billing doesn't make anyone like the product — it moves the moment you find out.
**Apply when.** Deciding whether to offer or discount annual billing, or the team celebrates annual sales while 30% of the base hasn't logged in for 60 days.
**The move.** Do the break-even: R$200/month vs 12-for-the-price-of-10 annual (R$2,000 upfront). At 5% monthly churn a monthly customer pays ~9 installments (~R$1,840) in year one; break-even sits at ~3.4% monthly churn — above it the discounted annual wins, and the upfront cash can fund more aggressive acquisition (raising LTV, "albeit artificially," in Richard's words). Below ~3.4%, the discount costs money; offer a different benefit. Then judge the product by engagement, not billing: with monthly you find out in month 2, when there's still time to fix it; with annual you find out at renewal, when the customer has already decided, stopped opening it, and stopped answering — or you eat a chargeback. Pushing annual is strategic in low-ticket B2C, where retention is hard; in B2B the game is different.
**Evidence.** SaaS Capital's 2020 retention benchmarks (1,400+ companies, 2019 data): companies billing annually upfront had 90% gross retention vs 91% for monthly billing.
**Voice.** "Like the guy who paid the gym's annual plan on January 1st and never went back."
**Source.** [@richardrx · 2026-11-13](https://x.com/richardrx/status/2121265412402827501) and [@richardrx · 2026-09-09](https://x.com/richardrx/status/2097664585373299156)

## Show the price unless every deal needs its own proposal
**Principle.** Three plans behind the same "talk to sales" button leave buyers to compare without the only information that helps them compare. Hiding the price makes sense when the ticket is six figures and each account needs a custom proposal; at R$400–1,500/month — often paid on the card of someone who pays for Notion without asking anyone — it filters out the buyers you want and books the ones you don't.
**Apply when.** Your pricing page shows Starter/Pro/Enterprise with green checkmarks and no prices, while conversion is low and demos fill with off-profile leads.
**The move.** Buyers with budget and urgency see a silent page, imagine a high number, and leave for the competitor that shows its price, without telling anyone. Who stays and books the call is whoever has time to find out — an agency benchmarking for a client, a curious pre-revenue founder — so your SDR spends the week on calls that were never going to close, CAC rises, and the blame game starts. Check your CRM: of the last 30 demos, separate those who left the call knowing the price and vanished before the proposal; if that's more than half, the page could be doing for free the triage your SDR now does on calls.
**Evidence.** Wynter (Peep Laja) asked 50 B2B SaaS leaders in April how they set prices: 62% hide the whole price behind "talk to sales", and 58% have never tested their pricing page.
**Voice.** "Three plans to compare, without the only information that serves to compare them."
**Source.** [@richardrx · 2026-11-04](https://x.com/richardrx/status/2118090470899564756)

## Make the paywall a window, not a wall — and check that users reach it
**Principle.** The right discomfort converts: a paywall that shows what's locked on the other side makes the value the user already felt look small next to the whole product, and that gap is the reason to pay. A blind wall that blocks without showing what exists teaches the user the product ends there. And no paywall converts users who never reach it, or who hit it before they've felt any value.
**Apply when.** Designing an upgrade screen or paywall, or a founder says the problem is price while trial-to-paid stays low.
**The move.** Show the locked outputs with a note on what each unlocks, and expose the cost (e.g., per generation) before any click. Match aggressiveness to the value already felt: before first value, an aggressive wall only brings churn forward; after it, a timid wall only lowers trial-to-paid. Give the screen its own KPI — upgrade conversion from the paywall. Before touching price, check what share of users even sees the paywall, count the screens between opening the app and first value and cut to the minimum, then place the gate right after the moment the user feels they built something (endowment effect: people demand about twice as much to give up what feels theirs as they'd pay to get it). Fix account-flow bugs before changing a comma of the price. Read with "Frame the upgrade as a loss at the moment of value" (2026-04-21), whose PDF-export gate fires once the report already exists; here export *was* the first value, so gating it meant the user never had anything to lose.
**Evidence.** In one client's app only half of those who opened it ever saw the paywall (Richard puts the market average above 85%), export sat behind payment, and the 7-day trial converted 29%; 19% of paying users lost their subscription when creating a second account, thought they were being scammed, and were handled one by one on the founder's personal WhatsApp — involuntary churn that looks like support (Kahneman, Knetsch & Thaler: people accept paying a lot but don't forgive what feels unfair). The window-style paywall was designed for an AI rendering client and was not yet live when posted.
**Visual.** The window-style paywall for an AI rendering product: three locked renders with handwritten arrows to what each unlocks, an upgrade button, and the per-generation cost visible behind the modal — `../assets/2102077564839690371__1.jpg`
**Voice.** "The aggressiveness of the paywall follows the value the user has already felt."
**Source.** [@richardrx · 2026-11-03](https://x.com/richardrx/status/2117720250070241638) and [@richardrx · 2026-09-21](https://x.com/richardrx/status/2102077564839690371)

## Use a disfluent font for genuine deals — and name tiers for the mix you want
**Principle.** A uniformly polished pricing page can be easy to scan yet weak at selling. For a genuinely favorable promotion, a disfluent (ugly) font on the price can make people process the number more deeply. Tier labels can change purchase incidence and which tier buyers choose — and those effects can run in opposite directions.
**Apply when.** Pricing looks clean but plan distribution has been flat for months, or every company's pricing cards feel interchangeable.
**The move.** Keep the rest of the page legible, but test a deliberately ugly or disfluent font on a genuine promotional price — never make the whole UI ugly. Choose labels by the outcome: in Wang et al.'s experiments, a superior-sounding metal ladder (Silver/Gold/Platinum) reduced choice deferral but moved the mix down, while an inferior-sounding ladder (Bronze/Silver/Gold) moved it toward higher-priced tiers. Richard applies that result to functional names such as Basic/Standard/Essential; treat that mapping as a hypothesis and measure purchase incidence and initial tier selection separately. Read with "Build a single value axis, then tune the decoy's distance to your target plan" (2026-02-02): that post recommends aspirational Starbucks-style tier names to lift the brand, this one prices that choice — aspirational names sell more units, unglamorous ones sell more high tier, so pick by the metric you are optimizing.
**Evidence.** Motyka et al. (2016) found that disfluent fonts on price promotions prompt deeper processing and increase purchase behavior when the offer is a deal, even though people like the display less. Across five experiments (1,954 participants), Wang et al. (2024) found superior-sounding labels increased purchase incidence but shifted choices toward cheaper options; inferior-sounding labels increased higher-priced choices.
**Visual.** Three pricing screenshots from the quoted post by @pankajstwt — 3-column Basic/Starter/Pro with near-identical includes; 2-column Launch/Scale; one-time Starter/Premium/Pro plus Ultimate — clean generic templates Richard challenges the reader to tell apart: `../assets/2092692547244007852__q__1.jpg`, `../assets/2092692547244007852__q__2.jpg`, `../assets/2092692547244007852__q__3.jpg`
**Source.** [@richardrx · 2026-08-26](https://x.com/richardrx/status/2092692547244007852)

## Price from cost+margin floor and value ceiling — never tarot or competitor-minus-20%
**Principle.** Two calculations give your floor and ceiling. Floor = cost to serve + target margin (infra, support, tools, tokens; if R$10/account and 80% margin, floor is R$50). But two traps: price too low signals low quality before use, and CAC math can eat the margin (CAC R$100 + margin R$40/mo = 2.5-month payback; churn at month 3 = you worked 3 months for R$20). Ceiling = reference value — what the client pays today to solve it their way (Excel + 1.5h/day of admin; or the loss they absorb by not solving).
**Apply when.** Setting or revisiting SaaS pricing.
**The move.** Quantify the delta in money for them: an ICP auto repair shop loses ~12 quotes/month to no follow-up × R$800 ticket × 30% margin × recovering 1/3 → R$3,200/mo revenue, R$960/mo profit. Then the sliding scale: value easy to prove, buyer convinced, little competition → move the price up; value hard to prove, skeptical buyer, a competitor on every corner → settle for ~10% of the value generated and be grateful. Commodity features (work orders, scheduling, reports) don't sustain price — they just put you in the same comparison table.
**Source.** [@richardrx · 2026-08-03](https://x.com/richardrx/status/2084250609687884144)

## The freemium trap, in numbers: higher conversion, far lower cash
**Principle.** A free plan lifts signup conversion but can crush the economics — the higher top-of-funnel number hides a worse business.
**Apply when.** You're tempted by freemium's better conversion rate.
**The move.** Run the funnel (same R$80k/mo traffic, plans from R$199). **With freemium:** ~8% → 800 signups → 80% activate → 5% pay = 32 payers (R$6,368 MRR), saturating ~160 payers under 20% churn, while 768 free users burn AI tokens (~$0.08 each) — real CAC ≈ R$2,540/payer, payback ~13 months. **Without:** ~3% → 300 payers = R$59,700 MRR (~10×), CAC ~R$275, payback ~6 weeks, LTV:CAC 5:1 that reinvests its own profit. Freemium only pays off if free brings *organic/viral* users you didn't pay for.
**Voice.** "One scenario reinvests its own profit; the other funds losses until the money runs out."
**Source.** [@richardrx · 2026-07-01](https://x.com/richardrx/status/2072312844784152628)

## Whether freemium works is decided by the cost to serve a free user
**Principle.** Freemium isn't good or bad in the abstract — the *cost of free* decides, and it hinges on (1) how much it costs to serve non-payers and (2) how long/expensive activation is.
**Apply when.** Considering a free plan, especially as a bootstrapped (non-bigtech) founder.
**The move.** If serving a free user costs almost nothing and TTV is short, free becomes an acquisition channel (Slack — first message in minutes; it's the short TTV, not the cash, that sustains it). If the product runs on AI (dollar-priced tokens) or activation is long, a free account is an expensive bet that a small fraction funds — which needs deep pockets (the exception, not the average founder). On a friendly average, only ~3–4% of freemium converts. Otherwise: charge — well, and early.
**Voice.** "For an AI product, your free user was never free."
**Source.** [@richardrx · 2026-06-30](https://x.com/richardrx/status/2071962778072469560)

## Price is the cheapest money — stop anchoring it to the cheapest competitor
**Principle.** Pricing is a SaaS's biggest lever, yet ~90% of products are underpriced — the founder, who knows every limitation, anchors on the cheapest competitor instead of on value delivered. The buyer only sees the problem solved.
**Apply when.** Setting or revisiting price; fearing a "no."
**The move.** Raise toward value. A 30% price increase doesn't yield 30% MRR (some churn), but what remains is nearly pure cash — no acquisition in between — while growing a channel 30% costs money, time, and has a ceiling. Low price costs you later: less budget to reach your ICP, a CAC-obsession trap (the real metric is the CAC↔LTV *gap*, which price widens on both sides), and higher churn (cheap attracts uncommitted buyers). Design link: the number must be sustained by perceived value — your page and first use justify or destroy it.
**Voice.** "Charging more without seeming to be worth more is just raising the price of rejection."
**Source.** [@richardrx · 2026-06-29](https://x.com/richardrx/status/2071634185228329219)

## 1% on price beats 1% on acquisition — you raise prices too little and too late
**Principle.** A 1% price improvement drives ~8–11% more profit (ProfitWell) on typical SaaS margins, while a 1% acquisition improvement yields ~2%. Yet 70% of executives rank acquisition as the most important growth lever — the one that pays least. Price is left untouched because of loss aversion (fear of losing what you have screams louder than the chance to gain).
**Apply when.** It's been >12 months since a price change and the product improved meanwhile.
**The move.** Test the new price only on new customers, don't touch the base. If the conversion drop is offset by the higher ticket, it wins. Users who pay more churn less. Raise gradually, anchored in value — communicate what improved, never a naked increase. Forget A/B testing price (you lack volume); segment and run willingness-to-pay research instead.
**Voice.** "If 1% on price pays five times more than 1% on acquisition, why is nearly all your energy at the top of the funnel?"
**Source.** [@richardrx · 2026-06-03](https://x.com/richardrx/status/2062127283977019757)

## Competing on price is adverse selection — you filter in the worst client
**Principle.** Price-led copycats attract bargain hunters: they enter because you're cheapest and leave the second someone is R$1 cheaper. High churn, zero loyalty, most support tickets. Price as bait is a filter for the client you least want. Better: Kawasaki's "Be a baker, not an eater" — bake your own pie via niche (CRM for facial-aesthetics clinics, not another CRM) and charge 5x with no comparison. Use the giant's weight against it (jiu-jitsu): big players' blind spots are in public complaints — ReclameAqui, app stores, Google Places, communities, FB/WhatsApp groups, niche sites. Each complainer represents ~26 equally unhappy silent ones.
**Apply when.** Tempted to differentiate purely on being cheaper than a big player.
**The move.** Mine complaints for the niche, angle, vocabulary, pain, and promise for your LP. Accept you'll be copied — storefronts look equal but the model underneath (your niche, angle, economics) isn't. McDonald's is a real-estate company dressed as a burger joint; BK is royalties. Same storefront, different machine.
**Source.** [@richardrx · 2026-06-03](https://x.com/richardrx/status/2062314549483589691)

## Make the middle plan the one you actually want to sell
**Principle.** Each plan has a behavioral job, not just a price; the plan you most want to sell should sit in the middle, flanked by a decoy below and an anchor above.
**Apply when.** Building or auditing a SaaS pricing page, especially if you copied competitors without assigning each tier a role.
**The move.** Use the decoy effect: place your target (e.g. Pro) in the middle; make the tier below it clearly inferior on one important attribute (user cap, no critical integration, no priority support) so Pro looks obvious. Keep exactly three plans — four+ triggers the paradox of choice and users stall. Add a top tier (Enterprise) purely to anchor price perception. Ask: "What is my decoy today?" If you can't name one, it likely doesn't exist.
**Evidence.** Ariely's MIT test of The Economist's tiers: with the print-only decoy, 16%/84% chose online/combo; removing it flipped choices to 68%/32%, cutting combo revenue by more than half. Estimated +30–43% subscription revenue.
**Visual.** Economist subscription page; the decoy's removal shifts combo-plan share from 84% down to 32% — `../assets/2059951433827426437__1.jpg`
**Voice.** "Option B was never built to be sold — it was built to make C look obvious. It's the bait."
**Source.** [@richardrx · 2026-05-28](https://x.com/richardrx/status/2059951433827426437)

## Ask for the card in trial — but optimize for the right ICP, not raw conversion
**Principle.** Requiring a credit card multiplies trial-to-paid conversion but shrinks signups; the goal is the model that attracts and retains the right ICP, not the one with the highest headline conversion.
**Apply when.** Choosing trial-with-card vs trial-without-card (or freemium), or designing recurring billing for a Brazilian market.
**The move.** Weigh the funnel both ways. Trial-with-card converts harder but starves you of volume; trial-without-card floods the funnel with low-intent users. Run the full math, not just the conversion rate. In Brazil, also account for PIX recorrente, whose dynamics differ from monthly card billing.
**Evidence.** ChartMogul 2026 (US, 200 products): trial-with-card converts ~31.4% vs 8.9% without — 3x+. Worked funnel: 1,000 visitors → 30 trials → 9.4 paying (with card) vs 85 trials → 7.5 paying (without). Author observes PIX-recorrente cohorts churn more than card cohorts.
**Voice.** "Don't ask which model converts more — ask which model attracts and retains the right ICP."
**Source.** [@richardrx · 2026-05-15](https://x.com/richardrx/status/2055247161349054950)

## Frame the upgrade as a loss at the moment of value, not a feature you're selling
**Principle.** Low upgrade rates are usually a framing-and-timing problem, not a price problem; remind users what they've already invested and what they stand to lose.
**Apply when.** A happy, active free user never upgrades, or your upgrade rate sits below 5%.
**The move.** Three framings beat generic limit/discount/feature-gate prompts. (1) Sunk cost: surface the assets they've built — "You created 47 custom reports. On the free plan you lose access to 40." (2) Loss aversion: framing loss outconverts framing gain — "You'll lose access to 8 months of history" beats "Get unlimited history." (3) Limited-access gate timed to an imminent, known result — "Your report is ready. To export as PDF, activate Pro." The timing/context of the gate matters more than the gate itself.
**Voice.** "If your upgrade rate is below 5%, the problem probably isn't price — it's how and when you're asking."
**Source.** [@richardrx · 2026-04-21](https://x.com/richardrx/status/2046544442216054981)

## Engineer the comparison frame with a decoy and a high anchor — and drop Free from the top
**Principle.** Conversion shifts when you change the frame of comparison, not the product; equal-looking options cause delay, and showing Free first anchors everyone to zero so everything else feels expensive.
**Apply when.** You run the default Free / Pro / Enterprise (sob consulta) ladder and Pro isn't converting.
**The move.** Insert a decoy: a Starter just below Pro with irritating limitations (e.g. R$79 vs Pro R$99) so users compare Starter↔Pro and Pro wins for R$20 more. Remove Free from the visible top so the first number isn't zero — anchoring means the first price seen sets the reference; lead with a higher/previous/Enterprise price so Pro at R$99 reads as cheap.
**Evidence.** The Economist sold 3x more print+digital after adding a same-price print-only decoy nobody bought. Author cites documented tests lifting conversion 10–20% via reframing alone.
**Voice.** "You're competing against your own free plan. And losing."
**Source.** [@richardrx · 2026-04-14](https://x.com/richardrx/status/2044014136770580743)

## Tie the trial's end to value consumed, not the calendar
**Principle.** Blocking access on a fixed day count (7/14/28) is a lazy rule; the billing trigger should fire on value consumption, after the user's first real win.
**Apply when.** You copied a competitor's 14-day trial and paid conversion is failing, or you're setting trial length from scratch.
**The move.** Never paywall before a clear micro-win or solving the core problem — doing so kills conversion and breeds bad word of mouth. Set length using four variables: (1) Product complexity — enterprise needs time for compliance/security review, not just the user. (2) Time to Value — Spotify delivers in seconds, a CRM needs days of data. (3) Usage frequency — rarely-used products may need long trials, or none at all (a once-a-year tax tool shouldn't have a trial). (4) Card entry — no card means a shorter trial to create urgency; with card, watch silent next-month churn. Note: sunk cost only bites if the user built a real asset — a bad onboarding produces frustration, not switching cost.
**Voice.** "Locking access purely on the calendar is a lazy rule that can cost you dearly — you're burning CAC without knowing where value lands."
**Source.** [@richardrx · 2026-03-16](https://x.com/richardrx/status/2033502548301091057)

## Order pricing rows by the serial-position effect: killer feature first, differentiator last
**Principle.** Users don't read pricing lists linearly; attention and memory cluster on the first and last items, so feature order is itself a conversion lever.
**Apply when.** Laying out the feature rows inside a pricing card or comparison table.
**The move.** Exploit the serial-position effect (primacy + recency). Top: value anchor — never "24/7 support"; lead with the core/killer feature that solves the ICP's main pain and justifies ~80% of the ticket and the ROI. Middle: utilitarian features (exports, integrations, storage limits) the user won't memorize but will scan to compare against the next plan. Bottom (nearest the CTA): the differentiator, bonus, or loss-aversion hook — a lifetime guarantee or dedicated support. The middle of the list is "a cognitive black hole."
**Visual.** Pricing card emphasizing the bold first row (core feature) and bold last row (super bonus), with greyed utilitarian middle rows — `../assets/2029623167900061970__1.jpg`
**Voice.** "Pricing success depends not just on what you deliver, but on the order the brain is led to process the value."
**Source.** [@richardrx · 2026-03-05](https://x.com/richardrx/status/2029623167900061970)

## Engineer the pricing page with Good-Better-Best and control the comparison
**Principle.** Lost LTV is rarely about price — it's analysis paralysis from a missing choice architecture. The brain is lazy and judges by relative comparison (priming + anchoring), so if you don't design the anchor, users compare you to "nothing" or to the cheapest competitor.
**Apply when.** Designing or fixing a pricing page; conversions die at the final step despite strong CAC spend.
**The move.** Use a Good-Better-Best (GBB) structure: **Good** = a stripped entry plan that anchors a low price but is limited enough to make users feel pain and look up (never make it free — then everything above looks expensive). **Better** = your standard plan, the target for ~80% of buyers; price it closer to Good than to Best so users think "paying only ~20% more I get double?" **Best** = the value anchor that exists mainly to make Better look cheap (bicycle analogy: without the carbon-fiber Best, the carbon-wheel Better looks expensive). Golden rule: keep comparisons on one axis — don't pit "10,000 tokens" against "Priority Support"; prefer linear, ideally asymmetric, growth. Cap at 2–5 plans (6 = anxiety, paradox of choice). Then control which attributes you compare — your own "Brazil vs Paraguay" table — choosing indicators that favor your value thesis. Highlight Better with color/size/badges. "Stop making the user do the math — do the math for them."
**Evidence.** Cites Briesch et al. (1997) and Mazumdar et al. (2005) on reference-price models, and Chernev (2015) on choice overload.
**Visual.** Two mirrored BR-vs-PY indicator tables prove framing: swapping which metrics are shown flips which country "wins" — `../assets/2018693884449009956__2.jpg`, `../assets/2018693884449009956__3.jpg`. Four-tier mockup highlights a "Most Popular" target beside a high anchor (Hick's law / few options) — `../assets/2018693884449009956__4.jpg`
**Voice.** "Your pricing page is killing your LTV — and I can prove it."
**Source.** [@richardrx · 2026-02-03](https://x.com/richardrx/status/2018693884449009956)

## Build a single value axis, then tune the decoy's distance to your target plan
**Principle.** A plan ladder must read as one clear progression of value; mixing quantitative and qualitative axes muddles it, and where you place the decoy's price decides which plan looks like the deal.
**Apply when.** Naming and pricing tiers, or the "value staircase" between your plans isn't obvious to users.
**The move.** Pick one progression — quantitative (rising credits/users) or qualitative (24/7 human support, special features) — rather than blending both. Borrow Starbucks-style naming (Tall/Grande/Venti) so every tier sounds good and lifts the brand. Then position the decoy: place it near the most expensive plan and the expensive plan looks cheap; place it near the cheapest and the decoy itself becomes the most attractive option. Read with "Use a disfluent font for genuine deals — and name tiers for the mix you want" (2026-08-26): aspirational names lift purchase incidence, but unglamorous ones shift the mix toward higher-priced tiers.
**Visual.** Decorative 3D price-tag illustration — no data.
**Source.** [@richardrx · 2026-02-02](https://x.com/richardrx/status/2018357024543715480)
