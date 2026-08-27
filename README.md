# The AOV Engine

**A Claude skill that designs your Shopify store's post-purchase upsell funnel from your real data, and writes the pages.**

Built by [Impact Conversion](https://impactconversion.com), a CRO consultancy for D2C brands. It runs a five-phase engagement in your own AI assistant:

1. **Store audit**: connects to your Shopify (or walks you through connecting it) and audits your live storefront's offer structure
2. **Owner interview**: asks only what it couldn't pull itself
3. **Review mining**: finds your customers' exact words in your reviews, competitor reviews, and forums, verbatim only
4. **Offer architecture**: a problem map with evidence, your frontend structure, a 2 to 4 offer post-purchase chain with pricing and downsells, economics computed on your numbers
5. **The pages**: written upsell page copy for every approved offer, plus an implementation checklist

Its rules: no invented numbers, no invented quotes, no invented credentials. Everything it recommends traces to your store, your answers, or your customers' words.

**This skill is the companion to the Free Money playbook**, the full guide to the system it runs: [assets.impactconversion.com/free-money-playbook](https://assets.impactconversion.com/free-money-playbook/)

## Install

### Claude Code

```bash
git clone https://github.com/Jonomtla/aov-engine ~/.claude/skills/aov-engine
```

Then start a session and type `/aov-engine`. If your Claude Code has a Shopify integration connected, or you're willing to create a read-only API token, the Engine pulls your store numbers itself.

### claude.ai with Skills enabled

Download this repo as a zip (green Code button), then Settings, Capabilities, Skills, upload. Start a chat: "Run the AOV Engine on my store".

### Any chat assistant, zero setup

No skills support, or on ChatGPT? Grab the single-file version from the [playbook page](https://assets.impactconversion.com/free-money-playbook/): attach it to a new chat and say "Read this file and run the AOV Engine on my store."

## What to have ready

Your store URL, and 45 to 60 minutes. Rough AOV, order volume, and product margins help, but if your Shopify is connected it pulls those itself. The review-mining phase is the slow part and the most valuable.

## Who made this

Impact Conversion builds and A/B tests conversion systems for D2C brands: offers, product pages, and funnels like the one this skill designs. If you'd rather have the whole thing built, tested, and iterated for you: [impactconversion.com](https://impactconversion.com)
