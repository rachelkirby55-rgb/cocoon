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
- Enhanced conversions: already enabled, managed through the Google tag (checked Oct 15, 2026).
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
- Price asset: must show CAD prices (its own campaign-level asset: from CA$53.24/mo subscription, CA$68.00, CA$177.48).
- **Watch rule (Rachel OK, Oct 26, 2026):** count from the Oct 14 target change. Once Canada has spent CA$600 or more, if cost per sale is over ~CA$126 (1.5x the CA$84 target, under the CA$139 lifetime profit), the weekly check proposes a fix (lower budget or pause). Rachel approves any change first. Cost per sale so far: CA$456 and 2 sales (~CA$228) as of Oct 25.

### US: "US Sales | Search | Max CPC | Oct 2026" (id 24353842296), launched Oct 15, 2026
- Bidding: Maximize Clicks, **per-click cap CA$4.00**, **CA$40/day**, US only, English.
- 5 phrase keywords: dim supplement, acne supplements, hormonal acne supplement, supplements for hormonal acne, estrogen balance supplement. About 69 negatives.
- Ad lands on cocoonsupplements.com/products/balance.
- Price asset: its own campaign-level USD asset (from US$39.15/mo subscription, US$50.00, US$130.50). Never share one price asset between Canada and US: editing a shared asset changes it in both.
- Copy rules: never say "treat". "Acne" is fine. Never say "Canadian-made" **in US ads only**: US shoppers don't care, and it could wrongly suggest duties. In Canada ads "Canadian-Made" is fine and stays.
- **Kill rule:** about CA$500 spent with fewer than 2 sales means pause and rethink.
- **Graduation rule:** at about 15 US sales, switch to target CPA.
- The old "US Sales | Search | Clicks | May 2026" campaign stays paused.

### Rejected on purpose
Performance Max, Display Expansion, broad match, Shopping campaign reactivation, budget optimizer, dynamic images, Customer Match, and adding Add-to-cart/Begin-checkout as goals.
- Shopping evidence: "Sales | Shopping | Clicks | Nov 2025" (Nov 2025 to Feb 2026) spent CA$2,040 for ~31 sales = ~CA$66 per sale, vs Search CA$2,819 for ~74 sales = ~CA$38 over the same months. Both double-counted, so real numbers are roughly double, but Shopping cost ~1.7× Search per sale. Revisit only if Search runs out of room.
- Performance Max: revisit only once the account gets 30+ real sales a month.

## Monthly review (end of each month)
1. **Results first.** For each campaign, compare cost per purchase, purchases, spend and conversion rate with last month and with the target.
   - Canada: compare actual cost per purchase with CA$84. Google usually lands about 1.5× above the target, so judge the real number.
   - US: check sales count against the kill and graduation rules.
2. **Search terms report.** Add negatives for irrelevant searches. Add searches that convert repeatedly as new phrase keywords.
3. **Keywords.** Pause or adjust only the ones with 2–3 months of poor data. Remember that match types include plurals and close variants.
4. **Bidding and budget (only if it makes sense):**
   - Budget raises: no fixed rule (Rachel, Oct 16, 2026). Bring the numbers to each monthly review and discuss. Context: the CA$84 target is chosen because Google lands ~1.5× over it (~CA$126), just under the CA$139 lifetime profit, which is the real limit. Sizing formula if a raise is agreed: new budget = current ÷ (1 − Search lost IS (budget)).
   - Revisit the target CPA if the average order or reorder behaviour has changed.
   - US (per-click): adjust the per-click cap, budget and locations. Cost per customer ≈ cost per click ÷ conversion rate (about 3%).
5. **Every 2–3 months:** replace the headline with the worst cost per sale, if it has enough data (about CA$300+ spent). Google no longer shows "Low/Good/Best" ratings; use per-headline cost and conversions (Windsor `ad_group_ad_asset_view` fields with the ad id filter). Note that headlines share credit, so compare them against each other, not against the target.
6. **Limit:** one or two big changes a month. Don't change target, budget and keywords all at once.
7. **Log** every change below, with the date and reason.

## Change log
- Sept 16, 2026: Canada target CPA $42 → $80. GA4 purchase set to Secondary.
- Oct 14, 2026: Canada target $84, budget $50/day. Paused broad "acne supplements" and "heal hormonal acne". Added phrase "acne supplements". Added about 48 negatives. Excluded Quebec.
- Oct 15, 2026: Launched US Max CPC campaign. Canada price asset updated. Merchant Center now syncs Canada + US. Decided to switch Shopify payouts back to CAD.
- Oct 15, 2026: Canada: added 22 phrase-match negatives from the September review (other brands, local salon, diet/recipe questions, myo inositol, thistle oil, vitamin B5, iHerb spelling, one birth-control question). Why: about CA$300 spent since Aug with 0 sales. No change to target (CA$84), budget or bidding: cost per sale is CA$131 since Sept 16, above target, and the target changed Oct 14, so wait for a clean month. Exception noted: broad "dim supplement" stays on because it makes sales at about CA$70 each.
- Oct 15, 2026: Account-level Final URL suffix set to `utm_source=google&utm_medium=cpc&utm_campaign={campaignid}` (auto-tagging was already on). Why: Shopify showed ad clicks as free "Google, SEO" visits, so Google's sales couldn't be matched to real orders. From now on, ad orders show utm medium "cpc" in Shopify's customer journey. Note: ~54 of September's ~86 orders were subscription renewals, which never have a source; compare Google's sales only with website orders.
- Oct 15, 2026: GA4 property 373783616 (already named "cocoonsupplements.com - GA4"; Windsor still shows the old name) switched from Los Angeles time / USD to Toronto time / CAD, to match Google Ads and Shopify. Applies from Oct 15 onward; earlier GA4 data stays in LA time / USD.
- Oct 15, 2026: Canada ad 756182653564: replaced headline "Root Cause Acne Relief" with "With DIM & Glutathione" (edited in place by Rachel; the ad keeps its history). Why: Sept 16 to Oct 14 it got ~4,500 impressions and CA$564 for ~1.7 sales (~CA$338 per sale) vs ~CA$110 for the ad overall. Check the new headline in the October review. Also watch "DIM-Powered Hormone Support" (~CA$190 per sale) and "Trusted by 1,000+ Canadians" (CA$104, 0 sales): not enough data yet.
- Oct 15, 2026: Price assets split by country. The Canada and US campaigns were sharing one price asset (in USD, so Canada ads showed US$50). Rachel edited it to CAD for Canada, removed it from the US campaign, and added a new campaign-level USD price asset (Product tiers, "From") to "US Sales | Search | Max CPC | Oct 2026". Both pending Google review (confirmed Oct 22: Canada asset in CAD and US asset in USD, both serving). Canada shipping zone confirmed CAD with free shipping over CA$70 (US: USD, free over US$70).
- Oct 16, 2026: **Product page now opens on 1-month + Subscribe & Save** (was 3-month since ~June 2026). Theme "Cocoon — 1-month default + best value (preview)" (id 131597271104) published by Rachel: 1-month pill first, "Best value" badge on 3-month, pills equal height. Balance variant order changed so 1-month is first (that sets the default). Ad links with ?variant= still open the linked option (checked). Why: search-visitor purchase rate fell ~2.9% → ~1.8% after the 3-month default. **Measure:** search-traffic add-to-cart rate, purchase rate, average order, new customers for Oct 16–Nov 6 vs Jun 1–Oct 15 (baseline: add-to-cart 3.1%, purchase 1.8%). Undo: move 3-month back to first in the Balance variants.
- Oct 16, 2026 (note): Google ad links checked. Canada ad → ?variant=39429510135872 (1-month); US ad → plain product page (now 1-month); sitelinks → plain pages; price-asset rows link to their own option (correct). So paid Google visitors never saw the Jun–Oct 3-month default; only organic search did. The ~38% drop in search-traffic purchase rate therefore isn't fully explained by the default (other suspects: .ca → .com move in Sept, summer traffic mix). Judge the page change on the Oct 16–Nov 6 before/after, split paid (utm_medium=cpc) vs organic. Rachel recalls switching the Google ad links to the 3-month option when the default changed (~June), in which case paid visitors did see 3-month over the summer and the current 1-month link is a later change; check Google Ads change history if it matters.

- Oct 26, 2026: **Paused "US Sales | Search | Max CPC | Oct 2026"** (campaign 24353842296), approved by Rachel. Why: kill rule (~CA$500 spent with under 2 sales): ~CA$467 spent Oct 15 to 26, 0 purchases, ~190 clicks. Undo: enable the campaign. Revisit after Canada proves out; no Google changes until Logan is back in Dec except by Rachel's OK.
- Oct 26, 2026: Added the Canada watch rule (see Campaigns > Canada). Rachel OK. No campaign setting changed.

## Open items
- Merchant Center US listings. Checked Oct 19–22, 2026: there are no shopify_US listings in USD. The US view shows only the 2 Canadian listings (shopify_CA, CA$ prices), both "Limited" for "Mismatched currency in shipping information" (US shipping is in USD, product price in CAD). Merchant Center has only 2 products in total (the app's "4" is 2 products x 2 countries). Shopify itself is set up right: an active United States market, and contextual price US$50. The app's "Countries and languages" is manual (automatic sync Off) with Canada + United States, and it stays that way: turning automatic sync on pulls in the ~100-country International market. Oct 22: the app's own help says it only targets one country (based on store currency); other countries are just extra targets on the same feed, which causes the mismatch. Decision: parked. Free listings had 0 clicks, so it's not worth a feed app now. Revisit only if we run US Shopping ads. Free listings only; doesn't affect the Search ads. Fix before Black Friday.
- Canada budget is CA$50/day (confirmed Oct 15) and shows "Limited by budget". The Oct 7 to 13 capping was before the Oct 14 raise. Only raise further if cost per sale reaches CA$84 or lower (rule in step 4).
- .ca → .com (cocoonsupplements.com is the official site for both Canada and US). Checked Oct 15, 2026: all live ads and sitelinks, the Shopify primary domain, Merchant Center (confirmed by Rachel) and GA4 tracking are already on .com. Search Console has the .com as a Domain property with its sitemap read (39 pages); Search Console was then removed from Windsor (Basic plan = 3 sources: Google Ads, Meta, GA4); reconnect it when SEO work starts. Still to do:
  - The paused "US Sales | Search | Clicks | May 2026" ad still links to cocoonskincare.ca, which is shut down (no redirect, confirmed Oct 15, 2026). Never re-enable it without changing the link.
- Later: French site and a Quebec campaign; Meta relaunch; SEO rebuild for the new domain.
