# Cocoon Google Ads: Operating Manual

Brief for Claude (or any person) running Cocoon's monthly Google Ads review. Last updated Oct 15, 2026 (September review changes logged).

## How to work with Rachel
- Explain things very simply, like to a five-year-old. When she's right, say so plainly; don't repeat her point back in different words.
- Be direct, with no hedging. If you were wrong, say so.
- For anything she has to click through, give one step at a time.
- **Never make changes without her OK.** Analyze first, propose specific changes, then make the ones she approves.
- Read full context before stating facts, and use 2–3 months of data before judging anything small.

## Access
- Google Ads account **742-164-2243** (currency CAD), reached through the Windsor.ai connector `google_ads`. Use `get_data` to read and `execute_action` to make changes; run `list_actions` to see what's possible.
- Windsor can't edit Price assets, Merchant Center or Tag Manager. Give Rachel UI steps for those.
- Shopify connector: read orders, markets and prices. It has no access to payouts.
- Conversions are tracked by the Shopify **Google & YouTube app** ("Google Shopping App Purchase" is the Primary goal). GA4 purchase is Secondary as of mid-Sept 2026, so **conversion data before mid-Sept 2026 is inflated (double-counted)**.

## Business numbers
- Product: Balance (hormonal acne supplement with DIM + glutathione). New site: **cocoonsupplements.com** (moved from cocoonskincare.ca because of Health Canada claim limits; no redirect possible, so SEO starts from zero).
- Margin about 62%. Google 90-day average first order about CA$120. Lifetime value about CA$224 revenue, about CA$139 profit. Google customers reorder at least as much as others.
- Prices: Canada CA$68 for 1 month (CA$61.20 on subscription), CA$177.48 for 3 months. US US$50 for 1 month (US$45 on subscription), US$130.50 for 3 months. Free shipping over 70 in either currency.
- Ad spend ceiling: up to about CA$250/day across all Google markets, **only if it's making at least a little money (not losing)**. Leftover budget goes to Meta.

## Campaigns
### Canada: "Sales | Search | Clicks | June 2025" (id 22635751841)
- Bidding: **target CPA CA$84**, set at the campaign level. Leave the ad group target blank, because it overrides the campaign. Chosen on purpose for lifetime-value profit; Rachel accepts waiting months to earn it back.
- Budget **CA$50/day**.
- Keywords: phrase "acne supplements" plus the existing set. Broad "acne supplements" and "heal hormonal acne" are paused. Broad "dim supplement" is kept on on purpose: about CA$70 per sale, the best keyword, an exception to the no-broad rule.
- **Quebec excluded** (site isn't in French). Bid adjustments do nothing under target CPA; only exclusions work.
- Negatives: competitors, iHerb, topicals, misspellings, unrelated ingredients. **Never block "glutathione" or "DIM"; they're ingredients.**
- Price asset: must show CAD prices.

### US: "US Sales | Search | Max CPC | Oct 2026" (id 24353842296), launched Oct 15, 2026
- Bidding: Maximize Clicks, **per-click cap CA$4.00**, **CA$40/day**, US only, English.
- 5 phrase keywords: dim supplement, acne supplements, hormonal acne supplement, supplements for hormonal acne, estrogen balance supplement. About 69 negatives.
- Ad lands on cocoonsupplements.com/products/balance.
- Copy rules: never say "treat". "Acne" is fine. Never say "Canadian-made".
- **Kill rule:** about CA$500 spent with fewer than 2 sales means pause and rethink.
- **Graduation rule:** at about 15 US sales, switch to target CPA.
- The old "US Sales | Search | Clicks | May 2026" campaign stays paused.

### Rejected on purpose
Performance Max, Display Expansion, broad match, Shopping campaign reactivation, budget optimizer, dynamic images, Customer Match, and adding Add-to-cart/Begin-checkout as goals.

## Monthly review (end of each month)
1. **Results first.** For each campaign, compare cost per purchase, purchases, spend and conversion rate with last month and with the target.
   - Canada: compare actual cost per purchase with CA$84. Google usually lands about 1.5× above the target, so judge the real number.
   - US: check sales count against the kill and graduation rules.
2. **Search terms report.** Add negatives for irrelevant searches. Add searches that convert repeatedly as new phrase keywords.
3. **Keywords.** Pause or adjust only the ones with 2–3 months of poor data. Remember that match types include plurals and close variants.
4. **Bidding and budget (only if it makes sense):**
   - Raise the budget only if cost per purchase is at or under target. New budget = current ÷ (1 − Search lost IS (budget)).
   - Revisit the target CPA if the average order or reorder behaviour has changed.
   - US (per-click): adjust the per-click cap, budget and locations. Cost per customer ≈ cost per click ÷ conversion rate (about 3%).
5. **Every 2–3 months:** replace any headlines rated "Low".
6. **Limit:** one or two big changes a month. Don't change target, budget and keywords all at once.
7. **Log** every change below, with the date and reason.

## Change log
- Sept 16, 2026: Canada target CPA $42 → $80. GA4 purchase set to Secondary.
- Oct 14, 2026: Canada target $84, budget $50/day. Paused broad "acne supplements" and "heal hormonal acne". Added phrase "acne supplements". Added about 48 negatives. Excluded Quebec.
- Oct 15, 2026: Launched US Max CPC campaign. Canada price asset updated. Merchant Center now syncs Canada + US. Decided to switch Shopify payouts back to CAD.
- Oct 15, 2026: Canada: added 22 phrase-match negatives from the September review (other brands, local salon, diet/recipe questions, myo inositol, thistle oil, vitamin B5, iHerb spelling, one birth-control question). Why: about CA$300 spent since Aug with 0 sales. No change to target (CA$84), budget or bidding: cost per sale is CA$131 since Sept 16, above target, and the target changed Oct 14, so wait for a clean month. Exception noted: broad "dim supplement" stays on because it makes sales at about CA$70 each.
- Oct 15, 2026: Account-level Final URL suffix set to `utm_source=google&utm_medium=cpc&utm_campaign={campaignid}` (auto-tagging was already on). Why: Shopify showed ad clicks as free "Google, SEO" visits, so Google's sales couldn't be matched to real orders. From now on, ad orders show utm medium "cpc" in Shopify's customer journey. Note: ~54 of September's ~86 orders were subscription renewals, which never have a source; compare Google's sales only with website orders.

## Open items
- Check that Merchant Center shows shopify_US listings in USD with no price-mismatch warnings.
- Canada shipping zone set to CAD (CA$70 free shipping threshold).
- Add a USD Price asset to the US campaign.
- Check headlines rated "Low" (due; not done in September review).
- Check what the Canada daily budget is set to: it was capped Oct 7 to 13 (lost to budget 20 to 86%).
- Switch everything still on cocoonskincare.ca to cocoonsupplements.com (the official site for both Canada and US): ad final URLs and sitelinks, GA4 property, Search Console, Merchant Center, Windsor connections.
- Later: French site and a Quebec campaign; Meta relaunch; SEO rebuild for the new domain.
