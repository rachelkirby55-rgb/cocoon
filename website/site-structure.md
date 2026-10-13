# cocoonsupplements.com: proposed site structure

Status: **DRAFT, needs Rachel's sign-off.** Full copy gets written once this is approved and the two product briefs are in.
Sources: `research/navigation-conversion-audit.md` (GA4 May 2023–Oct 2026, Shopify orders Nov 2022–Oct 2026, Klaviyo), `research/seo-audit.md` (Search Console Jun 2025–Oct 2026, Google Ads, Keyword Planner) and `research/current-site-copy.md` (live site, 13 Oct 2026).

## The recommendation in one paragraph
Keep every URL that already ranks or sells, and add a range layer on top. The **home page** becomes the brand's front door and targets "supplements for hormonal acne". A new **Shop** collection targets "clear skin supplements" and helps shoppers choose between the three formulas. Each **product page** works as a complete sales page on its own, with reviews, guarantee, ingredients and a safety FAQ built in, because that's where 95% of add-to-carts happen and almost nobody visits standalone trust pages. The **quiz** becomes the "find your formula" recommender that sends people to the right product. The **blog** stays for SEO under a Learn hub, and moves out of the main menu. Everything is designed for mobile first (82% of sessions).

## Why (the data behind each decision)
| Decision | Evidence |
|---|---|
| Product pages carry the sale, so trust content lives on them | `/products/balance` brought 42% of landing sessions and 44% of GA4 revenue, and gets 95% of add-to-carts. `/pages/reviews` had 7 views in 3.4 years, the guarantee page 285, the FAQ 1.3% of views. |
| The home page shows all products, one tap each | Home converts at 3.4% and brings 30% of revenue. Brand searches landing there convert at 5.8%. 42% of clicks from home go to the product page. |
| The quiz becomes the product recommender | 25% of first-time buyers completed the quiz before their first order. 11.6% of people who finish it buy, 78% of them within 7 days. Yet the quiz end screens never link to a product, and the high-androgen results already promise "additional formulas in development". |
| Blog moves to the footer and Learn hub, but every URL is kept | 3,604 article landings → 7 purchases. But the tea article is the biggest non-brand SEO asset (157k impressions), so its URL must stay. |
| "Manage subscription" link in the header | Subscriptions were 40% of all orders, and 55% in 2026. 11% of site searches are about cancelling, returns or orders. |
| Say "supplements" plainly, and keep "formerly Cocoon Skincare" | 40% of site searches were for skincare products Cocoon doesn't sell. The top brand search is "cocoon skincare" (6,114 impressions). |
| 3-month and subscribe options built into every product page | In 2026, 3-month packs were 25% of orders and 48% of product sales. |
| Built for Canada as well as the US | Canada was 72% of 2026 orders. US conversion was 0.95% in 2026, against 2.62% for Canada. |

## Main navigation (mobile first)
```
[Logo]                                    [Search] [Account ▾] [Cart]
Shop ▾ | Find Your Formula (quiz) | Results | Learn | About
  Shop ▾
    All Supplements        → /collections/skin-supplements
    Balance                → /products/balance
    [New product A]        → /products/[a]
    [New product B]        → /products/[b]
    Bundles                → (only if we offer them; see Q3)
  Account ▾
    Log in / My orders
    Manage subscription    → Appstle customer portal
Announcement bar: rotates between "New: [product]" and "Free shipping on $70+ & all subscriptions"
```
Footer: Shop links · Learn hub · Blog · FAQ · Money-back guarantee · Shipping · Affiliate · Wholesale · Contact · Policies · supplement disclaimer.

## Sitemap and the job of each page
| # | Page | URL | Primary keyword | Page's job | Status |
|---|---|---|---|---|---|
| 1 | Home | `/` | supplements for hormonal acne `[CLAIM CHECK]` | Brand promise, the 3 formulas side by side, quiz CTA, proof, guarantee | Keep URL, rewrite |
| 2 | Shop all | `/collections/skin-supplements` | clear skin supplements | Compare the formulas ("Which one is right for me?") and sell bundles | **New** |
| 3 | Balance | `/products/balance` | DIM supplement for women / estrogen balance | Full standalone sales page | Keep URL, rewrite (H1 is just "BALANCE") |
| 4 | [Product A] | `/products/[a]` | from the brief + keyword research | Same template as Balance | **New** |
| 5 | [Product B] | `/products/[b]` | from the brief + keyword research | Same template as Balance | **New** |
| 6 | Quiz | `/pages/quiz` | acne quiz / what type of acne do I have | Recommend the right formula, capture email | Keep URL, retitle, add ~300 words of indexable copy, add product links to result screens |
| 7 | Results | `/pages/results` | Cocoon reviews | Before/afters + all Okendo reviews in one place | Keep. Merge `/pages/reviews` into it |
| 8 | Learn hub | `/pages/learn` | hormonal acne | Root-cause education, linking to concern articles, quiz and products | Keep URL, rewrite, fix broken links |
| 9 | Estrogen dominance & acne | existing post `/blogs/cocoon-blog/estrogen-dominance-in-women-symptoms-causes-and-natural-treatment` | estrogen dominance acne | Concern hub feeding Balance | Keep URL, retitle (drop "treatment") |
| 10 | Concern hubs for the new products | e.g. androgens/DHT | from the briefs | One hub per new product's root cause | `[NEED FROM RACHEL: briefs]` |
| 11 | Blog | `/blogs/cocoon-blog` + all article slugs | per article (see SEO audit 8e) | SEO traffic → quiz/product CTAs | Keep every slug. Refresh tea + coffee; merge the 2 diet posts |
| 12 | About | `/pages/about` | Cocoon supplements / formerly Cocoon Skincare | Founder story, naturopath, why a range now | Keep URL, rewrite |
| 13 | FAQ | `/pages/faq` | — | Grouped: products, safety, subscriptions, shipping, returns | Keep URL, rewrite for 3 products |
| 14 | Money-back guarantee | `/pages/money-back-guarantee` | — | Terms, now covering all products | Keep URL, update |
| 15 | Shipping, Contact, Affiliate, Policies | existing URLs | — | Update legal name, domain, currency, links | Keep URLs, update |

### Product page template (used for all 3 products)
1. Buy box: name + one-line benefit, rating stars (Okendo), price, 1-month / 3-month, subscribe & save (shown first), free-shipping note, guarantee badge
2. "Is this for you?" with the signs and symptoms this formula targets, and a link to the quiz for anyone unsure
3. How it works: the root cause in plain language
4. Ingredients and doses, with the supplement facts panel
5. What to expect and when (**one** consistent timeline across the site)
6. Results and reviews
7. Safety FAQ: birth control, pregnancy/breastfeeding, medications, side effects, men
8. Pairs well with (links between the 3 formulas and the stack)
9. Guarantee + subscription details
10. Supplement disclaimer

## Redirect map (301s)
Shopify keeps paths across the domain change, so most `.ca → .com` redirects are automatic. Spot-check them in a browser, because the .ca domain couldn't be reached from here. Add these:

| From | To | Why |
|---|---|---|
| `/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2025` | `/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2026` | 404 today; 854 impressions |
| `/pages/refund-policy` | `/policies/refund-policy` | 404 today |
| 7 old/malformed tea slugs (listed in SEO audit §4) | `/blogs/cocoon-blog/best-teas-for-hormone-balance` | 404 today |
| `/blogs/cocoon-blog/goodbye-hair-skin-nail-gummies-why-hormonal-acne-needs-more-specif` | full slug | 404, truncated |
| `/blogs/cocoon-blog/the-truth-authorization-prescription-acne-medications` | `/blogs/cocoon-blog/the-truth-about-prescription-acne-medications` | 404, malformed |
| `/pages/results-1` | `/pages/results` | duplicate |
| `/pages/reviews` | `/pages/results` | merged |
| the diet post we drop | the diet post we keep | merged |
| `/collections/all` | `/collections/skin-supplements` | one shop page |
| `/products/dim`, `/pages/learn-1` | (already redirect) | keep |

## Before launch (not copy, but they affect results)
- [ ] Add cocoonsupplements.com to Google Search Console and run Change of Address from the .ca property. **Most urgent:** .ca impressions fell about 85% from 4 Oct.
- [ ] Keep cocoonskincare.ca registered and redirecting for at least a year.
- [ ] Move Google Merchant Center to the new domain (it still sends `country=CA&currency=CAD` links).
- [ ] Rename the Shopify product type from "Skincare" to "Supplements" and remove the "…Treatment" tags.
- [ ] Add Organization schema with `alternateName: "Cocoon Skincare"`.
- [ ] Update Terms and Privacy (they still say cocoonskincare.ca and Cocoon Skincare Inc.).

## Decisions needed from Rachel
1. **Canada vs US.** Canada is 72% of 2026 orders. Proposal: one site that sells to both countries, with CAD prices for Canadians through Shopify Markets. Should the copy use US spelling (my default for a .com) or Canadian spelling?
2. **Canadian claims.** Does Balance have an NPN? Will the new products? If so, please send the licensed claims, because Canadian copy has to stay within them.
3. **Bundles.** Will there be a stack or bundle price (e.g. Balance + new product)? This decides whether "Bundles" goes in the menu.
4. **Naturopath.** Can we name the formulator(s)? Right now the site only says "naturopath-formulated".
5. **Results timeline.** The site currently says "1 week to 3 months", "3–6 months" and "60–90 days" on different pages. Which is right? (FTC requires typical results.)
6. **Product briefs** for the two new products (`product-briefs/TEMPLATE.md`).
