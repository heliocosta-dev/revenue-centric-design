# Metrics, Experimentation & Business Math

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Benchmark against your own model and definition, not the blended median
**Principle.** A blended benchmark sets impossible targets: medians mix sectors and kinds of conversion, so the team chases a number even the best of its own sector rarely hits — swaps a layout that worked, tests headlines without a hypothesis, and concludes "landing pages don't work for us." The same rate can be good, acceptable or bad depending on the model.
**Apply when.** Someone asks "is our conversion good?" or sets a target from an industry-wide benchmark.
**The move.** Compare only within your sector, model, and definition of conversion — in SaaS a trial signup, a demo request and a newsletter signup have completely different bars. Read free-to-paid against your model: 4% is good in freemium, acceptable in a no-card trial, bad in a card-upfront trial. Then translate the gap into CAC: R$8,000 of media and 500 no-card trial signups at 4% = 20 customers (R$400 CAC); at 10% = 50 customers (R$160) — same campaign, same page, 2.5× lower CAC, all decided between signup and first value. Note that trial's conversion edge disappears once you count how many visitors sign up at all.
**Evidence.** Unbounce's 2024 benchmark (41k landing pages, 464M unique visitors, 57M conversions; data from July 2023 to July 2024): overall median 6.6%, SaaS 3.8% — the lowest of nine sectors, so hitting 6.6% means beating the SaaS median by 74%. Kyle Poyar with ChartMogul (2026, 200 B2B products): freemium good 3–5%, great 8–12%; no-card trial good 4–6%, great 10–15%; card-upfront trial good 25–35%, great 50–60%.
**Visual.** Richard's chart of median landing-page conversion by sector from Unbounce's 41k pages: SaaS lowest at 3.8%, events & entertainment highest at 12.3%, a dashed line at the 6.6% overall median (the chart's caption dates the data Q4 2024) — `../assets/2116228538588107068__1.jpg`
**Source.** [@richardrx · 2026-11-12](https://x.com/richardrx/status/2120951006821228969) and [@richardrx · 2026-10-30](https://x.com/richardrx/status/2116228538588107068)

## Divide churn by the start-of-month base — better yet, read cohorts
**Principle.** The most common way to compute churn makes the number look better every month you grow. The more new customers a campaign brings, the lower churn looks on the dashboard, so the founder pours more into acquisition while the product leaks. It shows up late, because new customers haven't had time to cancel; when acquisition slows, the real churn appears all at once.
**Apply when.** Reporting monthly churn, especially during an acquisition push.
**The move.** Same 10 cancellations, base of 100 that added 50 in the month: ÷ 100 (start of month) = 10%; ÷ 140 (end of month) = 7.1%; ÷ 150 (everyone who passed through) = 6.7%. If you use a monthly average, use the starting base: monthly churn = cancellations in the month ÷ customers at the start of the month. Better: measure by cohort — how many of January's customers still pay in April says more about the product than any monthly average.
**Source.** [@richardrx · 2026-11-11](https://x.com/richardrx/status/2120488014887416205)

## Test what visitors can't find, not the button they never reach
**Principle.** Testing the button is the most repeated CRO tip, and it's exactly where an A/B test has the least to gain. Teams test the button because it's the part they see — they already know where the plan, the price and every screen are. Visitors don't, and many never reach the button being tested (curse of knowledge).
**Apply when.** Choosing the next A/B test, especially a CTA color or label test.
**The move.** Before the next CTA test, open the page's scroll map and see how many visitors reach the button. Favor hypotheses that help users find what they're looking for or add real urgency (no fake countdowns), and scroll/engagement tests. Build the experiment well — hypothesis written first, the right metric, enough traffic — which is worth more than the test idea itself. Read with "Don't bet your product on an underpowered A/B test" (2026-06-01).
**Evidence.** Richard cites Optimizely's 2026 report on 173k experiments from 1,200+ companies (2018–2026): over 90% measure one of five things (CTA click, pageview, checkout, signup, add to cart); win rates by hypothesis — helping users find what they seek 60%, urgency 56%, making value clearer 41% (over a quarter of everything tested); the top two make up only 14% of tests; scroll/engagement tests are 1.4% of the total yet deliver some of the largest average impacts; well-built experiments win 58% of the time vs 35% for poorly built ones.
**Source.** [@richardrx · 2026-10-30](https://x.com/richardrx/status/2116154769895039477)

## Judge a funnel test by revenue per user, not the step it touched
**Principle.** A test can lower the rate of the step it changed and still make more money. If your onboarding or paywall tests are decided by a single step's rate, you may be switching off winners without knowing — and celebrating tests that bring in less.
**Apply when.** Deciding paywall, trial or onboarding experiments on trial-to-paid or any one-step conversion.
**The move.** Decide on revenue per user, and read the step rates as diagnostics. Expect mix shifts: a more inviting step lets more undecided people in, so a smaller fraction of a much larger base can pay more. Don't kill a test in week two because one number fell.
**Evidence.** Foodnoms, a nutrition app, replaced its paywall's list of premium features with a trial timeline — the model known as the Blinkist paywall: you start today, we remind you on day 5, and how to cancel is explained right there — betting the blocker was fear of forgetting the trial and getting charged out of nowhere. Against the old paywall over the same period: started a trial or subscribed +58%, trial-to-paid −15.9%, actually paid +59.6%, revenue per user +23.3% (RevenueCat data published by the consultant who ran it, with cohorts still maturing).
**Source.** [@richardrx · 2026-10-23](https://x.com/richardrx/status/2113676403988181125)

## In B2B, measure activation per account, not per user
**Principle.** Measuring activation at the user level in a product sold to companies is the error Richard finds most often in founder dashboards: the account grows, the team inside it is dead, and the denominator hides it.
**Apply when.** A B2B PLG or self-serve product with multi-seat accounts.
**The move.** Define activation for the account (the company reaching value), not for each login. Keep the segmentation question that defines that denominator — cutting it as "friction" is the mistake: when Richard halves an onboarding, what goes are decisions and questions that lead nowhere, while a question that defines the activation denominator pays for its own friction. And never block Gmail signups: they're common in SMBs, and people often test with a personal email before signing up with a company address that needs IT or compliance validation. (Three of Richard's seven B2B PLG "nevers".)
**Voice.** "The account grows, the team is dead, and the denominator hides it."
**Source.** [@richardrx · 2026-09-22](https://x.com/richardrx/status/2102446532251238636)

## Duolingo's lesson: optimize the metric that moves DAU, not the borrowed mechanic
**Principle.** Duolingo copied game mechanics twice and failed both (a Gardenscapes moves-counter: neutral; a referral program copied from Uber: +3% because the reward excluded the best users). They stopped picking mechanics and modeled which number to move: bucketing users by engagement and simulating +2%/quarter for 3 years, CURR (current-user retention rate) had ~5x the impact of the next-best metric. Then gamification worked: CURR +21% over 4 years, daily churn of best users −40%+, DAU ×4.5. Leaderboards alone +17% total learning time and tripled highly-engaged learners — because they switched to competing with users of *similar prior-week engagement* (auto opt-in = default effect, no extra tasks).
**Apply when.** Adding gamification by copying a mechanic instead of finding your CURR.
**The move.** Find the single retention metric that compounds your DAU before choosing mechanics. PBL (points, badges, leaderboards) is the free sample — there are ~290 gamification mechanics. Useful three: competition (defined start/middle/end missions), progress bars as trajectory achievement (not just onboarding), engagement-unlocked content (a forecast panel opens only after 30 real entries — blocked as a ladder, not a paywall).
**Visual.** Duolingo's DAU curve from mid-2018 to mid-2022, marked "Started working on CURR" at the inflection, with a 4.5× arrow from there to the top right — `../assets/2081714430811730162__1.jpg`
**Source.** [@richardrx · 2026-07-27](https://x.com/richardrx/status/2081714430811730162)

## Don't mistake signups for traction
**Principle.** Signups are the cheapest action a user takes, so they measure curiosity, not value — especially in freemium. Real growth is whether people come back and do the action that delivers value.
**Apply when.** A rising signup curve on the dashboard feels like proof of traction, particularly under a freemium model.
**The move.** Treat signups as top-of-funnel only — never stop reading there. Track who returns on day 2 and day 7 (D1/D7 retention) and how many complete the value-delivering action (activation). Paid media can inflate signups while real retention stays flat.
**Voice.** "The signup curve climbs with paid traffic, but usage and activation only climb with a good product."
**Source.** [@richardrx · 2026-06-11](https://x.com/richardrx/status/2065082771987394651)

## Don't bet your product on an underpowered A/B test
**Principle.** Most A/B tests in small SaaS lack the volume to prove anything, yet founders swap the whole product on the result. Testing without enough sample to conclude is the trap.
**Apply when.** You're in traction or survival stage, ran a test for a week, saw "variant B won by 12%," and want to ship it everywhere.
**The move.** Before running, compute the minimum sample size (free calculators exist); if you can't hit that floor in reasonable time, don't start. Test big things (headline, offer, pricing structure, onboarding) since large effects need less sample. Never stop a test because the number looked pretty mid-way. With no volume, decide by qualitative research — five good interviews beat an underpowered A/B test. Beware the law of small numbers and confirmation bias.
**Evidence.** ProfitWell is categorical: don't A/B test price — you'll never have the volume or context for it to mean anything.
**Source.** [@richardrx · 2026-06-01](https://x.com/richardrx/status/2061463480868229189)

## Celebrate signal quality, not list size
**Principle.** A waitlist exists to validate that a pain is one people pay to solve — not to sell. Absolute size is a vanity metric; conversion-weighted quality is the real signal.
**Apply when.** You launch a waitlist and feel tempted to celebrate raw headcount.
**The move.** Convert size to expected customers before reacting: a good waitlist converts 15–20% to paying, above 30% is excellent. 53 people at 20% = 10 customers; 1,000 people at 1% = 10 customers — same result, different perception. Until there's a transaction, there's no validated hypothesis.
**Voice.** "Founders celebrate the size of the list when they should celebrate the quality of the signal."
**Source.** [@richardrx · 2026-04-17](https://x.com/richardrx/status/2045094511106220220)

## Translate churn points into LTV, not percentages
**Principle.** Most people watch churn %, but few compute what each point costs in accumulated LTV over 12 months. Cutting churn is a cash lever that needs no price hike or new acquisition.
**Apply when.** You're staring at a churn percentage and treating it as a vanity number rather than money.
**The move.** Do the churn→LTV math: at 25% monthly churn on 1,000 users you must add 250 new users/month just to break even — kill paid traffic and the product dies in ~4 months. Then improve retention without Figma: define the Aha Moment, measure time-to-value (TTV) from signup to it, ask "how do I deliver this faster?", break it into micro-wins if you can't, then test, measure, repeat.
**Evidence.** Finance SaaS, ARPU R$120: cutting churn 5 points (25%→20%) is +R$72,000/year in cash, with no price change and no extra acquisition.
**Source.** [@richardrx · 2026-04-06](https://x.com/richardrx/status/2041184077106004289)

## Nine product metrics, each telling one thing
**Principle.** ARR = size (not necessarily health). Burn rate = risk (time until death). CAC = efficiency (but obsessing over lowering it can worsen conversion with a less-qualified cohort). DAU/MAU = engagement (<20% = bad sign). LTV = product (does the customer see value?). Churn = fit (user doesn't understand or see value → cancels). NRR = real growth (>100% = good). Gross margin = model (<70% in SaaS = problem, except AI wrappers). Runway = survival (<12 months = danger). Metrics are like a blood panel — one bad reading is critical, but all-good is real health.
**Apply when.** A founder fixates on one number or conflates what each metric diagnoses.
**The move.** Use each metric as a diagnostic for its matching layer, then read the full panel before prescribing a fix: ARR alone cannot prove health, low CAC can hide a weak cohort, and strong growth without margin or runway can still be fatal. Treat one bad result as a specific warning and the bundle as the business's health check.
**Source.** [@richardrx · 2026-01-12](https://x.com/richardrx/status/2010675817483817384)
