# The Build Guide

Impact Conversion Resources. How to take the approved chain and the written pages live in a real app. This is where most funnels die: designed, written, never built. Your job is a build plan so specific the owner can execute it this afternoon.

## Rule zero: describe outcomes, not clicks

App interfaces change monthly and vary by plan. Never invent menu paths or button names. Describe what each screen must end up containing, tell the owner to follow the app's own setup flow to get there, and offer to fetch the app's current help docs if you can browse. A wrong click-path destroys trust; an outcome description never does.

## Step 1: Pick the app by fit, not hype

All post-purchase apps live inside the same Shopify ceiling: one post-purchase app active per store, three ACCEPTED offers per checkout (declines don't count), pages assembled from Shopify-managed blocks with no custom code, and express-wallet, buy-now-pay-later and gift-card orders never see offers at all.

Within that ceiling, fit differs:

| App | Funnel shape | Strengths | Watch out |
|---|---|---|---|
| Zipify OneClickUpsell | 2 upsells + 1 downsell per funnel; unlimited funnels | Most flexible page blocks; genuine inline video block; strong split testing | The 2+1 shape means a 4-slot design must be trimmed (Step 2) |
| AfterSell | Multi-step chains, e.g. upsell 1 → upsell 2 → downsell 1 → downsell 2 | Clean sequenced funnels with real declined-branches | Video opens in a new tab, so don't design video-led offers on it |
| ReConvert (Upsell.com) | Chains across post-purchase pages plus the thank-you page | Best accept/decline conditional branching; cheapest way in | Widget-style pages, least long-form; pricing tiers change often, check the live listing |

Pick with the owner based on: which frontend price band their offers sit in (video tier points at Zipify), how many slots the approved chain needs, and budget. State the choice and the reason in the build plan.

## Step 2: Fit the chain to the app's slots

The approved chain from Phase 4 may not fit the chosen app's shape. Trim by expected money, never by order in the document:

1. Offer one and its downsell are untouchable; they carry most of the revenue.
2. If a slot must go, cut the LAST upsell first, then its downsell.
3. Never cut the subscription slot if one exists; move it earlier instead.
4. Remember only three acceptances can happen per checkout anyway; a fourth offer only ever shows when earlier ones were declined.

Show the owner the fitted chain next to the original so the trim is a decision, not a surprise.

## Step 3: Translate the pages into blocks

Each written page maps onto managed blocks. Give the owner a block-by-block assembly list per page, in order. The standard mapping:

- "Please read this whole page carefully" line → first text block, small
- Authority open / reaffirm section → heading block + text block (+ founder image block if they have a real photo)
- Why-this-offer-exists / why-they-need-it → text block
- Benefits and mechanism → text block or two short ones; product image block between them
- Video tier → video block at top (inline video, captions on), offer visible below it without scrolling on mobile
- Offer specifics and price → the app's buy box / offer block; disclose any recurring price at full size here
- The decline link → the app's built-in "no thanks", kept visible; never hidden or shrunk

Long paragraphs from the written page get split across blocks rather than compressed; cut nothing for the sake of the tool.

## Step 4: Triggers

Set each funnel to trigger on the specific frontend product it was designed for, starting with the bestseller. A generic all-orders funnel is the fallback only after product-specific funnels exist. If the app supports excluding orders that already contain the upsell product, turn that on; offering someone what they just bought (outside a deliberate more-of-the-same play) reads as broken.

## Step 5: Measurement setup

Before launch, agree where the numbers will be read and write it into the plan:

- **Take rate per offer, measured against eligible orders** (the app's own dashboard usually reports offer views; views are the eligible base, since wallet and BNPL orders never see the page).
- **Revenue per eligible order**, the real scoreboard, per Part F of the offer architecture.
- **The leave-it-alone rule**: no changes until 800 orders have passed through. Have the owner write the current order count somewhere visible.
- Refund rate watched as a guardrail, expected to not move.

## The build plan deliverable

One page: chosen app and why; the fitted chain (with any trims shown); per-page block assembly lists; trigger settings; measurement plan with the 800-order line; and a first-test note (the highest-leverage contrast from the Phase 4 testing plan, to run only after the leave-it-alone window). End it with: "Build time: about an afternoon. The only step that can't be done today is waiting."
