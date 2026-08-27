# Store Audit

Impact Conversion Resources. How to audit a Shopify store's offer structure before recommending anything.

## What to fetch

Fetch these live pages (adjust paths to the store's actual structure):

1. Homepage
2. The best-selling product page (ask which if unclear)
3. The main collection page
4. `/cart` if reachable
5. Any bundle, kit, or subscription page they have

Ask the owner for the bestseller's exact URL rather than guessing slugs. If a page won't fetch, say so. And know the silent failure: modern storefronts render buy boxes in JavaScript that a text fetch never sees, so a "successful" fetch can still be missing the part that matters. When buy-box details are invisible, ask the owner three named questions (what options the buy box shows, which one is pre-selected, what if anything appears after payment) or have them send a screenshot. Never audit from imagination.

## The audit checklist

Work through every item. For each: what you observed, and whether it's a gap.

### Product and pricing

- What do they sell, in one sentence a stranger would understand?
- Price points: cheapest, flagship, most expensive
- Is the frontend under $50, $50 to $150, or over $150? (This decides upsell page format later.)
- Consumable, durable, or mixed catalogue?
- Single-product brand or multi-product?

### Frontend offer structure

- Does the buy box offer quantity options (1 / 2 / 3 or 1 / 3 / 6)? Which option is pre-selected?
- Any bundles? Are they anchored against full retail value?
- Any subscription option? Is it the default selection or an afterthought?
- Is there a free-shipping threshold, and is it visible?
- What risk reversal exists (guarantee, returns), and does it scale with the size of the commitment?

### Existing AOV activity

- Cart cross-sells or drawer upsells? (Note: these can distract from checkout. Record what exists.)
- Any post-purchase offer today? Ask the owner directly; if unsure, they can place a small test order themselves and see what fires after payment.
- A thank-you page doing any selling at all?

### Perceived value signals

- Does the product page sell one problem solved, or a complete route to the outcome?
- Is the desire behind the product named (health, status, belonging, attractiveness, safety), or only features?
- Does design and photography read premium enough to support higher prices?
- Social proof: volume, recency, specificity

### Signals for the upsell chain (feed these to Phase 4)

- Products that naturally pair with the bestseller
- Consumables hiding in the catalogue that could anchor a subscription
- The problem their product creates or reveals once it works (the owner interview digs here too)
- Anything customers must do or buy elsewhere to get full value from the product

## Output format

Present as a short report:

1. **What this store is** (two sentences)
2. **Offer structure today** (buy box, bundles, subscription, post-purchase: present or absent)
3. **The gaps, ranked** (biggest missing AOV lever first)
4. **Raw material spotted** (products and problems that could become upsells)
5. **What I need from you** (anything unfetchable or ambiguous)

Keep it under a page. The audit is a foundation, not the deliverable.
