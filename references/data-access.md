# Data Access

Impact Conversion Resources. Get real store numbers before asking the owner a single question a computer could answer. Work down this ladder and stop at the first rung that works. Tell the owner which rung you're on.

## Rung 1: Shopify connected

Check your available tools for a Shopify connection (an MCP server, connector, or integration with Shopify in the name).

**If you don't find one, offer to get it connected before dropping down the ladder.** Say something like: "I don't see a Shopify connection in this chat. If you connect one, I can pull your products, orders, and AOV myself instead of asking you for numbers. Want to set that up first? It takes about two minutes." Then point them to the right place for their platform: on claude.ai it's Settings, then Connectors, search Shopify; in a desktop or coding environment it's the integrations or MCP settings, adding the Shopify connector and signing into their store. Once connected, they may need to start a fresh message for the tools to appear. If they'd rather not, drop to the next rung without friction.

If a connection is present, pull:

- Product list with prices and variants (SKU count comes free)
- Order count for the last 30 and 90 days
- Total sales for the same windows, then compute AOV = sales / orders
- Cost per item where the merchant has filled it in (lives on the inventory item)
- Any subscription or selling-plan products

Show the owner what you pulled and the date ranges, and ask them to sanity-check the AOV figure. Numbers you pull still get confirmed, never silently trusted.

## Rung 2: You can browse with the owner

If you're running somewhere you can drive or view a browser alongside the user (a browser extension or screen access), ask them to log into their Shopify admin, then navigate together:

- **Analytics overview**: average order value, online store conversion rate, total orders. Set the date range to the last 30 days.
- **Products list**: product count; open the flagship product for price and the cost-per-item field.
- **Orders list**: spot-check a few real orders for what people actually buy together. Multi-item orders are upsell evidence.

Read the numbers from the screen; don't ask the owner to retype what you can both see.

## Rung 3: Coding environment, no connection

If you're in a coding environment (CLI or code interpreter with network access), offer the API route. The owner creates a private access token: Shopify admin, Settings, then Apps and sales channels, then Develop apps, then Create an app, with scopes `read_products` and `read_orders`. Then:

```
curl -s -H "X-Shopify-Access-Token: TOKEN" \
  "https://STORE.myshopify.com/admin/api/2025-01/orders/count.json?status=any&created_at_min=DATE_30_DAYS_AGO"

curl -s -H "X-Shopify-Access-Token: TOKEN" \
  "https://STORE.myshopify.com/admin/api/2025-01/products.json?limit=250"
```

Replace DATE_30_DAYS_AGO with the actual ISO date 30 days before today.

Warn them the token is a live credential: they paste it into their own terminal or environment variable, they revoke the app when done, and they never paste it into a chat they don't control.

Only offer this rung to owners comfortable with it. If they hesitate, drop to rung 4 without making it a thing.

## Rung 4: Guided ask

No connection, no browser, no API. Ask for the numbers, but tell them exactly where each one lives so it takes two minutes:

| Number | Where it lives in Shopify admin |
|---|---|
| AOV | Analytics overview, "Average order value", date range last 30 days |
| Conversion rate | Analytics overview, "Online store conversion rate" |
| Orders per month | Analytics overview, "Total orders", last 30 days |
| Product / SKU count | Products list, count at the top |
| COGS | Products, open the product, "Cost per item" field. If blank, it's on their supplier invoice; a rough number is fine |

Whatever rung you land on, the ladder only covers numbers. You still fetch and audit the live storefront yourself per the Store Audit section of this system; never audit from the owner's description of their own site.

## The opportunity-scan pull (rung 1 and rung 3 only)

When you have live store data, also pull what the Phase 6 opportunity scan needs, in the same session:

- Total sales per product for the last 90 days
- Sessions or page views per product page for the same window, if the connection or its analytics reports expose them
- From those, revenue per session for each significant product

Traffic per product is the piece most connections lack. If you can't get it, note that the scan will be skipped and move on; never estimate traffic. If the owner is on rung 2 (browsing together), the same numbers live in Shopify admin under Analytics reports (sales by product, sessions by landing page); grab them while you're both in there.

## COGS, on any rung

Cost per item is the number merchants most often haven't recorded. Ask for it per product that matters: the flagship frontend product and each candidate upsell product. A rough figure is fine; say so, since people freeze when asked for precision they don't have.

## Support emails and DMs

The richest unmined source they own. Offer two paths: easy mode, they answer from memory ("what do customers keep asking for, complaining about, or asking whether it works with"); thorough mode, they export or paste a batch of recent support emails and you mine them like reviews (same rules as the Review Mining section of this system, verbatim quotes only). Take whichever they'll actually do. Memory beats an export that never happens.
