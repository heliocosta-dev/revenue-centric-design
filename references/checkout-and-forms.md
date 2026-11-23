# Checkout & Forms (Conversion-Completion Layer)

> Curated, distilled wisdom from @richardrx ("Richard — Design for startups"), translated from Portuguese. Each entry is a reusable principle linked to its source post. The checkout is where ~70% of drops happen — it's the highest-leverage page most founders treat as an afterthought.

## Mark both required and optional fields
**Principle.** When only one kind of field is marked, people have to guess the other, guess wrong, hit a validation error — and the field turns red on the very screen where they were about to pay you.
**Apply when.** A checkout or signup form marks only required fields with an asterisk, or only optional ones — especially Brazilian SaaS checkouts that pull invoice (nota fiscal) data into the form: CPF or CNPJ (personal or company tax ID), full address, phone, and a municipal registration number the customer may not know they have.
**The move.** Asterisk on required fields and "(optional)" written out on optional ones — a fix that fits in an afternoon. Remember that a fiscal form like this was designed by someone who already knows the answer to every field.
**Evidence.** In Baymard's checkout usability testing, marking only optional fields led 32% of participants to leave at least one required field blank, and Baymard recommends marking both. Most large e-commerce sites still don't: in its 2021 benchmark only 14% marked both.
**Source.** [@richardrx · 2026-11-05](https://x.com/richardrx/status/2118384265180135935)

## Open the calendar right after the demo form, not a thank-you page
**Principle.** Most leads who request a demo and don't book on the spot never book. At the moment of the click the lead has their calendar open and their intent at its peak; "Thanks! A specialist will contact you soon" sends them away, and the SDR's WhatsApp the next day turns into three days of "how about Thursday?"
**Apply when.** B2B demo requests end on a thank-you page and wait for SDR outreach, or scheduling needs a second form.
**The move.** Show scheduling immediately after the form, with no second form. Test it yourself: fill in your own demo form and time how long it takes to have a slot on the calendar — if the answer is "depends on when the SDR calls," your thank-you page may be costing more than half your meetings. Richard tested this on RepareCar before posting.
**Evidence.** Chili Piper's look at almost 4 million B2B demo forms in 2024: when the calendar opens right after the form, 66.7% of qualified leads leave with a meeting booked, vs a ~30% market average when scheduling happens later; the report also cites a company that lifted conversion 50% just by removing a second scheduling form. The ~30% average is the report's own, unsourced figure, and Richard flags that Chili Piper sells scheduling software, so the data is biased.
**Source.** [@richardrx · 2026-10-21](https://x.com/richardrx/status/2112982264585871825)

## Don't end signup at "check your email"
**Principle.** A confirm-your-email wall filters the hurried more than the bad lead. The user signed up between two meetings, the email landed in Gmail's Promotions tab, and their curiosity ran out before they found it. Most teams never chose this: the auth provider shipped with confirmation on by default, and whoever tests their own signup knows where to look for the email.
**Apply when.** Signup ends on a "Verify your email" screen.
**The move.** Validate the address silently at signup — a service checks the mailbox exists without sending anything. Good addresses go straight into the product with a request to confirm, and only sensitive actions stay locked until they do; doubtful addresses keep the old flow. Then pull how many accounts created last month never confirmed: some of them had already decided to try the product, and you paid to bring them.
**Evidence.** Richard cites the founder of ROSS Intelligence (a Y Combinator startup), who measured that users who didn't confirm at signup practically never did — under 1% verified after the second or third reminder. After the switch, the invalid-email rate stayed at the same 10% as before, despite the team's fear of fake accounts.
**Source.** [@richardrx · 2026-10-16](https://x.com/richardrx/status/2111068431105638463)

## Offer the payment method your buyer actually uses — not just the card
**Principle.** Card-only recurring billing loses buyers who were ready to pay. In Brazil, Pix (the Central Bank's instant-payment system) has overtaken the credit card in e-commerce, and in small-business B2B the person who wants the product often isn't the one holding the company card: the trial ends, the screen asks for a card, and the lead becomes "I'll check with my partner" — logged as a cold lead in the CRM, never as a payment problem.
**Apply when.** Your SaaS charges recurring plans by card only — because it's what the gateway docs show first and "Pix doesn't work for subscriptions" — especially when selling B2B to SMBs.
**The move.** Add at least one relevant local method next to the card. Pix now works for recurring billing: the Central Bank's Pix Automático has existed since June 2025. In B2B, also offer boleto (bank slip) — bad in B2C, but sensible when the user generates it and forwards it to HR, IT or purchasing, a point Richard takes up from a reply by @marcoscosta — and always include an extra billing-email field for the same reason. To diagnose, pull last month's trials that reached the payment screen and didn't finish, and ask five of them why they stopped; if the answer mentions "card" or "partner," the leak is in the checkout, not the product.
**Evidence.** Pix took 42% of Brazilian e-commerce in 2025 vs 41% for credit cards (PCMI data analyzed by EBANX). Stripe ran a controlled experiment across 50+ payment methods: showing at least one relevant method besides cards raised conversion 7.4% and revenue 12% on average; iDEAL alone lifted conversion 39% in the Netherlands, BLIK 46% in Poland.
**Source.** [@richardrx · 2026-10-16](https://x.com/richardrx/status/2111042272380809347) and [@richardrx · 2026-10-15](https://x.com/richardrx/status/2110747740258902394)

## Friction kills conversion — field count, input type, and perceived risk all compound
**Principle.** More fields = lower conversion, but the *type* of input matters too: text fields usually generate less impact, while dropdowns and textareas hurt more. Phone number drops conversion; any data that raises perceived risk or invasiveness does the same. And perceived effort ≠ real effort — 5 steps with 2 fields per screen can beat 2 screens with 7 fields each.
**Apply when.** Optimizing lead forms, pre-checkout, signup.
**The move.** Count perceived effort, not steps. A screen full of text, warnings, secondary info raises cognitive load even without interaction. Ask: how much effort can I remove without destroying the business value of that data? Sometimes the fix is between things — more breathing room, less noise, clearer hierarchy. Your form should look like a corridor, not an interrogation room.
**Evidence.** HubSpot study across 40,000+ landing pages: 3-field forms convert above 25%; adding fields trends conversion down. Phone field drops conversion to ~13.5% vs 19% without.
**Source.** [@richardrx · 2026-08-12](https://x.com/richardrx/status/2087502085151424711)

## Microcopy at the point of fraud risk beats friction everywhere else
**Principle.** Design must protect the user from the real environment the product lives in — especially in low-trust economies. One line of microcopy in the right place prevents scams that cost more than the friction of adding it.
**Apply when.** Users are getting scammed through a flow your product enables (delivery PIN sharing, social engineering).
**The move.** Add microcopy at the exact risk moment: "Never share your number outside the app. The store and courier already have your contact via chat." Transparency is the antidote in low-trust verticals (auto repair, delivery).
**Voice.** "Scam costs more than friction."
**Source.** [@richardrx · 2026-06-29](https://x.com/richardrx/status/2071546806987538924)

## You lose money on the boring screens
**Principle.** Registration forms are where you lose users one input at a time, creating holes in your bucket and wasting CAC — while founders polish the hero. The idea is to remove cognitive load until the flow is so smooth the user doesn't notice it.
**Apply when.** Conversion leaks between signup and first value; form-heavy onboarding.
**The move.** (1) Ask less — only what's relevant at that specific step; more questions = less conversion. (2) Avoid typing when possible (swipe/tap costs less than entering data, especially mobile). (3) Explain when asking for sensitive data (documents) — increases completion. (4) Never block paste (card numbers, CEP get copied, not memorized). (5) Help users not mistype passwords (optional visibility toggle). (6) Avoid dropdowns — they hide the answers from the user; with fewer than ~6 options, use a button group instead.
**Voice.** "You lose money on the boring screens."
**Source.** [@richardrx · 2025-12-23](https://x.com/richardrx/status/2003495704849760387)

## Checkout is where ~70% of drops happen — every extra input is less conversion
**Principle.** At checkout, less is more. Each extra input is less conversion; ask for the minimum possible. Any new negative surprise is a reason to cancel — expensive shipping, paid shipping at all, service fee, packaging fee — embed every extra charge into the product price, never as a hidden extra.
**Apply when.** Auditing or building any checkout, signup-to-paid flow, or high-stakes form.
**The move.** (1) Minimum fields only. (2) No surprise fees — bake costs into the price. (3) Show security signals (even a lock icon with "Compra segura" — "Secure purchase" — lifts conversion). (4) Show an extra discount in the cart if you have one (anchoring works for you there). (5) Display the CNPJ (Brazilian company-registration number) — a real company converts more. (6) Show product photos even for digital products. (7) Split what you can to reduce barriers and cognitive load. (8) Use mobile-appropriate inputs (numeric keyboard for phone). (9) Yes, social proof in checkout works. (10) Test — different ICPs perceive risk differently.
**Visual.** Richard's own checkout applying the list at once: lock icon + "Site Seguro" in the header, four fields only (name, surname, e-mail, +55 phone with a numeric mask), a product thumbnail in the order summary, "Desconto 5% PIX" and free shipping on the receipt, a "Compre com confiança" trust list (100% money-back, support 7 days a week, 10,000+ sales) with a named testimonial, and the CNPJ in the footer — `../assets/1999584679247134761__1.jpg`
**Voice.** "I worked at PayPal literally designing checkouts for the biggest e-commerces and brands in Brazil. Hundreds of them."
**Source.** [@richardrx · 2025-12-12](https://x.com/richardrx/status/1999584679247134761)

## 97% of visitors buy nothing — the leaks are known and fixable
**Principle.** Cart abandonment reasons are mapped and mostly design-fixable: late extra costs (49%), forced account creation (24%), slow delivery (19%), complicated checkout (18%), distrust of the site (17%), unclear price (17%), site errors (12%), bad return policy (11%).
**Apply when.** Diagnosing why traffic isn't converting to purchase.
**The move.** Treat this as a checklist: eliminate late costs, allow guest checkout, show delivery time early, simplify checkout, add trust signals, show total price upfront, test for errors, publish return policy. Amazon shows international products with "no additional costs after" — do the same.
**Voice.** "You can frame this as winning new conversions, or as better capturing what you're losing today."
**Source.** [@richardrx · 2025-12-09](https://x.com/richardrx/status/1998432350842016222)
