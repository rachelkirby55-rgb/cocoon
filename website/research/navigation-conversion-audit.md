# Navigation & Conversion Data Audit

Prepared for the cocoonsupplements.com multi-product restructure. This was a read-only audit: no store, ads or Klaviyo settings were changed. Pulled 13 Oct 2026.

**Date ranges available (earliest data found):**
- GA4 (property 373783616): **10 May 2023 → 12 Oct 2026**. Nothing before 10 May 2023. Universal Analytics history is gone.
- Shopify orders: **30 Nov 2022 (order #1001) → 12 Oct 2026**, 4,302 orders. There are no 2020–2022 orders in this store, so any pre-Nov-2022 history lives somewhere else.
- Shopify sessions (ShopifyQL): 2022 → 12 Oct 2026. Meaningful volume starts in 2023.
- Klaviyo: 2022 → 12 Oct 2026. Google Ads: 2023 → 2026. Meta Ads: the API only returns the last 37 months, and the campaign table below covers 2025–2026.

---

## What this means for the new site structure

1. **Product pages are where people buy. Build every product page to close the sale without sending people elsewhere.** `/products/balance` brings in 42% of landing sessions and 44% of GA4 revenue. It is also the landing page for 49% of Shopify web orders, and 95% of all add-to-carts fire on it. Visitors rarely go to separate trust pages: in 3.4 years `/pages/reviews` got **7 views**, the guarantee page got 285 (0.15% of views) and the FAQ got 1.3%. So reviews, guarantee, FAQ, safety and ingredients belong *on each product page*. Separate pages can stay for SEO and footer links.
2. **The homepage is the second-biggest converter and works as the brand-search landing page.** It converts at 3.4% and brings in 30% of GA4 revenue. Brand searches that land on the homepage convert at **5.8%** (6,806 sessions, 395 purchases). Branded Google Ads terms ("cocoon skin care", "cocoon supplement") convert at 13% of clicks. 42% of clicks from the homepage go straight to the product page. With more products, the homepage has to send people to each product in one tap (a "shop" grid plus a "find your formula" route) and keep ranking for the brand name.
3. **The quiz brings in leads; it doesn't close sales in the same session. Make it the product recommender.** It accounts for 26% of landing sessions and 27% of page views, but quiz landings convert at only 0.76% in-session. Even so, **25% of all first-time buyers (389 of 1,578) completed the quiz before their first order**. 11.6% of people who complete it go on to buy, and 78% of those buy within 7 days (Klaviyo profile join). With several products, the quiz should recommend a product (Balance or a new SKU) and keep collecting emails. Don't send paid search traffic to it: 6,846 paid-search sessions landed on the quiz and produced 8 purchases (0.12%).
4. **The blog is for SEO, not sales.** 37 articles produced 3.1% of page views, 3,601 landing sessions and **7 purchases ($392)** in 3.4 years. The top article, *best-teas-for-hormone-balance*, had 1,639 landings and no sales. Only 16% of clicks out of articles go to a product. Keep every blog URL with 301 redirects and group the articles under a Learn hub. Add CTAs to the quiz or product that match each article's topic. Don't give the blog top-level navigation priority over Shop or the quiz.
5. **The Learn page works alongside the product page, so make it a per-product "How it works / The science" page.** 40% of Learn visits come from the product page, and 40% of clicks out of Learn go back to it. FAQ and About behave the same way: they are side trips from the product page, not entry points.
6. **Subscriptions and accounts need a permanent spot in the header.** 40% of all orders (1,700) are recurring Appstle subscription orders, rising to 55% in 2026. Account and subscription pages get 3.8% of all page views. 11% of site searches are about returns, cancelling, subscriptions or orders.
7. **3-month packs are growing, so make the supply/subscribe selector a clear part of every product page.** In 2026, 3-month packs were 25% of Balance product orders and 48% of product sales (1-month: 75% of orders / 52% of sales). The old 60/90/120-count variants (2023–24) made up 5% / 3% / 1% of product orders. That is the only history for multi-count SKUs before the new 60- and 90-count launches.
8. **Canada is still the core market even though the site is moving to a US domain.** Canada was 72% of 2026 orders and 78% of 2026 new customers. The US share of orders fell from 49% (2024) to 24% (2026), and US session conversion fell to 0.95% in 2026 (Canada: 2.62%). The structure has to keep Canadian shoppers (CAD pricing/market, redirects from cocoonskincare.ca) while it grows the US.
9. **Site search shows the old "skincare" name confused people, and that people want ingredient and safety answers.** 40% of the 309 site searches were for skincare brands or products Cocoon doesn't sell (toner, Caudalie, La Roche-Posay, Embryolisse and others). 17% were for ingredients or product facts, and 7% were safety questions (birth control/the pill, pregnancy, side effects, weight gain). Navigation should say "supplements" plainly, and each product page needs an ingredient panel and a safety FAQ. A shared ingredients page would cover several products.
10. **The site is used mostly on mobile.** 82% of GA4 sessions and 78% of Shopify sessions are on mobile. Mobile converts as well as or better than desktop (GA4 2.24% vs 2.19%; Shopify 2.23% vs 1.74%), so design the navigation for mobile first.

---

## Data quality notes (read before using the numbers)

- **Shopify store identity.** The Shopify MCP is connected to `rachelkirbystore.myshopify.com` (store name "Cocoon", domain cocoonsupplements.com). Windsor and the brief use `cocoonskincare.myshopify.com`. Both return the same 4,302 orders, so they are the same store. The myshopify handle in `.claude/agents/website.md` may need correcting.
- **Currency.** ShopifyQL reports in **USD** (the store's current currency). Windsor order values are in **CAD**, the currency the orders were placed in: 4,287 of 4,302 orders. GA4 revenue is **USD**. Each table names its currency; don't mix them.
- **GA4 vs Shopify.** GA4 recorded 2,184 purchases. Shopify had 2,448 non-subscription-renewal orders in the same window, so GA4 captures about 89% of web orders. GA4 doesn't see recurring subscription orders, because they never touch the site.
- **Paths.** Through Windsor, GA4 offers no path exploration, entrances or exits fields. Page-to-page paths below come from `page_referrer` → `page_path` page-view pairs, which show one step at a time, not full sessions. Shopify checkout pages report only the site's root as referrer, so "Home → Checkout" pairs are a tracking artifact and are left out of the conclusions.
- **Channel definitions.** GA4 puts some Meta traffic in "Paid Other" (utm_medium=paid with numeric campaign-ID sources). In this report, Meta = Paid Social + Paid Other.
- **Ad platforms over-count conversions** compared with GA4 (see Q8).

---

## Q1. Top landing pages: sessions, conversion, revenue

**GA4, 10 May 2023 – 12 Oct 2026, by page type** (revenue in USD; CR = purchases ÷ sessions)

| Landing page type | Sessions | % of sessions | Engaged | Add to carts | Purchases | CR | Revenue | % of revenue |
|---|---|---|---|---|---|---|---|---|
| Product page | 41,285 | 41.6% | 31% | 2,159 | 983 | 2.38% | $63,639 | 44.0% |
| Quiz (`/pages/quiz` + `/pages/typeform`) | 25,358 | 25.6% | 65% | 582 | 193 | 0.76% | $11,910 | 8.2% |
| Home | 18,708 | 18.9% | 59% | 1,325 | 633 | 3.38% | $43,505 | 30.0% |
| Blog article | 3,604 | 3.6% | 36% | 13 | 7 | 0.19% | $392 | 0.3% |
| (not set) | 2,562 | 2.6% | 3% | 3 | 0 | 0.00% | $0 | 0.0% |
| Account/subscriptions | 1,650 | 1.7% | 46% | 38 | 27 | 1.64% | $1,920 | 1.3% |
| Learn | 824 | 0.8% | 41% | 26 | 15 | 1.82% | $1,015 | 0.7% |
| Cart (returning to a saved cart) | 654 | 0.7% | 99% | 162 | 155 | 23.70% | $11,163 | 7.7% |
| Checkout (resumed) | 596 | 0.6% | 42% | 63 | 130 | 21.81% | $8,389 | 5.8% |
| FAQ | 588 | 0.6% | 37% | 12 | 11 | 1.87% | $718 | 0.5% |
| Blog index | 505 | 0.5% | 50% | 4 | 2 | 0.40% | $88 | 0.1% |
| About | 504 | 0.5% | 48% | 11 | 4 | 0.79% | $323 | 0.2% |
| Quiz results | 489 | 0.5% | 59% | 29 | 14 | 2.86% | $1,053 | 0.7% |
| Collection | 215 | 0.2% | 9% | 0 | 0 | 0.00% | $0 | 0.0% |
| Guarantee | 87 | 0.1% | 36% | 1 | 0 | 0.00% | $0 | 0.0% |
| Reviews | 4 | 0.0% | 0% | 0 | 0 | 0.00% | $0 | 0.0% |
| **Total** | **99,172** | | | **4,451** | **2,184** | **2.20%** | **$144,778** | |

**Top individual landing pages (GA4, same period)**

| Landing page | Sessions | Engaged | ATC | Purchases | CR | Revenue (USD) |
|---|---|---|---|---|---|---|
| `/products/balance` | 41,181 | 31% | 2,139 | 978 | 2.37% | $63,355 |
| `/pages/quiz` | 21,294 | 67% | 458 | 148 | 0.70% | $9,129 |
| `/` | 18,708 | 59% | 1,325 | 633 | 3.38% | $43,505 |
| `/pages/typeform` | 4,064 | 53% | 124 | 45 | 1.11% | $2,781 |
| `/blogs/cocoon-blog/best-teas-for-hormone-balance` | 1,639 | 40% | 0 | 0 | 0.00% | $0 |
| `/pages/learn` | 824 | 41% | 26 | 15 | 1.82% | $1,015 |
| `/cart` | 654 | 99% | 162 | 155 | 23.70% | $11,163 |
| `/pages/faq` | 588 | 37% | 12 | 11 | 1.87% | $718 |
| `/blogs/cocoon-blog` | 505 | 50% | 4 | 2 | 0.40% | $88 |
| `/pages/about` | 504 | 48% | 11 | 4 | 0.79% | $323 |
| `/pages/results` | 489 | 59% | 29 | 14 | 2.86% | $1,053 |
| `/blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse` | 393 | 32% | 0 | 0 | 0.00% | $0 |
| `/account/login` | 307 | 47% | 9 | 11 | 3.58% | $911 |
| `/apps/subscriptions` | 295 | 37% | 8 | 8 | 2.71% | $397 |
| `/blogs/cocoon-blog/hormone-safe-sunscreens` | 253 | 43% | 0 | 0 | 0.00% | $0 |
| `/pages/contact-us` | 227 | 37% | 0 | 1 | 0.44% | $44 |
| `/collections/all` | 196 | 6% | 0 | 0 | 0.00% | $0 |
| `/pages/affiliate-program` | 106 | 58% | 1 | 0 | 0.00% | $0 |
| `/products/balance-thermae` | 102 | 59% | 20 | 5 | 4.90% | $284 |
| `/pages/money-back-guarantee` | 87 | 36% | 1 | 0 | 0.00% | $0 |

**Shopify's own sessions by landing page** (ShopifyQL, 2022 – 12 Oct 2026; Shopify counts sessions differently from GA4)

| Landing page | Sessions | Sessions w/ cart add | Reached checkout | Completed checkout | CR |
|---|---|---|---|---|---|
| `/products/balance` | 45,277 | 2,098 | 1,870 | 1,135 | 2.51% |
| `/` | 27,032 | 1,367 | 1,247 | 725 | 2.68% |
| `/pages/quiz` | 22,921 | 619 | 412 | 192 | 0.84% |
| `/blogs/cocoon-blog/best-teas-for-hormone-balance` | 2,423 | 0 | 0 | 0 | 0.00% |
| `/pages/typeform` | 2,388 | 54 | 38 | 24 | 1.01% |
| `/pages/learn` | 945 | 15 | 15 | 11 | 1.16% |
| `/blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse` | 738 | 0 | 0 | 0 | 0.00% |
| `/pages/about` | 682 | 12 | 11 | 7 | 1.03% |
| `/pages/faq` | 680 | 15 | 18 | 13 | 1.91% |
| `/cart` | 613 | 122 | 149 | 93 | 15.17% |
| `/blogs/cocoon-blog` | 612 | 6 | 4 | 3 | 0.49% |
| `/pages/results` | 607 | 34 | 31 | 14 | 2.31% |
| `/pages/money-back-guarantee` | 104 | 1 | 1 | 0 | 0.00% |

**Landing page of each Shopify web order** (Windsor `order_customer_last_visit_landing_page`; 2,270 of 2,437 one-time and first-subscription web orders have it; Nov 2022 – Oct 2026; net sales in CAD)

| Landing page type | Orders | % of orders | Net sales (CAD) | Of which first-ever orders |
|---|---|---|---|---|
| Product page | 1,121 | 49.4% | $95,338 | 786 |
| Home | 668 | 29.4% | $60,398 | 305 |
| Quiz (`/pages/quiz` 136 + `/pages/typeform` 19) | 155 | 6.8% | $13,955 | 148 |
| Checkout / cart (resumed) | 224 | 9.9% | $21,872 | 144 |
| Account/subscriptions | 26 | 1.1% | $2,481 | 4 |
| Quiz results | 16 | 0.7% | $1,507 | 12 |
| Blog (articles 13 + index 2) | 15 | 0.7% | $1,209 | 12 |
| FAQ | 11 | 0.5% | $881 | 7 |
| Learn | 10 | 0.4% | $1,174 | 7 |
| About | 9 | 0.4% | $985 | 8 |

**Landing page × channel, selected (GA4, USD)**

| Landing → channel | Sessions | Purchases | CR | Revenue |
|---|---|---|---|---|
| Home ← Organic Search (mostly brand) | 6,806 | 395 | 5.80% | $27,115 |
| Home ← Direct | 7,885 | 153 | 1.94% | $10,376 |
| Product ← Paid Search | 5,000 | 152 | 3.04% | $10,838 |
| Product ← Paid Social | 12,766 | 145 | 1.14% | $8,679 |
| Product ← Paid Other (Meta, ID-tagged) | 8,025 | 133 | 1.66% | $7,434 |
| Product ← Direct | 5,125 | 131 | 2.56% | $8,906 |
| Product ← Organic Search | 2,773 | 113 | 4.07% | $7,823 |
| Product ← Email | 513 | 69 | 13.45% | $5,311 |
| Quiz ← Direct | 9,319 | 77 | 0.83% | $4,336 |
| Quiz ← Paid Search | 6,846 | 8 | 0.12% | $456 |
| Quiz ← Organic Social | 2,195 | 42 | 1.91% | $2,880 |
| Quiz ← Paid Social | 1,942 | 16 | 0.82% | $1,097 |

---

## Q2. Most viewed pages and page-to-page paths

**Page views by page type** (GA4, 10 May 2023 – 12 Oct 2026; 192,378 views in total)

| Page type | Views | % of views | Sessions with a view |
|---|---|---|---|
| Product page | 66,512 | 34.6% | 56,174 |
| Quiz (`/pages/quiz` 29,313 + `/pages/typeform` 23,304) | 52,617 | 27.4% | 45,751 |
| Home | 26,017 | 13.5% | 22,493 |
| Checkout | 7,330 | 3.8% | 6,081 |
| Account/subscriptions | 7,295 | 3.8% | 5,165 |
| Cart | 7,105 | 3.7% | 4,635 |
| Blog articles | 6,054 | 3.1% | 5,529 |
| Learn | 3,822 | 2.0% | 3,277 |
| About | 2,968 | 1.5% | 2,502 |
| Quiz results | 2,845 | 1.5% | 2,604 |
| Other info pages (contact, shipping, policies, affiliate) | 2,737 | 1.4% | 2,349 |
| FAQ | 2,535 | 1.3% | 2,346 |
| Blog index | 2,291 | 1.2% | 1,474 |
| Collection | 353 | 0.2% | 334 |
| Search results | 309 | 0.2% | 218 |
| Guarantee | 285 | 0.15% | 248 |
| Reviews | 7 | 0.0% | 7 |

**Where people go next** (GA4 `page_referrer` → `page_path` pairs; page views, same period)

| From | Onward views | Top next pages |
|---|---|---|
| Home | 21,012 | Product 42% · Quiz 11% · Account 9% · About 4% · Cart 3% · Learn 3% |
| Quiz | 7,372 (excl. 17,270 steps inside the quiz) | Product 64% (4,701) · Home 10% · Results 9% (688) · Cart 5% · Learn 3% · About 3% |
| Quiz results | 1,782 | Product 57% · Learn 12% · Quiz 9% · About 5% · FAQ 4% · Cart 3% |
| Product page | 15,704 | Cart 29% · Product (variant/reload) 19% · Quiz 16% · Learn 10% · Home 8% · About 3% · FAQ 3% |
| Learn | 2,151 | Product 40% · About 11% · FAQ 10% · Quiz 9% · Blog article 7% |
| About | 1,916 | Product 24% · FAQ 17% · Learn 15% · Other info 12% · Quiz 8% |
| FAQ | 1,227 | Product 30% · Other info 12% · About 11% · Blog index 9% · Blog article 8% |
| Blog index | 1,862 | Blog article 69% · Product 7% · About 4% · Home 4% · FAQ 3% |
| Blog article | 1,290 | Blog index 31% · Another article 29% · Product 16% · Quiz 6% · Home 5% |
| Guarantee | 94 | Other info 32% · Product 28% · FAQ 11% |
| Cart | 3,501 | Checkout 36% · Home 22% · Product 22% |

**Where page views come from**

| Into | Views | Top sources |
|---|---|---|
| Product page | 66,512 | Direct/no referrer 39% · Social 15% · Search engines 14% · Home 13% · Quiz 7% · Results 2% |
| Cart | 7,105 | Product 64% · Direct 11% · Home 10% · Quiz 5% |
| Quiz results | 2,845 | Quiz 24% · Direct 24% · Home 18% · Product 14% · Search engines 12% |
| Learn | 3,822 | Product 40% · Home 15% · Direct 14% · About 7% · Quiz 7% |
| FAQ | 2,535 | Product 19% · Home 17% · Direct 13% · About 13% · Learn 9% |
| Blog article | 6,054 | Direct 37% · Search engines 28% · Blog index 21% |

**Common converting paths:**
1. **Ad, search or email → product page → cart → checkout.** 95% of add-to-carts fire on the product page (4,245 of 4,451), and 64% of cart views come straight from it.
2. **Brand search → home → product → cart.** Organic home landings convert at 5.8%, and 42% of clicks from home go to the product page.
3. **Quiz → product (directly or via results) → cart, often days later after Klaviyo emails** (see below).
4. **Blog → product almost never happens:** 206 blog-to-product views and 7 blog-landing purchases in 3.4 years.

**How much each support page matters in converting journeys**

| Page | Share of views | Landing CR (GA4) | Evidence |
|---|---|---|---|
| Quiz | 27.4% | 0.76% | **25% of first-time buyers completed it before ordering** (Klaviyo, below). In-session conversion is low; the payoff comes later through email. |
| Quiz results | 1.5% | 2.86% | 57% of onward clicks go to the product page. Only 2,604 sessions reached it, against 3,528 quiz completions, so many completers skip it (the Typeform may redirect elsewhere). |
| Learn | 2.0% | 1.82% | A side trip from the product page: 40% of views come from the product page and 40% of onward clicks return to it. |
| FAQ | 1.3% | 1.87% | 11 Shopify orders landed here. Used during product research. |
| About | 1.5% | 0.79% | 24% of onward clicks go to the product page. |
| Guarantee | 0.15% | 0% (87 sessions) | Hardly visited as a page. The guarantee message needs to be on the product page and in the cart. |
| Reviews page | 0.004% (7 views) | n/a | Unused as a standalone page. Reviews are shown on the product page (Okendo and Stamped appear as order referrers). |
| Blog | 4.3% (articles + index) | 0.19–0.40% | 7 purchases from 3,604 article landings. |

**Quiz funnel** (Klaviyo "Filled Out Form" = Typeform completions, joined by Klaviyo profile ID to Shopify "Placed Order" events; GA4 for quiz starts)

| Year | Sessions on `/pages/quiz` (GA4) | Quiz completions (Klaviyo) | Completion rate | Completers (new) | Later bought | Buy rate | Bought within 7 days |
|---|---|---|---|---|---|---|---|
| 2023 | 1,085 (May–Dec only) | 425 | n/a (GA4 covers part of the year) | 419 | 84 | 20.0% | 53 |
| 2024 | 1,918 | 349 | 18.2% | 341 | 74 | 21.7% | 62 |
| 2025 | 19,872 | 2,130 | 10.7% | 2,114 | 185 | 8.8% | 149 |
| 2026 (to 12 Oct) | 4,157 | 488 | 11.7% | 472 | 45 | 9.5% | 40 |
| **All** | | **3,395 profiles** | | **3,349** | **389 (11.6%)** | | **304 (78% of buyers)** |

The 2025 paid push sent large volumes to the quiz (Jun–Oct 2025). Completions rose about 6x, but the completion rate and the buy rate both roughly halved. First-time purchasers who completed the quiz before their first order: 2023 22.5%, 2024 21.1%, 2025 28.2%, 2026 24.1%.

---

## Q3. Funnel: sessions → add to cart → checkout → purchase

**Overall**

| Source | Sessions | Add to cart | Checkout | Purchase | CR |
|---|---|---|---|---|---|
| GA4, May 2023 – Oct 2026 (event counts) | 98,183 | 4,451 (4.5%) | 2,965 (3.0%) | 2,184 | 2.22% |
| Shopify, 2022 – Oct 2026 (sessions with step) | 112,320 | 4,500 (4.0%) | 4,352 (3.9%) | 2,391 | 2.13% |

Express and Shop Pay checkouts skip the add-to-cart step, so in some months checkouts are higher than add-to-carts.

**By year (GA4 events)**

| Year | Sessions | Add to cart | Checkout | Purchases (CR) |
|---|---|---|---|---|
| 2023 (from 10 May) | 9,288 | 504 (5.4%) | 436 (4.7%) | 362 (3.90%) |
| 2024 | 21,146 | 830 (3.9%) | 646 (3.1%) | 536 (2.53%) |
| 2025 | 46,774 | 2,101 (4.5%) | 1,393 (3.0%) | 844 (1.80%) |
| 2026 (to 12 Oct) | 22,062 | 1,016 (4.6%) | 490 (2.2%) | 442 (2.00%) |

Shopify CR by year: 2023 3.33% · 2024 2.37% · 2025 1.88% · 2026 1.79%.

**By device**

| Device | GA4 sessions | GA4 ATC | GA4 checkout | GA4 purchases | GA4 CR | Shopify sessions | Shopify cart | Shopify checkout | Shopify orders | Shopify CR |
|---|---|---|---|---|---|---|---|---|---|---|
| Mobile | 80,101 (82%) | 3,482 (4.3%) | 2,360 (2.9%) | 1,793 | 2.24% | 87,896 (78%) | 3,643 (4.1%) | 3,486 (4.0%) | 1,958 | 2.23% |
| Desktop | 17,576 (18%) | 951 (5.4%) | 599 (3.4%) | 385 | 2.19% | 23,659 (21%) | 821 (3.5%) | 825 (3.5%) | 412 | 1.74% |
| Tablet | 503 | 17 | 5 | 6 | 1.19% | 427 | 14 | 9 | 4 | 0.94% |

**By channel (GA4 session default channel group; revenue in USD)**

| Channel | Sessions | % | Engaged | ATC (rate) | Checkout (rate) | Purchases | CR | Revenue | AOV | Rev/session |
|---|---|---|---|---|---|---|---|---|---|---|
| Direct | 30,041 | 30.6% | 51% | 1,250 (4.2%) | 1,018 (3.4%) | 612 | 2.04% | $39,355 | $64 | $1.31 |
| Paid Social (Meta) | 15,595 | 15.9% | 23% | 414 (2.7%) | 173 (1.1%) | 183 | 1.17% | $11,385 | $62 | $0.73 |
| Organic Search | 14,200 | 14.5% | 60% | 1,053 (7.4%) | 793 (5.6%) | 584 | 4.11% | $40,700 | $70 | $2.87 |
| Paid Search (Google Ads) | 13,480 | 13.7% | 59% | 395 (2.9%) | 166 (1.2%) | 197 | 1.46% | $14,179 | $72 | $1.05 |
| Paid Other (Meta, ID-tagged UTMs) | 8,181 | 8.3% | 20% | 225 (2.8%) | 129 (1.6%) | 137 | 1.67% | $7,715 | $56 | $0.94 |
| Organic Social | 6,663 | 6.8% | 57% | 358 (5.4%) | 206 (3.1%) | 129 | 1.94% | $8,190 | $63 | $1.23 |
| Unassigned | 4,555 | 4.6% | 32% | 252 (5.5%) | 195 (4.3%) | 145 | 3.18% | $9,451 | $65 | $2.07 |
| Referral (incl. affiliates/partners) | 1,772 | 1.8% | 60% | 181 (10.2%) | 113 (6.4%) | 54 | 3.05% | $2,881 | $53 | $1.63 |
| Paid Shopping | 1,487 | 1.5% | 50% | 59 (4.0%) | 22 (1.5%) | 16 | 1.08% | $896 | $56 | $0.60 |
| Email (Klaviyo) | 1,190 | 1.2% | 55% | 196 (16.5%) | 115 (9.7%) | 101 | 8.49% | $7,953 | $79 | $6.68 |
| Organic Shopping | 526 | 0.5% | 55% | 63 (12.0%) | 33 (6.3%) | 24 | 4.56% | $1,933 | $81 | $3.67 |

Meta combined (Paid Social + Paid Other): 23,776 sessions, 320 purchases, 1.35% CR, $19,100.

**Mobile vs desktop CR by channel (GA4)**

| Channel | Mobile sessions | Mobile CR | Desktop sessions | Desktop CR |
|---|---|---|---|---|
| Direct | 22,647 | 2.37% | 7,240 | 1.01% |
| Organic Search | 10,311 | 4.08% | 3,839 | 4.25% |
| Paid Social | 15,427 | 1.15% | 61 | (too small) |
| Paid Search | 12,245 | 1.31% | 1,158 | 3.02% |
| Organic Social | 5,487 | 2.17% | 1,145 | 0.79% |
| Email | 798 | 9.15% | 389 | 7.20% |
| Referral | 402 | 5.97% | 1,368 | 2.19% |

**Shopify channel view (ShopifyQL referrer source, 2022 – Oct 2026)**

| Referrer source | Sessions | Cart | Checkout | Orders | CR |
|---|---|---|---|---|---|
| Direct | 63,255 | 2,381 | 2,606 | 1,293 | 2.04% |
| Search | 25,694 | 1,274 | 1,048 | 684 | 2.66% |
| Social | 20,720 | 673 | 543 | 323 | 1.56% |
| Unknown | 1,686 | 113 | 102 | 59 | 3.50% |
| Email | 248 | 38 | 31 | 18 | 7.26% |

**Order attribution (Shopify last-visit source on 2,437 one-time and first-subscription web orders, Nov 2022 – Oct 2026, CAD)**

| Source | Orders | % | First-ever orders | % of first orders | Net sales | AOV |
|---|---|---|---|---|---|---|
| Direct | 824 | 34% | 505 | 33% | $74,851 | $91 |
| Search engine (organic + untagged Google Ads) | 654 | 27% | 370 | 24% | $60,938 | $93 |
| Meta paid social (UTM-tagged) | 303 | 12% | 281 | 18% | $23,301 | $77 |
| Email (Klaviyo / mail apps) | 209 | 9% | 83 | 5% | $18,428 | $88 |
| Organic / untagged social | 186 | 8% | 148 | 10% | $15,999 | $86 |
| No visit data | 167 | 7% | 111 | 7% | $14,460 | $87 |
| holistico.ca (partner referral) | 29 | 1% | 20 | 1% | $2,203 | $76 |
| Google Shopping free listings | 17 | 1% | 17 | 1% | $1,212 | $71 |
| Other referral / Shop app / reviews / unknown | 48 | 2% | 14 | 1% | $4,344 | — |

The affiliate program can't be isolated: there is no affiliate UTM or referral-code data in GA4 or Shopify visit fields. Only one partner domain, holistico.ca, shows up.

---

## Q4. Blog: traffic and conversion

GA4, 10 May 2023 – 12 Oct 2026. Totals across 37 article URLs: 6,049 views, 3,601 landing sessions, 13 add-to-carts, **7 purchases, $392 (USD)**. 1,290 onward clicks, of which 206 (16%) went to a product page and 100 (8%) to the quiz.

| Article | Views | Landing sessions | Engaged | → Product | → Quiz | ATC | Purchases | Revenue |
|---|---|---|---|---|---|---|---|---|
| best-teas-for-hormone-balance | 1,817 | 1,639 | 40% | 20 | 2 | 0 | 0 | $0 |
| can-coffee-make-hormonal-acne-worse | 485 | 393 | 32% | 2 | 1 | 0 | 0 | $0 |
| balancing-hormones-with-food | 414 | 178 | 31% | 19 | 9 | 4 | 3 | $167 |
| hormone-safe-sunscreens | 411 | 253 | 43% | 15 | 0 | 0 | 0 | $0 |
| how-to-know-what-type-of-hormonal-acne-you-have | 368 | 249 | 33% | 17 | 29 | 1 | 1 | $39 |
| the-biggest-triggers-for-hormonal-acne-and-how-to-fix-them | 341 | 179 | 22% | 24 | 6 | 0 | 0 | $0 |
| the-best-am-pm-skincare-routine-for-hormonal-acne | 306 | 69 | 33% | 31 | 15 | 0 | 0 | $0 |
| natural-topical-ingredients-acne | 240 | 65 | 28% | 5 | 8 | 0 | 0 | $0 |
| the-truth-about-prescription-acne-medications | 216 | 96 | 25% | 3 | 3 | 0 | 0 | $0 |
| hormonal-acne-diet-building-hormone-balancing-meals | 209 | 59 | 27% | 3 | 3 | 1 | 0 | $0 |
| xenoestrogens | 181 | 34 | 38% | 3 | 2 | 1 | 0 | $0 |
| estrogen-dominance-in-women-symptoms-causes-and-natural-treatment | 166 | 60 | 38% | 26 | 4 | 1 | 1 | $42 |
| how-to-treat-hormonal-acne-in-2025 | 149 | 58 | 43% | 6 | 5 | 1 | 0 | $0 |
| can-hormonal-acne-be-caused-by-stress | 132 | 44 | 23% | 4 | 2 | 0 | 0 | $0 |
| 7-myths-and-facts-about-hormonal-acne-debunking-common-misconceptions | 105 | 37 | 32% | 7 | 2 | 0 | 0 | $0 |
| which-produce-is-worth-buying-organic | 93 | 27 | 26% | 0 | 0 | 0 | 0 | $0 |
| is-hormonal-acne-related-to-the-menstrual-cycle | 81 | 11 | 0% | 11 | 6 | 0 | 0 | $0 |
| balancing-hormones-through-diet | 75 | 49 | 29% | 2 | 0 | 2 | 1 | $40 |
| does-endometriosis-cause-adult-acne | 56 | 17 | 35% | 5 | 0 | 2 | 1 | $103 |
| building-hormone-balancing-meals | 51 | 23 | 35% | 1 | 0 | 0 | 0 | $0 |
| best-teas-for-hormonal-acne | 50 | 27 | 33% | 1 | 0 | 0 | 0 | $0 |

The other 16 articles had fewer than 25 views each. Shopify agrees: 13 orders in 4 years landed on a blog article. The articles that send the most people to the quiz or product page are the diagnostic and root-cause ones (*how-to-know-what-type…*: 29 to the quiz; *estrogen-dominance…*: 26 to product; *am-pm-routine*: 31 to product). Lifestyle articles (teas, coffee, sunscreen) attract traffic that doesn't move on. Look at Search Console before deciding what to do with any article, because some may hold ranking value that this data doesn't show.

---

## Q5. Product / variant mix, AOV, returning customers, subscriptions

**Supply-length mix, Balance, excluding wholesale** (ShopifyQL, USD; counts are orders that included each variant)

| Year | 1-month (bottle, refill) orders / share of sales | 2-month (60ct) | 3-month (3-mo, Stock-Up, Starter, 90ct) | 4-month (120ct) | Total product orders | Net sales |
|---|---|---|---|---|---|---|
| 2023 | 382 (67%) / 49% | 108 (19%) / 24% | 56 (10%) / 18% | 25 (4%) / 10% | 571 | $33,537 |
| 2024 | 749 (77%) / 64% | 101 (10%) / 13% | 107 (11%) / 19% | 16 (2%) / 4% | 973 | $48,656 |
| 2025 | 1,235 (78%) / 58% | — | 344 (22%) / 42% | — | 1,579 | $83,768 |
| 2026 (to 12 Oct) | 853 (75%) / 52% | — | 286 (25%) / 48% | — | 1,139 | $66,103 |
| **All time** | **3,223 (76%) / 56%** | 210 (5%) / 6% | **793 (19%) / 35%** | 41 (1%) / 2% | 4,267 | $232,216 |

Wholesale (BALANCE (WHOLESALE)): 19 orders, $13,486 USD (2025–26). First-ever orders (Windsor line items): 1-month 1,031 (66%), 3-month 313 (20%), legacy multi-count 216 (14%).

**Orders, AOV and new vs returning** (Windsor, CAD, excluding cancelled/voided orders; "first" = the customer's first-ever order)

| Year | Orders | Net sales (CAD) | AOV net (CAD) | AOV (USD, ShopifyQL) | First-ever orders | Repeat orders | Recurring subscription orders |
|---|---|---|---|---|---|---|---|
| 2022 (Nov–Dec) | 3 | $207 | $69.00 | $46.34 | 3 | 0 | 0 |
| 2023 | 559 | $44,038 | $78.78 | $60.39 | 327 (58%) | 232 (42%) | 76 (14%) |
| 2024 | 980 | $67,655 | $69.04 | $51.83 | 374 (38%) | 606 (62%) | 373 (38%) |
| 2025 | 1,565 | $123,651 | $79.01 | $58.84 | 626 (40%) | 939 (60%) | 626 (40%) |
| 2026 (to 12 Oct) | 1,132 | $98,545 | $87.05 | $64.74 | 232 (20%) | 900 (80%) | 625 (55%) |
| **All** | **4,239** | **$334,096** | **$78.81** | | **1,562** | **2,677** | **1,700 (40%)** |

- Customers: 1,562 in total. **43% (667) ordered more than once**, averaging 2.71 orders per customer. AOV on first orders was $82.67 CAD; on repeat orders, $76.57 CAD.
- Shopify returning-customer rate (ShopifyQL): 2023 38% · 2024 52% · 2025 44% · 2026 64%.
- **Subscriptions (Appstle):** 449 customers (29% of all customers) have subscribed. There were 495 first subscription orders and 1,700 recurring orders. Subscriptions (first + recurring orders) made up 21% of net sales in 2023, 47% in 2024, 34% in 2025 and 45% in 2026.
- What subscribers buy: first subscription orders were 81% 1-month bottles, 9% 3-month and 9% legacy multi-count. Recurring orders were 48% 1-month bottle and 48% 1-month refill. Subscribers almost always stay on a monthly cadence.
- Channel AOV (GA4, USD): Email $79, Organic Search $70, Paid Search $72, Paid Social $62.

---

## Q6. Country split over time

**Shopify orders by shipping country** (Windsor; % of net sales in CAD; "new customers" = first-ever orders)

| Year | Orders | Canada | US | Other | Sales: CA / US / Other | New customers: CA / US / Other |
|---|---|---|---|---|---|---|
| 2023 | 559 | 358 (64%) | 201 (36%) | 0 | 67% / 33% / 0% | 206 (63%) / 121 (37%) / 0 |
| 2024 | 980 | 497 (51%) | 480 (49%) | 3 | 52% / 47% / 0% | 190 (51%) / 182 (49%) / 2 |
| 2025 | 1,565 | 1,030 (66%) | 461 (29%) | 74 (5%) | 70% / 25% / 4% | 426 (68%) / 158 (25%) / 42 (7%) |
| 2026 (to 12 Oct) | 1,132 | 819 (72%) | 267 (24%) | 46 (4%) | 78% / 18% / 3% | 181 (78%) / 38 (16%) / 13 (6%) |

The "Other" orders were mainly the UK (67) and Australia (32). Most US orders were paid in CAD: across all years, only 781 orders were presented in USD.

**Shopify sessions and CR, Canada vs US** (ShopifyQL)

| Year | Canada sessions | Canada CR | US sessions | US CR |
|---|---|---|---|---|
| 2023 | 8,479 | 3.62% | 4,775 | 3.35% |
| 2024 | 10,698 | 2.78% | 10,457 | 2.28% |
| 2025 | 27,305 | 2.25% | 11,728 | 1.85% |
| 2026 | 14,489 | 2.62% | 7,445 | **0.95%** |

**GA4 sessions by country** (USD revenue; "Other" = everything that isn't Canada or the US)

| Year | Total sessions | Canada sessions / purchases / CR | US sessions / purchases / CR | Other sessions / purchases / CR |
|---|---|---|---|---|
| 2023 (from May) | 9,288 | 4,704 (51%) / 213 / 4.53% | 4,105 (44%) / 148 / 3.61% | 479 (5%) / 1 / 0.21% |
| 2024 | 21,146 | 10,826 (51%) / 297 / 2.74% | 8,881 (42%) / 235 / 2.65% | 1,439 (7%) / 4 / 0.28% |
| 2025 | 46,774 | 25,589 (55%) / 569 / 2.22% | 11,190 (24%) / 200 / 1.79% | 9,995 (21%) / 75 / 0.75% |
| 2026 | 22,062 | 13,314 (60%) / 346 / 2.60% | 4,591 (21%) / 66 / 1.44% | 4,157 (19%) / 30 / 0.72% |

**Domain move timing** (GA4 hostname): cocoonsupplements.com first shows up in September 2026 (235 sessions). From 1–12 October it had 544 sessions and 8 purchases, against 1 session on cocoonskincare.ca. That's too little data on the new domain to draw any conclusions. Klaviyo campaign names ("US Tariff Notification", 2025) suggest a tariff or pricing change for US buyers in 2025, which may explain part of the US decline. This audit doesn't confirm that.

---

## Q7. Site search terms

GA4 `search` event, 10 May 2023 – 12 Oct 2026: **309 searches by 207 users** (low volume, but useful as a signal).

| Theme | Searches | Share | Examples |
|---|---|---|---|
| Other brands / skincare products Cocoon doesn't sell | 124 | 40% | toner (8), korres kyma (4), eucerin (3+2), embryolisse (3), caudalie (4), la roche posay / uvmune (5), argan/castor/mineral oil (13), vichy, bioderma, belif, typologie, eye cream, face wash |
| Ingredients & product facts | 51 | 17% | ingredients (12 + 6 misspellings), "where this product made from" (6), dim, glutathione, diindolylmethane, vitex, saw palmetto, vitamin A, vegan, dairy, tested on animals, "approved by health canada" |
| Hormones, acne & conditions | 45 | 15% | acne (7), estrogen (8 incl. misspellings), estrogen dominance (5), quiz (3), hormone, pcos, melasma, spironolactone, adapalene, azelaic acid, "how to know you have hormonal acne" |
| Orders, returns, subscriptions, contact | 35 | 11% | return (5), subscription/cancel subscription/how to cancel (10), money back guarantee (2), review (2), shipping, change payment, update address |
| Balance product / variants | 33 | 11% | balance (17), refill, 60ct, 90 days, "BALANCE -90ct", supplement |
| Safety / compatibility | 21 | 7% | pregnancy (4), birth control / the pill (6), side effects (3), weight gain (3), headache, red urine, detox symptoms |

People expected skincare products from "Cocoon Skincare". The remaining searches are pre-purchase questions (ingredients, safety, compatibility with the pill) that a product page should answer directly.

---

## Q8. Klaviyo and ads (secondary)

**Google Ads** (all campaigns, full history; platform-reported conversions, which GA4 doesn't confirm: GA4 credits Paid Search with 197 purchases in total)

| Campaign | Clicks | Spend | Conv. | Conv. value |
|---|---|---|---|---|
| Sales \| Search \| Clicks \| June 2025 | 12,142 | $13,291 | 362.5 | $37,528 |
| Sales \| Shopping \| Clicks \| Nov 2025 | 1,651 | $2,040 | 30.8 | $2,685 |
| US Sales \| Search \| Clicks \| May 2026 | 249 | $1,515 | 5 | $326 |
| June 2023 / June 2025 (small tests) | 278 | $450 | 0 | $0 |

**Google Ads search terms grouped by theme** (search-term report; 8,412 clicks are covered, because low-volume terms are hidden)

| Theme | Clicks | Spend | Conv. | Conv./click | Cost/conv. |
|---|---|---|---|---|---|
| Brand ("cocoon …") | 646 | $453 | 86 | 13.3% | $5 |
| Hormonal acne (incl. "hormonal acne supplements") | 1,904 | $2,077 | 43 | 2.2% | $48 |
| Ingredient (DIM / glutathione / CDG) | 130 | $306 | 3 | 2.3% | $102 |
| Acne, general ("how to get rid of acne" etc.) | 3,925 | $3,837 | 28 | 0.7% | $138 |
| Hormone balance, general | 567 | $539 | 1 | 0.2% | $403 |
| Supplement/vitamin, generic | 268 | $552 | 0 | 0% | — |
| Estrogen / estrogen dominance | 71 | $70 | 0 | 0% | — |

Top converting non-brand terms: "hormonal acne supplements" (143 clicks, 10.5 conv.), "hormonal acne treatment" (143 clicks, 6.8), "supplements for hormonal acne" (49 clicks, 3.0). The biggest informational terms ("how to get rid of acne": 350 clicks; "hormonal acne": 177; "how to get rid of hormonal acne": 108) produced **0 conversions**. People searching with buying intent want a product page. People searching for information belong on content and quiz pages. ("Treatment" wording can't be used on the US site; see the claims rule.)

**Meta Ads, 2025 – Oct 2026** (platform-reported purchases; GA4 credits all Meta traffic with 320 purchases over its whole history)

| Campaign | Spend | Link clicks | Purchases | Value |
|---|---|---|---|---|
| Sales \| June 2025 | $11,972 | 4,418 | 320 | $39,726 |
| Balance \| Sales \| Evergreen Winners | $4,549 | 2,003 | 40 | $5,388 |
| Awareness Video Views | $2,558 | 418 | 0 | $0 |
| Balance \| Sales \| Creative Testing | $2,371 | 746 | 25 | $3,634 |
| Cocoon Balance \| Sales \| Creative Testing | $1,919 | 711 | 27 | $4,662 |
| Feb Awareness (Reach) | $1,067 | 751 | 0 | $0 |
| Feb Conversion Campaign | $1,039 | 497 | 24 | $3,260 |
| New Year Sale 2025 Manual Conversion | $822 | 191 | 24 | $1,782 |
| 2025 Spring Sale Campaign | $511 | 99 | 0 | $0 |
| 2026 Spring Sale Retargeting | $414 | 126 | 13 | $2,554 |

Meta traffic has the lowest engagement of any channel (Paid Social 23% engaged, Paid Other 20%). 87% of Meta landings went to the product page (20,791 of 23,776 GA4 sessions).

**Klaviyo campaigns, 2025 – Oct 2026 (top by conversions)**

| Campaign | Recipients | Conv. | Value | Click rate |
|---|---|---|---|---|
| BFCM 2025 – Nov 24 Launch (buyers) | 770 | 16 | $1,617 | 2.6% |
| BFCM 2025 – Nov 28 (buyers) | 774 | 16 | $1,501 | 1.6% |
| 2026 New Year Sale | 3,995 | 15 | $1,316 | 0.7% |
| BFCM 2025 – Dec 1 (all) | 4,241 | 10 | $2,173 | 0.5% |
| Spring Sale 2026 – Apr 6 Launch | 4,578 | 10 | $1,113 | 0.9% |
| Price Increase Notice – Appstle subscribers | 141 | 10 | $579 | 5.0% |
| Spring Sale 2026 – Apr 9 | 4,565 | 9 | $1,222 | 0.6% |
| Flash Sale 2026 – Aug 29 | 4,906 | 9 | $1,243 | 0.6% |
| Refills Are Back | 4,523 | 9 | $913 | 0.5% |
| 2025 Spring Sale | 1,406 | 9 | $827 | 1.2% |

Emails to past buyers convert far better than emails to non-buyers. In the BFCM 2025 launch, 770 buyers produced 16 conversions while 3,517 non-buyers produced 2. Educational newsletters produced 0–5 conversions each. Sales and bundle or refill announcements drive most email revenue. The email channel converts at 8.5% in GA4 (the highest of any channel), so the site should make email signup easy, through the quiz and a footer form.

---

## Questions not answered or only partly answered

| Question | Status | Why |
|---|---|---|
| Full multi-step session paths (e.g. home → quiz → results → product → purchase as a single sequence) | Partly | GA4 path exploration, entrances and exits aren't available through Windsor. One-step referrer pairs plus a Klaviyo quiz → order join were used instead. |
| History before May 2023 (GA4) and before Nov 2022 (Shopify) | Not available | GA4 starts 10 May 2023 and UA data is gone. This Shopify store's first order is #1001 on 30 Nov 2022. If the brand sold from about 2020, that history is in another store or platform. |
| Affiliate program performance | Not answerable | There is no affiliate UTM, referral code or discount-code mapping in GA4 or Shopify visit data. The `/pages/affiliate-program` page got 344 views and no sales. An affiliate-app export would be needed. |
| Reviews page role | Answered: effectively unused | 7 views in 3.4 years. Reviews appear to be embedded on the product page (Okendo/Stamped referrals). |
| Klaviyo flows (welcome, quiz follow-up, abandoned cart) performance | Not answered | The Windsor Klaviyo flow report timed out three times. Campaigns were pulled instead. Worth pulling directly from Klaviyo, because the quiz's value depends on its follow-up flow. |
| Meta history before Sept 2023 | Not available | The Meta API limits data to 37 months. |
| Search Console queries | Out of scope here | Covered by the separate SEO audit (`sc-domain:cocoonskincare.ca`). Needed before deciding which blog URLs and pages to keep. |
| Conversion on cocoonsupplements.com specifically | Too early | The new domain has had GA4 data only since September 2026 (779 sessions, 8 purchases). |
