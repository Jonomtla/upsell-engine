# Offer Architecture

Impact Conversion Resources. How to design the frontend structure and the post-purchase chain. The premise: AOV and conversion rate are not directly coupled. Most AOV levers raise perceived value rather than cut price, so they leave conversion alone or lift it. Buying happens when perceived value exceeds price; the job is widening that gap upward.

## Part A: Four perceived-value levers (apply everywhere)

1. **Solve more problems.** One product solving one problem is worth less than a system delivering the whole outcome. Bundle complements into the complete route.
2. **Tie the offer to a deep human desire.** Health, attractiveness, status, belonging, safety. Name the desire the mined language points at, not just the feature.
3. **Be uncomparable.** Positioning as a better or cheaper version of a known brand invites a price war a smaller brand loses. Own an angle nobody else pushes.
4. **Look premium.** Design and packaging move willingness to pay on their own.

## Part B: Frontend structure (pick exactly one)

- **Quantity tiers** when people naturally buy more than one or gift it. Shapes: 1 / 2 / 3 with growing discounts and gifts, or 1 / 3 / 6 for consumables (full price, then about 15% off, then about 35% off).
- **Bundle** when the product lives inside a routine or system. Anchor the bundle against full retail value. Components must map to desires found in mining, so the stack reads as the complete path, not a random add-on.
- **Subscription** when the product is consumed and rebought. A subscription is a quantity tier on a time axis.

Two rules across all three: pre-select the highest-value option, never the cheapest. And scale the risk reversal with the commitment (a 90-day plan deserves a 90-day guarantee).

Always compute unit economics first. Discounting a $51 product with $20 COGS down to $36 leaves $16 of breakeven headroom and demands brutal ad efficiency. Value-led structures beat discounts on every axis. Show this arithmetic with the store's real numbers.

## Part C: The four post-purchase angles

Post-purchase offers add order value with no effect on conversion or CPA, because payment already happened. Offers must be incentive-based: they complement what was just bought. Four angles cover every winning offer:

1. **More of the same**, usually discounted. Skip when it makes no sense.
2. **Faster results.** The thing that gets them to the outcome quicker.
3. **Longer-term results.** The best subscription angle: keep the result rather than lose it.
4. **Results to the next problem.** The problem that appears after the product works. Most of the money lives here, and the review-mining next-problem shortlist is where you find it.

## Part D: The problem map

Do not brainstorm products. Put the customer in the exact moment of product use and list every problem present in that moment, using evidence. Two evidence grades count: mined customer quotes (strongest), and owner-reported patterns from the interview, labelled "owner-reported". A problem supported by both is a priority slot. If the evidence is thin for a problem, say so rather than padding the map. The frontend solves problem one; problems two, three and four become the offer chain.

## Part E: Sequence and pricing

**Sequence:** upsell; downsell on decline; upsell again; downsell again; ending only at the order confirmation page. On acceptance show the next upsell; only downsell after a decline. Two to four offers is the normal range. Put a subscription in the chain whenever something in the catalogue is genuinely consumed and rebought. When nothing is, state plainly that no subscription slot exists and why; never invent an "accessory club" to fill the slot.

**Pricing (decision procedure, in order):**
1. More-of-the-same, single extra unit: below the first purchase, via a discount with a stated reason.
2. More-of-the-same, multiples: total above the frontend price, discounted per unit; downsell to one.
3. Different product: at or above the price of the item just bought where the product supports it. Price sensitivity is at its lowest right after purchase; don't get shy.
4. Downsells: roughly half the declined upsell, or clearly lower.
- Do not assume deeper discounts convert better; published testing has shown 15% off beating 20% off. Discount framing matters as much as depth ("10% off" has beaten "$3 off" by a wide margin at similar value). Treat both as things to test, not laws.

## Part F: Benchmarks and the metric that matters

Take rates from well-run funnels: offer one 20-30%, offer two 10-20%, offer three 10-15%. Hitting those captures roughly 80% of the available money, as an industry rule of thumb. Present these as industry reference points; public averages have moved over the years, so they diagnose rather than promise.

The benchmarks printed in this system are approved reference points: using them in a clearly labelled scenario is not invention and does not violate the no-invented-numbers rule. Invention means a number with no source at all presented as fact.

The take rate is not the goal. Published testing has shown a lower-converting multi-unit offer earning far more revenue per visitor than the higher-converting single-unit version. Judge every offer on revenue per eligible order, or contribution profit per order where margins are known. Say this explicitly in the decision document.

## Part G: Page format follows frontend price

"Frontend price" means the price of the item in the order that triggers the offer. Designing before knowing which item triggers? Use the flagship product's price. Never use the store's AOV; a multi-item cart doesn't change how much persuasion one upsell needs. And yes, the format follows what they just spent, not what the offer costs: a $29 offer after a $100 purchase still gets the letter, because the persuasion budget is set by how much money has already left their pocket.

- Under $50: one section. Product, discount, scarcity, urgency. No sales letter.
- $50 to $150: text sales letter.
- Over $150: video sales letter script. More money already spent means more persuasion needed.

## Part H: Testing rules

**The leave-it-alone rule:** after any launch or change, no further changes until at least 800 orders have passed through the funnel. Referenced by name elsewhere in this system; this is its definition.

Test, in order of leverage: the offer itself, framing and copy, price, sequence. Decide on order volume, not elapsed time: one decision every 800 to 2,000 orders through the funnel, more when volume allows. Small effects need enormous samples (a one-point lift on a 10% take rate needs roughly 29,500 orders to prove), so test big contrasts first: different product, different quantity, same item versus complement. Never call a winner from a three-day dashboard.

## The decision document

Phase 4's output. Contains: the problem map with evidence, the frontend recommendation with reasoning, the offer chain (angle, product, price, downsell per slot, subscription placement), the economics scenario computed with real numbers and visible arithmetic, and the testing plan. Every recommendation traces to something observed in the audit, said in the interview, or mined from customers. If a recommendation has no trace, cut it.
