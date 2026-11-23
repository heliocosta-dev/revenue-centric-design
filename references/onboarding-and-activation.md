# Onboarding & Activation

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Audit the trial emails as one sequence — every unsubscribe cuts a reactivation channel
**Principle.** Each team hangs its own email on the trial sequence — onboarding, marketing, customer success, billing — and nobody adds them up. A trial user who unsubscribes loses the only channel that could bring them back to activate, and a trial that doesn't activate churns before paying the first month.
**Apply when.** Several teams send automated email during the trial, or activation is weak despite "plenty of nurturing."
**The move.** Five-minute test: (1) list every automated send a user gets in the first 14 days of trial, adding onboarding, marketing and transactional; (2) count them; (3) next to each, note whether it leads the person to do something inside the product or only informs; (4) pull each email's unsubscribe rate. If most only inform, your sequence talks about you instead of taking the user to first value. If one email concentrates the unsubscribes, it's the first cut — even if someone on the team likes it.
**Evidence.** Richard cites a 2026 Baymard survey of US online shoppers: 48% of people who unsubscribe from a newsletter leave because one specific brand sends too much email. The research is e-commerce; he suspects trial sequences share the problem.
**Source.** [@richardrx · 2026-10-29](https://x.com/richardrx/status/2115926984710668624)

## Make the invite modal say what the invitee can't see
**Principle.** Nobody brings another person into their company's system without knowing what that person will see inside. That's why an invite button that has existed since the MVP still leaves most accounts with a single user: the modal asks for an email and stops there.
**Apply when.** Accounts rarely add a second user, or you're shipping a role-specific invite (accountant, agency, partner).
**The move.** Put the sentence that scopes the access right above the email field. In RepareCar's invite for the shop's accountant — usually sent by whoever handles the cash, often the owner's wife — the most important line says what the accountant can't do or see: "doesn't issue or cancel invoices, doesn't see work orders, the yard, the dashboard or your account data." Ship the screen with a single KPI. Then split accounts that invited someone from those that never did and compare their churn; a big gap means you found hidden churn on a screen nobody has opened in Figma since the MVP.
**Evidence.** In 90 days, a third of the 100 shops that opened the modal sent the invite.
**Visual.** RepareCar's accountant-invite modal: what the accountant can do (configure and export the shop's tax data) and can't (issue or cancel invoices, see work orders, yard, dashboard or account data), above the email field and a copyable invite link — `../assets/2108257345222389995__1.jpg`
**Source.** [@richardrx · 2026-10-08](https://x.com/richardrx/status/2108257345222389995)

## The salesperson is the onboarding you haven't designed
**Principle.** Some SaaS have an excellent demo: the seller walks the client exactly to what they need to see, explaining every detail and answering every question. Then the client gets a login and conversion collapses. It looks like an onboarding problem, but sometimes it's worse — the demo was masking the product's complexity, and the seller doesn't log in with the customer.
**Apply when.** Demo-assisted conversion is strong but self-serve conversion, or activation after handoff, is weak.
**The move.** One-hour diagnosis: record a demo and note every time the seller explained, pointed, or clicked for the client. Each item on that list is a place where the product, on its own, loses people — and the gap between demo-assisted and self-serve conversion is exactly the size of the list. The same recording trick works on the landing page: see "Win the first 30 seconds with the hero" (2026-10-22).
**Voice.** "The salesperson is the onboarding you haven't designed yet, and he doesn't log in with the customer."
**Source.** [@richardrx · 2026-09-22](https://x.com/richardrx/status/2102421181324276215)

## Map the whole journey to value — then fix the biggest drop, not the first step
**Principle.** Founders rush to the top of the funnel when activation falls, but the leak is usually in the middle — the step where effort is already high and the user hasn't seen proof it's worth it. Method: (1) Define what "value" is (the first moment the user gets the promised result — measurable, visible in data). (2) List every step between signup and that value (every screen, click, wait, field — always more than you remember). (3) Measure drop per step; find the steepest fall. (4) Fix the biggest drop first — that's where the money is. (5) Diagnose why: friction (cut), confusion (direct attention), ordering (deliver value before asking effort).
**Apply when.** Activation is low and you're not sure where the leak is.
**The move.** Count the steps before first value — each is a chance to quit. High activation lives in the shortest path to first result, not the most complete product before it. Almost every founder has this map in their head and never on paper; the head version always looks shorter.
**Source.** [@richardrx · 2026-07-08](https://x.com/richardrx/status/2074814716824731651)

## An onboarding video welcomes — it doesn't teach
**Principle.** A good onboarding video isn't a manual (nobody reads their car's or iPhone's). It welcomes, builds connection, shows the product at a glance, and points to where value comes fastest.
**Apply when.** Designing first-run onboarding or a welcome video.
**The move.** Aim it at cutting TTV, support tickets, and the lost feeling — not at educating. Length follows your ICP's urgency (someone rushing vs. someone happy to build Lego). No actor or fancy set — Richard recorded his in Screen Studio and it beat many big products'.
**Visual.** A "Your account was created!" welcome modal with an embedded intro-video thumbnail and a single "Next" CTA — `../assets/2067987722954735812__1.jpg`
**Voice.** "Your product doesn't need a manual either — have you read your car's?"
**Source.** [@richardrx · 2026-06-19](https://x.com/richardrx/status/2067987722954735812)

## Rising MRR with rising churn means you lost them on day one
**Principle.** When MRR and churn climb together, the user didn't leave in month 2 — they were lost the first day, dropped into a dead empty-state dashboard with nothing guiding them to value.
**Apply when.** Churn is creeping up and you're tempted to blame the product or add features.
**The move.** It isn't a feature gap — measure **TTV** (time-to-value) and get obsessed with shrinking it. CAC, LTV and activation are *product* metrics, not marketing; with weak retention, acquiring more just fills a leaky bucket faster.
**Voice.** "It took two months to cancel, but you lost him the first day after signup."
**Source.** [@richardrx · 2026-06-18](https://x.com/richardrx/status/2067591574138052804)

## Measure activation, not signups
**Principle.** Technical founders track the wrong onboarding metrics; signups, session time, and tour completion all flatter you without proving the user reached value.
**Apply when.** You're judging onboarding by signups, time-in-product, or "completed the tour."
**The move.** Swap each vanity metric for its real counterpart: signups → activation rate, session time → time-to-first-useful-action (and its repetition), onboarding completion → D7 retention. Find your aha moment empirically: look at what every paying customer did in week one that churned users didn't (often a collaborative act — invite, share, comment). Anchor on TTV/time-to-value.
**Evidence.** Userpilot benchmark (547 companies): avg TTV 1d 12h 23m; top performers under 5 min. SaaS activation rate avg 30–37%, top quartile 40%+, under 20% = structural problem. D7 retention avg 10–15%, over 30% is strong.
**Voice.** "If you can't say how long your user takes from signup to aha moment, you're not measuring what matters."
**Source.** [@richardrx · 2026-05-27](https://x.com/richardrx/status/2059616501544468624)

## Put friction in the right place, not zero friction everywhere
**Principle.** Friction in the wrong place kills the product; friction in the right place qualifies and retains. "Less friction" is not a universal law.
**Apply when.** You're reflexively cutting clicks and fields, or your human sales team is doing qualification the product should do.
**The move.** Remove friction at trial signup (it kills acquisition), but add calibrated friction in three spots: (1) trial with card upfront filters commercial intent; (2) mandatory onboarding before the dashboard turns users into power-users faster; (3) a 6–8 field enterprise demo form (role, team size, current tool, budget, timeline) lowers lead volume but raises close rate. The mechanism is effort justification (Aronson & Mills, 1959) — same root as the endowment and IKEA effects.
**Evidence.** ChartMogul 2026: opt-in trial (no card) converts 8.9%; opt-out (with card) converts 31.4%. Superhuman requires a 30-min human call before access.
**Voice.** "How much qualification effort is your human seller doing that the product should do before they even step in?"
**Source.** [@richardrx · 2026-05-21](https://x.com/richardrx/status/2057436163841941980)

## Never ship a blank dashboard
**Principle.** The empty dashboard arrives at the user's peak of curiosity and answers it with a void — this is where most SaaS loses the trial. Every second spent deciding what to do is a second closer to quitting.
**Apply when.** A new user lands post-signup on a screen with no data and no direction.
**The move.** Four fixes: (1) empty state with a next-action hint — the CTA points straight to value; (2) seed sample data so they see the destination before starting; (3) one single clear action ("Import your first spreadsheet"), not eight, not a 12-step tour; (4) visible progress from the first click — start the bar at 20%, not 0%, so completion feels already underway.
**Voice.** "A blank dashboard looks neutral, even tidy — but it just makes the user stop and think about what to do."
**Source.** [@richardrx · 2026-05-12](https://x.com/richardrx/status/2054283657934758021)

## Design onboarding as a behavioral trigger, not a feature tour
**Principle.** Silent non-activation — users who sign up, vanish in five minutes, and never formally churn — is an activation problem, not a product one. Onboarding should fire a behavior, not narrate features.
**Apply when.** New users evaporate without complaint and you never learn their name.
**The move.** Find the single behavior that statistically separates retained from lost users, make it your activation north star, and measure every onboarding decision against it. Shift focus from explaining features to forcing that behavior fast. Exploit the Zeigarnik effect: open small loops (complete profile, invite 3 colleagues, send first message) so the user carries an unfinished task.
**Evidence.** Slack: teams exchanging 2,000 messages had 93% probability of staying. Facebook's equivalent: 7 friends in 10 days — the company's single focus, repeated at every all-hands.
**Voice.** "What's the number that separates who stays from who evaporates — and how does the user hit it in under 24h?"
**Source.** [@richardrx · 2026-05-11](https://x.com/richardrx/status/2053878928494690414)

## Map the journey from session replays, not from your diagram
**Principle.** The founder's 12-step journey is built top-down (what the product wants); the user runs 4 steps bottom-up (the specific problem they opened the tab to solve). The gap between them is where avoidable early-stage churn lives — and it's invisible because the founder only ever lived the creator's journey.
**Apply when.** You "know" the happy path but can't state what % of users actually execute it.
**The move.** Three steps, no Figma: (1) write your version of the user journey in numbered steps, on paper; (2) open five real session recordings from the first 7 days and note what each user actually does, in order, with timing — including what they try and abandon; (3) lay both lists side by side. The report is in the differences; each divergence is a hypothesis to confirm or kill.
**Voice.** "The user journey is what shows up in the replay; what's in Figma and Excalidraw is a hypothesis."
**Source.** [@richardrx · 2026-05-08](https://x.com/richardrx/status/2052711138572263474)

## Add declarative friction, cut administrative friction
**Principle.** "Good onboarding is short onboarding" is incomplete. There are two frictions: administrative (collects data the system uses later, buys the user nothing) and declarative (forces the user to state what they came to do — costs a beat, buys commitment, customization, and journey direction).
**Apply when.** Auditing onboarding steps; deciding what to cut versus expand.
**The move.** Test each step: is it collecting data or making the user declare intent? Collecting only → candidate to cut. Declaring intent → candidate to expand. A declaration ("what do you sell, what's your long-term goal?") creates a micro-commitment to the outcome before the user touches the product, and lets the journey branch (recommendations, tutorials, next actions) off that answer.
**Evidence.** Brazilian payments platform cut time-from-signup-to-first-sale from 24.2 to 2.5 days by adding a ~30-second intent step (positioned between signup and product), not by removing steps.
**Voice.** "Onboarding is also the first chance the user has to declare to themselves what they came to do."
**Source.** [@richardrx · 2026-05-07](https://x.com/richardrx/status/2052350703541039324)

## Trial conversion is a journey problem, not a pricing problem
**Principle.** A trial is a test of value; if the user never proves value to themselves, no price or trial length saves it. Conversion fails for three diagnosable reasons.
**Apply when.** Users sign up, do "a bunch of nothing," and never return.
**The move.** Diagnose which failure mode applies: (1) blank dashboard → make the first step obvious and immediate, drive to value or a micro-win, drop "explore our product"; (2) lost before value → install Clarity, watch where they stall, optimize that click; (3) lost to life → send a progress email ("you created 3 reports, your team accessed 12 times, you're in the top 20%"), not a generic "trial ending."
**Voice.** "The longest trial in the world doesn't save bad onboarding."
**Source.** [@richardrx · 2026-05-06](https://x.com/richardrx/status/2052096365128273956)

## Make onboarding active, not passive
**Principle.** Passive onboarding (tooltips, guided tour, docs — learn if you want) assumes the user will explore. They won't: they have 47 tabs open, WhatsApp pinging, and will do the bare minimum before deciding whether to return. Active onboarding designs a sequence where each action delivers value and that value triggers the next.
**Apply when.** Your onboarding opens with "Welcome, here's the documentation."
**The move.** Assume you know the shortest path to value better than the user does. Design that path, strip the friction, and make sure they arrive. Don't ask "what's the minimum the user must do?" — ask "what's the smallest action that delivers the most value in the least time?"
**Evidence.** Slack drops you into a channel and makes you send a message first — you use the product before any tutorial.
**Voice.** "Understanding by doing beats understanding by reading."
**Source.** [@richardrx · 2026-04-22](https://x.com/richardrx/status/2046959126245249288)

## Treat sub-30-day churn as an onboarding fix, not a feature gap
**Principle.** Most early-stage SaaS churn happens in the first 30 days — which means it's onboarding, not product. Adding features only makes it worse by adding complexity.
**Apply when.** Users leave before they ever liked what you built, and you're tempted to ship more features.
**The move.** Diagnose with three questions: (1) how long to the first real result? If "it depends" or over a day, you're bleeding users; (2) does the user know where they are? Use a progress bar/checklist — Progress effect: someone seeing 30% done is likelier to finish than someone at 0%, so starting at 0% is a design error; (3) what happens when they drop mid-flow — email, push, nothing? Use the Zeigarnik effect to remind them they started.
**Voice.** "Sub-30-day churn rarely dies to features; it dies to the right sequence of micro-interactions that deliver value before asking for effort."
**Source.** [@richardrx · 2026-04-20](https://x.com/richardrx/status/2046212675017887881)

## Deliver the promised result before teaching mechanics
**Principle.** Nobody wants to learn to use your product; they want the result you promised in the landing-page hero. Teaching mechanics first ("create a project → add a member → configure integrations") is boring; delivering value first converts.
**Apply when.** Your onboarding is a checklist of setup mechanics rather than a path to the outcome.
**The move.** Lead with the outcome ("In 2 minutes you'll see your first report → let's start with the data you already have → done, that's the insight competitors pay consultants for"). Reframe progress with the Progress effect by crediting effort already spent ("You've done the hard part, just 3 steps left"). Keep loops small (Zeigarnik effect — people close loops only if they look closable). Pre-select the right plan from data you collected instead of asking, then offer the upsell.
**Voice.** "The gap between 5% and 15% trial conversion is in these details — not features, not price — in the sequence of micro-decisions you designed without realizing you were designing."
**Source.** [@richardrx · 2026-04-16](https://x.com/richardrx/status/2044785090832543998)

## Qualify by behavior, not by a long signup form
**Principle.** Friction at the wrong moment kills conversion, and qualification by behavior is more precise than qualification by form. The "more qualified leads" argument for long forms usually loses.
**Apply when.** You're weighing an 8-field signup form against email + password.
**The move.** Default to the minimal form and let qualification happen later, inside the product, from real behavior. Deciding where to add versus remove friction is what separates a product that grows from one that spins its wheels — but it's contextual ("it depends").
**Evidence.** Same product, two founders: 8-field form (name, email, company, role, phone, segment, team size, how-did-you-hear) → 12% signup rate; email + password only → 34%.
**Visual.** Annotated onboarding step (DevNoodles): an ICP/intent question flagged "Zeigarnik effect" (the step progress dots) and a B2C/B2B card selector flagged "Default effect" (the B2C card is pre-badged "Mais comum") — showing where each bias is engineered into the flow. — `../assets/2042558822825239030__1.jpg`
**Source.** [@richardrx · 2026-04-10](https://x.com/richardrx/status/2042558822825239030)

## Celebrate the activation moment, don't just confirm it
**Principle.** At the emotional peak of activation, a number is data but a rising graph is progress — and progress triggers dopamine and an emotional memory tied to the product. Most SaaS confirms where it should celebrate.
**Apply when.** A user completes a hard-won first action (first transaction, first integration) and you respond with a static success state.
**The move.** Engineer the peak moment precisely at the point of highest emotional vulnerability in activation — right after the user clears the effort. Show motion and accomplishment proportional to the effort invested. This is the peak-end rule: users judge an experience by its emotional peak and its ending, rarely by the average.
**Evidence.** Stripe shows a rising graph (not a number) the moment the first transaction processes — the founder who integrated it at 3am remembers exactly where they were.
**Voice.** "A number would have done the job. The graph created a customer."
**Source.** [@richardrx · 2026-04-04](https://x.com/richardrx/status/2040415841628651689)

## Cut time-to-value by reorder and removal, not feature changes
**Principle.** High TTV is almost never product complexity — it's the form and order in which things happen. Each day between signup and first result is another day of abandonment risk; abandonment = churn.
**Apply when.** Your activation flow is slow and you assume the product itself is the bottleneck.
**The move.** Three iteration cycles, no product changes: (1) reduce cognitive load by grouping and standardizing what the user must fill in; (2) work with legal/compliance to strip everything required by habit but not by actual necessity; (3) invert the sequence so the user feels value before facing the heaviest step.
**Evidence.** Major Brazilian payments platform: 24 days → 2.5 days to first sale (89.7% reduction), no product changes, no cutting of mandatory compliance steps.
**Visual.** Month-by-month TTV table: Jan 24.2d → Feb 19.6d → Mar 16.8d → Apr 9.3d → May 2.5d, alongside accounts created / approved / new sellers per month. — `../assets/2037583944283996418__1.jpg`
**Source.** [@richardrx · 2026-03-27](https://x.com/richardrx/status/2037583944283996418)

## Give the trial an active goal, not passive access
**Principle.** A passive trial ("use it if you want, cancel guilt-free") builds no commitment; a trial with an active goal builds commitment before billing. Each completed day raises the psychological cost of canceling — the user starts defending a decision they already made, before paying.
**Apply when.** Your trial is open-ended access with no challenge or target.
**The move.** Set a recurring daily goal during the trial that the user opts into and completes. The named mechanism is progressive commitment. The product can be good or bad — done right, the onboarding itself is excellent.
**Evidence.** Wispr Flow challenges trial users to dictate 100+ words a day for 7 days — looks generous, is behavioral science.
**Source.** [@richardrx · 2026-03-26](https://x.com/richardrx/status/2037316988981174464)

## Calibrate the first step to the user's real willingness
**Principle.** Users don't rationally evaluate the first task — they evaluate perceived effort. Ask too much up front and the cognitive cost of even imagining the task is paralyzing, and they quit before starting. This is the activation-barrier effect.
**Apply when.** Your first onboarding step bundles setup, data import, team invites, and project creation — or demands a campaign-sized action.
**The move.** Two biases fix it: (1) started-progress effect — show what the user has already done before what's left; a loyalty card with the first stamp pre-filled beats a blank 9-stamp card, because the starting point changes perceived distance to the finish; (2) small-steps effect — "Create one story today" has radically lower perceived cost than "post 5×/week," even when the underlying task is identical. Sequence effort so the user hits first value before noticing how much they invested; build momentum.
**Evidence.** Instagram A/B test made "Create 5 new public reels" the first task — for someone who barely posts weekly, that's paralyzing.
**Visual.** Bad first-step example: a weekly-progress checklist at "0% completed" whose top item is "Create 5 new public reels (0/5)." — `../assets/2036461688505909250__1.jpg`
**Voice.** "Asking for more isn't necessarily the problem; asking for all of it at once, with no progress anchor and no commitment ladder, is."
**Source.** [@richardrx · 2026-03-24](https://x.com/richardrx/status/2036461688505909250)

## Treat onboarding as the bridge between CAC and LTV
**Principle.** Founders obsess over CAC and landing-page conversion but are blind to activation cost. Onboarding isn't an interface tutorial — it's the bridge from CAC to LTV and the point of maximum leverage to expand revenue. Cancellation happens on day one; it's merely formalized when Stripe's billing reminder lands.
**Apply when.** Users enter the trial without intent to a result and ghost before ever paying.
**The move.** Two fixes: (1) turn support into UX — every onboarding support ticket is a design failure; map recurring setup questions and convert the answers into features or in-flow tooltips; (2) compress TTV obsessively — make the user experience the product's core promise in the least time possible. If they must configure 5 screens before any result, you've already lost.
**Voice.** "Letting a user into the trial without intent of a result isn't self-service. Design's job doesn't end at signup — that's where it starts paying you back."
**Source.** [@richardrx · 2026-03-13](https://x.com/richardrx/status/2032485654811083005)

## Pick onboarding patterns by awareness × flow complexity
**Principle.** There's no best onboarding in the abstract — only the one that removes friction and delivers value early for your users. Treat the nine patterns as behavior-shaping mechanisms, not UI components, and select by two axes.
**Apply when.** Choosing or combining onboarding patterns for a new flow (SaaS, PLG, B2B early stage).
**The move.** The nine patterns (pattern → ideal use / tradeoff): **1. Welcome modal** → high-awareness ICP or low-complexity products; easy to build, easy to ignore. **2. Wizard / product tour** → B2B and complex/high-cost-of-error flows (fintech, compliance); long tours cause boredom and need constant upkeep. **3. Contextual tooltips** → advanced/secondary features; slashes support tickets but users may miss them if contrast is poor. **4. Empty state** (his favorite) → dashboards, lists, data-dependent areas; if executed well it's mandatory, directs the first action and accelerates TTV. **5. Personalization** → products serving many ICPs with different journeys; great CRM data, but too long kills signup conversion. **6. Checklists** → critical flows with mandatory prerequisites (webhook, KYC); exploits the Zeigarnik effect, but a long list breeds aversion — every item must move toward value, no bureaucratic tasks. **7. Goal-setting** → habit products (finance, productivity, health); uses commitment bias, but a broken goal can break the emotional contract. **8. Sample data** → sell the dream of a full, organized product before the user inputs anything (distinct from skeleton screens). **9. Use cases / demos** → products burning expensive resources (AI tokens) with infinite outputs; show max potential without forcing creativity from scratch.
Selection rule — two axes: **awareness level** (low = needs guidance; high = needs speed) × **flow complexity** (high = needs structure). Four cases: low-awareness + high-complexity → tours + checklists + personalization; low + low → modal + empty state; high + high → checklist + tooltip + empty state; high + low → modal + empty state (then get out of the user's way). Build vs. buy is financial/operational, not aesthetic — buy (Wistia, PostHog, Sprig) when speed is critical, dev is overloaded, or you're running A/B tests; build when onboarding is strategic, you need perfect aesthetic integration, or you must avoid third-party dependence.
**Voice.** "Onboarding's job isn't to teach the user — nobody likes an instruction manual — it's to remove cognitive effort and deliver utility as fast as possible. TTV correlates directly with churn."
**Source.** [@richardrx · 2026-02-04](https://x.com/richardrx/status/2019019293761941566)
