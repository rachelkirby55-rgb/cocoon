# Cocoon Meta Ads: Operating Manual

Brief for Claude (or any person) running Cocoon's Meta Ads. Last updated Oct 15, 2026.

## How to work with Rachel
- Explain things very simply, like to a five-year-old. When she's right, say so plainly; don't repeat her point back in different words.
- Be direct, with no hedging. If you were wrong, say so.
- For anything she has to click through in Ads Manager, give one step at a time and wait for her to confirm before the next.
- **Never make changes without her OK.** Analyze first, propose specific changes, then make the ones she approves.
- Act like a Meta expert: tell her exactly what to do and why, in one or two sentences. Don't hand her a menu of options unless the choice is genuinely hers.

## Access
- Meta ad account **554752048834670** ("Cocoon"), currency CAD, reached through the Windsor.ai connector `facebook`.
  - Read with `get_data`. Make changes with `execute_action`. Run `list_actions` first.
  - Through Windsor, Claude can: pause and enable campaigns, ad sets and ads; set budgets; create campaigns, ad sets and ads; upload images and videos; edit ad copy, headlines and links (`update_ad_creative`). Meta allows at most 4 budget changes per ad set per hour.
  - Claude can't: see the ads visually the way Rachel does, change Events Manager or Business Settings. Give Rachel UI steps for those.
- Meta only returns data from the last 37 months. Pass dates from about 36 months back at the earliest.
- **Decision metric: 7-day click only.** Pull with `options: {"attribution_window": "7d_click"}`. Meta's default (7-day click + 1-day view) counts people who only saw the ad, which overstates results for Cocoon. Use it only as a side comparison.
- Purchase field: `actions_offsite_conversion_fb_pixel_purchase`. Revenue: `action_values_offsite_conversion_fb_pixel_purchase`.
- Windsor is on the Basic plan (bought Oct 15, 2026) with 3 sources: Google Ads, Meta Ads, GA4. Adding a fourth pauses ALL reads until one is removed. Swap GA4 for Search Console when SEO work starts. Shopify data comes through the Shopify connector, not Windsor.

## Tracking
- Dataset (pixel) **3561456130627090**, fed by the Shopify Facebook & Instagram app with Maximum data sharing (pixel + Conversions API). Purchase match quality 8/10 (Oct 2026).
- cocoonsupplements.com is verified in Business Settings (Oct 15, 2026). Purchases fire on the new domain.
- **Tracking broke around Feb 2026 and was working again by March 2026** (corrected Oct 16, 2026; this manual used to say "until Sept"). Evidence: from March on, Meta recorded the full funnel every month with normal checkout-to-purchase rates (28–71%, vs 34–65% in Oct 2025–Jan 2026). No ads ran in Feb, so the exact dates can't be seen. **Treat Mar–Aug 2026 results as real.**
- **But the website converted far worse from about Feb 2026** (Shopify: visitors who buy ~2.7% in Nov–Jan → ~1.1% in Jul–Sep; new customers per month roughly halved from Feb). Ads still got clicks at about the same cost (~CA$2–3 per click); fewer clicks turned into sales. Likely cause under review: the product page default switched to the 3-month subscription (CA$159.73), see open items. Judge 2026 ad results against each other, not against 2023–2025 numbers.
- A "data sharing restrictions" notice exists because it's a supplement. It doesn't block ads.

## Business numbers
- Product: Balance (hormonal acne supplement with DIM + glutathione). Site: **cocoonsupplements.com**.
- Margin about 62%. Meta blended first order about CA$97, so first-order break-even is about CA$60. Lifetime value about CA$224 revenue, about CA$139 profit.
- Prices: Canada CA$68 for 1 month (CA$61.20 on subscription), CA$177.48 for 3 months. US US$50 for 1 month (US$45 on subscription), US$130.50 for 3 months. Free shipping over 70 in either currency.

## Judging ads (7-day click cost per sale)
- **Under CA$60: scale.** Raise its ad set budget.
- **CA$60–100: keep.** Subscription reorders make this profitable over time.
- **Kill:** no sale after about CA$140 spent, OR cost per sale above CA$140 after 2 weeks.
- Don't judge an ad before it has spent about CA$100, or before 7 days, unless it's clearly broken.
- **Tired ad signs:** frequency above about 3 per week and cost per sale rising for 2 weeks in a row. Refresh it (new hook or first 3 seconds) or replace it.

## Campaign structure (agreed approach)
One always-on campaign per country. Never move an ad to a new campaign; that throws away what Meta learned.

**"Balance | Sales | CA"** (Sales objective, optimize for Purchase, Canada)
- Budgets set on each ad set (not campaign budget), so tests always get money.
- Audience: Advantage+ audience, ages 25–44 as a suggestion, women. Exclude Quebec (site isn't in French).
- Ad set **"Proven"**, about CA$30/day: the 3–6 best ads. This is where most money goes.
- Ad set **"Testing"**, about CA$15/day: 2–4 new ads at a time.
- **When a test ad wins** (under CA$60 after about CA$150 spend): add it to Proven **using the existing post** ("Use existing post" in Ads Manager, same post ID), so it keeps its likes and comments. Pause it in Testing. Do this in batches, at most once every 2 weeks, because adding ads to Proven nudges it back into learning.
- **When a Proven ad dies** (kill rule): pause it. Don't delete it.

**Retargeting:** no always-on retargeting. Advantage+ already shows ads to warm people. Run short retargeting campaigns only around sales (manual audiences, "Use as a suggestion" unchecked), with the Before/After carousel.

**US:** a separate campaign, "Balance | Sales | US", only after Canada proves the ads still work (cost per sale under about CA$100 for 2 weeks). Never mix countries in one ad set. US copy rules below.

**Changes that reset learning (avoid):** budget jumps of more than about 20% at once, editing an ad's media or copy, changing targeting, adding many ads at once. After a change, leave that ad set alone for 7 days.

**Advantage+ creative settings:** keep Website Summaries, Site Links, Website Highlights ON. Turn Products, Promotions and all AI video/text changes OFF.

**Rejected:** catalog ads (Balance is rejected in the catalog), awareness/reach and video-view campaigns (about CA$3,900 spent in 2025, zero sales).

## Copy rules
- Never say "treat". "Acne" is fine.
- Say "drug-free, nature-backed ingredients", not "natural". "Science-backed" is fine for headlines.
- Excess estrogen is "a common, overlooked cause" of hormonal acne, never "the" cause. Exception: Rachel's own story ("high estrogen was the root cause" of *her* acne) is fine.
- Never say "Health Canada approved" (Rachel, Oct 15, 2026). "Naturopath-formulated" and the 30-day money-back guarantee are fine.
- US: never say "Canadian-made".
- All links must point to **cocoonsupplements.com**, never cocoonskincare.ca.
- Ask Rachel before using any other credential claims. The domain moved because of Health Canada claim limits.

## Ad library (results from history, 7-day click, CAD)
### Proven winners: start here
| Ad | Ad ID | Cost per sale | Sales | When |
|---|---|---|---|---|
| Video Ad 3: Founder Ad (Quiz) | 120225068657950301 | $42 | 47 | 2025 |
| Video Ad 1: DIM Comment | 120225006723890301 | $48 | 43 | 2025 |
| CA Founder Ad (original) | 23856934920440300 | $49 | 182 | 2023 |
| NY Sale Founder Video V1 + V2 | 120237595971690301 / 120237596511840301 | $49 | 5 | Jan 2026 |
| ASMR Product Video | 120237539030230301 | $50 | 5 | Jan 2026 |

Caution: Founder Ad and DIM Comment reran Mar–Aug 2026 at about $206 and $228 per sale (real numbers, tracking was working). They were still the best of 2026, so the drop is mostly the weaker website, not tired ads.

### Worth retesting
| Ad | Ad ID | Cost per sale | Sales |
|---|---|---|---|
| Carousel: Education + Before/After | 120225079426660301 | $74 | 38 |
| Updated Founder Ad (2024) | 120210697259880301 | $75 | 112 |
| Kaija UGC (K7) | 120233881284350301 | $76 | 8 |
| Video Ad 4: Testimonial 1 | 120225080698100301 | $85 | 23 |

### Retargeting only
| Ad | Ad ID | Cost per sale | Sales |
|---|---|---|---|
| Carousel: Before/After | 120214136333980301 | $30 | 15 |
| Testimonials video | 120214136188380301 | $57 | 4 |
| Educational Carousel | 120215928222020301 | $62 | 11 |

### Ran Mar–Aug 2026 (tracking working, weaker website), 7-day click
| Ad | Spent | Sales | Cost per sale |
|---|---|---|---|
| Founder Ad (2026 version) | $2,065 | 10 | $206 |
| Carousel: Education + Before/After | $623 | 3 | $208 |
| Video Ad 1: DIM Comment | $1,827 | 8 | $228 |
| Founder Montage with VO | $1,399 | 6 | $233 |
| "No One Knows I Have the Answer" (won its Jun–Aug test group) | $1,717 | 3 | $572 |
| Bailey Testimonial (+ quiz version) | $507 | 0 | none |
| Coffee Shop/Restaurant | $237 | 1 | $237 |
| "Goodbye Skin, Hair & Nail Gummies" | $269 | 0 | none |
| "Until I Fixed My Hormones" (dropped: the teaching is in the caption, not the video) | $32 | 0 | not tested |
| Spring sale video (sale only) | $332 | 4 | $83 |

### Don't rerun
Awareness/video-view ads (Cocoon Anniversary, Dirty Pillowcase, Candice images, Green Background images), Black Friday 2024 (about $300 per sale), Birth Control Ad ($106), 2025 Spring Sale images, US Founder Ad 2023 (no sales), the Nov 2025 BFCM batch (no signal).

## Routine
### Weekly check (Mondays, about 10 minutes)
Meta moves faster than Google, so check weekly, not just monthly.
1. Spend and sales (7-day click) for last 7 days, by ad set and by ad.
2. Apply the kill rule. Propose pauses.
3. Flag any ad under $60 that's ready to scale or graduate.
4. Check frequency for tired ads.
5. Confirm Purchase events are still coming in (sales showing in Meta roughly match Shopify).

### Monthly review (end of month)
1. Results: cost per sale, sales, spend for the month vs last month and vs the $60 / $100 targets.
2. Graduate winners from Testing to Proven (existing post ID). Pause losers.
3. Budget: raise only where cost per sale is under $60, by at most 20% per week.
4. Creative pipeline: Testing needs 2–4 fresh ads each month. Tell Rachel what kinds of ads to make next, based on what's winning (hook, format, who's on camera).
5. US: check whether Canada meets the bar to launch the US campaign.
6. One or two big changes a month at most.
7. Log every change below with the date and reason.

## Change log
- Oct 15, 2026: Confirmed tracking works on cocoonsupplements.com (Purchase active, 8/10 match quality) and the domain is verified. Reviewed full ad history. Agreed on one campaign per country with Proven and Testing ad sets; winners are added to Proven by existing post ID, not moved to a new campaign. Canada first, US later.

## Open items
- Confirm Meta daily budget (proposed: CA$45/day, $30 Proven + $15 Testing).
- **Every old ad links to cocoonskincare.ca, which is shut down with no redirect (confirmed Oct 15, 2026).** Never re-enable an old ad. Each winner is rebuilt as a new ad (same video/images and copy, link to cocoonsupplements.com), which starts a new post without the old likes/comments. From then on, reuse the NEW post IDs ("Use existing post") so social proof builds again. Check the copy against the copy rules while rebuilding.
- Build the "Balance | Sales | CA" campaign with Proven (top 3 winners) and Testing (first untested batch).
- Rachel to share any never-tested creatives for the Testing ad set.
- Later: US campaign; hire or brief someone for creative production.
