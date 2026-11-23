# Conversion & Landing Pages

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post.

## Don't let the hero look like the end of the page
**Principle.** A "false floor" — a first block that looks finished (a full-screen video or image, a color band closing it off, empty space, a line across the screen) — makes people conclude the page ends there. Without a cue that there's more, they leave without converting.
**Apply when.** Your hero fills the viewport (`height: 100vh`) or ends in a visual "closing" element.
**The move.** Suspect the 100vh hero first: it forces the block to screen height, so the fold lands exactly at its end — and on mobile the address bar makes 100vh taller than the visible area, hiding the next block even more. Check Clarity's scroll depth (the % of visitors reaching each height); a sharp drop at one point gives the anomaly away. And make the hero say who the product is for even without scrolling — one doesn't replace the other. Pre-PMF this is expensive, because traffic is small and the hero can't yet sell the whole product.
**Evidence.** NN/g asked 8 people to find out what Maple, a New York delivery service, sold: 6 didn't realize the page scrolled, clicked the full-screen video's "Start" button, and landed in signup windows with no information about the service — the explanation sat just below. That's qualitative (it shows how, not a rate); at scale, NN/g eyetracking found the 100 pixels just above the fold got 102% more attention than the 100 just below.
**Source.** [@richardrx · 2026-11-20](https://x.com/richardrx/status/2123828802010689646)

## On Google, give every search intent its own landing page
**Principle.** On Google, the landing page does the job the creative does on Meta — and Google gives you for free what Meta makes you guess: the person types their intent into the search box. Yet teams test 20 creatives a week on Meta while almost every SaaS sends all Google searches to the same home page and blames the CPC.
**Apply when.** Running search ads (or SEO) where every keyword lands on the home page.
**The move.** Map one page per intent (the search-taxonomy lens Richard learned studying SEO with Fábio Ricotta): **problem** search ("how to write an auto-shop quote") → a page that teaches and shows the problem solved; **comparison** ("best auto-shop software") → a page comparing options, yours included; **competitor** ("alternative to [current tool]") → an honest us-vs-them page covering what changes in the migration; **category/brand** ("auto-shop software") → the product page with pricing. At minimum, repeat the searched words in the page title. The math: R$30k/month at R$5 CPC buys 6,000 clicks; a generic home converting 2% yields 120 signups at R$250 each; a page matching the search at 3% yields 180 at ~R$167 — one conversion point, 50% more signups, zero extra media.
**Voice.** "Whoever searches 'how to write a quote' and lands on a home shouting 'free 14-day trial' leaves before the second paragraph — and you paid R$5 for it."
**Source.** [@richardrx · 2026-10-28](https://x.com/richardrx/status/2115572033639575650)

## Win the first 30 seconds with the hero — then give the survivors the whole pitch
**Principle.** Landing pages don't lose visitors gradually; they lose almost all of them in the first seconds. So "short or long page?" — both, at different moments. The hero has one job: survive the first ~30 seconds by saying who it's for and what changes in that person's life. Everything below — testimonials, comparisons, FAQ, objections — is for those who stayed, and they read calmly. Founders do the opposite: a "Welcome to the new way to manage your business" hero with a generic 3D illustration, and the argument that closes the sale saved for the sixth scroll.
**Apply when.** The founder closes on calls but the page doesn't sell; the page is a hero, three icons and a "Start free" button.
**The move.** Record your next sales call, transcribe it, and mark every argument, example, or answered objection that moved the buyer forward; then look for each one on the page — whatever you can't find is missing. The founder can't see the gap because the closing arguments live only in their head, and from inside it the page looks complete (curse of knowledge). Then the 10-second test: open your page, count 10 seconds, close it — what you read is all most visitors will ever know about the product. Read with "Design the features page for skimming" (2026-02-09): skimmers and survivors are different readers of the same page.
**Evidence.** Microsoft Research analyzed dwell times on ~205k pages and found that on 98.5% of them, the longer someone has stayed, the less likely they are to leave; Jakob Nielsen's NN/g reading of the study adds that the first 10 seconds are the most critical, the risk stays high until ~30 seconds, and visitors who pass that point often stay 2 minutes or more. Moz: CEO Rand Fishkin sold live at any conference, the site didn't; the agency had him pitch them as if they were the customer and recorded it — he needed 5+ minutes while the page was a one-minute summary that barely showed eBay, Disney and Marriott as clients and omitted the experts-answer-your-questions feature subscribers loved most. The new page, 6× longer, sold 52% more in an A/B test with 5,000+ visitors; a US$1 first month (on a US$79 plan) then surfaced ~500 replies fearing an annual-contract catch, fixed by one explanatory email — ~170% more conversion over 4 months and US$1M+ a year (figures from Conversion Rate Experts' own case study).
**Source.** [@richardrx · 2026-10-22](https://x.com/richardrx/status/2113245288953483423) and [@richardrx · 2026-10-14](https://x.com/richardrx/status/2110364139549773892)

## Make social proof verifiable — real names, the original post, even a link out
**Principle.** Organic proof beats produced proof. In his first e-commerce, in 1999, Richard saw organic product photos outsell the manufacturer's official ones; 27 years later UGC still beats produced campaigns. A customer's crooked, badly lit WhatsApp screenshot is more credible than a designed testimonial card with a little avatar.
**Apply when.** Your SaaS buys cold traffic and leans on testimonial cards nobody can check.
**The move.** Import proof from outside the page: real names, screenshots that look like the original LinkedIn post, and a link to it. Infoproduct sellers convert with "trash" pages because credibility was built in their content and the audience arrives warm; a SaaS buying cold traffic gets no ready-made credibility, so the page has to import it (other brands, customers) or earn it through time on screen. This is a deliberate exception to "No clicks out, plus brutal CTA contrast" (2026-02-05) — the outbound link risks the visitor running into an objection the page doesn't answer, and it still won.
**Evidence.** On the Baralho de Vieses (bias card deck) site, testimonials with real names and a link to the original LinkedIn post performed almost 22% better than the same testimonials without link or identifier.
**Visual.** The tested section: LinkedIn-style testimonial cards (name, title, LinkedIn icon, the customer's own photo) under a "used by 10,000+ professionals" header with client logos — `../assets/2099482067247448484__1.jpg`
**Source.** [@richardrx · 2026-09-14](https://x.com/richardrx/status/2099482067247448484)

## Performance is conversion: 31% better LCP → +8% sales (Vodafone A/B)
**Principle.** You can raise conversion before opening Figma — web performance is a conversion lever, not an engineering nicety. Vodafone Italy A/B tested web-vitals optimization (LCP 31% better than control, same offer/creative/screen, 100k clicks and 34k visits/day per variant, paid traffic): +8% sales, +15% lead-to-visit, +11% cart-to-visit.
**Apply when.** Founders separate "conversion work" from performance work.
**The move.** Treat LCP/web vitals as a conversion experiment with the same rigor as copy tests — especially on paid traffic where every bounce is paid for.
**Source.** [@richardrx · 2026-08-04](https://x.com/richardrx/status/2084589988843299217)

## Compliments aren't validation — "what's missing for you to PIX now?" is
**Principle.** Everyone loves your idea, nobody bought. Compliments are free and worth nothing (like your freemium). The simplest validation test: try to sell. If you can't close inside your ICP, ask directly: "Falta o que pra você fazer o PIX agora?" ("What's missing for you to send the PIX instant payment right now?") The pause reveals the truth — either the real objection (your build list) or excuses (the "loved it" was just politeness). Follow up: "If it had that, would you pay now?" Then do 20 sales this way.
**Apply when.** Collecting praise but no revenue.
**The move.** Sell before building. Richard sold 20 subscriptions off a gray clickable wireframe — the QR code wasn't even real. Nobody said "paint the wireframe"; they asked for invoices and a second mechanic login. Those doubts became sales arguments and FAQ items. The gray was enough to prove the only thing that mattered: people with the pain and in a hurry to pay. Design came after, to scale what conversation already proved sells.
**Source.** [@richardrx · 2026-07-07](https://x.com/richardrx/status/2074539418266812580) and [@richardrx · 2026-06-24](https://x.com/richardrx/status/2069743203863962080)

## "Paint the button" is judging the last line of a long cascade
**Principle.** The visual layer of a landing page is the tip of a cascade that begins at the ICP — so "make it more colorful" critiques the *end* of a process as if it were the start.
**Apply when.** Gathering or acting on LP feedback, or reaching for button color first.
**The move.** Work the cascade in order: ICP → the buyer's **awareness level** (Eugene Schwartz's 5 stages) → what you say and how → visual positioning (tone → form, color, type, space). Low awareness: open on the problem, name the pain in the first fold, then the mechanism and your fix. Higher awareness: go straight to your advantages vs. alternatives. Jump to button color and you've silently (and probably wrongly) answered who you sell to, their awareness, which pain, and what tone.
**Voice.** "They're looking at the end of a process and thinking it's the beginning."
**Source.** [@richardrx · 2026-06-23](https://x.com/richardrx/status/2069469303464730988)

## Scaling cold traffic is an honesty test for your page
**Principle.** Conversion measured on warm audiences (existing followers) is inflated — they forgive the page's flaws. Only cold traffic reveals how much of your rate is the page versus borrowed trust.
**Apply when.** Ad spend goes up but revenue barely moves, and the conversion rate "drops" even though you fixed nothing.
**The move.** Treat any baseline built on warm public as fiction, not a performance number. When you scale budget into cold traffic and the rate collapses, that gap is the page's real ceiling — fix the obvious page defects first, then judge media.
**Evidence.** A founder tripled ad spend; revenue rose only 11%. Warm-traffic conversion of ~3% (driven by Instagram followers) cratered to 0.5% on cold traffic; fixing the obvious lifted it to 2% — 4x the real number.
**Voice.** "Scaling budget into cold traffic works like an honesty test: it shows how much of your conversion is your page and how much is borrowed trust."
**Source.** [@richardrx · 2026-06-08](https://x.com/richardrx/status/2063972594223661127)

## Test hero comprehension with a stranger from your ICP
**Principle.** The cheapest usability test nobody runs: show your LP hero to one person for 5 seconds, take it away, ask "What does this product do? For whom?" If they can't answer, the hero failed — no matter how pretty it is. In those seconds the brain asks three questions, almost in order: what is this → is this for me → why should I care now. The mechanism is cognitive load: every second spent decoding what you do is a second closer to giving up — clarity beats cleverness at the top of the funnel, always.
**Apply when.** A hero trades clarity for "creativity" ("Revolutionize your workflow" doesn't say what it does; "The definitive productivity platform" doesn't say for whom).
**The move.** A hero needs: (1) a headline saying what the product does, in the customer's language, not internal jargon; (2) a subheadline nailing the ICP and the concrete result; (3) real visual proof — a screenshot of the product working, not a generic smiling illustration; (4) a specific CTA; (5) immediate social proof (a logo or a number) above the fold. Specificity sells: "Controle de comandas pra oficina mecânica" ("Work-order control for auto repair shops") beats "Software de gestão" ("Management software"). If you covered everything on the page except the hero, could a stranger from your ICP say what you sell in 5 seconds? Read with "Pass the 5-second test — lead with the problem, not the feature" (2026-05-01): that post argues for a pain-led headline, this one for a what-it-does headline — both demand the what / for whom / why-now answers inside 5 seconds.
**Source.** [@richardrx · 2026-05-29](https://x.com/richardrx/status/2060409264683044995)

## Write the CTA microcopy, not the button color
**Principle.** The CTA label moves conversion far more than button color or shape — it's the last thing the user reads before deciding, so it must reduce the mental effort of simulating what happens next.
**Apply when.** A technical founder is A/B testing button colors for weeks over a 0.3% (non-significant) delta while the label still says "Sign up" with no click trigger.
**The move.** Make the CTA answer the three questions the brain asks before clicking: (1) what happens when I click, (2) how long it takes, (3) what it costs/commits. "Sign up" answers none; "Start free in 30s" answers two. Add a click trigger (the small line under the CTA) to answer the rest and break an objection: "Start Free Trial" + "14 days, no card". Rooted in outcome bias and Construal Level Theory (making the outcome concrete).
**Voice.** "The button is the last thing the user reads before deciding — treat it as such."
**Source.** [@richardrx · 2026-05-25](https://x.com/richardrx/status/2058875777739866490)

## Cut CAC by filtering on the landing page, not the media
**Principle.** High CAC is rarely a media problem — it's usually a filtering problem. The landing page can qualify leads before the form, killing deals that were never going to close.
**Apply when.** Clicks become leads, leads become SDR calls, calls don't close, and founders react by swapping creative or channel (or blaming the SDR).
**The move.** Pull three filtering levers so the lead self-selects without feeling filtered: (1) copy specificity — "Cash flow for service providers billing R$500k–R$3M" beats "Organize your finances"; (2) visible pricing — screens out no-budget leads so sales only meets real objections; (3) a qualification question as the first interaction (or copy/examples that play that role). CAC is cost per closed deal, not cost per lead.
**Evidence.** If you close 1 in 50 leads, dropping to 30 leads with 1 close nearly doubles media efficiency — same spend, lower CAC.
**Voice.** "The lead with no money won't magically generate money between the landing page and the sales call."
**Source.** [@richardrx · 2026-05-18](https://x.com/richardrx/status/2056385204785213446)

## Aim for 4.2–4.5 stars, not a perfect 5
**Principle.** A flawless rating reads as fake; consumers distrust unanimity. A profile that includes constructive criticism feels more authentic and converts better than pure praise.
**Apply when.** Building or curating reviews/ratings and social proof on a landing page or product.
**The move.** Let imperfection show. Stack the highest-converting combination: a detailed case study with quantifiable ROI, ideally a video testimonial from a brand recognizable to your ICP, plus customer logos. Avoid the common failure — social proof done badly: identical cards, first-name-only, all 5 stars, generic avatars instead of a real photo. Make each review verifiable (e.g., link to the actual LinkedIn post).
**Evidence.** Northwestern: purchase probability peaks at 4.2–4.5 stars, not 5. Testimonials lift LP conversion up to 34% (VWO); 5+ reviews → 270% more likely to be bought (Yotpo); 93% read reviews before buying (BrightLocal).
**Visual.** A social-proof wall done right: real faces, names + roles, verifiable reviews, and recognizable client logos (Volkswagen, Coca-Cola, Samsung, Itaú, Volvo, DocuSign, Hotmart) under a "+10,000 professionals" headline — `../assets/2054910531132183030__1.jpg`
**Voice.** "Credibility drives conversion."
**Source.** [@richardrx · 2026-05-14](https://x.com/richardrx/status/2054910531132183030)

## Compress the decision window — shorten the path to action below the path to doubt
**Principle.** The purchase decision is mostly made before checkout. Conversion is architecture: the user converts when the path to the action is shorter than the path to doubt, because every extra second of deliberation raises the odds they close the tab.
**Apply when.** You're optimizing the checkout, CTA, or headline while ignoring the deliberation time upstream.
**The move.** Compress decision time two ways: pressurize the environment with real scarcity ("Only 1 room left at this price", "Booked 3 times in the last hour") — driven by loss aversion (Kahneman: losing hurts up to ~2x more than the equivalent gain), so "1 left" registers as "I'll lose this"; or remove steps entirely (Amazon's patented 1-Click ordering).
**Evidence.** Booking runs 1,000+ simultaneous experiments (per Lukas Vermeer, 8 yrs leading experimentation); showing sold-out hotels alongside available ones *raised* bookings by sharpening perceived scarcity.
**Voice.** "The user converts when the path to the action is shorter than the path to doubt."
**Source.** [@richardrx · 2026-05-11](https://x.com/richardrx/status/2053832356293738914)

## Don't clone the page — the converting layer is invisible
**Principle.** A converting sales page is the visible shell of an invisible system. Copying the layout copies what's cheapest to produce; the expensive part (research) stays invisible and gets left behind.
**Apply when.** A page "looks like it works" and you're tempted to clone it for your own offer.
**The move.** Before copying, ask: what on this page is a function of the *product*, and what is a function of the *customer research* done before writing each line and placing each element? The hidden layer is customer vocabulary pulled from interviews, objections ordered to the ICP's specific fear, social proof hand-picked to resonate, and a core promise tuned to the stated desire. This error has a name: cargo cult — replicating the visible ritual hoping to summon the result, without grasping the causal mechanism.
**Evidence.** Two ~95%-identical pages, same niche/offer/order: 4% vs 0.6%. The 4% page belonged to Richard's client; the 0.6% was a near-pixel clone by a builder — who unknowingly DM'd the original team to complain it wasn't converting.
**Voice.** "There's a name for copying the form expecting the function. It's called cargo cult."
**Source.** [@richardrx · 2026-05-09](https://x.com/richardrx/status/2053086365781205142)

## Pass the 5-second test — lead with the problem, not the feature
**Principle.** A visitor scans your LP for ~5 seconds. If they can't answer what it does, who it's for, and why they should care, they leave — they won't stay to figure it out. Conversion begins on the first line.
**Apply when.** Your hero opens by describing what the product *is/does* (a feature/category) instead of the visitor's pain.
**The move.** Open with the visitor's problem, not yourself. "AI-powered project management platform" → meh; "Your team loses 6 hours a week hunting for information" → keep going. One talks about itself, the other talks about me. If the first line doesn't connect with the pain, the rest of the page goes invisible.
**Voice.** "If you who built it can't answer in 5 seconds, your visitor can't either."
**Source.** [@richardrx · 2026-05-01](https://x.com/richardrx/status/2050280273682510230)

## Fix contrast, layout, and trust before rewriting copy
**Principle.** The brain processes three pre-verbal variables — contrast, on-screen placement, and trust — before it reads the words, and they usually move the needle more than any headline.
**Apply when.** You're rewriting home copy for weeks chasing conversion without touching the visual/attentional layer.
**The move.** (1) Contrast is relative to surroundings, not an isolated color — a big, differently-shaped button in whitespace is *seen before it's read* (accessibility ratio 4.5:1 is a floor, not the goal). (2) Placement: Fitts's law (closer, bigger targets get clicked more) plus the F-pattern (Nielsen Norman eyetracking) — a CTA bottom-right with no visual anchor sits outside the attentional map. (3) Trust is built in four reinforcing layers: a real (non-stock) human face, a known brand or specific verifiable proof, an offer that fits the stated problem, and a solution mechanism logically coherent with the promise. When all four align, the user converts without knowing why; when one fails, they invent a rational reason to leave.
**Voice.** "Optimizing copy without working contrast, placement, and trust is masking the symptom."
**Source.** [@richardrx · 2026-04-28](https://x.com/richardrx/status/2049215050997784774)

## Specificity is the difference between decoration and persuasion
**Principle.** Generic LP copy gets discarded by the brain; specific messages are processed faster and generate more trust. A converting LP shows the *transformation* the product causes, not just what it does.
**Apply when.** Your hero reads "The complete platform for [generic category]", a 5-feature subtitle, "Start free", and no real social proof — the default Brazilian SaaS template.
**The move.** Fix the four standard failures: (1) "Complete platform" means nothing → "Cut new-dev onboarding time 40%"; (2) features on top → lead with the pain, feature as the solution (nobody wakes up wanting a "custom report feature"); (3) "Start free" is the weakest CTA (no value, no risk reduction, no urgency) → "See your first report in 2 minutes"; (4) "Used by Company X" proves nothing → "We cut Company X's churn from 12% to 6%". One page describes, the other sells.
**Evidence.** Across 30 Brazilian SaaS LPs: descriptive vs transformation-led ran 0.5% vs 3% conversion — same traffic, 6x more leads — driven by argument sequence and promise specificity, not visual design.
**Source.** [@richardrx · 2026-04-17](https://x.com/richardrx/status/2045154631974539650)

## Users scan, they don't read — give the primary action obvious contrast
**Principle.** Users scan interfaces, weighing cognitive effort against payoff, and ignore most of it. They enter with one question — "What can I do here?" — so the primary action must win on contrast within seconds.
**Apply when.** The main CTA competes with 6 other elements, or the most important action is buried inside a dropdown that requires a click to reveal.
**The move.** Make the primary action visually dominant so it's found in a glance. If the key button competes with too many elements it loses prominence; if it's hidden behind interaction it's effectively invisible. Leverage image superiority to guide attention down the page.
**Visual.** A login screen annotated with two biases — "limited choice bias" (a single dominant Google sign-in button) and "image superiority" (a vivid hero illustration pulling the eye) — `../assets/2042013751742705816__1.jpg`
**Source.** [@richardrx · 2026-04-08](https://x.com/richardrx/status/2042013751742705816)

## Judge a landing page by conversion, not by beauty
**Principle.** A landing page isn't a beauty contest — it has one measurable job: qualify the user and lower CAC by turning traffic into revenue. Evaluating a static image with no context is nearly useless.
**Apply when.** The timeline turns into "AI vs human" / "who designed it better" debates that ignore conversion, while obvious conversion flaws go unaddressed.
**The move.** Treat conversion as a continuous loop, never an isolated event: form a thesis → ship the interface and collect data → find where the user hesitated, form a new hypothesis, and optimize the next cycle. The debate defaults to aesthetics because it's easier to opine on looks than to measure results — which is exactly what keeps most LPs underperforming.
**Visual.** A side-by-side "Google Stitch vs Human" LP comparison being judged on looks alone — context for the argument, not a model to copy — `../assets/2034638793219694734__q__1.jpg`
**Voice.** "Product design doesn't compete with art. It sells."
**Source.** [@richardrx · 2026-03-19](https://x.com/richardrx/status/2034638793219694734)

## Converting pages are often ugly — design for performance, not applause
**Principle.** There's an invisible war between branding (looking good in the screenshot) and performance (conversion, retention, expansion). The page that puts money in the till is often visually aggressive, text-heavy, and far from the Apple aesthetic founders dream of.
**Apply when.** You're choosing between a page that wins design compliments and one built to convert.
**The move.** Engineer the converting pattern even if the artist in you cringes: (1) one obvious attention point — eyes go where they must; (2) a high-contrast CTA with redundancy; (3) a clear promise delivering easily-perceived value; (4) guarantee, social proof, and a free element to reduce risk aversion; (5) organic images by the second fold to back the offer and build trust.
**Evidence.** The analyzed page (quoted): 100 visits → 19 signups, a 19% conversion rate.
**Visual.** An "ugly-but-converts" waterproofing LP: urgency bar, high-contrast orange CTAs, a short above-the-fold form, stat row (12,500+ / 4.9★ / 20+ yrs / 100%), and a trust-badge strip (incl. lifetime warranty) — `../assets/2023777916673220817__q__1.jpg`
**Voice.** "Some LPs go after compliments, others go after conversion."
**Source.** [@richardrx · 2026-02-17](https://x.com/richardrx/status/2023777916673220817)

## Design the features page for skimming, not reading
**Principle.** Almost nobody reads your features page — they skim three bullets and hunt for a demo video. Design for that behavior (with the caveat that the more conscious, technical slice of your ICP *will* read the detail).
**Apply when.** You're packing a features page with dense prose expecting visitors to read it top to bottom.
**The move.** Front-load three crisp bullets and make a demo video easy to find; let the deep copy serve the minority of technical, high-awareness buyers who actually read it.
**Source.** [@richardrx · 2026-02-09](https://x.com/richardrx/status/2020815036168437814)

## No clicks out, plus brutal CTA contrast
**Principle.** For conversion you want little distraction and lots of redundancy. Any clickable element that leads off-page is lost conversion — no matter how prestigious the source.
**Apply when.** You're tempted to link out to a glowing NY Times piece or a top influencer's video, or your CTA blends into the interface.
**The move.** Kill outbound clicks entirely. Make the CTA generate strong contrast against the rest of the interface in position, size, and color — if it isn't easy to notice and click, it won't be clicked.
**Visual.** A wireframe showing the level of contrast a CTA button needs against the surrounding interface — `../assets/2019514730696565238__1.jpg`
**Source.** [@richardrx · 2026-02-05](https://x.com/richardrx/status/2019514730696565238)

## Debug ICP and awareness level before touching design
**Principle.** Conversion is context engineering — who arrives, with what pain, at what stage, needing what proof. Two invisible variables must be debugged before writing a line of code: the Who (ICP) and the When (awareness level). Visual design comes last.
**Apply when.** Your LP underperforms and you reach for button-color tweaks; or you define ICP by demographics.
**The move.** (1) Reject the demographic fallacy: geography/age/income is a bad proxy — King Charles and Ozzy Osbourne are demographic twins with opposite needs. Real ICP is *buying criteria* (trigger, pain, prior attempt, proof needed); persona is just biography, the spec for your user. (2) Map the visitor's Eugene Schwartz awareness level. Rule: headline speaks to the current stage; proof pushes them one stage forward. Selling "Solution" to the "Unaware" is proposing on a first date. Debug order: ICP wrong → awareness wrong → proof insufficient for the stage → only then touch visual design.

Awareness → angle / hero / proof:
- **Unaware** — symptom & identity / "Still doing X this way?" / simple diagnostic, checklist, benchmark
- **Problem-aware** — cost & urgency / "If you have X, you're losing Y" / numbers, before/after, calculation
- **Solution-aware** — trade-offs & selection / "3 ways to solve X — why the 3rd scales" / honest comparison, matrix
- **Product-aware** — differentiation & proof stack / "Why us, why now" / cases, demo, objections
- **Most aware** — final risk & friction / "Swap X for Y in Z days, no risk" / guarantees, onboarding, effort reduction

**Visual.** Schwartz's 5 awareness stages as a rising ramp (Unaware → Problem → Solution → Product → Most Aware) — `../assets/2011427153133351046__3.jpg`; plus the demographic-twins diagram (Charles vs Ozzy, identical on paper) — `../assets/2011427153133351046__2.jpg`
**Voice.** "There's no 'conversion rate' in a vacuum. There's contextualized conversion."
**Source.** [@richardrx · 2026-01-14](https://x.com/richardrx/status/2011427153133351046)

## The 2026 landing page checklist
**Principle.** An all-in-one checklist for a converting LP — @namyakhann's (Supafast) list, which Richard translated and endorsed in full: Hero (1 clear promise / 1 specific audience / 1 exact-action CTA / show-don't-explain visual / trust seal above the fold). Copy (headline <10 words, benefit before feature, customer language, one central transformation, scannable in 5s). Social proof (logos if you have names, metrics if you have traction, specific result testimonials, zero generic praise). Structure (Hero → Pain → Solution → Proof → CTA; max 3 feature sections; FAQ kills top 5 objections; CTA repeated 2–3x). Technical (<3s load, real mobile-first, single-scroll flow).
**Apply when.** Auditing or building any LP.
**The move.** Run the checklist top to bottom. Mantra: Clarity > creativity. Result > feature. Speed > polish. If it doesn't convert in 2026, it's not your traffic — it's your page.
**Source.** [@richardrx · 2026-01-02](https://x.com/richardrx/status/2007216871607771303)

## Click triggers: one line of risk-reducing microcopy next to the CTA
**Principle.** A single line of text reducing perceived risk can save conversion — in CRO these are "click triggers" (marketing calls it objection-breaking): "Lifetime guarantee," "Free shipping," "7 days free, no card." It's certainty placed on top of a known ICP doubt.
**Apply when.** Users hesitate right before the CTA.
**The move.** Find the real objections by talking to customers and reading complaint pages (ReclameAqui) and app-store comments; then test which click trigger performs best. No mystery, just work — and it works.
**Source.** [@richardrx · 2025-12-19](https://x.com/richardrx/status/2002076748112875558)

## Founder LP guide: platform doesn't matter, load time does; proof must outweigh the promise
**Principle.** Profits are more sensitive to conversions than to costs, and the landing page is often the first gate between a founder's product and its users. The platform matters less than speed, clarity, contrast, proof, and direct action.
**Apply when.** Building a first LP cheaply.
**The move.** Follow five rules: (1) use any platform, but deliver content fast and target an "A" on GTMetrix; (2) lead with a short pain or clear benefit, then make the promise tangible in the subhead; (3) create visual contrast with what the ICP sees daily; (4) ensure proof ≥ promise, moving from strong/shallow at the top to denser evidence below; (5) use direct CTAs tied to the outcome about every 1.5 sections.
**Voice.** "Nobody wants to know about your product's features — they want what it generates or the pain it kills. Not 6GB of space, 3,000 songs in your pocket."
**Source.** [@richardrx · 2025-11-10](https://x.com/richardrx/status/1987842649261261240)

## Match CTA microcopy to the funnel stage
**Principle.** Button text should change with the user's progress in the funnel — the verb matches the mental state at each stage. First interaction: "Descubra como funciona" ("See how it works"). Product page: "Quero esse produto" ("I want this product"). Checkout: "Finalizar minha compra" ("Complete my purchase"). Short (≤4 words), clear, directional. This discreet personalization raises perceived control, confidence, and conversion.
**Apply when.** One generic CTA label serves the whole journey.
**The move.** Audit every CTA against the stage it appears in; test stage-matched variants. Small adjustments, large results.
**Source.** [@richardrx · 2025-11-07](https://x.com/richardrx/status/1986836679953719632)

## Real humans outconvert models — banner blindness explains why
**Principle.** Highrise, the 37signals CRM, tested homepage variants with different human figures; real users and actual team developers converted best on average — above stock-photo models. (37signals later became Basecamp.) Likely explanation: banner blindness — we learn to ignore what looks like advertising and give attention to what's organic or unusual.
**Apply when.** Choosing imagery for LPs and proof sections.
**The move.** Prefer real users/team over polished models; user-generated reviews and simple real photos often beat studio shots. Chinese sites exploit this at scale with gamified UGC.
**Evidence.** The stock-model / team-developer comparison is the post's. 37signals' own writeup of the test ([Signal v. Noise, "Behind the scenes: A/B testing part 3"](https://signalvnoise.com/posts/2991-behind-the-scenes-ab-testing-part-3-final)) photographed only real Highrise customers — no stock models, no staff — and found the specific person barely mattered: the lift came from the person-photo layout beating the long-form page.
**Visual.** The Highrise homepage test side by side — the illustrated "original design" vs the "person design" fronted by a real customer's photo and quote, marked +102.5% — `../assets/1985681720104903142__1.jpg`
**Source.** [@richardrx · 2025-11-04](https://x.com/richardrx/status/1985681720104903142)
