# SEO data audit: cocoonskincare.ca → cocoonsupplements.com

Prepared 13 Oct 2026 for the website restructure. This is a read-only audit: nothing was changed in Shopify, Google Ads or anywhere else.

**Sources and date ranges**
- **Google Search Console** (`sc-domain:cocoonskincare.ca`, via Windsor.ai): **13 Jun 2025 to 11 Oct 2026**. That is the full ~16 months the API keeps; the earliest day it accepts is 13 Jun 2025 and the latest day with data is 11 Oct 2026.
- **Google Ads** (account 742-164-2243, via Windsor.ai): search terms and campaigns, **Jun 2025 to 12 Oct 2026**. The account has no data before June 2025.
- **Google Keyword Planner** (through the same Google Ads connection): US, English, Google Search, average monthly searches over the past 12 months. Treat these as Google's rounded estimates.
- **Live site** (`curl`, 13 Oct 2026): home, /products/balance, /pages/quiz, /pages/learn, /blogs/cocoon-blog, plus sitemap.xml, products.json and the status code of every URL Search Console knows about.

**Read this before using the numbers**
- Every query figure below is a **Search Console impression** (the number of times a cocoonskincare.ca page appeared in results) or a click. **Impressions are not search volume.** They only count searches where we already showed up, so a topic where we rank on page 6 gets few impressions even if lots of people search for it. The only real search volumes in this file are in section 7 (Keyword Planner), and they are labelled.
- **Query-level data does not cover all traffic.** Google hides rare/anonymised queries. Rows with a query add up to 2,755 clicks and 124,791 impressions, but the site as a whole got 6,136 clicks and 353,603 impressions (from the monthly totals). Page-level totals (section 4) do include the hidden queries, so they are the right numbers for the redirect list.
- **Country split:** query × country covers US + Canada only (1,964 clicks / 85,607 impressions). Site-wide country totals are complete. A page × country pull came back much lower than the page totals (for example the home page: 1,484 clicks for US + CA against 3,270 in total), so I have not used it.
- **Average position** for a group of queries is weighted by impressions.
- **The domain move shows in the data.** Daily impressions for cocoonskincare.ca dropped from about 520 to 600 a day (1 to 3 Oct) to 243 on 4 Oct and 65 to 150 a day from 5 to 11 Oct 2026. That fits Google starting to follow redirects to the new domain, but **we can't see the new domain's performance because cocoonsupplements.com isn't connected to Search Console yet.**

---

## What this means for the new site

1. **Connect cocoonsupplements.com to Search Console now, then run Change of Address.** Our .ca impressions fell about 85% after 4 Oct. Without the new property we can't confirm the redirects are passing equity, and we can't track the US. Submit `https://cocoonsupplements.com/sitemap.xml` and keep the .ca domain registered and connected in Shopify (redirecting) for at least a year. I couldn't test the .ca → .com 301s from this environment, because the network proxy blocks cocoonskincare.ca.
2. **Most of today's organic traffic is brand traffic, so protect brand searches first.** Brand queries brought in **84.6% of the clicks we can attribute to a query** (2,332 of 2,755), and the US and Canada are about the same (86% and 87%). Non-brand queries got 86.7% of the impressions but only 413 clicks in 16 months. The biggest brand query is **"cocoon skin care / cocoon skincare"** (6,114 impressions, 833 clicks), and that name is about to change. Keep "Cocoon (formerly Cocoon Skincare)" in visible copy and in Organization schema (`alternateName`) for the transition. Google Ads backs this up: brand terms produced about 85 of the ~164 conversions that can be traced to a search term.
3. **The biggest commercial gap is "supplements for hormonal acne", and no page clearly owns it.** That cluster had 10,077 impressions at an average position of 27.8 and brought 41 clicks. The home page (44% of those impressions) and the Balance page (33%) compete with each other for it. "Hormonal acne supplements" ranks 10.8 in Canada but 20.9 in the US, and "supplements for hormonal acne" ranks 10.3 in Canada against 34.1 in the US. In Google Ads, these are the non-brand terms that convert. Give the term **one owner**. I recommend the home page, since it already holds the most equity for it. The new shop-all collection should take "clear skin supplements" / "acne supplements", and Balance should take its ingredients (DIM and estrogen metabolism). Details are in section 8.
4. **Keep the tea article's URL exactly as it is and refresh the article.** `/blogs/cocoon-blog/best-teas-for-hormone-balance` is the biggest non-brand asset on the site: **156,535 impressions and 1,049 clicks**, with 335 clicks in Jul to Sep 2026 alone. It has 96 striking-distance tea queries (32,782 impressions) sitting at positions 5 to 11. Pushing these into the top 3 is the cheapest traffic gain available. The post also needs a clear path to the quiz and to Balance.
5. **Fix the coffee and diet articles: they get seen but not clicked.** The coffee article had 48,320 impressions but a 0.1% CTR, at position 14. Its title doesn't match the way people search ("does coffee cause acne" and similar). "Hormonal acne diet" had 1,607 impressions at position 56, and the whole diet cluster got 0 clicks. There are now two diet posts (`balancing-hormones-with-food` and `hormonal-acne-diet-building-hormone-balancing-meals`) competing for the same term. Merge them into one and 301 the other.
6. **The US is where the growth is, and our US rankings are weaker.** Over the period, the US gave us 139,076 impressions against Canada's 77,304. But it gave fewer clicks (1,652 against 2,459) at worse positions (13.7 against 10.3). Write all new copy in US English and for US searches.
7. **Quiz demand comes mostly from the US, and the quiz page isn't optimised for it.** The quiz cluster had 5,566 impressions, 81% from the US, at an average position of 36. People search "acne quiz", "what type of acne do I have quiz" and "what is causing my acne quiz". The page's title is about "high estrogen" and is 69 characters long. Branded "hormonal acne quiz" already ranks at position 2.4 with a 15% CTR, so retitling the page around "acne quiz" is a low-risk win.
8. **"Treatment" wording has almost no organic value for us, so the compliance fix costs little.** Queries containing treat/treatment/cure/heal/remedy/get rid of/medication/fix total 2,119 impressions and **2 clicks**, mostly at positions 40 to 80. But the live site still says "Treat Hormonal Acne" in the home title and "Natural Hormonal Acne Treatment" in the About title, uses product tags like "Hormonal Acne Treatment" and "Hormonal Pimples Treatment", and has product type "Skincare". **None of the five audited pages shows a DSHEA disclaimer.** Section 8 has compliant wording. `[CLAIM CHECK]`
9. **Ingredient searches are large, but "internal skincare" isn't a search term.** In US Keyword Planner, "DIM supplement" gets 27,100 searches a month, "DIM supplement for women" 5,400, "estrogen dominance" 8,100, "calcium d-glucarate" 6,600, "hormone balance supplements for women" 2,400 and "supplements for pimples" 2,900. **"Internal skincare" gets 20.** Use "internal skincare" as the brand idea and tagline, not as a keyword. Keyword Planner returned **no rows at all for any seed containing "acne"**, so we still have no real search volume for acne terms.
10. **Redirect list:** 64 URLs have Search Console data (section 4). Every content URL that matters already resolves on the new domain at the same path. **Eleven old URLs return 404 on cocoonsupplements.com and need 301s.** The most important is `/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2025` (854 impressions), which should go to the 2026 version. The rest are `/pages/refund-policy` and nine malformed blog URLs. Google Merchant Center still sends `/products/balance?…country=CA&currency=CAD` links, so the product feed needs to switch to the .com domain and USD.

---
## 1. Trend: whole site, US and Canada (Search Console, by month)

| Month | All clicks | All impr. | All avg pos | US clicks | US impr. | US pos | CA clicks | CA impr. | CA pos |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Jun 2025 (from 13th) | 93 | 7,622 | 30.5 | 23 | 2,952 | 29.0 | 42 | 1,178 | 12.1 |
| Jul 2025 | 277 | 12,801 | 30.6 | 55 | 5,282 | 32.6 | 106 | 3,411 | 25.5 |
| Aug 2025 | 820 | 14,609 | 29.0 | 291 | 6,710 | 31.2 | 138 | 3,667 | 21.0 |
| Sep 2025 | 545 | 11,286 | 20.8 | 233 | 5,313 | 24.5 | 137 | 3,139 | 14.6 |
| Oct 2025 | 332 | 7,844 | 11.1 | 119 | 3,056 | 11.9 | 119 | 2,695 | 9.8 |
| Nov 2025 | 372 | 10,885 | 11.4 | 83 | 3,310 | 14.9 | 196 | 4,832 | 8.2 |
| Dec 2025 | 286 | 9,743 | 15.9 | 69 | 3,591 | 22.0 | 157 | 3,429 | 10.6 |
| Jan 2026 | 343 | 21,702 | 11.9 | 69 | 8,605 | 14.0 | 204 | 6,125 | 9.4 |
| Feb 2026 | 337 | 22,220 | 9.6 | 79 | 8,471 | 11.2 | 181 | 5,604 | 8.1 |
| Mar 2026 | 393 | 31,386 | 8.6 | 89 | 14,189 | 8.9 | 202 | 7,121 | 8.6 |
| Apr 2026 | 454 | 39,987 | 7.8 | 123 | 17,952 | 8.2 | 215 | 8,842 | 6.8 |
| May 2026 | 386 | 33,886 | 10.3 | 116 | 15,069 | 10.6 | 155 | 6,877 | 9.1 |
| Jun 2026 | 326 | 24,490 | 10.8 | 83 | 10,976 | 11.8 | 174 | 5,453 | 9.7 |
| Jul 2026 | 325 | 27,150 | 10.7 | 68 | 12,075 | 11.4 | 164 | 5,127 | 9.0 |
| Aug 2026 | 323 | 26,956 | 10.8 | 76 | 12,366 | 11.0 | 135 | 5,166 | 8.7 |
| Sep 2026 | 299 | 19,031 | 8.5 | 72 | 8,343 | 9.2 | 122 | 4,049 | 7.9 |
| Oct 2026 (1st to 11th) | 25 | 2,005 | 9.4 | 4 | 816 | 10.1 | 12 | 589 | 9.8 |
| **Total** | **6,136** | **353,603** | | **1,652** | **139,076** | **13.7** | **2,459** | **77,304** | **10.3** |

Site-wide by country for the whole period: Canada 2,459 clicks / 77,304 impressions; US 1,652 / 139,076; UK 354 / 16,021; Australia 202 / 9,036; every other country is under 100 clicks.

How to read it: the jump in impressions from Jan to Apr 2026 is almost entirely the tea article starting to rank (9,410 impressions in Jan, 26,095 in Apr). Clicks stayed at roughly 300 to 450 a month because most of those impressions are informational and US-based. The August 2025 spike (820 clicks) came from the home page (644 clicks that month), which points to a burst of brand searches.

## 2. Query clusters (themes)

I sorted every query into one theme using keyword rules (the first matching rule wins, in the order: brand, then topic, then supplement wording, then general). Totals are for queries Google discloses. "Main ranking page" is the page with the largest share of that cluster's impressions.


| Cluster | Queries | Impr. | Clicks | CTR | Avg pos (impr-weighted) | US impr. | CA impr. | Main ranking page (share of cluster impr.) | Top queries |
|---|---:|---:|---:|---:|---:|---:|---:|---|---|
| Teas for hormones / acne | 2855 | 47,178 | 252 | 0.5% | 8.1 | 21,777 | 6,909 | /blogs/cocoon-blog/best-teas-for-hormone-balance (100%); /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse (0%) | tea for hormonal acne, tea for hormonal imbalance, best tea for hormonal acne, what tea is good for acne |
| Coffee / caffeine and acne | 408 | 15,915 | 13 | 0.1% | 22.8 | 5,984 | 4,734 | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse (100%); /blogs/cocoon-blog/best-teas-for-hormone-balance (0%) | does coffee cause acne, coffee and acne, does caffeine cause acne, can coffee cause acne |
| Brand: Cocoon (ours) | 158 | 11,434 | 2,332 | 20.4% | 4.6 | 3,743 | 3,439 | / (20%); /pages/results (14%) | cocoon skin care, cocoon skincare, cocoon supplement, cocoon acne supplement |
| Supplements for hormonal acne | 160 | 10,077 | 41 | 0.4% | 27.8 | 3,365 | 3,394 | / (44%); /products/balance (33%) | hormonal acne supplements, supplements for hormonal acne, hormonal acne supplement, natural supplements for hormonal acne |
| Supplements for acne / clear skin (non-hormonal wording) | 265 | 6,772 | 26 | 0.4% | 23.1 | 1,006 | 5,282 | / (45%); /products/balance (37%) | acne supplements, acne supplements canada, skincare supplement, supplements for acne |
| Acne / hormone quizzes | 92 | 5,566 | 52 | 0.9% | 36.4 | 4,523 | 212 | /pages/quiz (98%); /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have (2%) | acne quiz, what type of acne do i have quiz, what is causing my acne quiz, what kind of acne do i have quiz |
| Brand: ambiguous "cocoon" (other businesses / bare word) | 81 | 5,171 | 10 | 0.2% | 15.7 | 711 | 4,106 | / (54%); /pages/shipping-policy (8%) | cocoon, cocoon delivery, cocoon apothecary, cocooncenter canada |
| Hormonal acne: what / causes / types | 377 | 3,822 | 2 | 0.1% | 51.2 | 1,342 | 1,288 | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have (34%); /blogs/cocoon-blog/balancing-hormones-with-food (31%) | how to balance hormones for acne, hormonal acne, hormonal acne types, fungal acne vs hormonal acne |
| Diet / food | 140 | 3,630 | 0 | 0.0% | 54.9 | 2,213 | 196 | /blogs/cocoon-blog/balancing-hormones-with-food (97%); /blogs/cocoon-blog/which-produce-is-worth-buying-organic (2%) | hormonal acne diet, hormonal imbalance acne diet, foods for hormonal imbalance acne, foods for hormonal acne |
| Sunscreen / endocrine disruptors | 209 | 2,568 | 4 | 0.2% | 16.0 | 1,607 | 233 | /blogs/cocoon-blog/hormone-safe-sunscreens (94%); /blogs/cocoon-blog/xenoestrogens (6%) | how to choose sunscreen that doesn’t mess with hormones, sunscreen without endocrine disruptors, hormone safe sunscreen, hormone-friendly sunscreen ingredients |
| Estrogen dominance / high estrogen / progesterone | 463 | 2,452 | 8 | 0.3% | 23.1 | 1,091 | 743 | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have (61%); /blogs/cocoon-blog/best-teas-for-hormone-balance (17%) | estrogen dominance acne, low progesterone acne, does low progesterone cause acne, can low progesterone cause acne |
| General acne (non-hormonal wording) | 348 | 2,084 | 2 | 0.1% | 30.7 | 860 | 793 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications (24%); /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse (21%) | best organic acne treatments, do oral acne medicines often cause dry skin, headaches, or mood changes?, acne wuiz, aldactone acne |
| How to treat / get rid of / fix hormonal acne | 155 | 1,516 | 2 | 0.1% | 45.3 | 651 | 543 | /blogs/cocoon-blog/balancing-hormones-with-food (27%); /pages/learn (23%) | foods that help hormonal acne, hormonal acne treatment, best herbs for hormonal acne, herbs for hormonal acne |
| Prescription meds (spironolactone, Accutane, etc.) | 210 | 1,392 | 0 | 0.0% | 50.6 | 720 | 290 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications (97%); /blogs/cocoon-blog/natural-topical-ingredients-acne (1%) | hormonal acne medication, does accutane help hormonal acne, hormonal acne prescription, how does acne medication work |
| Other / unrelated | 822 | 1,280 | 2 | 0.2% | 14.9 | 447 | 488 | /blogs/cocoon-blog/best-teas-for-hormone-balance (58%); / (23%) | clearzine, infusiones para el acné, bell clear skin, yes |
| Stress / cortisol | 89 | 896 | 0 | 0.0% | 51.4 | 416 | 84 | /blogs/cocoon-blog/can-hormonal-acne-be-caused-by-stress (99%); /blogs/cocoon-blog/the-biggest-triggers-for-hormonal-acne-and-how-to-fix-them (0%) | stress hormonal acne, cortisol and acne, hormonal acne and stress, cortisol acne |
| Topicals / skincare routine | 114 | 869 | 1 | 0.1% | 41.5 | 292 | 409 | / (53%); /blogs/cocoon-blog/natural-topical-ingredients-acne (17%) | hormonal skincare, best natural skincare for hormonal acne, best skin care products for hormonal acne, affordable acne skincare bundles money-back guarantee |
| DIM | 35 | 542 | 2 | 0.4% | 14.0 | 14 | 510 | /products/balance (98%); /blogs/cocoon-blog/the-truth-about-prescription-acne-medications (1%) | dim supplement for acne, dim supplement acne, dim acne supplement, dim supplement for hormonal acne |
| Hormone balance / imbalance (general) | 121 | 484 | 3 | 0.6% | 18.8 | 114 | 51 | /blogs/cocoon-blog/best-teas-for-hormone-balance (68%); /blogs/cocoon-blog/hormone-safe-sunscreens (14%) | teh untuk jerawat hormon, té para el acné hormonal, infusiones para el acné hormonal, sun protection hormonal health |
| Affiliate / wholesale | 8 | 469 | 1 | 0.2% | 8.6 | 449 | 4 | /pages/affiliate-program (100%) | acne affiliate programs, acne affiliate program, best acne affiliate programs, affiliate program |
| Other named ingredients (glutathione, CDG, zinc, probiotics, etc.) | 109 | 303 | 0 | 0.0% | 35.4 | 117 | 123 | /blogs/cocoon-blog/hormone-safe-sunscreens (31%); /products/balance (28%) | clear skin probiotics, calcium d glucarate acne, calcium d glucarate for acne, is zinc oxide safe |
| Chin / jawline / location acne | 108 | 260 | 0 | 0.0% | 54.6 | 42 | 207 | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have (67%); /pages/learn (19%) | hormonal breakouts on chin, hormonal breakouts on forehead, hormonal acne cheeks, cheek acne hormonal |
| Endometriosis / perimenopause / cycle | 48 | 48 | 0 | 0.0% | 12.6 | 25 | 10 | /blogs/cocoon-blog/best-teas-for-hormone-balance (54%); /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have (29%) | 7 natural menopause treatments that really work, acne breakout during ovulation, acne flare up during ovulation, acne in perimenopause |
| Birth control / post-pill | 17 | 32 | 2 | 6.2% | 27.7 | 15 | 16 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications (41%); /products/balance (25%) | post pill acne supplements, norlyda birth control skin, can iud cause acne, acne after copper iud removal |
| Gut / liver | 6 | 25 | 0 | 0.0% | 71.5 | 3 | 11 | /pages/shipping-policy (88%); /blogs/cocoon-blog/best-teas-for-hormone-balance (8%) | skincare delivery, benefits of beef liver for women, estimated delivery times, gut gegen akne |
| PCOS | 6 | 6 | 0 | 0.0% | 38.7 | 3 | 2 | /products/balance (67%); /blogs/cocoon-blog/the-truth-about-prescription-acne-medications (17%) | does it help with pcos, how to increase progesterone in pcos, pcos acne supplements, supplements for pcos acne |

What stands out:
- **Tea alone is 44% of all non-brand impressions** (47,178 of 108,186). It ranks well (position 8.1) but converts readers poorly into clicks (0.5%), and probably into sales too, since it's informational.
- **The commercial clusters rank worst.** "Supplements for hormonal acne" sits at position 27.8 and "supplements for acne / clear skin" at 23.1, together 16,849 impressions and 67 clicks. That is exactly the traffic the shop needs.
- **Diet, causes/types, stress, prescription meds and chin/jawline all rank around positions 45 to 55** and get almost no clicks. These are content gaps, not equity to protect.
- **Hardly anyone finds us through PCOS, birth control or gut** (6 to 32 impressions each). We have no presence there yet, so anything we build there is new ground.
- **The bare word "cocoon" is ambiguous** (2,710 impressions at 0.2% CTR, mostly Canada, alongside Cocoon Apothecary, Cocooncenter and others). Lean on "Cocoon Supplements" as the brand phrase.

---

## 3. Striking-distance opportunities

These are queries with an average position of 5 to 20, at least 100 impressions and no brand term: a page that matches the query better could reach the top 3. They are sorted by impressions.

**By cluster**


| Cluster | Queries | Impr. | Clicks |
|---|---:|---:|---:|
| Teas for hormones / acne | 96 | 32,782 | 193 |
| Coffee / caffeine and acne | 23 | 5,387 | 9 |
| Supplements for hormonal acne | 2 | 3,610 | 21 |
| Supplements for acne / clear skin (non-hormonal wording) | 5 | 2,785 | 18 |
| Sunscreen / endocrine disruptors | 4 | 1,072 | 1 |
| Estrogen dominance / high estrogen / progesterone | 5 | 921 | 6 |
| Acne / hormone quizzes | 3 | 824 | 6 |
| Affiliate / wholesale | 1 | 418 | 1 |
| DIM | 1 | 197 | 1 |
| General acne (non-hormonal wording) | 1 | 144 | 0 |
| How to treat / get rid of / fix hormonal acne | 1 | 143 | 0 |
| Hormonal acne: what / causes / types | 1 | 103 | 1 |

**All striking-distance queries (143)**


| # | Query | Impr. | Clicks | CTR | Avg pos | US impr. | CA impr. | Cluster | Page ranking now | "Treat"-type wording? |
|---|---|---:|---:|---:|---:|---:|---:|---|---|---|
| 1 | hormonal acne supplements | 3,480 | 20 | 0.6% | 17.2 | 502 | 1,968 | Supplements for hormonal acne | / |  |
| 2 | tea for hormonal acne | 2,225 | 29 | 1.3% | 5.7 | 1,015 | 153 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 3 | tea for hormonal imbalance | 2,117 | 6 | 0.3% | 10.7 | 218 | 208 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 4 | best tea for hormonal acne | 1,801 | 14 | 0.8% | 5.2 | 635 | 134 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 5 | what tea is good for acne | 1,217 | 0 | 0.0% | 10.2 | 1,025 | 127 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 6 | best tea for hormonal imbalance | 1,027 | 3 | 0.3% | 7.9 | 136 | 140 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 7 | best tea for acne | 1,022 | 5 | 0.5% | 8.4 | 331 | 412 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 8 | herbal tea for acne | 883 | 6 | 0.7% | 10.2 | 645 | 55 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 9 | acne supplements | 864 | 3 | 0.4% | 13.0 | 12 | 840 | Supplements for acne / clear skin (non-hormonal wording) | / |  |
| 10 | acne supplements canada | 796 | 7 | 0.9% | 9.0 | 5 | 780 | Supplements for acne / clear skin (non-hormonal wording) | / |  |
| 11 | what tea is good for hormonal acne | 796 | 7 | 0.9% | 5.1 | 489 | 49 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 12 | herbal teas for acne | 765 | 5 | 0.7% | 5.9 | 100 | 17 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 13 | what tea helps with acne | 724 | 0 | 0.0% | 9.1 | 600 | 82 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 14 | what tea helps with hormonal acne | 626 | 1 | 0.2% | 5.3 | 463 | 28 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 15 | hormonal acne tea | 575 | 7 | 1.2% | 6.8 | 181 | 29 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 16 | tea that helps with acne | 553 | 1 | 0.2% | 11.4 | 466 | 41 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 17 | teas for hormonal acne | 549 | 18 | 3.3% | 5.1 | 311 | 37 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 18 | tea to balance female hormones | 543 | 3 | 0.5% | 8.6 | 220 | 110 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 19 | best herbal tea for hormonal imbalance | 538 | 2 | 0.4% | 9.0 | 60 | 15 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 20 | estrogen tea | 516 | 2 | 0.4% | 8.6 | 309 | 60 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 21 | how to choose sunscreen that doesn’t mess with hormones | 506 | 0 | 0.0% | 6.7 | 502 | 0 | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |  |
| 22 | supplements for acne | 474 | 1 | 0.2% | 16.5 | 19 | 426 | Supplements for acne / clear skin (non-hormonal wording) | / |  |
| 23 | what tea is good for hormonal imbalance | 473 | 3 | 0.6% | 8.9 | 167 | 59 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 24 | herbal tea for hormonal imbalance | 465 | 1 | 0.2% | 9.7 | 103 | 27 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 25 | which tea is good for hormonal imbalance | 449 | 2 | 0.4% | 8.6 | 30 | 64 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 26 | teas that help with acne | 448 | 6 | 1.3% | 7.5 | 291 | 46 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 27 | acne affiliate programs | 418 | 1 | 0.2% | 6.7 | 413 | 1 | Affiliate / wholesale | /pages/affiliate-program |  |
| 28 | does coffee make you break out | 415 | 0 | 0.0% | 13.8 | 156 | 149 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 29 | can coffee cause hormonal acne | 414 | 1 | 0.2% | 8.8 | 269 | 48 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 30 | caffeine and acne | 392 | 0 | 0.0% | 16.2 | 106 | 187 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 31 | estrogen dominance acne | 371 | 4 | 1.1% | 11.0 | 133 | 132 | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 32 | best tea for estrogen dominance | 365 | 0 | 0.0% | 5.6 | 208 | 47 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 33 | tea for acne | 357 | 0 | 0.0% | 10.8 | 152 | 195 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 34 | skin supplements for acne | 350 | 0 | 0.0% | 16.6 | 1 | 347 | Supplements for acne / clear skin (non-hormonal wording) | / |  |
| 35 | hormonal imbalance tea | 348 | 2 | 0.6% | 8.9 | 72 | 29 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 36 | what is causing my acne quiz | 344 | 4 | 1.2% | 12.1 | 229 | 30 | Acne / hormone quizzes | /pages/quiz |  |
| 37 | dandelion tea for acne | 334 | 2 | 0.6% | 9.3 | 148 | 70 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 38 | teas for hormonal balance | 330 | 1 | 0.3% | 9.3 | 86 | 75 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 39 | can caffeine cause acne | 322 | 0 | 0.0% | 19.8 | 44 | 219 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 40 | can coffee make you break out | 322 | 0 | 0.0% | 14.5 | 101 | 119 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 41 | is coffee bad for acne | 320 | 0 | 0.0% | 18.8 | 40 | 201 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 42 | best teas for acne | 314 | 5 | 1.6% | 6.7 | 46 | 102 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 43 | best tea for hormone balance | 306 | 0 | 0.0% | 10.1 | 100 | 63 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 44 | what teas help with acne | 306 | 0 | 0.0% | 8.9 | 238 | 20 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 45 | caffeine acne | 304 | 0 | 0.0% | 16.1 | 107 | 120 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 46 | acne supplement | 301 | 7 | 2.3% | 10.8 | 10 | 276 | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |  |
| 47 | tea that helps with hormonal acne | 300 | 2 | 0.7% | 5.8 | 196 | 11 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 48 | hormone balance tea | 288 | 0 | 0.0% | 10.7 | 121 | 104 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 49 | teas that help with hormonal imbalance | 287 | 0 | 0.0% | 10.3 | 180 | 9 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 50 | teas that help with hormonal acne | 285 | 3 | 1.1% | 5.2 | 200 | 17 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 51 | el café es malo para el acné hormonal | 284 | 1 | 0.4% | 5.6 | 37 | 0 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 52 | coffee and hormonal acne | 267 | 3 | 1.1% | 7.1 | 172 | 20 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 53 | what tea helps acne | 265 | 0 | 0.0% | 9.5 | 229 | 27 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 54 | el cafe causa acne | 263 | 0 | 0.0% | 10.8 | 32 | 0 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 55 | what tea is best for acne | 261 | 0 | 0.0% | 8.5 | 195 | 42 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 56 | hormone balancing tea | 257 | 1 | 0.4% | 14.2 | 40 | 112 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 57 | which tea is best for hormonal imbalance | 251 | 1 | 0.4% | 7.5 | 30 | 34 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 58 | caffeine and hormonal acne | 249 | 1 | 0.4% | 5.2 | 111 | 82 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 59 | hormonal tea | 248 | 2 | 0.8% | 8.7 | 51 | 41 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 60 | herbal tea for acne skin | 247 | 1 | 0.4% | 9.6 | 231 | 6 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 61 | why am i breaking out quiz | 240 | 1 | 0.4% | 11.7 | 209 | 3 | Acne / hormone quizzes | /pages/quiz |  |
| 62 | why do i have acne quiz | 240 | 1 | 0.4% | 13.6 | 196 | 11 | Acne / hormone quizzes | /pages/quiz |  |
| 63 | is coffee bad for hormonal acne | 236 | 0 | 0.0% | 8.0 | 116 | 25 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 64 | which tea is good for hormonal acne | 230 | 3 | 1.3% | 5.4 | 58 | 25 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 65 | best teas for hormone balance | 227 | 2 | 0.9% | 8.1 | 40 | 43 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 66 | sunscreen without endocrine disruptors | 226 | 0 | 0.0% | 8.2 | 89 | 12 | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |  |
| 67 | tea for hormone balance | 225 | 0 | 0.0% | 10.4 | 118 | 96 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 68 | what teas are good for acne | 225 | 0 | 0.0% | 6.8 | 161 | 30 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 69 | what tea helps hormonal acne | 221 | 2 | 0.9% | 5.3 | 173 | 18 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 70 | teas for acne | 219 | 2 | 0.9% | 8.6 | 124 | 65 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 71 | raspberry leaf tea estrogen dominance | 218 | 6 | 2.8% | 7.1 | 141 | 21 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 72 | herbal tea for hormonal acne | 217 | 3 | 1.4% | 5.7 | 71 | 10 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 73 | does black coffee cause acne | 216 | 0 | 0.0% | 18.1 | 56 | 105 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 74 | hormone balancing teas | 216 | 0 | 0.0% | 12.3 | 182 | 16 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 75 | tea good for hormonal acne | 215 | 3 | 1.4% | 5.4 | 114 | 18 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 76 | hormonal imbalance tea for females | 214 | 2 | 0.9% | 8.5 | 83 | 8 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 77 | what teas help with hormonal acne | 206 | 2 | 1.0% | 5.5 | 178 | 8 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 78 | can coffee break you out | 202 | 1 | 0.5% | 8.9 | 82 | 51 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 79 | low progesterone acne | 200 | 1 | 0.5% | 20.0 | 32 | 102 | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 80 | herbal teas for hormone balance | 199 | 0 | 0.0% | 8.5 | 15 | 7 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 81 | dim supplement for acne | 197 | 1 | 0.5% | 10.3 | 0 | 197 | DIM | /products/balance |  |
| 82 | what tea helps with hormonal imbalance | 197 | 0 | 0.0% | 9.1 | 140 | 3 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 83 | best tea for women's hormones | 194 | 0 | 0.0% | 8.6 | 61 | 31 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 84 | hormone safe sunscreen | 189 | 1 | 0.5% | 5.9 | 105 | 19 | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |  |
| 85 | best herbal tea for acne | 186 | 4 | 2.1% | 7.4 | 14 | 25 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 86 | herbal tea for hormone balance | 181 | 0 | 0.0% | 15.4 | 8 | 20 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 87 | teas for hormone balance | 181 | 0 | 0.0% | 9.7 | 120 | 9 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 88 | teas that increase estrogen | 180 | 0 | 0.0% | 10.6 | 136 | 16 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 89 | raspberry leaf tea benefits hormones | 179 | 1 | 0.6% | 10.0 | 27 | 105 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 90 | dandelion tea for hormonal acne | 177 | 1 | 0.6% | 7.1 | 104 | 8 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 91 | el cafe empeora el acne | 177 | 1 | 0.6% | 9.3 | 18 | 0 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 92 | tea for estrogen | 172 | 0 | 0.0% | 8.2 | 105 | 19 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 93 | el cafe da acne | 165 | 0 | 0.0% | 10.9 | 11 | 0 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 94 | nettle tea benefits for hormones | 164 | 0 | 0.0% | 4.9 | 21 | 79 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 95 | tea for hormonal balance | 164 | 0 | 0.0% | 10.6 | 58 | 34 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 96 | which tea is good for acne | 160 | 1 | 0.6% | 7.7 | 91 | 45 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 97 | herbal teas for hormonal imbalance | 160 | 0 | 0.0% | 9.3 | 47 | 21 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 98 | herbal teas for hormones | 160 | 0 | 0.0% | 8.0 | 5 | 1 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 99 | which tea is best for hormonal acne | 158 | 1 | 0.6% | 5.7 | 45 | 7 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 100 | tea for women's hormones | 157 | 0 | 0.0% | 12.1 | 141 | 6 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 101 | what tea is good for hormone balance | 157 | 0 | 0.0% | 8.5 | 91 | 7 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 102 | dandelion root tea for acne | 156 | 4 | 2.6% | 9.7 | 97 | 30 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 103 | does caffeine make you break out | 156 | 0 | 0.0% | 13.0 | 84 | 61 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 104 | best tea for hormones | 155 | 0 | 0.0% | 7.7 | 42 | 31 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 105 | dandelion tea acne | 154 | 2 | 1.3% | 10.0 | 64 | 32 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 106 | hormone-friendly sunscreen ingredients | 151 | 0 | 0.0% | 10.0 | 151 | 0 | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |  |
| 107 | tea good for hormonal imbalance | 149 | 0 | 0.0% | 8.1 | 33 | 20 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 108 | do oral acne medicines often cause dry skin, headaches, or mood changes? | 144 | 0 | 0.0% | 9.3 | 142 | 0 | General acne (non-hormonal wording) | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |  |
| 109 | best herbs for hormonal acne | 143 | 0 | 0.0% | 12.1 | 31 | 19 | How to treat / get rid of / fix hormonal acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 110 | tea that helps with hormonal imbalance | 141 | 0 | 0.0% | 10.0 | 60 | 6 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 111 | what tea helps balance hormones | 140 | 0 | 0.0% | 10.1 | 104 | 8 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 112 | hormone balancing teas for women | 135 | 1 | 0.7% | 9.6 | 79 | 17 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 113 | teas for hormonal imbalance | 133 | 3 | 2.3% | 8.6 | 54 | 17 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 114 | best tea to drink for acne | 133 | 0 | 0.0% | 10.5 | 77 | 14 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 115 | what tea helps with hormones | 132 | 1 | 0.8% | 9.4 | 92 | 7 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 116 | hormonal tea for women | 132 | 0 | 0.0% | 8.6 | 16 | 19 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 117 | supplement for hormonal acne | 130 | 1 | 0.8% | 14.8 | 8 | 107 | Supplements for hormonal acne | /products/balance |  |
| 118 | is dandelion tea good for acne | 130 | 0 | 0.0% | 9.4 | 68 | 23 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 119 | tea for hormones | 129 | 0 | 0.0% | 8.8 | 33 | 22 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 120 | which tea helps with hormonal imbalance | 129 | 0 | 0.0% | 9.4 | 37 | 8 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 121 | does low progesterone cause acne | 126 | 0 | 0.0% | 20.5 | 34 | 78 | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 122 | tea for hormonal imbalance in females | 124 | 0 | 0.0% | 10.0 | 30 | 12 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 123 | does coffee break you out | 123 | 0 | 0.0% | 9.0 | 43 | 46 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 124 | can caffeine cause hormonal acne | 122 | 1 | 0.8% | 7.4 | 103 | 7 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 125 | can low progesterone cause acne | 122 | 1 | 0.8% | 19.1 | 48 | 65 | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 126 | best tea for hormonal imbalance in women | 121 | 0 | 0.0% | 8.5 | 15 | 7 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 127 | dandelion root tea acne | 117 | 0 | 0.0% | 10.1 | 64 | 20 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 128 | does dandelion tea help with acne | 113 | 1 | 0.9% | 10.2 | 86 | 16 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 129 | can caffeine make you break out | 113 | 0 | 0.0% | 14.2 | 54 | 48 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 130 | does coffee cause hormonal acne | 111 | 0 | 0.0% | 8.3 | 69 | 13 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 131 | is caffeine bad for acne | 108 | 0 | 0.0% | 13.9 | 30 | 71 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 132 | tea to increase estrogen | 108 | 0 | 0.0% | 10.3 | 50 | 30 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 133 | best tea for hormonal balance | 107 | 2 | 1.9% | 13.4 | 42 | 11 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 134 | tea for hormone imbalance | 107 | 0 | 0.0% | 11.7 | 82 | 3 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 135 | does coffee make acne worse | 106 | 0 | 0.0% | 13.7 | 33 | 64 | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |  |
| 136 | hormonal balance tea | 106 | 0 | 0.0% | 8.4 | 33 | 52 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 137 | tea to help with hormonal acne | 103 | 3 | 2.9% | 6.5 | 78 | 1 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 138 | fungal acne vs hormonal acne | 103 | 1 | 1.0% | 19.6 | 15 | 79 | Hormonal acne: what / causes / types | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 139 | tea good for acne | 103 | 0 | 0.0% | 9.2 | 49 | 52 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 140 | what is the best tea for acne | 103 | 0 | 0.0% | 6.8 | 65 | 20 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 141 | estrogen dominance and acne | 102 | 0 | 0.0% | 11.7 | 42 | 19 | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |  |
| 142 | what teas are good for hormonal acne | 101 | 2 | 2.0% | 5.5 | 62 | 10 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |
| 143 | what tea is good for hormones | 101 | 0 | 0.0% | 8.1 | 51 | 13 | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |  |

**Commercial queries ranking past position 20.** These won't reach the top with tweaks; they need a dedicated page (see sections 8a to 8c).


| Query | Impr. | Clicks | Avg pos | US impr. | CA impr. | Page ranking now |
|---|---:|---:|---:|---:|---:|---|
| supplements for hormonal acne | 1,489 | 6 | 27.3 | 671 | 441 | / |
| hormonal acne supplement | 756 | 7 | 21.2 | 268 | 143 | / |
| natural supplements for hormonal acne | 590 | 0 | 32.1 | 222 | 73 | / |
| skincare supplement | 533 | 0 | 21.8 | 21 | 472 | /products/balance |
| natural supplements for acne | 421 | 0 | 28.3 | 23 | 359 | / |
| tablets for hormonal acne | 349 | 0 | 60.1 | 113 | 1 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| hormonal acne tablets | 340 | 0 | 65.0 | 120 | 1 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| supplements for clear skin | 276 | 0 | 37.4 | 24 | 220 | / |
| hormonal acne natural supplements | 262 | 0 | 31.2 | 28 | 9 | / |
| gummies for hormonal acne | 221 | 0 | 30.3 | 213 | 1 | / |
| best organic acne treatments | 209 | 0 | 27.9 | 2 | 206 | /blogs/cocoon-blog/natural-topical-ingredients-acne |
| clear skin supplements | 204 | 0 | 30.5 | 0 | 200 | / |
| hormonal acne pills | 192 | 3 | 53.9 | 79 | 39 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| hormonal acne medication | 192 | 0 | 66.2 | 107 | 20 | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| acne hormone imbalance supplement | 182 | 0 | 20.5 | 172 | 1 | / |
| organic gnld acne supplements | 158 | 0 | 37.3 | 158 | 0 | /products/balance |
| acne treatment quiz | 156 | 0 | 44.0 | 142 | 9 | /pages/quiz |
| natural gnld acne supplements | 156 | 0 | 33.5 | 156 | 0 | /products/balance |
| hormonal acne treatment | 144 | 0 | 64.2 | 17 | 104 | /pages/learn |
| supplements hormonal acne | 116 | 0 | 29.0 | 55 | 25 | / |
| best supplements for hormonal acne | 111 | 0 | 35.5 | 53 | 27 | /products/balance |
| supplement for acne | 110 | 3 | 30.4 | 29 | 61 | / |
| vitamins for hormonal acne | 110 | 0 | 23.9 | 24 | 50 | /products/balance |
| hormonal acne vitamins | 106 | 0 | 33.2 | 41 | 29 | /products/balance |
| clear skin vitamins | 104 | 0 | 39.0 | 2 | 92 | / |
| organic gnld acne vitamins | 101 | 0 | 47.5 | 101 | 0 | /products/balance |

---

## 4. Pages: the URLs that must be preserved or redirected

Totals per URL for the full period. Page-level totals include anonymised queries, so they add up to 5,980 clicks. I checked the "same path on cocoonsupplements.com" column with `curl` on 13 Oct 2026; Shopify keeps paths when the primary domain changes. **Every URL with clicks must keep resolving.** Pages 1 to 13 hold 98% of the clicks (5,836 of 5,980).


| # | URL (cocoonskincare.ca) | Clicks | Impr. | CTR | Avg pos | Clicks Jul-Sep 2026 | Same path on cocoonsupplements.com (13 Oct 2026) |
|---|---|---:|---:|---:|---:|---:|---|
| 1 | https://cocoonskincare.ca/ | 3,270 | 40,626 | 8.0% | 14.5 | 401 | 200 |
| 2 | https://cocoonskincare.ca/blogs/cocoon-blog/best-teas-for-hormone-balance | 1,049 | 156,535 | 0.7% | 7.5 | 335 | 200 |
| 3 | https://cocoonskincare.ca/products/balance | 727 | 31,252 | 2.3% | 12.9 | 71 | 200 |
| 4 | https://cocoonskincare.ca/pages/quiz | 201 | 16,400 | 1.2% | 16.6 | 22 | 200 |
| 5 | https://cocoonskincare.ca/pages/results | 191 | 16,912 | 1.1% | 4.7 | 34 | 200 |
| 6 | https://cocoonskincare.ca/pages/faq | 70 | 10,181 | 0.7% | 4.2 | 6 | 200 |
| 7 | https://cocoonskincare.ca/blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have | 63 | 11,102 | 0.6% | 18.2 | 15 | 200 |
| 8 | https://cocoonskincare.ca/blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse | 61 | 48,320 | 0.1% | 14.1 | 4 | 200 |
| 9 | https://cocoonskincare.ca/blogs/cocoon-blog/hormone-safe-sunscreens | 59 | 11,227 | 0.5% | 9.8 | 10 | 200 |
| 10 | https://cocoonskincare.ca/pages/about | 51 | 12,614 | 0.4% | 4.5 | 9 | 200 |
| 11 | https://cocoonskincare.ca/pages/shipping-policy | 37 | 2,583 | 1.4% | 11.5 | 11 | 200 |
| 12 | https://cocoonskincare.ca/pages/affiliate-program | 31 | 1,745 | 1.8% | 8.6 | 4 | 200 |
| 13 | https://cocoonskincare.ca/pages/learn | 26 | 11,127 | 0.2% | 13.6 | 4 | 200 |
| 14 | https://cocoonskincare.ca/products/balance?variant=39429510135872&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic | 25 | 70 | 35.7% | 4.2 | 3 | 200 |
| 15 | https://cocoonskincare.ca/products/balance-thermae | 18 | 2,320 | 0.8% | 4.3 | 3 | 200 |
| 16 | https://cocoonskincare.ca/pages/contact-us | 12 | 5,433 | 0.2% | 9.2 | 2 | 200 |
| 17 | https://cocoonskincare.ca/blogs/cocoon-blog/natural-topical-ingredients-acne | 12 | 2,812 | 0.4% | 19.3 | 5 | 200 |
| 18 | https://cocoonskincare.ca/blogs/cocoon-blog/the-truth-about-prescription-acne-medications | 11 | 6,280 | 0.2% | 37.5 | 4 | 200 |
| 19 | https://cocoonskincare.ca/blogs/cocoon-blog/the-biggest-triggers-for-hormonal-acne-and-how-to-fix-them | 10 | 3,780 | 0.3% | 15.7 | 1 | 200 |
| 20 | https://cocoonskincare.ca/pages/money-back-guarantee | 8 | 1,237 | 0.6% | 8.4 | 1 | 200 |
| 21 | https://cocoonskincare.ca/pages/results-1 | 7 | 1,278 | 0.5% | 5.5 | 0 | 200 |
| 22 | https://cocoonskincare.ca/blogs/cocoon-blog/7-myths-and-facts-about-hormonal-acne-debunking-common-misconceptions | 7 | 495 | 1.4% | 14.8 | 0 | 200 |
| 23 | https://www.cocoonskincare.ca/ | 5 | 449 | 1.1% | 7.7 | 0 | 200 |
| 24 | https://cocoonskincare.ca/account/login | 4 | 480 | 0.8% | 13.3 | 1 | 200 |
| 25 | https://cocoonskincare.ca/products/balance?variant=40492143312960&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic | 4 | 19 | 21.1% | 3.6 | 1 | 200 |
| 26 | https://cocoonskincare.ca/pages/terms-of-service | 3 | 492 | 0.6% | 12.7 | 1 | 200 |
| 27 | https://cocoonskincare.ca/cart | 3 | 117 | 2.6% | 36.7 | 0 | 200 |
| 28 | https://cocoonskincare.ca/blogs/cocoon-blog?page=2 | 3 | 86 | 3.5% | 10.9 | 0 | 200 |
| 29 | https://cocoonskincare.ca/blogs/cocoon-blog/balancing-hormones-with-food | 2 | 7,346 | 0.0% | 46.2 | 1 | 200 |
| 30 | https://cocoonskincare.ca/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2025 | 2 | 854 | 0.2% | 19.6 | 0 | 404 - needs redirect |
| 31 | https://cocoonskincare.ca/blogs/cocoon-blog/goodbye-hair-skin-nail-gummies-why-hormonal-acne-needs-more-specific-support | 2 | 204 | 1.0% | 9.2 | 2 | 200 |
| 32 | https://cocoonskincare.ca/products/balance?variant=39429510135872&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&gQT=1 | 2 | 9 | 22.2% | 3.6 | 0 | 200 |
| 33 | https://cocoonskincare.ca/products/dim | 1 | 3,370 | 0.0% | 3.1 | 1 | 301 to /products/balance |
| 34 | https://cocoonskincare.ca/blogs/cocoon-blog/which-produce-is-worth-buying-organic | 1 | 639 | 0.2% | 18.6 | 0 | 200 |
| 35 | https://cocoonskincare.ca/blogs/cocoon-blog/xenoestrogens | 1 | 377 | 0.3% | 40.3 | 0 | 200 |
| 36 | https://cocoonskincare.ca/products/balance?variant=40492180570176&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic | 1 | 2 | 50.0% | 8.0 | 0 | 200 |
| 37 | https://cocoonskincare.ca/blogs/cocoon-blog/can-hormonal-acne-be-caused-by-stress | 0 | 2,240 | 0.0% | 30.6 | 0 | 200 |
| 38 | https://cocoonskincare.ca/pages/learn-1 | 0 | 1,645 | 0.0% | 3.4 | 0 | 301 to /pages/learn |
| 39 | https://cocoonskincare.ca/blogs/cocoon-blog | 0 | 987 | 0.0% | 6.9 | 0 | 200 |
| 40 | https://cocoonskincare.ca/pages/privacy-policy | 0 | 373 | 0.0% | 15.0 | 0 | 200 |
| 41 | https://cocoonskincare.ca/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2026 | 0 | 284 | 0.0% | 7.7 | 0 | 200 |
| 42 | https://cocoonskincare.ca/blogs/cocoon-blog/does-endometriosis-cause-adult-acne | 0 | 89 | 0.0% | 12.8 | 0 | 200 |
| 43 | https://cocoonskincare.ca/pages/refund-policy | 0 | 34 | 0.0% | 9.9 | 0 | 404 - needs redirect |
| 44 | https://cocoonskincare.ca/policies/shipping-policy | 0 | 30 | 0.0% | 15.0 | 0 | 200 |
| 45 | https://cocoonskincare.ca/blogs/cocoon-blog/internal-skincare-what-it-actually-means-for-hormonal-acne | 0 | 27 | 0.0% | 25.7 | 0 | 200 |
| 46 | https://cocoonskincare.ca/blogs/cocoon-blog/best-herbal-teas-to-help-with-hormonal-imbalance-acne | 0 | 26 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 47 | https://cocoonskincare.ca/pages/reviews | 0 | 22 | 0.0% | 6.8 | 0 | 200 |
| 48 | https://cocoonskincare.ca/products/balance?variant=40363600707648&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic | 0 | 4 | 0.0% | 2.2 | 0 | 200 |
| 49 | https://cocoonskincare.ca/products/balance?variant=39429510135872&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&com_cvv=8fb3d522dc163aeadb66e08cd7450cbbdddc64c6cf2e8891f6d48747c6d56d2c | 0 | 3 | 0.0% | 1.0 | 0 | 200 |
| 50 | https://cocoonskincare.ca/products/balance?variant=40492180570176&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&gQT=1 | 0 | 2 | 0.0% | 8.0 | 0 | 200 |
| 51 | https://cocoonskincare.ca/products/balance?variant=40363600707648&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&gQT=1 | 0 | 2 | 0.0% | 2.5 | 0 | 200 |
| 52 | http://cocoonskincare.ca/cdn/shop/files/Cocoon_Skincare_Logo_-_Social_1200x1200.png?v=1670272560 | 0 | 2 | 0.0% | 15.0 | 0 | 200 |
| 53 | https://cocoonskincare.ca/blogs/cocoon-blog/best-for-hormone-balance | 0 | 2 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 54 | https://cocoonskincare.ca/blogs/cocoon-blog/best-herbal-teas-for-hormone-balance | 0 | 2 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 55 | https://cocoonskincare.ca/blogs/cocoon-blog/best-hormone-balance | 0 | 2 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 56 | https://cocoonskincare.ca/cdn/shop/files/paulina-hormonal-acne-supplement-balance-results-before-after_2a7db2f0-9ea0-4033-b609-3113c17ddd0c_300x300.png?v=1754931929 | 0 | 1 | 0.0% | 68.0 | 0 | 200 |
| 57 | http://cocoonskincare.ca/cdn/shop/files/cocoon-hormonal-acne-supplement-starter-set_39caf885-9a1c-4a46-bbcb-458f39035c27_1200x1200.jpg?v=1738955533 | 0 | 1 | 0.0% | 15.0 | 0 | 200 |
| 58 | https://cocoonskincare.ca/products/balance?variant=40716691832896&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic | 0 | 1 | 0.0% | 1.0 | 0 | 200 |
| 59 | https://cocoonskincare.ca/products/balance?variant=40363600707648&country=CA&currency=CAD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&com_cvv=8fb3d522dc163aeadb66e08cd7450cbbdddc64c6cf2e8891f6d48747c6d56d2c | 0 | 1 | 0.0% | 1.0 | 0 | 200 |
| 60 | https://cocoonskincare.ca/blogs/cocoon-blog/best-herbal-teas-that-help-with-hormonal-imbalance-acne | 0 | 1 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 61 | https://cocoonskincare.ca/blogs/cocoon-blog/best-hormone-imbalance-acne | 0 | 1 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 62 | https://cocoonskincare.ca/blogs/cocoon-blog/best-teas-for-horone-balance | 0 | 1 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 63 | https://cocoonskincare.ca/blogs/cocoon-blog/goodbye-hair-skin-nail-gummies-why-hormonal-acne-needs-more-specif | 0 | 1 | 0.0% | 1.0 | 0 | 404 - needs redirect |
| 64 | https://cocoonskincare.ca/blogs/cocoon-blog/the-truth-authorization-prescription-acne-medications | 0 | 1 | 0.0% | 1.0 | 0 | 404 - needs redirect |

**Redirects to add or keep**

| From (path) | To | Why |
|---|---|---|
| `/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2025` | `/blogs/cocoon-blog/how-to-treat-hormonal-acne-in-2026` | 404 now; 854 impressions |
| `/pages/refund-policy` | `/policies/refund-policy` | 404 now |
| `/blogs/cocoon-blog/best-herbal-teas-to-help-with-hormonal-imbalance-acne`, `best-herbal-teas-for-hormone-balance`, `best-herbal-teas-that-help-with-hormonal-imbalance-acne`, `best-for-hormone-balance`, `best-hormone-balance`, `best-hormone-imbalance-acne`, `best-teas-for-horone-balance` | `/blogs/cocoon-blog/best-teas-for-hormone-balance` | 404 now; old or malformed slugs of the tea article |
| `/blogs/cocoon-blog/goodbye-hair-skin-nail-gummies-why-hormonal-acne-needs-more-specif` | `/blogs/cocoon-blog/goodbye-hair-skin-nail-gummies-why-hormonal-acne-needs-more-specific-support` | 404 now; truncated slug |
| `/blogs/cocoon-blog/the-truth-authorization-prescription-acne-medications` | `/blogs/cocoon-blog/the-truth-about-prescription-acne-medications` | 404 now; malformed slug |
| `/pages/results-1` | `/pages/results` | duplicate page (1,278 impressions) |
| one of the two diet posts | the one that's kept | consolidation (section 8e) |
| `/products/dim`, `/pages/learn-1` | already 301 to `/products/balance` and `/pages/learn` | keep these |
| any URL renamed in the restructure | its closest new match | rule: keep proven URLs (`/`, `/products/balance`, `/pages/quiz`, `/pages/results`, `/pages/faq`, `/pages/about`, `/pages/learn`, every blog slug) |

**Which queries bring traffic to the key pages** (impressions / clicks / position)


| Page | Top queries (impr. / clicks / pos) |
|---|---|
| / | cocoon skin care (3,807/429/4); hormonal acne supplements (2,687/5/21); cocoon (2,685/6/6); cocoon skincare (2,141/363/4); supplements for hormonal acne (1,240/2/32); cocoon supplement (983/516/1) |
| /products/balance | cocoon skin care (2,163/13/7); hormonal acne supplements (2,119/7/25); cocoon skincare (1,162/2/4); cocoon supplement (981/50/1); cocoon acne supplement (777/57/1); acne supplements canada (566/2/13) |
| /blogs/cocoon-blog/best-teas-for-hormone-balance | tea for hormonal acne (2,225/29/6); tea for hormonal imbalance (2,117/6/11); best tea for hormonal acne (1,801/14/5); what tea is good for acne (1,217/0/10); best tea for hormonal imbalance (1,027/3/8); best tea for acne (1,022/5/8) |
| /pages/quiz | cocoon skin care (1,823/1/3); cocoon skincare (929/0/4); acne quiz (851/2/32); what type of acne do i have quiz (572/0/45); cocoon (366/0/12); what is causing my acne quiz (344/4/12) |
| /pages/results | cocoon skin care (2,958/5/3); cocoon skincare (1,312/3/3); cocoon supplement (815/2/1); cocoon acne supplement (482/3/1); cocoon skin (402/0/5); cocoon (378/0/11) |
| /pages/faq | cocoon skin care (1,822/0/3); cocoon supplement (832/7/1); cocoon skincare (795/0/3); cocoon acne supplement (527/2/1); hormonal acne supplements (286/0/12); cocoon skin (241/1/3) |
| /pages/about | cocoon skin care (2,774/6/3); cocoon skincare (1,244/2/3); cocoon supplement (935/2/1); cocoon acne supplement (721/3/1); cocoon (364/0/12); cocoon skin (336/0/3) |
| /pages/learn | cocoon skin care (844/2/4); cocoon supplement (805/9/1); cocoon skincare (570/1/4); cocoon acne supplement (556/5/1); hormonal acne (430/0/50); hormonal acne supplements (341/0/14) |
| /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse | does coffee cause acne (1,336/0/38); coffee and acne (1,101/0/26); does caffeine cause acne (613/0/30); can coffee cause acne (551/0/31); does coffee make you break out (415/0/14); can coffee cause hormonal acne (414/1/9) |
| /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have | estrogen dominance acne (337/4/11); low progesterone acne (190/1/19); does low progesterone cause acne (126/0/20); can low progesterone cause acne (122/1/19); hormonal acne types (119/0/66); fungal acne vs hormonal acne (103/1/20) |
| /blogs/cocoon-blog/hormone-safe-sunscreens | how to choose sunscreen that doesn’t mess with hormones (506/0/7); sunscreen without endocrine disruptors (226/0/8); hormone safe sunscreen (189/1/6); hormone-friendly sunscreen ingredients (151/0/10); hormone disruptors in sunscreen (102/0/34); endocrine disruptors sunscreen (93/0/35) |
| /blogs/cocoon-blog/balancing-hormones-with-food | hormonal acne diet (1,606/0/56); how to balance hormones for acne (947/0/53); hormonal imbalance acne diet (220/0/56); foods for hormonal imbalance acne (206/0/52); foods for hormonal acne (188/0/49); foods that help hormonal acne (172/0/53) |
| /blogs/cocoon-blog/the-truth-about-prescription-acne-medications | tablets for hormonal acne (349/0/60); hormonal acne tablets (339/0/65); hormonal acne medication (192/0/66); hormonal acne pills (155/0/64); do oral acne medicines often cause dry skin, headaches, or mood changes? (144/0/9); aldactone acne (123/0/83) |
| /products/dim | cocoon skin care (1,616/0/2); cocoon skincare (516/1/2); cocoon skin (65/0/2); cocoon skin care products (24/0/10); cocoon balance (17/0/2); the cocoon skincare (17/0/8) |

---

## 5. Brand vs non-brand

"Brand" means queries containing cocoon or a misspelling of it (cocoon skin care, cocoon supplement, cocoon balance, cocoon acne, cocoonskincare.ca, and so on). "Ambiguous" means the bare word "cocoon" plus other businesses (Cocoon Apothecary, Cocooncenter, cocoon delivery and similar). "balance supplement" (282 impressions, position 3.8, mostly CA) is counted as non-brand, but it is probably people looking for our product.


| Segment | Clicks | % of clicks | Impr. | % of impr. |
|---|---:|---:|---:|---:|
| brand | 2,332 | 84.6% | 11,434 | 9.2% |
| brand-ambiguous | 10 | 0.4% | 5,171 | 4.1% |
| non-brand | 413 | 15.0% | 108,186 | 86.7% |
| total (query-level) | 2,755 | 100% | 124,791 | 100% |

| Country | Brand clicks | Ambiguous clicks | Non-brand clicks | Brand share of clicks | Brand impr. | Non-brand impr. |
|---|---:|---:|---:|---:|---:|---:|
| United States | 647 | 0 | 109 | 85.6% | 3,743 | 47,076 |
| Canada | 1,046 | 9 | 153 | 86.6% | 3,439 | 26,532 |

| Top brand queries | Clicks | Impr. | CTR | Avg pos |
|---|---:|---:|---:|---:|
| cocoon supplement | 587 | 999 | 58.8% | 1.2 |
| cocoon acne supplement | 501 | 784 | 63.9% | 1.0 |
| cocoon skin care | 457 | 3,932 | 11.6% | 4.0 |
| cocoon skincare | 376 | 2,182 | 17.2% | 4.0 |
| cocoon skin | 101 | 632 | 16.0% | 5.5 |
| cocoon acne | 60 | 99 | 60.6% | 1.4 |
| cocoon canada | 51 | 784 | 6.5% | 10.0 |
| cocoon balance | 46 | 122 | 37.7% | 1.0 |
| cocoon skin care reviews | 40 | 365 | 11.0% | 2.8 |
| cocoonskincare.ca | 24 | 37 | 64.9% | 1.0 |
| cocoonskincare | 19 | 37 | 51.3% | 3.3 |
| cocoon skincare reviews | 16 | 120 | 13.3% | 1.9 |
| cocoon balance hormonal acne supplement | 9 | 40 | 22.5% | 4.9 |
| cocoon acne supplement reviews | 8 | 28 | 28.6% | 1.2 |
| cocoon hormone balance | 6 | 15 | 40.0% | 1.2 |

Reading it: about 85% of clicks are brand in both countries. Non-brand gets 108,186 impressions at a 0.4% CTR. The opportunity is to turn those impressions into clicks; there isn't much non-brand traffic at risk in the move.

---

## 6. Google Ads search terms that converted (Jun 2025 to 12 Oct 2026)

Account totals for the period: about 398 conversions on about 17,046 spend (in the account currency; I didn't confirm whether that's CAD or USD), across 4 campaigns: "Sales | Search | Clicks | June 2025" (~362 conversions), "Sales | Shopping | Clicks | Nov 2025" (~31), "US Sales | Search | Clicks | May 2026" (5) and "June 2025" (0).

About 164 of the ~398 conversions can be tied to a specific search term. Google hides low-volume terms, and Shopping/automated traffic accounts for the rest. Conversion counts include fractions because the account uses data-driven attribution. The conversion and value columns are complete for each term. Windsor returned clicks and cost only for the days a term converted, so I've left those columns out rather than understate them.

**Brand terms (~85 conversions, ~8,544 value)**

| Search term | Conversions | Conv. value |
|---|---:|---:|
| cocoon skin care | 25.0 | 2,045 |
| cocoon supplement | 20.3 | 2,232 |
| cocoon balance | 13.2 | 1,428 |
| cocoon acne supplement | 12.7 | 1,520 |
| cocoon skin | 5.0 | 369 |
| cocoon skincare | 4.1 | 537 |
| cocoon acne supplement reddit | 4.0 | 272 |
| cocoon supplements | 1.0 | 141 |

**Non-brand terms that converted (~78 conversions). These are the commercial-intent keywords.**

| Search term | Conversions | Conv. value | Note |
|---|---:|---:|---|
| hormonal acne supplements | 10.5 | 628 | Search + Shopping |
| hormonal acne treatment | 6.8 | 848 | Shopping. Converts, but we can't use "treatment" as a claim |
| supplements for hormonal acne | 3.0 | 412 | |
| supplement for hormonal acne | 2.1 | 286 | |
| heal hormonal acne | 2.0 | 319 | claim wording |
| best female hormone balance supplements for acne | 2.0 | 313 | |
| acne supplement | 2.0 | 313 | |
| acne vitamins | 2.0 | 245 | |
| acne supplements for women | 2.0 | 245 | |
| spirulina for hormonal acne | 2.0 | 235 | |
| dietary supplements for hormonal acne | 2.0 | 233 | |
| best probiotic for acne | 2.0 | 136 | gut/skin angle |
| dim for acne | 2.0 | 122 | US campaign |
| supplements for hormonal cystic acne | 2.0 | 122 | |
| best supplement for acne | 2.0 | 120 | |
| natural vitamins for acne | 2.0 | 108 | |
| diet to reduce hormonal acne | 2.0 | 108 | |
| natural hormonal acne treatment | 1.8 | 322 | claim wording |
| ovira acne supplement | 1.7 | 118 | competitor |
| acne supplements | 1.6 | 189 | |
| acne pills treatment | 1.6 | 106 | |
| skin supplements for acne | 1.3 | 138 | |
| diindolylmethane for women | 1.0 | 160 | |
| herbal supplements for hormonal acne | 1.0 | 160 | |
| how to get rid of acne on chin | 1.0 | 157 | chin/jawline angle |
| hormone imbalance causing acne | 1.0 | 157 | |
| hormone balancing after birth control | 1.0 | 157 | post-pill angle |
| hormone imbalance women acne | 0.9 | 149 | |
| supplements for cystic acne, supplements to clear acne, best supplements for hormonal acne, best way to get rid of hormonal acne, how to improve hormonal acne, zinc supplement for acne, pantothenic acid for acne, eliminate dairy for clear skin, acne supplements canada, diane 35 for acne | 1.0 each | 54 to 108 | |
| competitor names: ecloura acne out bar, mondaymuseskin, pore favor acne supplement, the skin complex, cocoon apothecary | 0.7 to 1.0 each | 41 to 177 | |

**Paid terms with lots of clicks and no conversions in the visible data:** "how to get rid of acne" (251+ clicks, 0 conversions), "hormonal acne" (37+ clicks, 0), "how to get rid of hormonal acne" (15+, 0), "hormonal acne treatment" on Search (14+, 0) and "hormonal imbalance" (9+, 0). These are minimums, because Windsor filtered by day. The pattern is clear, though: **"supplement" wording converts and "how to get rid of" wording doesn't.** That matches organic, where informational terms get impressions and commercial terms get sales.

---

## 7. Search volume from Keyword Planner (US, monthly average, past 12 months)

This is the only real search-volume data in the audit. It comes from Google Keyword Planner through the Ads account: US (location 2840), English, Google Search. Google rounds these figures into buckets. **Every seed that contained "acne" returned zero ideas, and no idea containing "acne" came back for any seed.** Keyword Planner seems to suppress acne terms for this account or this connector, so the acne-term volumes are still unknown. Semrush and Ahrefs aren't connected.

| Keyword (US) | Avg monthly searches | Competition (ads) | Relevance |
|---|---:|---|---|
| dim supplement | 27,100 | High | Balance's lead ingredient |
| glutathione supplement | 22,200 | High | Balance ingredient (much of this demand is about skin lightening, so be careful how the page is positioned) |
| pcos supplements | 9,900 | High | only if a new SKU fits PCOS `[NEED FROM RACHEL]` |
| estrogen dominance | 8,100 | Low | core concern for Balance |
| calcium d glucarate | 6,600 | High | Balance ingredient |
| dim supplement for women | 5,400 | High | Balance |
| supplements for skin health | 5,400 | Medium | shop-all / range |
| best gut health supplement | 5,400 | High | gut/skin angle `[NEED FROM RACHEL]`: does a new SKU cover gut? |
| spearmint tea for hormonal balance | 3,600 | Low | tea article gap |
| pcos vitamins | 3,600 | High | as above |
| supplements for pimples | 2,900 | High | shop-all (Keyword Planner lets "pimples" through where it blocks "acne") |
| vitamins for pimples | 2,400 | High | shop-all |
| hormone balance supplements for women | 2,400 | High | home / collection |
| female hormone balance supplements | 2,400 | High | home / collection |
| tea for hormone balance | 2,400 | High | tea article |
| tea for hormonal imbalance | 2,400 | High | tea article |
| probiotics for skin health | 2,400 | High | gut/skin |
| best skin supplements | 1,600 | High | shop-all |
| post birth control syndrome | 1,600 | Low | post-pill concern page |
| calcium d glucarate benefits | 1,300 | High | ingredient page |
| estrogen dominance treatment | 1,300 | High | intent to capture with compliant wording |
| clear skin supplements | 1,000 | High | shop-all |
| skin supplements | 1,000 | High | shop-all |
| dim estrogen | 1,000 | High | Balance / DIM explainer |
| skin probiotic | 1,000 | High | gut/skin |
| best dim supplement | 880 | High | Balance |
| vitamins for clear skin | 880 | High | shop-all |
| dim hormone balance / dim for hormonal imbalance | 720 each | High | Balance |
| best hormone balancing supplements for women | 720 | High | collection |
| female too much estrogen / high estrogen and low progesterone | 720 each | Low | estrogen concern page |
| estrogen dominance diet | 480 | Medium | diet article |
| dim and calcium d glucarate | 390 | High | Balance |
| dim supplement for estrogen dominance | 390 | Low | Balance |
| supplements for estrogen dominance | 320 | High | estrogen concern page |
| best vitamins for clear skin | 260 | High | shop-all |
| best supplements for clear skin | 210 | High | shop-all |
| clear skin probiotics | 140 | High | gut/skin |
| dim for skin | 40 | High | not worth targeting |
| **internal skincare** | **20** | High | **positioning only, not a keyword** |
| (for scale) hair skin and nails vitamins | 27,100 | High | category we're positioned against (we have the "Goodbye hair, skin & nail gummies" post) |

---
## 8. Keyword recommendations

The rule throughout: **one primary keyword per page, and no two pages targeting the same primary.** At the moment the home page and /products/balance compete for "hormonal acne supplements". The titles, metas and H1s below are examples to show the keyword in use. They are not final copy. Anything that pairs a product with acne is marked `[CLAIM CHECK]` for regulatory review. I'm not a lawyer, and the FDA treats acne as a disease, so even "for hormonal acne-prone skin" next to a product needs her reviewer's sign-off.

### (a) Home page (`/`), keep the URL
- **Primary: "supplements for hormonal acne" and its close variant "hormonal acne supplements".** The home page already has 44% of this cluster's 10,077 impressions. Its position (21 for "hormonal acne supplements", 32 for "supplements for hormonal acne") is the main thing to improve. Ads confirms the term converts: about 15.6 conversions across its three main variants. `[CLAIM CHECK]`
- **Secondary:** "natural supplements for hormonal acne" (590 impressions, position 32), "hormone balance supplements for women" (US Keyword Planner 2,400), "acne supplements for women" (Ads: 2 conversions) and the brand terms "Cocoon supplements" and "Cocoon Skincare" (6,114 impressions on "cocoon skin care/skincare").
- Example title (49 characters): `Supplements for Hormonal Acne-Prone Skin | Cocoon` `[CLAIM CHECK]`
- Example meta (134 characters): `Naturopath-formulated supplements that target a root cause of hormonal breakouts. Take the 2-minute quiz. 30-day money-back guarantee.`
- Example H1: "Internal skincare for hormonal breakouts". The owner's "internal skincare" idea fits here as a brand line; the keyword goes in the title, an H2 and the first paragraph.

### (b) Balance product page (`/products/balance`), keep the URL
- **Primary: "DIM supplement for women" with an estrogen-balance angle.** US Keyword Planner: 5,400/month; "dim supplement" 27,100. Our current DIM visibility is almost all Canadian (510 of 542 DIM-cluster impressions are from CA; "dim supplement for acne" ranks 10.3 in CA and has 0 US impressions).
- **Secondary:** "DIM and calcium D-glucarate" (390), "dim estrogen" (1,000), "dim supplement for estrogen dominance" (390), "estrogen balance supplement", "Cocoon Balance" (brand: 122 impressions and 46 clicks at position 1, plus 13 Ads conversions) and "dim supplement for acne" (197 impressions, CA) `[CLAIM CHECK]`.
- Today the H1 is just "BALANCE" and og:title is "BALANCE". Put the keyword in the H1.
- Example title (54 characters): `Balance: DIM + Calcium D-Glucarate Supplement | Cocoon`
- Example meta (147 characters): `Balance supports healthy estrogen metabolism with DIM, glutathione and calcium D-glucarate, for clearer-looking skin from within. 30-day guarantee.`
- Example H1: "Balance: DIM + Calcium D-Glucarate for Healthy Estrogen Balance".
- Watch-out: much of the "glutathione supplement" demand (22,200) is about skin lightening. Mention glutathione as an ingredient, but don't make it the page's keyword.

### (c) Shop-all / collection page (new, e.g. `/collections/skin-supplements`; the URL is a best-practice suggestion)
- **Primary: "clear skin supplements"** (US Keyword Planner 1,000), to cover the "acne supplements" family without leaning on the disease word. GSC "acne supplements" had 864 impressions at position 13, "acne supplements canada" 796 at 9.0, "supplements for acne" 474 at 16.5, "skin supplements for acne" 350, "skincare supplement" 533 at 21.8, and "supplements for clear skin" plus "clear skin supplements" 480 at positions 30 to 37. Most of these are Canadian (5,282 of the cluster's 6,772 impressions).
- **Secondary:** "acne supplements" `[CLAIM CHECK]`, "supplements for pimples" (US Keyword Planner 2,900), "vitamins for pimples" (2,400), "best skin supplements" (1,600), "skin supplements" (1,000) and "vitamins for clear skin" (880).
- Example title (51 characters): `Clear Skin Supplements for Acne-Prone Skin | Cocoon` `[CLAIM CHECK]`
- Example meta (129 characters): `Shop Cocoon's naturopath-formulated supplements for acne-prone skin. Find the right formula for your skin with our 2-minute quiz.`
- Shopify's default `/collections/all` is thin and gives no keyword signal. Use a named collection and make it the main "Shop" link in the navigation.

### (d) Concern / category pages worth creating or upgrading (in order of data strength)

| Page | Primary keyword | Evidence | Status / action |
|---|---|---|---|
| **Acne quiz** (`/pages/quiz`, keep the URL) | "acne quiz", with "what type of acne do I have quiz" | Quiz cluster: 5,566 impressions (81% US), average position 36.4, 52 clicks. "acne quiz" 851 impressions at position 31.6; "what type of acne do i have quiz" 572 at 45; "what is causing my acne quiz" 344 at 12.1; "hormonal acne quiz" 265 at 2.4 with 15% CTR | Retitle (the current title is 69 characters and leads with "high estrogen"). Example: `Acne Quiz: What Type of Acne Do I Have? \| Cocoon` (48). Add about 300 words of indexable copy under the quiz |
| **Estrogen dominance & acne** (hub; upgrade the existing post `/blogs/cocoon-blog/estrogen-dominance-in-women-symptoms-causes-and-natural-treatment` or make it a page) | "estrogen dominance acne" | GSC estrogen cluster: 2,452 impressions at position 23.1, now landing mostly on the acne-types post. "estrogen dominance acne" 371 at 11.0; "estrogen dominance and acne" 102 at 11.7; "low progesterone acne" variants ~450 at ~20. Keyword Planner: "estrogen dominance" 8,100; "female too much estrogen" 720; "supplements for estrogen dominance" 320 | The post's slug and title say "natural treatment". Retitle along the lines of `Estrogen Dominance & Acne: Signs and Natural Support` (52) and keep the URL. Link it to Balance |
| **Hormonal acne guide** (`/pages/learn`, keep the URL) | "hormonal acne" | "hormonal acne" 470 impressions at position 47 (360 of them CA); "how to balance hormones for acne" 948 at 53; types/causes cluster 3,822 impressions at position 51 with 2 clicks; "fungal vs hormonal acne" variants ~280 at 16 to 21 | Retitle (69 characters now). Example: `Hormonal Acne: Causes, Types & What Helps \| Cocoon` (50). Add "fungal vs hormonal" and "chin/jawline" sections |
| **Post-birth-control skin** | "post birth control syndrome" / "acne after stopping birth control" | GSC: only 32 impressions (no equity). Keyword Planner "post birth control syndrome" 1,600 (US). Ads: "hormone balancing after birth control" converted (~1) | Best-practice assumption. Start as a blog post; promote to a concern page if a new SKU fits `[NEED FROM RACHEL: do the new products have a post-pill angle?]` |
| **Chin & jawline breakouts** | "hormonal chin acne" | GSC: 260 impressions at position 55 (weak). Ads: "how to get rid of acne on chin" converted 1 | Best-practice. Blog section or post, not a standalone page yet |
| **PCOS** | "pcos supplements" | GSC: 6 impressions. Keyword Planner 9,900 | Only if a new SKU is formulated for it, and with careful claims (PCOS is a disease) `[NEED FROM RACHEL]` `[CLAIM CHECK]` |
| **Gut-skin** | "probiotics for skin health" | GSC: 25 impressions. Keyword Planner 2,400; "best gut health supplement" 5,400. Ads: "best probiotic for acne" 2 conversions | Depends on the new SKUs `[NEED FROM RACHEL]` |

Note: `website/product-briefs/` doesn't exist in the repo yet, so I couldn't map the two new SKUs to concerns. The concern pages above are based on search data only.

### (e) Blog: refreshes and gaps, in order of impressions at stake

| # | Article | Target keyword | Data | What to do |
|---|---|---|---|---|
| 1 | **Refresh** `best-teas-for-hormone-balance` (keep the URL) | "tea for hormonal acne" | 47,178 cluster impressions, 252 clicks, 96 striking-distance queries (32,782 impressions) at positions 5 to 11. "tea for hormonal acne" 2,225 at 5.7; "best tea for hormonal acne" 1,801 at 5.2; "what tea is good for acne" 1,217 at 10.2 (0 clicks) | Example title: `7 Best Teas for Hormonal Acne & Hormone Balance` (47). Add spearmint (Keyword Planner 3,600), "estrogen tea" (516 at 8.6), "best tea for estrogen dominance" (365 at 5.6), dandelion and raspberry leaf. Add FAQ schema and a quiz/Balance CTA |
| 2 | **Rewrite title/H1** `can-coffee-make-hormonal-acne-worse` (keep the URL) | "does coffee cause acne" | 48,320 page impressions, 61 clicks (0.1% CTR). "does coffee cause acne" 1,336 at 37.9; "coffee and acne" 1,101 at 26.2; hormonal variants rank 5 to 9 | Example title: `Does Coffee Cause Acne? Caffeine and Hormonal Skin` (50). The current title is 2 titles joined with "\|" |
| 3 | **Merge** `balancing-hormones-with-food` + `hormonal-acne-diet-building-hormone-balancing-meals` | "hormonal acne diet" | Diet cluster: 3,630 impressions at position 54.9, **0 clicks**. "hormonal acne diet" 1,607 at 56; "foods for hormonal acne" variants ~800 | Keep one URL and 301 the other. The old URL has only 2 clicks in 16 months, so the better slug can win. Example title: `Hormonal Acne Diet: Foods That Support Clearer Skin` (51) |
| 4 | **New** "Hormonal acne pills vs supplements" | "hormonal acne pills" | "tablets for hormonal acne" 349 at 60; "hormonal acne tablets" 340 at 65; "hormonal acne pills" 192 at 54; "hormonal acne medication" 192 at 66; "gummies for hormonal acne" 221 at 30. These now land on the prescription-meds post | Example title: `Hormonal Acne Pills vs Supplements: How They Differ` (51). It can discuss prescription treatments factually; product mentions stay structure/function `[CLAIM CHECK]` |
| 5 | **New** DIM explainer | "DIM for hormonal acne" | Keyword Planner "dim supplement" 27,100, "dim estrogen" 1,000. GSC DIM cluster: only 542 impressions, 14 of them US | Example title: `DIM for Hormonal Acne: What It Does & Who It Suits` (50) `[CLAIM CHECK]`. Link to Balance |
| 6 | **New** calcium D-glucarate explainer | "calcium d glucarate benefits" | Keyword Planner 1,300 ("calcium d glucarate" 6,600). GSC: "calcium d glucarate acne" 58 impressions combined | Ingredient education that links to Balance |
| 7 | **Refresh** `can-hormonal-acne-be-caused-by-stress` | "cortisol acne" / "stress hormonal acne" | Stress cluster: 896 impressions at position 51, 0 clicks | Retitle around cortisol |
| 8 | **Refresh** `hormone-safe-sunscreens` | "hormone safe sunscreen" | 2,568 cluster impressions at position 16.0; "how to choose sunscreen that doesn't mess with hormones" 506 at 6.7 (0 clicks) | Better title and meta for CTR |
| 9 | **Refresh** `how-to-know-what-type-of-hormonal-acne-you-have` | "hormonal acne types" | 11,102 page impressions, 63 clicks. "hormonal acne types" 119 at 66 | Handle the estrogen-dominance queries on the hub (see d) and keep this post on "types" |
| 10 | Redirect `how-to-treat-hormonal-acne-in-2025` (404) → `how-to-treat-hormonal-acne-in-2026` | - | 854 impressions | 301 now. Long term, use an evergreen slug instead of a new year each January |

### "Treatment" in queries and compliant wording

What the search data says: queries containing treat/treatment/cure/heal/remedy/"get rid"/medication/fix come to **275 queries, 2,119 impressions and 2 clicks** in Search Console (table G1 below). "hormonal acne treatment" itself had 144 impressions at position 64. Paid data is different: "hormonal acne treatment" got ~6.8 Shopping conversions and "natural hormonal acne treatment" 1.8. People do type "treatment" when they're ready to buy. We can match that intent in **ads targeting and page topic** without making a **treatment claim** on the page. `[CLAIM CHECK]`

| Searcher wording | Where it shows up today | Compliant on-page wording (suggestion) |
|---|---|---|
| "hormonal acne treatment", "natural hormonal acne treatment" | Home title "Treat Hormonal Acne With All-Natural Supplements"; About title "Natural Hormonal Acne Treatment"; product tags "Hormonal Acne Treatment" and "Hormonal Pimples Treatment" | "A natural, root-cause approach to hormonal breakouts"; "Targets a root cause of hormonal breakouts: estrogen balance" `[CLAIM CHECK]` |
| "heal / cure / get rid of hormonal acne" | Ads terms; blog titles "How to Treat Hormonal Acne in 2026" and "How To Identify and Treat Your Hormonal Acne Type" | Educational H2s such as "What helps hormonal acne? What the research says", with product mentions limited to "supports clearer skin". Consider "clear up", "calm" or "support" in brand-blog titles `[CLAIM CHECK]` |
| "supplements for hormonal acne" | Commercial; converts in Ads | "Supplements for hormonal acne-prone skin"; "supports clearer skin by supporting healthy estrogen metabolism" `[CLAIM CHECK]` |
| "acne pills / tablets / medication" | Ranks on the prescription-meds post | Comparison content: "pills vs supplements: how they differ". Never call Balance a medication |
| "estrogen dominance treatment" (Keyword Planner 1,300) | Blog post slug "...natural-treatment" | "Natural support for healthy estrogen balance" |
| "results", "works", "clear skin for good" | Home: "Get real results"; "clear skin, once and for all" | Show typical results with the timeframe, e.g. "Most customers see … after … weeks" `[NEED FROM RACHEL: typical-results data]` (FTC) |


**G1. Queries containing treat / treatment / cure / heal / remedy / get rid / medication / fix - 275 queries, 2,119 impressions, 2 clicks (top 25)**

| Query | Impr. | Clicks | Avg pos | Cluster |
|---|---:|---:|---:|---|
| best organic acne treatments | 209 | 0 | 27.9 | General acne (non-hormonal wording) |
| hormonal acne medication | 192 | 0 | 66.2 | Prescription meds (spironolactone, Accutane, etc.) |
| acne treatment quiz | 156 | 0 | 44.0 | Acne / hormone quizzes |
| hormonal acne treatment | 144 | 0 | 64.2 | How to treat / get rid of / fix hormonal acne |
| how does acne medication work | 61 | 0 | 13.7 | Prescription meds (spironolactone, Accutane, etc.) |
| medication for hormonal acne | 53 | 0 | 64.1 | Prescription meds (spironolactone, Accutane, etc.) |
| acne hormonal treatment toronto | 52 | 0 | 63.1 | How to treat / get rid of / fix hormonal acne |
| hormonal acne treatment near me | 52 | 0 | 44.0 | How to treat / get rid of / fix hormonal acne |
| acne treatment test | 51 | 0 | 50.7 | Acne / hormone quizzes |
| what acne treatment should i use quiz | 50 | 0 | 69.9 | Acne / hormone quizzes |
| acne medication for hormonal acne | 44 | 0 | 78.2 | Prescription meds (spironolactone, Accutane, etc.) |
| best treatments for hormonal acne 2026 | 44 | 0 | 7.4 | How to treat / get rid of / fix hormonal acne |
| hormonal acne treatment prescription | 41 | 0 | 82.1 | Prescription meds (spironolactone, Accutane, etc.) |
| oral medication for hormonal acne | 37 | 0 | 50.9 | Prescription meds (spironolactone, Accutane, etc.) |
| is well woman supplement get rid of acne | 30 | 0 | 66.2 | Supplements for acne / clear skin (non-hormonal wording) |
| best acne treatments | 29 | 0 | 6.8 | General acne (non-hormonal wording) |
| natural remedies for hormonal acne thanks worked | 29 | 0 | 36.4 | How to treat / get rid of / fix hormonal acne |
| hormone medication for acne | 27 | 0 | 77.8 | Prescription meds (spironolactone, Accutane, etc.) |
| natural hormonal acne treatment for women | 25 | 0 | 35.5 | How to treat / get rid of / fix hormonal acne |
| how do acne medications work | 19 | 0 | 25.2 | Prescription meds (spironolactone, Accutane, etc.) |
| vegan acne treatments | 19 | 0 | 69.5 | General acne (non-hormonal wording) |
| acne hormonal treatment | 16 | 0 | 80.7 | How to treat / get rid of / fix hormonal acne |
| acne hormonal medication | 15 | 0 | 70.2 | Prescription meds (spironolactone, Accutane, etc.) |
| best treatments for hormonal acne 2025 2026 | 15 | 0 | 8.6 | How to treat / get rid of / fix hormonal acne |
| hormonal breakout treatment | 15 | 0 | 66.9 | How to treat / get rid of / fix hormonal acne |

Add the DSHEA disclaimer wherever structure/function claims appear (product, home, collection, quiz results): *"These statements have not been evaluated by the Food and Drug Administration. This product is not intended to diagnose, treat, cure, or prevent any disease."* I didn't find it in the HTML of any of the five audited pages.

---

## 9. Live site on-page review (cocoonsupplements.com, fetched 13 Oct 2026)

| Page | Title (characters) | Meta description (characters) | H1 | Canonical | Issues |
|---|---|---|---|---|---|
| `/` | "Treat Hormonal Acne With All-Natural Supplements \| Cocoon" (57) | "Combat hormonal acne naturally… Get real results." (157, over 155) | "A natural solution for hormonal acne" | `https://cocoonsupplements.com/` ✅ | Disease-claim wording in the title, meta and og:title. Meta 2 characters too long. No DSHEA disclaimer. Only ~450 words of visible copy. Organization/WebSite schema present ✅ |
| `/products/balance` | "Natural Supplement For Hormonal Acne \| Cocoon" (45) | "Struggling with hormonal acne?… for clearer skin." (160, over 155) | "BALANCE" (no keyword) | self ✅ | H1 and og:title are just "BALANCE". Product type "Skincare" (should be a supplement type, which also matters for the Google Shopping category). Tags "Hormonal Acne Treatment" and "Hormonal Pimples Treatment" appear in the page JSON. "treatment"/"heal" in copy. No DSHEA disclaimer found. Product + AggregateRating schema and USD pricing ✅. Copy says "Canadian-made in a Health Canada licensed facility", which is fine as a fact; check the US quality/cGMP wording `[CLAIM CHECK]` |
| `/pages/quiz` | "Could High Estrogen Be Causing Your Acne? Take Our Free Quiz – Cocoon" (69, over 60) | 149 ✅ | "HORMONE IMBALANCE QUIZ" | self ✅ | The title gets truncated and misses "acne quiz" demand. Only ~270 words of indexable text |
| `/pages/learn` | "Guide to Hormonal Acne: Causes, Symptoms, & Natural Remedies – Cocoon" (69, over 60) | 134 ✅ | "UNDERSTANDING HORMONAL ACNE" | self ✅ | Title too long. "Hormonal Acne Treatment" string in the HTML. Ranks at position 47 for "hormonal acne" |
| `/blogs/cocoon-blog` | "Banish Breakouts: Discover Natural Solutions for Hormonal Acne – Cocoon" (71, over 60) | 145 ✅ | **Two H1s**: "A GUIDE" and "UNDERSTANDING & TREATING HORMONAL ACNE NATURALLY" | self ✅ | Duplicate H1. "Treating" in the H1. 12 images with empty alt. Post titles with "Treat" / "Treatment" |
| `/pages/about` (extra) | "Natural Hormonal Acne Treatment \| Cocoon" | "Our mission is clear: treat hormonal acne naturally…" | none | self ✅ | Disease-claim title and meta. No H1. Ranks for brand queries (12,614 impressions at position 4.5) |
| `/pages/results` (extra) | "Cocoon for Hormonal Breakouts \| Customer Reviews" | ✅ | none | self ✅ | No H1. This is the page Google shows for "cocoon skin care reviews" (365 impressions, 40 clicks). `/pages/results-1` is a near-duplicate with no meta description: 301 it to `/pages/results`. `/pages/reviews` gets almost nothing (22 impressions) |

Site-wide checks:
- **Canonicals:** all self-referencing on cocoonsupplements.com ✅. **No canonical, og:url or hreflang points to cocoonskincare.ca**: 0 references to the .ca domain in any audited page's HTML ✅. There are no hreflang tags at all. That's correct as long as .ca 301s to .com; don't add .ca hreflang alternates unless .ca goes back to being a separate live market.
- **Sitemap:** robots.txt points to `/sitemap.xml`, which lists 14 pages, 1 product, the blog and 21 articles on cocoonsupplements.com ✅. `/pages/typeform` is in the sitemap; check whether it should be indexed.
- **Currency:** USD (`Shopify.currency = USD`, schema priceCurrency USD) ✅. Balance shows 1-month $50.00 and 3-month $130.50 in products.json.
- **Old URLs on the new domain:** 11 URLs from Search Console return 404 (table D1). `/products/dim` → `/products/balance` and `/pages/learn-1` → `/pages/learn` already 301 ✅. `/products/balance-thermae` is `noindex,nofollow` but still had 2,320 impressions on .ca; leave it noindexed or 301 it to Balance if it's retired.
- **Merchant Center:** Search Console lists `/products/balance?variant=…&country=CA&currency=CAD&utm_…sag_organic` URLs (free listings). Update the feed to the .com domain and USD.

---

## 10. What I couldn't get

- **Search Console for cocoonsupplements.com:** not connected. We can't measure how much equity has transferred since the ~4 Oct cut-over.
- **Old-domain redirect test:** the network proxy here refused `cocoonskincare.ca` (HTTP 502 on CONNECT), so I couldn't confirm that each .ca URL 301s to the same path on .com. Please spot-check the top 15 URLs in table D1 from a browser, or with `curl -I`.
- **Search volume for acne keywords:** Keyword Planner returned zero rows for every seed containing "acne". Semrush/Ahrefs aren't connected. Every acne figure here is Search Console impressions, not volume.
- **Complete Google Ads search-term clicks and cost:** the unfiltered search-term pull was too large for the connector and failed, and filtered pulls only count the matching days. Conversions and conversion value per term are complete; clicks and cost per term are minimums.
- **Reliable page × country split:** the API's page × country totals didn't reconcile with the page totals, so I've left them out.
- **Anonymised queries:** about 55% of clicks (3,381 of 6,136) and 65% of impressions come from queries Google doesn't disclose.
- **Briefs for the new products:** `website/product-briefs/` isn't in the repo, so concern pages for the two new SKUs are marked `[NEED FROM RACHEL]`.
- **Not in scope / not pulled:** GA4 and Shopify landing-page conversion data, and backlink data. The latter would tell us which old URLs have external links worth protecting beyond the click data.

---
## Appendix A: top queries (full period, all countries)

US and CA columns show impressions with the average position in brackets; other countries make up the rest. "Top page" is the page with the most impressions for that query.

### A1. Top 100 queries by impressions

| # | Query | Clicks | Impr. | CTR | Avg pos | US impr. (pos) | CA impr. (pos) | Cluster | Top page |
|---|---|---:|---:|---:|---:|---:|---:|---|---|
| 1 | cocoon skin care | 457 | 3,932 | 11.6% | 4.0 | 1,869 (3.2) | 673 (1.4) | Brand: Cocoon (ours) | / |
| 2 | hormonal acne supplements | 20 | 3,480 | 0.6% | 17.2 | 502 (20.9) | 1,968 (10.8) | Supplements for hormonal acne | / |
| 3 | cocoon | 6 | 2,710 | 0.2% | 6.6 | 23 (8.5) | 2,652 (6.4) | Brand: ambiguous "cocoon" (other businesses / bare word) | / |
| 4 | tea for hormonal acne | 29 | 2,225 | 1.3% | 5.7 | 1,015 (5.5) | 153 (4.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 5 | cocoon skincare | 376 | 2,182 | 17.2% | 4.0 | 630 (3.4) | 421 (1.3) | Brand: Cocoon (ours) | / |
| 6 | tea for hormonal imbalance | 6 | 2,117 | 0.3% | 10.7 | 218 (11.2) | 208 (6.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 7 | best tea for hormonal acne | 14 | 1,801 | 0.8% | 5.2 | 635 (4.8) | 134 (4.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 8 | hormonal acne diet | 0 | 1,607 | 0.0% | 56.0 | 946 (52.5) | 15 (32.5) | Diet / food | /blogs/cocoon-blog/balancing-hormones-with-food |
| 9 | supplements for hormonal acne | 6 | 1,489 | 0.4% | 27.3 | 671 (34.1) | 441 (10.3) | Supplements for hormonal acne | / |
| 10 | does coffee cause acne | 0 | 1,336 | 0.0% | 37.9 | 730 (40.1) | 219 (12.6) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 11 | what tea is good for acne | 0 | 1,217 | 0.0% | 10.2 | 1,025 (10.9) | 127 (5.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 12 | coffee and acne | 0 | 1,101 | 0.0% | 26.2 | 610 (28.4) | 283 (9.9) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 13 | best tea for hormonal imbalance | 3 | 1,027 | 0.3% | 7.9 | 136 (6.0) | 140 (5.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 14 | best tea for acne | 5 | 1,022 | 0.5% | 8.4 | 331 (13.4) | 412 (4.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 15 | cocoon supplement | 587 | 999 | 58.8% | 1.2 | 248 (1.0) | 524 (1.1) | Brand: Cocoon (ours) | / |
| 16 | how to balance hormones for acne | 0 | 948 | 0.0% | 53.2 | 224 (66.6) | 23 (34.9) | Hormonal acne: what / causes / types | /blogs/cocoon-blog/balancing-hormones-with-food |
| 17 | herbal tea for acne | 6 | 883 | 0.7% | 10.2 | 645 (9.9) | 55 (6.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 18 | acne supplements | 3 | 864 | 0.4% | 13.0 | 12 (33.3) | 840 (12.7) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 19 | acne quiz | 2 | 851 | 0.2% | 31.6 | 664 (31.6) | 32 (19.6) | Acne / hormone quizzes | /pages/quiz |
| 20 | acne supplements canada | 7 | 796 | 0.9% | 9.0 | 5 (4.2) | 780 (9.1) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 21 | what tea is good for hormonal acne | 7 | 796 | 0.9% | 5.1 | 489 (5.4) | 49 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 22 | cocoon acne supplement | 501 | 784 | 63.9% | 1.0 | 234 (1.0) | 285 (1.0) | Brand: Cocoon (ours) | / |
| 23 | cocoon canada | 51 | 784 | 6.5% | 10.0 | 39 (5.6) | 601 (9.9) | Brand: Cocoon (ours) | / |
| 24 | herbal teas for acne | 5 | 765 | 0.7% | 5.9 | 100 (8.7) | 17 (6.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 25 | hormonal acne supplement | 7 | 756 | 0.9% | 21.2 | 268 (20.5) | 143 (8.4) | Supplements for hormonal acne | / |
| 26 | what tea helps with acne | 0 | 724 | 0.0% | 9.1 | 600 (9.6) | 82 (5.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 27 | cocoon skin | 101 | 632 | 16.0% | 5.5 | 134 (2.4) | 142 (1.0) | Brand: Cocoon (ours) | / |
| 28 | what tea helps with hormonal acne | 1 | 626 | 0.2% | 5.3 | 463 (5.5) | 28 (4.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 29 | does caffeine cause acne | 0 | 613 | 0.0% | 29.7 | 301 (38.0) | 214 (12.1) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 30 | natural supplements for hormonal acne | 0 | 590 | 0.0% | 32.1 | 222 (35.2) | 73 (11.6) | Supplements for hormonal acne | / |
| 31 | hormonal acne tea | 7 | 575 | 1.2% | 6.8 | 181 (6.4) | 29 (5.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 32 | what type of acne do i have quiz | 0 | 572 | 0.0% | 45.0 | 505 (45.1) | 7 (32.9) | Acne / hormone quizzes | /pages/quiz |
| 33 | cocoon delivery | 1 | 568 | 0.2% | 18.7 | 486 (17.8) | 2 (4.0) | Brand: ambiguous "cocoon" (other businesses / bare word) | /pages/shipping-policy |
| 34 | tea that helps with acne | 1 | 553 | 0.2% | 11.4 | 466 (12.3) | 41 (5.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 35 | can coffee cause acne | 0 | 551 | 0.0% | 30.9 | 160 (37.5) | 195 (11.8) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 36 | teas for hormonal acne | 18 | 549 | 3.3% | 5.1 | 311 (5.4) | 37 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 37 | tea to balance female hormones | 3 | 543 | 0.5% | 8.6 | 220 (8.7) | 110 (6.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 38 | best herbal tea for hormonal imbalance | 2 | 538 | 0.4% | 9.0 | 60 (9.7) | 15 (5.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 39 | skincare supplement | 0 | 533 | 0.0% | 21.8 | 21 (49.7) | 472 (19.7) | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |
| 40 | estrogen tea | 2 | 516 | 0.4% | 8.6 | 309 (8.9) | 60 (5.7) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 41 | how to choose sunscreen that doesn’t mess with hormones | 0 | 506 | 0.0% | 6.7 | 502 (6.7) | 0 (-) | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |
| 42 | supplements for acne | 1 | 474 | 0.2% | 16.5 | 19 (12.9) | 426 (16.9) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 43 | what tea is good for hormonal imbalance | 3 | 473 | 0.6% | 8.9 | 167 (9.6) | 59 (3.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 44 | hormonal acne | 1 | 470 | 0.2% | 47.1 | 47 (37.8) | 360 (49.5) | Hormonal acne: what / causes / types | /pages/learn |
| 45 | herbal tea for hormonal imbalance | 1 | 465 | 0.2% | 9.7 | 103 (11.8) | 27 (4.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 46 | which tea is good for hormonal imbalance | 2 | 449 | 0.4% | 8.6 | 30 (10.7) | 64 (4.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 47 | teas that help with acne | 6 | 448 | 1.3% | 7.5 | 291 (8.1) | 46 (5.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 48 | natural supplements for acne | 0 | 421 | 0.0% | 28.3 | 23 (58.5) | 359 (23.3) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 49 | acne affiliate programs | 1 | 418 | 0.2% | 6.7 | 413 (6.8) | 1 (4.0) | Affiliate / wholesale | /pages/affiliate-program |
| 50 | does coffee make you break out | 0 | 415 | 0.0% | 13.8 | 156 (13.4) | 149 (10.0) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 51 | can coffee cause hormonal acne | 1 | 414 | 0.2% | 8.8 | 269 (8.8) | 48 (6.2) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 52 | cocoon apothecary | 0 | 402 | 0.0% | 52.6 | 22 (60.3) | 314 (52.5) | Brand: ambiguous "cocoon" (other businesses / bare word) | / |
| 53 | caffeine and acne | 0 | 392 | 0.0% | 16.2 | 106 (20.1) | 187 (9.8) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 54 | best teas for hormonal acne | 11 | 378 | 2.9% | 4.3 | 195 (4.2) | 36 (3.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 55 | estrogen dominance acne | 4 | 371 | 1.1% | 11.0 | 133 (10.6) | 132 (8.1) | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |
| 56 | cocoon skin care reviews | 40 | 365 | 11.0% | 2.8 | 39 (2.6) | 128 (1.4) | Brand: Cocoon (ours) | /pages/results |
| 57 | best tea for estrogen dominance | 0 | 365 | 0.0% | 5.6 | 208 (5.9) | 47 (3.7) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 58 | tea for acne | 0 | 357 | 0.0% | 10.8 | 152 (13.4) | 195 (8.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 59 | skin supplements for acne | 0 | 350 | 0.0% | 16.6 | 1 (24.0) | 347 (16.6) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 60 | tablets for hormonal acne | 0 | 349 | 0.0% | 60.1 | 113 (62.8) | 1 (30.0) | Supplements for hormonal acne | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| 61 | hormonal imbalance tea | 2 | 348 | 0.6% | 8.9 | 72 (9.2) | 29 (6.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 62 | what is causing my acne quiz | 4 | 344 | 1.2% | 12.1 | 229 (13.2) | 30 (5.8) | Acne / hormone quizzes | /pages/quiz |
| 63 | hormonal acne tablets | 0 | 340 | 0.0% | 65.0 | 120 (61.4) | 1 (12.0) | Supplements for hormonal acne | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| 64 | dandelion tea for acne | 2 | 334 | 0.6% | 9.3 | 148 (10.5) | 70 (7.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 65 | teas for hormonal balance | 1 | 330 | 0.3% | 9.3 | 86 (11.3) | 75 (6.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 66 | can caffeine cause acne | 0 | 322 | 0.0% | 19.8 | 44 (36.9) | 219 (11.4) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 67 | can coffee make you break out | 0 | 322 | 0.0% | 14.5 | 101 (16.8) | 119 (8.4) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 68 | coffee acne | 1 | 320 | 0.3% | 21.5 | 87 (20.5) | 120 (9.8) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 69 | is coffee bad for acne | 0 | 320 | 0.0% | 18.8 | 40 (28.2) | 201 (11.0) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 70 | best teas for acne | 5 | 314 | 1.6% | 6.7 | 46 (11.5) | 102 (5.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 71 | best tea for hormone balance | 0 | 306 | 0.0% | 10.1 | 100 (14.0) | 63 (5.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 72 | what teas help with acne | 0 | 306 | 0.0% | 8.9 | 238 (9.6) | 20 (4.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 73 | cocooncenter canada | 2 | 304 | 0.7% | 11.0 | 9 (8.4) | 276 (10.5) | Brand: ambiguous "cocoon" (other businesses / bare word) | / |
| 74 | caffeine acne | 0 | 304 | 0.0% | 16.1 | 107 (18.1) | 120 (9.7) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 75 | acne supplement | 7 | 301 | 2.3% | 10.8 | 10 (14.7) | 276 (10.3) | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |
| 76 | tea that helps with hormonal acne | 2 | 300 | 0.7% | 5.8 | 196 (5.9) | 11 (4.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 77 | hormone balance tea | 0 | 288 | 0.0% | 10.7 | 121 (3.0) | 104 (12.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 78 | teas that help with hormonal imbalance | 0 | 287 | 0.0% | 10.3 | 180 (11.2) | 9 (4.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 79 | teas that help with hormonal acne | 3 | 285 | 1.1% | 5.2 | 200 (5.2) | 17 (3.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 80 | el café es malo para el acné hormonal | 1 | 284 | 0.4% | 5.6 | 37 (4.5) | 0 (-) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 81 | cacoon offers | 0 | 284 | 0.0% | 16.2 | 0 (-) | 274 (13.4) | Brand: ambiguous "cocoon" (other businesses / bare word) | /account/login |
| 82 | balance supplement | 2 | 282 | 0.7% | 3.8 | 1 (11.0) | 281 (3.8) | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |
| 83 | what kind of acne do i have quiz | 0 | 277 | 0.0% | 36.2 | 258 (36.7) | 7 (23.9) | Acne / hormone quizzes | /pages/quiz |
| 84 | supplements for clear skin | 0 | 276 | 0.0% | 37.4 | 24 (36.0) | 220 (37.6) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 85 | coffee and hormonal acne | 3 | 267 | 1.1% | 7.1 | 172 (6.8) | 20 (5.5) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 86 | hormonal acne quiz | 40 | 265 | 15.1% | 2.4 | 163 (2.5) | 15 (1.1) | Acne / hormone quizzes | /pages/quiz |
| 87 | what tea helps acne | 0 | 265 | 0.0% | 9.5 | 229 (10.2) | 27 (4.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 88 | el cafe causa acne | 0 | 263 | 0.0% | 10.8 | 32 (10.5) | 0 (-) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 89 | hormonal acne natural supplements | 0 | 262 | 0.0% | 31.2 | 28 (27.0) | 9 (11.4) | Supplements for hormonal acne | / |
| 90 | what tea is best for acne | 0 | 261 | 0.0% | 8.5 | 195 (9.1) | 42 (6.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 91 | hormone balancing tea | 1 | 257 | 0.4% | 14.2 | 40 (4.3) | 112 (13.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 92 | which tea is best for hormonal imbalance | 1 | 251 | 0.4% | 7.5 | 30 (10.5) | 34 (5.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 93 | hormonal skincare | 0 | 251 | 0.0% | 32.8 | 62 (52.7) | 150 (24.9) | Topicals / skincare routine | / |
| 94 | caffeine and hormonal acne | 1 | 249 | 0.4% | 5.2 | 111 (6.5) | 82 (2.2) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 95 | hormonal tea | 2 | 248 | 0.8% | 8.7 | 51 (10.9) | 41 (6.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 96 | herbal tea for acne skin | 1 | 247 | 0.4% | 9.6 | 231 (9.7) | 6 (6.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 97 | what tea is best for hormonal acne | 4 | 241 | 1.7% | 4.4 | 138 (4.5) | 11 (4.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 98 | why am i breaking out quiz | 1 | 240 | 0.4% | 11.7 | 209 (11.9) | 3 (6.7) | Acne / hormone quizzes | /pages/quiz |
| 99 | why do i have acne quiz | 1 | 240 | 0.4% | 13.6 | 196 (14.6) | 11 (7.4) | Acne / hormone quizzes | /pages/quiz |
| 100 | is coffee bad for hormonal acne | 0 | 236 | 0.0% | 8.0 | 116 (8.3) | 25 (6.2) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |

### A2. Top 100 queries by clicks

| # | Query | Clicks | Impr. | CTR | Avg pos | US impr. (pos) | CA impr. (pos) | Cluster | Top page |
|---|---|---:|---:|---:|---:|---:|---:|---|---|
| 1 | cocoon supplement | 587 | 999 | 58.8% | 1.2 | 248 (1.0) | 524 (1.1) | Brand: Cocoon (ours) | / |
| 2 | cocoon acne supplement | 501 | 784 | 63.9% | 1.0 | 234 (1.0) | 285 (1.0) | Brand: Cocoon (ours) | / |
| 3 | cocoon skin care | 457 | 3,932 | 11.6% | 4.0 | 1,869 (3.2) | 673 (1.4) | Brand: Cocoon (ours) | / |
| 4 | cocoon skincare | 376 | 2,182 | 17.2% | 4.0 | 630 (3.4) | 421 (1.3) | Brand: Cocoon (ours) | / |
| 5 | cocoon skin | 101 | 632 | 16.0% | 5.5 | 134 (2.4) | 142 (1.0) | Brand: Cocoon (ours) | / |
| 6 | cocoon acne | 60 | 99 | 60.6% | 1.4 | 37 (1.0) | 21 (1.0) | Brand: Cocoon (ours) | / |
| 7 | cocoon canada | 51 | 784 | 6.5% | 10.0 | 39 (5.6) | 601 (9.9) | Brand: Cocoon (ours) | / |
| 8 | cocoon balance | 46 | 122 | 37.7% | 1.0 | 18 (1.0) | 73 (1.0) | Brand: Cocoon (ours) | / |
| 9 | cocoon skin care reviews | 40 | 365 | 11.0% | 2.8 | 39 (2.6) | 128 (1.4) | Brand: Cocoon (ours) | /pages/results |
| 10 | hormonal acne quiz | 40 | 265 | 15.1% | 2.4 | 163 (2.5) | 15 (1.1) | Acne / hormone quizzes | /pages/quiz |
| 11 | tea for hormonal acne | 29 | 2,225 | 1.3% | 5.7 | 1,015 (5.5) | 153 (4.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 12 | cocoonskincare.ca | 24 | 37 | 64.9% | 1.0 | 7 (1.0) | 8 (1.0) | Brand: Cocoon (ours) | / |
| 13 | hormonal acne supplements | 20 | 3,480 | 0.6% | 17.2 | 502 (20.9) | 1,968 (10.8) | Supplements for hormonal acne | / |
| 14 | cocoonskincare | 19 | 37 | 51.3% | 3.3 | 12 (2.2) | 3 (1.0) | Brand: Cocoon (ours) | / |
| 15 | teas for hormonal acne | 18 | 549 | 3.3% | 5.1 | 311 (5.4) | 37 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 16 | cocoon skincare reviews | 16 | 120 | 13.3% | 1.9 | 22 (2.2) | 81 (1.6) | Brand: Cocoon (ours) | /pages/results |
| 17 | best tea for hormonal acne | 14 | 1,801 | 0.8% | 5.2 | 635 (4.8) | 134 (4.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 18 | best teas for hormonal acne | 11 | 378 | 2.9% | 4.3 | 195 (4.2) | 36 (3.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 19 | cocoon balance hormonal acne supplement | 9 | 40 | 22.5% | 4.9 | 2 (1.0) | 27 (1.1) | Brand: Cocoon (ours) | /products/balance |
| 20 | cocoon acne supplement reviews | 8 | 28 | 28.6% | 1.2 | 0 (-) | 24 (1.1) | Brand: Cocoon (ours) | /products/balance |
| 21 | acne supplements canada | 7 | 796 | 0.9% | 9.0 | 5 (4.2) | 780 (9.1) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 22 | what tea is good for hormonal acne | 7 | 796 | 0.9% | 5.1 | 489 (5.4) | 49 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 23 | hormonal acne supplement | 7 | 756 | 0.9% | 21.2 | 268 (20.5) | 143 (8.4) | Supplements for hormonal acne | / |
| 24 | hormonal acne tea | 7 | 575 | 1.2% | 6.8 | 181 (6.4) | 29 (5.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 25 | acne supplement | 7 | 301 | 2.3% | 10.8 | 10 (14.7) | 276 (10.3) | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |
| 26 | cocoon | 6 | 2,710 | 0.2% | 6.6 | 23 (8.5) | 2,652 (6.4) | Brand: ambiguous "cocoon" (other businesses / bare word) | / |
| 27 | tea for hormonal imbalance | 6 | 2,117 | 0.3% | 10.7 | 218 (11.2) | 208 (6.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 28 | supplements for hormonal acne | 6 | 1,489 | 0.4% | 27.3 | 671 (34.1) | 441 (10.3) | Supplements for hormonal acne | / |
| 29 | herbal tea for acne | 6 | 883 | 0.7% | 10.2 | 645 (9.9) | 55 (6.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 30 | teas that help with acne | 6 | 448 | 1.3% | 7.5 | 291 (8.1) | 46 (5.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 31 | raspberry leaf tea estrogen dominance | 6 | 218 | 2.8% | 7.1 | 141 (7.5) | 21 (5.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 32 | cocoon hormone balance | 6 | 15 | 40.0% | 1.2 | 5 (1.0) | 9 (1.3) | Brand: Cocoon (ours) | / |
| 33 | cocoon skin co | 6 | 9 | 66.7% | 1.1 | 2 (1.0) | 4 (1.0) | Brand: Cocoon (ours) | / |
| 34 | best tea for acne | 5 | 1,022 | 0.5% | 8.4 | 331 (13.4) | 412 (4.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 35 | herbal teas for acne | 5 | 765 | 0.7% | 5.9 | 100 (8.7) | 17 (6.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 36 | best teas for acne | 5 | 314 | 1.6% | 6.7 | 46 (11.5) | 102 (5.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 37 | estrogen dominance acne | 4 | 371 | 1.1% | 11.0 | 133 (10.6) | 132 (8.1) | Estrogen dominance / high estrogen / progesterone | /blogs/cocoon-blog/how-to-know-what-type-of-hormonal-acne-you-have |
| 38 | what is causing my acne quiz | 4 | 344 | 1.2% | 12.1 | 229 (13.2) | 30 (5.8) | Acne / hormone quizzes | /pages/quiz |
| 39 | what tea is best for hormonal acne | 4 | 241 | 1.7% | 4.4 | 138 (4.5) | 11 (4.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 40 | best herbal tea for acne | 4 | 186 | 2.1% | 7.4 | 14 (9.0) | 25 (4.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 41 | dandelion root tea for acne | 4 | 156 | 2.6% | 9.7 | 97 (10.8) | 30 (6.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 42 | cocoon skincare review | 4 | 104 | 3.9% | 4.4 | 53 (2.8) | 17 (3.8) | Brand: Cocoon (ours) | /pages/results |
| 43 | cocoon acne supplement reddit | 4 | 15 | 26.7% | 2.4 | 2 (2.5) | 12 (2.2) | Brand: Cocoon (ours) | / |
| 44 | best tea for hormonal imbalance | 3 | 1,027 | 0.3% | 7.9 | 136 (6.0) | 140 (5.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 45 | acne supplements | 3 | 864 | 0.4% | 13.0 | 12 (33.3) | 840 (12.7) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 46 | tea to balance female hormones | 3 | 543 | 0.5% | 8.6 | 220 (8.7) | 110 (6.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 47 | what tea is good for hormonal imbalance | 3 | 473 | 0.6% | 8.9 | 167 (9.6) | 59 (3.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 48 | teas that help with hormonal acne | 3 | 285 | 1.1% | 5.2 | 200 (5.2) | 17 (3.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 49 | coffee and hormonal acne | 3 | 267 | 1.1% | 7.1 | 172 (6.8) | 20 (5.5) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 50 | which tea is good for hormonal acne | 3 | 230 | 1.3% | 5.4 | 58 (4.5) | 25 (3.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 51 | herbal tea for hormonal acne | 3 | 217 | 1.4% | 5.7 | 71 (5.9) | 10 (3.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 52 | tea good for hormonal acne | 3 | 215 | 1.4% | 5.4 | 114 (5.9) | 18 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 53 | hormonal acne pills | 3 | 192 | 1.6% | 53.9 | 79 (63.5) | 39 (14.5) | Supplements for hormonal acne | /blogs/cocoon-blog/the-truth-about-prescription-acne-medications |
| 54 | teas for hormonal imbalance | 3 | 133 | 2.3% | 8.6 | 54 (10.6) | 17 (4.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 55 | supplement for acne | 3 | 110 | 2.7% | 30.4 | 29 (42.0) | 61 (11.1) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 56 | tea to help with hormonal acne | 3 | 103 | 2.9% | 6.5 | 78 (6.7) | 1 (1.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 57 | raspberry leaf tea estrogen | 3 | 77 | 3.9% | 8.9 | 38 (8.5) | 13 (8.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 58 | cocoon capsule | 3 | 23 | 13.0% | 10.1 | 2 (3.5) | 6 (1.3) | Brand: Cocoon (ours) | /products/balance |
| 59 | nettle tea acne | 3 | 22 | 13.6% | 14.0 | 6 (23.0) | 11 (9.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 60 | acne quiz | 2 | 851 | 0.2% | 31.6 | 664 (31.6) | 32 (19.6) | Acne / hormone quizzes | /pages/quiz |
| 61 | best herbal tea for hormonal imbalance | 2 | 538 | 0.4% | 9.0 | 60 (9.7) | 15 (5.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 62 | estrogen tea | 2 | 516 | 0.4% | 8.6 | 309 (8.9) | 60 (5.7) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 63 | which tea is good for hormonal imbalance | 2 | 449 | 0.4% | 8.6 | 30 (10.7) | 64 (4.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 64 | hormonal imbalance tea | 2 | 348 | 0.6% | 8.9 | 72 (9.2) | 29 (6.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 65 | dandelion tea for acne | 2 | 334 | 0.6% | 9.3 | 148 (10.5) | 70 (7.2) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 66 | cocooncenter canada | 2 | 304 | 0.7% | 11.0 | 9 (8.4) | 276 (10.5) | Brand: ambiguous "cocoon" (other businesses / bare word) | / |
| 67 | tea that helps with hormonal acne | 2 | 300 | 0.7% | 5.8 | 196 (5.9) | 11 (4.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 68 | balance supplement | 2 | 282 | 0.7% | 3.8 | 1 (11.0) | 281 (3.8) | Supplements for acne / clear skin (non-hormonal wording) | /products/balance |
| 69 | hormonal tea | 2 | 248 | 0.8% | 8.7 | 51 (10.9) | 41 (6.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 70 | best teas for hormone balance | 2 | 227 | 0.9% | 8.1 | 40 (10.1) | 43 (6.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 71 | what tea helps hormonal acne | 2 | 221 | 0.9% | 5.3 | 173 (5.5) | 18 (3.4) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 72 | teas for acne | 2 | 219 | 0.9% | 8.6 | 124 (10.1) | 65 (6.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 73 | hormonal imbalance tea for females | 2 | 214 | 0.9% | 8.5 | 83 (8.5) | 8 (6.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 74 | what teas help with hormonal acne | 2 | 206 | 1.0% | 5.5 | 178 (5.6) | 8 (3.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 75 | dandelion tea acne | 2 | 154 | 1.3% | 10.0 | 64 (10.8) | 32 (8.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 76 | best tea for hormonal balance | 2 | 107 | 1.9% | 13.4 | 42 (21.5) | 11 (4.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 77 | what teas are good for hormonal acne | 2 | 101 | 2.0% | 5.5 | 62 (5.8) | 10 (3.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 78 | spearmint tea estrogen dominance | 2 | 93 | 2.1% | 8.6 | 51 (9.6) | 7 (5.1) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 79 | the cocoon skincare | 2 | 93 | 2.1% | 6.2 | 42 (7.6) | 24 (1.3) | Brand: Cocoon (ours) | / |
| 80 | cocoon products | 2 | 87 | 2.3% | 9.6 | 18 (11.3) | 58 (5.9) | Brand: Cocoon (ours) | / |
| 81 | raspberry leaf tea acne | 2 | 67 | 3.0% | 3.9 | 43 (4.5) | 6 (2.5) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 82 | tea that helps hormonal acne | 2 | 65 | 3.1% | 7.5 | 38 (7.2) | 3 (6.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 83 | cocoon ca | 2 | 41 | 4.9% | 15.6 | 8 (1.0) | 23 (26.7) | Brand: Cocoon (ours) | / |
| 84 | edc free sunscreen | 2 | 18 | 11.1% | 7.4 | 9 (6.7) | 1 (3.0) | Sunscreen / endocrine disruptors | /blogs/cocoon-blog/hormone-safe-sunscreens |
| 85 | post pill acne supplements | 2 | 9 | 22.2% | 7.4 | 0 (-) | 9 (7.4) | Birth control / post-pill | /products/balance |
| 86 | cocoon supplements | 2 | 3 | 66.7% | 1.0 | 2 (1.0) | 1 (1.0) | Brand: Cocoon (ours) | / |
| 87 | what tea helps with hormonal acne | 1 | 626 | 0.2% | 5.3 | 463 (5.5) | 28 (4.3) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 88 | cocoon delivery | 1 | 568 | 0.2% | 18.7 | 486 (17.8) | 2 (4.0) | Brand: ambiguous "cocoon" (other businesses / bare word) | /pages/shipping-policy |
| 89 | tea that helps with acne | 1 | 553 | 0.2% | 11.4 | 466 (12.3) | 41 (5.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 90 | supplements for acne | 1 | 474 | 0.2% | 16.5 | 19 (12.9) | 426 (16.9) | Supplements for acne / clear skin (non-hormonal wording) | / |
| 91 | hormonal acne | 1 | 470 | 0.2% | 47.1 | 47 (37.8) | 360 (49.5) | Hormonal acne: what / causes / types | /pages/learn |
| 92 | herbal tea for hormonal imbalance | 1 | 465 | 0.2% | 9.7 | 103 (11.8) | 27 (4.9) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 93 | acne affiliate programs | 1 | 418 | 0.2% | 6.7 | 413 (6.8) | 1 (4.0) | Affiliate / wholesale | /pages/affiliate-program |
| 94 | can coffee cause hormonal acne | 1 | 414 | 0.2% | 8.8 | 269 (8.8) | 48 (6.2) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 95 | teas for hormonal balance | 1 | 330 | 0.3% | 9.3 | 86 (11.3) | 75 (6.8) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 96 | coffee acne | 1 | 320 | 0.3% | 21.5 | 87 (20.5) | 120 (9.8) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 97 | el café es malo para el acné hormonal | 1 | 284 | 0.4% | 5.6 | 37 (4.5) | 0 (-) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |
| 98 | hormone balancing tea | 1 | 257 | 0.4% | 14.2 | 40 (4.3) | 112 (13.6) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 99 | which tea is best for hormonal imbalance | 1 | 251 | 0.4% | 7.5 | 30 (10.5) | 34 (5.0) | Teas for hormones / acne | /blogs/cocoon-blog/best-teas-for-hormone-balance |
| 100 | caffeine and hormonal acne | 1 | 249 | 0.4% | 5.2 | 111 (6.5) | 82 (2.2) | Coffee / caffeine and acne | /blogs/cocoon-blog/can-coffee-make-hormonal-acne-worse |

### A3. Top 30 non-brand queries in United States (by impressions)

| # | Query | Clicks | Impr. | CTR | Avg pos | Cluster |
|---|---|---:|---:|---:|---:|---|
| 1 | what tea is good for acne | 0 | 1,025 | 0.0% | 10.9 | Teas for hormones / acne |
| 2 | tea for hormonal acne | 8 | 1,015 | 0.8% | 5.5 | Teas for hormones / acne |
| 3 | hormonal acne diet | 0 | 946 | 0.0% | 52.5 | Diet / food |
| 4 | does coffee cause acne | 0 | 730 | 0.0% | 40.1 | Coffee / caffeine and acne |
| 5 | supplements for hormonal acne | 0 | 671 | 0.0% | 34.1 | Supplements for hormonal acne |
| 6 | acne quiz | 1 | 664 | 0.2% | 31.6 | Acne / hormone quizzes |
| 7 | herbal tea for acne | 2 | 645 | 0.3% | 9.9 | Teas for hormones / acne |
| 8 | best tea for hormonal acne | 5 | 635 | 0.8% | 4.8 | Teas for hormones / acne |
| 9 | coffee and acne | 0 | 610 | 0.0% | 28.4 | Coffee / caffeine and acne |
| 10 | what tea helps with acne | 0 | 600 | 0.0% | 9.6 | Teas for hormones / acne |
| 11 | what type of acne do i have quiz | 0 | 505 | 0.0% | 45.1 | Acne / hormone quizzes |
| 12 | hormonal acne supplements | 2 | 502 | 0.4% | 20.9 | Supplements for hormonal acne |
| 13 | how to choose sunscreen that doesn’t mess with hormones | 0 | 502 | 0.0% | 6.7 | Sunscreen / endocrine disruptors |
| 14 | what tea is good for hormonal acne | 2 | 489 | 0.4% | 5.4 | Teas for hormones / acne |
| 15 | tea that helps with acne | 0 | 466 | 0.0% | 12.3 | Teas for hormones / acne |
| 16 | what tea helps with hormonal acne | 0 | 463 | 0.0% | 5.5 | Teas for hormones / acne |
| 17 | acne affiliate programs | 0 | 413 | 0.0% | 6.8 | Affiliate / wholesale |
| 18 | best tea for acne | 0 | 331 | 0.0% | 13.4 | Teas for hormones / acne |
| 19 | teas for hormonal acne | 10 | 311 | 3.2% | 5.4 | Teas for hormones / acne |
| 20 | estrogen tea | 0 | 309 | 0.0% | 8.9 | Teas for hormones / acne |
| 21 | does caffeine cause acne | 0 | 301 | 0.0% | 38.0 | Coffee / caffeine and acne |
| 22 | teas that help with acne | 3 | 291 | 1.0% | 8.1 | Teas for hormones / acne |
| 23 | can coffee cause hormonal acne | 1 | 269 | 0.4% | 8.8 | Coffee / caffeine and acne |
| 24 | hormonal acne supplement | 0 | 268 | 0.0% | 20.5 | Supplements for hormonal acne |
| 25 | what kind of acne do i have quiz | 0 | 258 | 0.0% | 36.7 | Acne / hormone quizzes |
| 26 | what teas help with acne | 0 | 238 | 0.0% | 9.6 | Teas for hormones / acne |
| 27 | herbal tea for acne skin | 1 | 231 | 0.4% | 9.7 | Teas for hormones / acne |
| 28 | what is causing my acne quiz | 1 | 229 | 0.4% | 13.2 | Acne / hormone quizzes |
| 29 | what tea helps acne | 0 | 229 | 0.0% | 10.2 | Teas for hormones / acne |
| 30 | how to balance hormones for acne | 0 | 224 | 0.0% | 66.6 | Hormonal acne: what / causes / types |

### A4. Top 30 non-brand queries in Canada (by impressions)

| # | Query | Clicks | Impr. | CTR | Avg pos | Cluster |
|---|---|---:|---:|---:|---:|---|
| 1 | hormonal acne supplements | 17 | 1,968 | 0.9% | 10.8 | Supplements for hormonal acne |
| 2 | acne supplements | 3 | 840 | 0.4% | 12.7 | Supplements for acne / clear skin (non-hormonal wording) |
| 3 | acne supplements canada | 7 | 780 | 0.9% | 9.1 | Supplements for acne / clear skin (non-hormonal wording) |
| 4 | skincare supplement | 0 | 472 | 0.0% | 19.7 | Supplements for acne / clear skin (non-hormonal wording) |
| 5 | supplements for hormonal acne | 6 | 441 | 1.4% | 10.3 | Supplements for hormonal acne |
| 6 | supplements for acne | 1 | 426 | 0.2% | 16.9 | Supplements for acne / clear skin (non-hormonal wording) |
| 7 | best tea for acne | 2 | 412 | 0.5% | 4.9 | Teas for hormones / acne |
| 8 | hormonal acne | 0 | 360 | 0.0% | 49.5 | Hormonal acne: what / causes / types |
| 9 | natural supplements for acne | 0 | 359 | 0.0% | 23.3 | Supplements for acne / clear skin (non-hormonal wording) |
| 10 | skin supplements for acne | 0 | 347 | 0.0% | 16.6 | Supplements for acne / clear skin (non-hormonal wording) |
| 11 | coffee and acne | 0 | 283 | 0.0% | 9.9 | Coffee / caffeine and acne |
| 12 | balance supplement | 2 | 281 | 0.7% | 3.8 | Supplements for acne / clear skin (non-hormonal wording) |
| 13 | acne supplement | 6 | 276 | 2.2% | 10.3 | Supplements for acne / clear skin (non-hormonal wording) |
| 14 | supplements for clear skin | 0 | 220 | 0.0% | 37.6 | Supplements for acne / clear skin (non-hormonal wording) |
| 15 | can caffeine cause acne | 0 | 219 | 0.0% | 11.4 | Coffee / caffeine and acne |
| 16 | does coffee cause acne | 0 | 219 | 0.0% | 12.6 | Coffee / caffeine and acne |
| 17 | does caffeine cause acne | 0 | 214 | 0.0% | 12.1 | Coffee / caffeine and acne |
| 18 | tea for hormonal imbalance | 3 | 208 | 1.4% | 6.4 | Teas for hormones / acne |
| 19 | best organic acne treatments | 0 | 206 | 0.0% | 27.8 | General acne (non-hormonal wording) |
| 20 | is coffee bad for acne | 0 | 201 | 0.0% | 11.0 | Coffee / caffeine and acne |
| 21 | clear skin supplements | 0 | 200 | 0.0% | 30.3 | Supplements for acne / clear skin (non-hormonal wording) |
| 22 | dim supplement for acne | 1 | 197 | 0.5% | 10.3 | DIM |
| 23 | can coffee cause acne | 0 | 195 | 0.0% | 11.8 | Coffee / caffeine and acne |
| 24 | tea for acne | 0 | 195 | 0.0% | 8.6 | Teas for hormones / acne |
| 25 | caffeine and acne | 0 | 187 | 0.0% | 9.8 | Coffee / caffeine and acne |
| 26 | tea for hormonal acne | 5 | 153 | 3.3% | 4.1 | Teas for hormones / acne |
| 27 | hormonal skincare | 0 | 150 | 0.0% | 24.9 | Topicals / skincare routine |
| 28 | does coffee make you break out | 0 | 149 | 0.0% | 10.0 | Coffee / caffeine and acne |
| 29 | hormonal acne supplement | 6 | 143 | 4.2% | 8.4 | Supplements for hormonal acne |
| 30 | best tea for hormonal imbalance | 1 | 140 | 0.7% | 5.3 | Teas for hormones / acne |
