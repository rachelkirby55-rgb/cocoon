# cocoonsupplements.com: proposed site structure

Status: **approved to build** (Rachel, 21 Oct 2026). Briefs are in `product-briefs/`. Product names: **Androgen Balance** (Jan 2027) and **Liver Support** (Apr 2027), both working names.

Built in Shopify on 21 Oct 2026, all hidden from the live site: the unpublished collection "All Supplements" (`/collections/skin-supplements`, Balance only for now), and the menus "NEW SITE – Main menu (draft)" (`new-site-main-menu`) and "NEW SITE – Footer menu (draft)" (`new-site-footer-menu`). The Root trial theme can't be edited through the API, so choose these menus in Root's theme editor, under Header and Footer.
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
Shop ▾ | Find Your Formula (quiz) | Results | Learn | About | FAQ | Guide (blog)   ← FAQ and Guide added at Rachel's request, 23 Oct 2026
  Shop ▾
    All Supplements        → /collections/skin-supplements
    Balance                → /products/balance
    Androgen Balance       → /products/androgen-balance (Jan 2027)
    Liver Support          → /products/liver-support (Apr 2027)
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
| 4 | Androgen Balance | `/products/androgen-balance` | from the brief + keyword research | Same template as Balance | **New** |
| 5 | Liver Support | `/products/liver-support` | from the brief + keyword research | Same template as Balance | **New** |
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
**cocoonskincare.ca does not redirect and can't be made to** (owner, 21 Oct 2026), so the old domain's rankings won't transfer. These redirects are all *within* cocoonsupplements.com. They fix broken links and merged pages:

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
- [x] cocoonsupplements.com is in Google Search Console. Change of Address isn't possible because there's no .ca redirect.
- [ ] Submit `https://cocoonsupplements.com/sitemap.xml` in Search Console, if it isn't already.
- [ ] Update the US labels: they still say "Questions? Email info@cocoonskincare.ca".
- [ ] Move Google Merchant Center to the new domain (it still sends `country=CA&currency=CAD` links).
- [ ] Rename the Shopify product type from "Skincare" to "Supplements" and remove the "…Treatment" tags.
- [ ] Add Organization schema with `alternateName: "Cocoon Skincare"`.
- [ ] Update Terms and Privacy (they still say cocoonskincare.ca and Cocoon Skincare Inc.).

## Decisions (Rachel, 21 Oct 2026)
1. Canadian spelling.
2. Balance has an NPN. Never mention it. The new products have no NPN.
3. Images: US packaging only.
4. Formulator can't be named; say "naturopath-formulated".
5. Use "acne" in copy, never "treat/treatment/cure".

## Still open
- Final product names (Androgen vs Metabolic Balance; Liver Support vs Booster).
- Bundles/stack pricing.
- One results timeline (the site currently gives three different ones; Alyssa to confirm for the new products).
- Approved claims wording for the new products (Alyssa).
